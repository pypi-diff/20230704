# Comparing `tmp/pyfem-0.1.0.tar.gz` & `tmp/pyfem-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfem-0.1.0.tar", last modified: Wed Jun 14 08:38:07 2023, max compression
+gzip compressed data, was "pyfem-0.1.1.tar", last modified: Tue Jul  4 03:24:57 2023, max compression
```

## Comparing `pyfem-0.1.0.tar` & `pyfem-0.1.1.tar`

### file list

```diff
@@ -1,84 +1,88 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 08:38:07.848612 pyfem-0.1.0/
--rw-rw-rw-   0        0        0    11525 2023-05-04 02:49:52.000000 pyfem-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      793 2023-06-14 08:38:07.848612 pyfem-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-05-19 03:01:04.000000 pyfem-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-14 08:38:07.849604 pyfem-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1067 2023-06-14 08:37:45.000000 pyfem-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-14 08:38:07.766603 pyfem-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-14 08:38:07.776603 pyfem-0.1.0/src/pyfem/
--rw-rw-rw-   0        0        0     1025 2023-06-13 08:12:20.000000 pyfem-0.1.0/src/pyfem/Job.py
--rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.0/src/pyfem/__init__.py
--rw-rw-rw-   0        0        0      277 2023-05-22 03:59:51.000000 pyfem-0.1.0/src/pyfem/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 08:38:07.787603 pyfem-0.1.0/src/pyfem/amplitude/
--rw-rw-rw-   0        0        0      924 2023-06-09 08:03:09.000000 pyfem-0.1.0/src/pyfem/amplitude/BaseAmplitude.py
--rw-rw-rw-   0        0        0     1357 2023-06-09 03:34:39.000000 pyfem-0.1.0/src/pyfem/amplitude/TabularAmplitude.py
--rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.0/src/pyfem/amplitude/__init__.py
--rw-rw-rw-   0        0        0      818 2023-06-09 03:34:39.000000 pyfem-0.1.0/src/pyfem/amplitude/get_amplitude_data.py
-drwxrwxrwx   0        0        0        0 2023-06-14 08:38:07.790604 pyfem-0.1.0/src/pyfem/assembly/
--rw-rw-rw-   0        0        0    10102 2023-06-13 04:25:07.000000 pyfem-0.1.0/src/pyfem/assembly/Assembly.py
--rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.0/src/pyfem/assembly/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 08:38:07.795614 pyfem-0.1.0/src/pyfem/bc/
--rw-rw-rw-   0        0        0     1564 2023-06-09 04:33:36.000000 pyfem-0.1.0/src/pyfem/bc/BaseBC.py
--rw-rw-rw-   0        0        0     2406 2023-06-09 08:02:29.000000 pyfem-0.1.0/src/pyfem/bc/DirichletBC.py
--rw-rw-rw-   0        0        0     3706 2023-06-09 08:02:51.000000 pyfem-0.1.0/src/pyfem/bc/NeumannBC.py
--rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.0/src/pyfem/bc/__init__.py
--rw-rw-rw-   0        0        0     1321 2023-06-09 04:19:15.000000 pyfem-0.1.0/src/pyfem/bc/get_bc_data.py
-drwxrwxrwx   0        0        0        0 2023-06-14 08:38:07.805603 pyfem-0.1.0/src/pyfem/elements/
--rw-rw-rw-   0        0        0     8145 2023-06-14 07:58:47.000000 pyfem-0.1.0/src/pyfem/elements/BaseElement.py
--rw-rw-rw-   0        0        0     2315 2023-05-30 06:11:08.000000 pyfem-0.1.0/src/pyfem/elements/IsoElementDiagram.py
--rw-rw-rw-   0        0        0    30821 2023-06-05 12:47:22.000000 pyfem-0.1.0/src/pyfem/elements/IsoElementShape.py
--rw-rw-rw-   0        0        0     9385 2023-06-14 07:58:47.000000 pyfem-0.1.0/src/pyfem/elements/SolidPlaneSmallStrain.py
--rw-rw-rw-   0        0        0    10151 2023-06-14 07:58:47.000000 pyfem-0.1.0/src/pyfem/elements/SolidVolumeSmallStrain.py
--rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.0/src/pyfem/elements/__init__.py
--rw-rw-rw-   0        0        0     2169 2023-06-13 04:20:37.000000 pyfem-0.1.0/src/pyfem/elements/get_element_data.py
--rw-rw-rw-   0        0        0     1842 2023-06-08 06:40:10.000000 pyfem-0.1.0/src/pyfem/elements/get_iso_element_type.py
-drwxrwxrwx   0        0        0        0 2023-06-14 08:38:07.808612 pyfem-0.1.0/src/pyfem/fem/
--rw-rw-rw-   0        0        0      897 2023-06-01 03:56:06.000000 pyfem-0.1.0/src/pyfem/fem/Timer.py
--rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.0/src/pyfem/fem/__init__.py
--rw-rw-rw-   0        0        0       68 2023-06-08 03:23:23.000000 pyfem-0.1.0/src/pyfem/fem/constants.py
-drwxrwxrwx   0        0        0        0 2023-06-14 08:38:07.822602 pyfem-0.1.0/src/pyfem/io/
--rw-rw-rw-   0        0        0      592 2023-06-09 03:34:39.000000 pyfem-0.1.0/src/pyfem/io/Amplitude.py
--rw-rw-rw-   0        0        0      888 2023-06-09 03:34:39.000000 pyfem-0.1.0/src/pyfem/io/BC.py
--rw-rw-rw-   0        0        0      614 2023-06-08 03:23:23.000000 pyfem-0.1.0/src/pyfem/io/Dof.py
--rw-rw-rw-   0        0        0     2438 2023-06-13 08:27:34.000000 pyfem-0.1.0/src/pyfem/io/Material.py
--rw-rw-rw-   0        0        0      538 2023-06-09 03:34:39.000000 pyfem-0.1.0/src/pyfem/io/Mesh.py
--rw-rw-rw-   0        0        0      612 2023-06-08 03:23:23.000000 pyfem-0.1.0/src/pyfem/io/Output.py
--rw-rw-rw-   0        0        0    10307 2023-06-09 03:34:39.000000 pyfem-0.1.0/src/pyfem/io/Properties.py
--rw-rw-rw-   0        0        0      852 2023-06-08 03:23:23.000000 pyfem-0.1.0/src/pyfem/io/Section.py
--rw-rw-rw-   0        0        0      821 2023-06-01 09:39:23.000000 pyfem-0.1.0/src/pyfem/io/Solver.py
--rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.0/src/pyfem/io/__init__.py
--rw-rw-rw-   0        0        0     1741 2023-06-14 08:37:45.000000 pyfem-0.1.0/src/pyfem/io/arguments.py
--rw-rw-rw-   0        0        0     4332 2023-06-08 03:23:23.000000 pyfem-0.1.0/src/pyfem/io/write_vtk.py
-drwxrwxrwx   0        0        0        0 2023-06-14 08:38:07.830611 pyfem-0.1.0/src/pyfem/materials/
--rw-rw-rw-   0        0        0     1233 2023-06-13 04:20:37.000000 pyfem-0.1.0/src/pyfem/materials/BaseMaterial.py
--rw-rw-rw-   0        0        0     6885 2023-06-13 04:20:37.000000 pyfem-0.1.0/src/pyfem/materials/ElasticIsotropic.py
--rw-rw-rw-   0        0        0     1303 2023-05-30 09:04:06.000000 pyfem-0.1.0/src/pyfem/materials/PlasticIsotropicHardening.py
--rw-rw-rw-   0        0        0     6730 2023-06-13 08:14:44.000000 pyfem-0.1.0/src/pyfem/materials/PlasticKinematicHardening.py
--rw-rw-rw-   0        0        0     5594 2023-06-14 07:58:47.000000 pyfem-0.1.0/src/pyfem/materials/ViscoElasticMaxwell.py
--rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.0/src/pyfem/materials/__init__.py
--rw-rw-rw-   0        0        0     1426 2023-06-14 05:02:11.000000 pyfem-0.1.0/src/pyfem/materials/get_material_data.py
-drwxrwxrwx   0        0        0        0 2023-06-14 08:38:07.834603 pyfem-0.1.0/src/pyfem/mesh/
--rw-rw-rw-   0        0        0     4977 2023-06-08 03:23:23.000000 pyfem-0.1.0/src/pyfem/mesh/ElementSet.py
--rw-rw-rw-   0        0        0     6572 2023-06-08 03:23:23.000000 pyfem-0.1.0/src/pyfem/mesh/MeshData.py
--rw-rw-rw-   0        0        0     5036 2023-06-08 03:23:23.000000 pyfem-0.1.0/src/pyfem/mesh/NodeSet.py
--rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.0/src/pyfem/mesh/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 08:38:07.839614 pyfem-0.1.0/src/pyfem/solvers/
--rw-rw-rw-   0        0        0      700 2023-06-09 03:34:39.000000 pyfem-0.1.0/src/pyfem/solvers/BaseSolver.py
--rw-rw-rw-   0        0        0     1382 2023-06-09 03:34:39.000000 pyfem-0.1.0/src/pyfem/solvers/LinearSolver.py
--rw-rw-rw-   0        0        0     7700 2023-06-14 07:58:16.000000 pyfem-0.1.0/src/pyfem/solvers/NonlinearSolver.py
--rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.0/src/pyfem/solvers/__init__.py
--rw-rw-rw-   0        0        0      991 2023-06-09 03:34:39.000000 pyfem-0.1.0/src/pyfem/solvers/get_solver_data.py
-drwxrwxrwx   0        0        0        0 2023-06-14 08:38:07.847602 pyfem-0.1.0/src/pyfem/utils/
--rw-rw-rw-   0        0        0     2350 2023-06-02 03:00:28.000000 pyfem-0.1.0/src/pyfem/utils/IntKeyDict.py
--rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.0/src/pyfem/utils/__init__.py
--rw-rw-rw-   0        0        0      795 2023-05-30 02:50:20.000000 pyfem-0.1.0/src/pyfem/utils/colors.py
--rw-rw-rw-   0        0        0     1518 2023-05-30 02:23:43.000000 pyfem-0.1.0/src/pyfem/utils/logger.py
--rw-rw-rw-   0        0        0     2352 2023-06-08 03:23:23.000000 pyfem-0.1.0/src/pyfem/utils/visualization.py
--rw-rw-rw-   0        0        0     1046 2023-05-30 02:47:20.000000 pyfem-0.1.0/src/pyfem/utils/wrappers.py
-drwxrwxrwx   0        0        0        0 2023-06-14 08:38:07.783604 pyfem-0.1.0/src/pyfem.egg-info/
--rw-rw-rw-   0        0        0      793 2023-06-14 08:38:07.000000 pyfem-0.1.0/src/pyfem.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2045 2023-06-14 08:38:07.000000 pyfem-0.1.0/src/pyfem.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 08:38:07.000000 pyfem-0.1.0/src/pyfem.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-06-14 08:38:07.000000 pyfem-0.1.0/src/pyfem.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       34 2023-06-14 08:38:07.000000 pyfem-0.1.0/src/pyfem.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-14 08:38:07.000000 pyfem-0.1.0/src/pyfem.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-04 03:24:57.895680 pyfem-0.1.1/
+-rw-rw-rw-   0        0        0    11525 2023-05-04 02:49:52.000000 pyfem-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     4373 2023-07-04 03:24:57.895680 pyfem-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3848 2023-06-15 07:05:17.000000 pyfem-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-04 03:24:57.895680 pyfem-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1067 2023-07-04 03:24:27.000000 pyfem-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:24:57.813681 pyfem-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-04 03:24:57.824681 pyfem-0.1.1/src/pyfem/
+-rw-rw-rw-   0        0        0     1025 2023-06-30 04:12:57.000000 pyfem-0.1.1/src/pyfem/Job.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.1/src/pyfem/__init__.py
+-rw-rw-rw-   0        0        0      277 2023-05-22 03:59:51.000000 pyfem-0.1.1/src/pyfem/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:24:57.834681 pyfem-0.1.1/src/pyfem/amplitude/
+-rw-rw-rw-   0        0        0      924 2023-06-09 08:03:09.000000 pyfem-0.1.1/src/pyfem/amplitude/BaseAmplitude.py
+-rw-rw-rw-   0        0        0     1357 2023-06-09 03:34:39.000000 pyfem-0.1.1/src/pyfem/amplitude/TabularAmplitude.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.1/src/pyfem/amplitude/__init__.py
+-rw-rw-rw-   0        0        0      818 2023-06-09 03:34:39.000000 pyfem-0.1.1/src/pyfem/amplitude/get_amplitude_data.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:24:57.836681 pyfem-0.1.1/src/pyfem/assembly/
+-rw-rw-rw-   0        0        0    10194 2023-07-03 09:00:51.000000 pyfem-0.1.1/src/pyfem/assembly/Assembly.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.1/src/pyfem/assembly/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:24:57.844679 pyfem-0.1.1/src/pyfem/bc/
+-rw-rw-rw-   0        0        0     1672 2023-06-30 06:18:06.000000 pyfem-0.1.1/src/pyfem/bc/BaseBC.py
+-rw-rw-rw-   0        0        0     2406 2023-06-29 04:23:17.000000 pyfem-0.1.1/src/pyfem/bc/DirichletBC.py
+-rw-rw-rw-   0        0        0     3706 2023-06-09 08:02:51.000000 pyfem-0.1.1/src/pyfem/bc/NeumannBC.py
+-rw-rw-rw-   0        0        0     2844 2023-07-03 03:24:41.000000 pyfem-0.1.1/src/pyfem/bc/NeumannBCConcentrated.py
+-rw-rw-rw-   0        0        0     8757 2023-06-30 10:22:55.000000 pyfem-0.1.1/src/pyfem/bc/NeumannBCDistributed.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.1/src/pyfem/bc/__init__.py
+-rw-rw-rw-   0        0        0     1555 2023-07-03 03:24:41.000000 pyfem-0.1.1/src/pyfem/bc/get_bc_data.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:24:57.854680 pyfem-0.1.1/src/pyfem/elements/
+-rw-rw-rw-   0        0        0     9323 2023-07-04 03:12:29.000000 pyfem-0.1.1/src/pyfem/elements/BaseElement.py
+-rw-rw-rw-   0        0        0     2315 2023-05-30 06:11:08.000000 pyfem-0.1.1/src/pyfem/elements/IsoElementDiagram.py
+-rw-rw-rw-   0        0        0    37158 2023-06-30 07:52:18.000000 pyfem-0.1.1/src/pyfem/elements/IsoElementShape.py
+-rw-rw-rw-   0        0        0     9927 2023-07-03 08:49:00.000000 pyfem-0.1.1/src/pyfem/elements/SolidPlaneSmallStrain.py
+-rw-rw-rw-   0        0        0    13761 2023-07-04 03:12:29.000000 pyfem-0.1.1/src/pyfem/elements/SolidThermalPlaneSmallStrain.py
+-rw-rw-rw-   0        0        0    10693 2023-07-03 08:47:31.000000 pyfem-0.1.1/src/pyfem/elements/SolidVolumeSmallStrain.py
+-rw-rw-rw-   0        0        0     7580 2023-07-04 03:12:29.000000 pyfem-0.1.1/src/pyfem/elements/ThermalStatic.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.1/src/pyfem/elements/__init__.py
+-rw-rw-rw-   0        0        0     2515 2023-07-04 03:12:29.000000 pyfem-0.1.1/src/pyfem/elements/get_element_data.py
+-rw-rw-rw-   0        0        0     1842 2023-06-08 06:40:10.000000 pyfem-0.1.1/src/pyfem/elements/get_iso_element_type.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:24:57.857680 pyfem-0.1.1/src/pyfem/fem/
+-rw-rw-rw-   0        0        0      897 2023-06-01 03:56:06.000000 pyfem-0.1.1/src/pyfem/fem/Timer.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.1/src/pyfem/fem/__init__.py
+-rw-rw-rw-   0        0        0       68 2023-06-08 03:23:23.000000 pyfem-0.1.1/src/pyfem/fem/constants.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:24:57.870678 pyfem-0.1.1/src/pyfem/io/
+-rw-rw-rw-   0        0        0      592 2023-06-09 03:34:39.000000 pyfem-0.1.1/src/pyfem/io/Amplitude.py
+-rw-rw-rw-   0        0        0      888 2023-06-09 03:34:39.000000 pyfem-0.1.1/src/pyfem/io/BC.py
+-rw-rw-rw-   0        0        0      614 2023-06-08 03:23:23.000000 pyfem-0.1.1/src/pyfem/io/Dof.py
+-rw-rw-rw-   0        0        0     2449 2023-06-19 04:15:35.000000 pyfem-0.1.1/src/pyfem/io/Material.py
+-rw-rw-rw-   0        0        0      538 2023-06-09 03:34:39.000000 pyfem-0.1.1/src/pyfem/io/Mesh.py
+-rw-rw-rw-   0        0        0      612 2023-06-08 03:23:23.000000 pyfem-0.1.1/src/pyfem/io/Output.py
+-rw-rw-rw-   0        0        0    10307 2023-06-09 03:34:39.000000 pyfem-0.1.1/src/pyfem/io/Properties.py
+-rw-rw-rw-   0        0        0      859 2023-07-03 03:48:49.000000 pyfem-0.1.1/src/pyfem/io/Section.py
+-rw-rw-rw-   0        0        0      821 2023-06-01 09:39:23.000000 pyfem-0.1.1/src/pyfem/io/Solver.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.1/src/pyfem/io/__init__.py
+-rw-rw-rw-   0        0        0     1741 2023-07-04 03:24:43.000000 pyfem-0.1.1/src/pyfem/io/arguments.py
+-rw-rw-rw-   0        0        0     4622 2023-07-04 03:12:29.000000 pyfem-0.1.1/src/pyfem/io/write_vtk.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:24:57.878680 pyfem-0.1.1/src/pyfem/materials/
+-rw-rw-rw-   0        0        0     1293 2023-07-04 03:12:29.000000 pyfem-0.1.1/src/pyfem/materials/BaseMaterial.py
+-rw-rw-rw-   0        0        0     7014 2023-07-03 08:58:44.000000 pyfem-0.1.1/src/pyfem/materials/ElasticIsotropic.py
+-rw-rw-rw-   0        0        0     6871 2023-07-04 03:12:29.000000 pyfem-0.1.1/src/pyfem/materials/PlasticKinematicHardening.py
+-rw-rw-rw-   0        0        0     2061 2023-07-04 03:12:29.000000 pyfem-0.1.1/src/pyfem/materials/ThermalIsotropic.py
+-rw-rw-rw-   0        0        0     5711 2023-07-04 03:12:29.000000 pyfem-0.1.1/src/pyfem/materials/ViscoElasticMaxwell.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.1/src/pyfem/materials/__init__.py
+-rw-rw-rw-   0        0        0     1551 2023-07-04 03:12:29.000000 pyfem-0.1.1/src/pyfem/materials/get_material_data.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:24:57.882681 pyfem-0.1.1/src/pyfem/mesh/
+-rw-rw-rw-   0        0        0     4977 2023-06-08 03:23:23.000000 pyfem-0.1.1/src/pyfem/mesh/ElementSet.py
+-rw-rw-rw-   0        0        0     6572 2023-06-08 03:23:23.000000 pyfem-0.1.1/src/pyfem/mesh/MeshData.py
+-rw-rw-rw-   0        0        0     5036 2023-06-08 03:23:23.000000 pyfem-0.1.1/src/pyfem/mesh/NodeSet.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.1/src/pyfem/mesh/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:24:57.887680 pyfem-0.1.1/src/pyfem/solvers/
+-rw-rw-rw-   0        0        0      700 2023-06-09 03:34:39.000000 pyfem-0.1.1/src/pyfem/solvers/BaseSolver.py
+-rw-rw-rw-   0        0        0     1603 2023-07-03 03:24:41.000000 pyfem-0.1.1/src/pyfem/solvers/LinearSolver.py
+-rw-rw-rw-   0        0        0     8733 2023-07-03 03:24:41.000000 pyfem-0.1.1/src/pyfem/solvers/NonlinearSolver.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.1/src/pyfem/solvers/__init__.py
+-rw-rw-rw-   0        0        0      991 2023-06-09 03:34:39.000000 pyfem-0.1.1/src/pyfem/solvers/get_solver_data.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:24:57.893680 pyfem-0.1.1/src/pyfem/utils/
+-rw-rw-rw-   0        0        0     2350 2023-06-02 03:00:28.000000 pyfem-0.1.1/src/pyfem/utils/IntKeyDict.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.1/src/pyfem/utils/__init__.py
+-rw-rw-rw-   0        0        0      795 2023-05-30 02:50:20.000000 pyfem-0.1.1/src/pyfem/utils/colors.py
+-rw-rw-rw-   0        0        0     1518 2023-05-30 02:23:43.000000 pyfem-0.1.1/src/pyfem/utils/logger.py
+-rw-rw-rw-   0        0        0     2352 2023-06-08 03:23:23.000000 pyfem-0.1.1/src/pyfem/utils/visualization.py
+-rw-rw-rw-   0        0        0     1046 2023-05-30 02:47:20.000000 pyfem-0.1.1/src/pyfem/utils/wrappers.py
+drwxrwxrwx   0        0        0        0 2023-07-04 03:24:57.830680 pyfem-0.1.1/src/pyfem.egg-info/
+-rw-rw-rw-   0        0        0     4373 2023-07-04 03:24:57.000000 pyfem-0.1.1/src/pyfem.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2198 2023-07-04 03:24:57.000000 pyfem-0.1.1/src/pyfem.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 03:24:57.000000 pyfem-0.1.1/src/pyfem.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-07-04 03:24:57.000000 pyfem-0.1.1/src/pyfem.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       34 2023-07-04 03:24:57.000000 pyfem-0.1.1/src/pyfem.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-04 03:24:57.000000 pyfem-0.1.1/src/pyfem.egg-info/top_level.txt
```

### Comparing `pyfem-0.1.0/LICENSE` & `pyfem-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.0/setup.py` & `pyfem-0.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyfem",
-    version="0.1.0",
+    version="0.1.1",
     author="Jingyu Sun",
     author_email="sun.jingyu@outlook.com",
     description="A finite element package for learning",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/sunwhale/pyfem",
     project_urls={
```

### Comparing `pyfem-0.1.0/src/pyfem/Job.py` & `pyfem-0.1.1/src/pyfem/Job.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.0/src/pyfem/amplitude/BaseAmplitude.py` & `pyfem-0.1.1/src/pyfem/amplitude/BaseAmplitude.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.0/src/pyfem/amplitude/TabularAmplitude.py` & `pyfem-0.1.1/src/pyfem/amplitude/TabularAmplitude.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.0/src/pyfem/amplitude/get_amplitude_data.py` & `pyfem-0.1.1/src/pyfem/amplitude/get_amplitude_data.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.0/src/pyfem/assembly/Assembly.py` & `pyfem-0.1.1/src/pyfem/assembly/Assembly.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,32 +91,32 @@
             for section in sections:
                 if element_set in section.element_sets:
                     self.section_of_element_set[element_set] = section
 
         for element_set_name, element_ids in element_sets.items():
             if element_set_name in self.section_of_element_set.keys():
                 section = self.section_of_element_set[element_set_name]
-                material = self.materials_dict[section.material_name]
-                material_data = get_material_data(material=material,
-                                                  dimension=dimension,
-                                                  option=section.type)
+                materials = [self.materials_dict[material_name] for material_name in section.material_names]
+                material_data_list = [get_material_data(material=material,
+                                                        dimension=dimension,
+                                                        section=section) for material in materials]
 
                 for element_id in element_ids:
                     connectivity = elements[element_id]
                     node_coords = nodes[connectivity]
                     iso_element_type = get_iso_element_type(node_coords)
                     iso_element_shape = iso_element_shape_dict[iso_element_type]
                     element_data = get_element_data(element_id=element_id,
                                                     iso_element_shape=iso_element_shape,
                                                     connectivity=connectivity,
                                                     node_coords=node_coords,
                                                     dof=dof,
-                                                    material=material,
+                                                    materials=materials,
                                                     section=section,
-                                                    material_data=material_data,
+                                                    material_data_list=material_data_list,
                                                     timer=timer)
 
                     element_data.assembly_conn = connectivity
                     element_data.create_element_dof_ids()
 
                     self.element_data_list.append(element_data)
```

### Comparing `pyfem-0.1.0/src/pyfem/bc/BaseBC.py` & `pyfem-0.1.1/src/pyfem/bc/BaseBC.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 """
 
 """
-from typing import Optional, Callable
+from typing import List, Optional, Callable, Tuple
 
 from numpy import empty, ndarray
 
 from pyfem.amplitude.BaseAmplitude import BaseAmplitude
 from pyfem.amplitude.get_amplitude_data import get_amplitude_data
 from pyfem.io.Amplitude import Amplitude
 from pyfem.io.BC import BC
@@ -29,14 +29,16 @@
             self.amplitude_data = BaseAmplitude()
             self.amplitude_data.set_f_amplitude([0, solver.total_time], [0, 1])
         self.get_amplitude: Callable = self.amplitude_data.get_amplitude
         self.bc_node_ids: ndarray = empty(0)
         self.bc_element_ids: ndarray = empty(0)
         self.dof_ids: ndarray = empty(0)
         self.dof_values: ndarray = empty(0)
+        self.bc_fext: ndarray = empty(0)
+        self.bc_surface: List[Tuple[int, str]] = []
 
     def to_string(self, level: int = 1) -> str:
         return object_dict_to_string_ndarray(self, level)
 
     def show(self) -> None:
         print(self.to_string())
```

### Comparing `pyfem-0.1.0/src/pyfem/bc/DirichletBC.py` & `pyfem-0.1.1/src/pyfem/bc/DirichletBC.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.0/src/pyfem/bc/NeumannBC.py` & `pyfem-0.1.1/src/pyfem/bc/NeumannBC.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.0/src/pyfem/bc/get_bc_data.py` & `pyfem-0.1.1/src/pyfem/bc/get_bc_data.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,24 +3,28 @@
 
 """
 from typing import Optional
 
 from pyfem.bc.BaseBC import BaseBC
 from pyfem.bc.DirichletBC import DirichletBC
 from pyfem.bc.NeumannBC import NeumannBC
+from pyfem.bc.NeumannBCConcentrated import NeumannBCConcentrated
+from pyfem.bc.NeumannBCDistributed import NeumannBCDistributed
 from pyfem.io.Amplitude import Amplitude
 from pyfem.io.BC import BC
 from pyfem.io.Dof import Dof
 from pyfem.io.Solver import Solver
 from pyfem.mesh.MeshData import MeshData
 from pyfem.utils.colors import error_style
 
 bc_data_dict = {
     'DirichletBC': DirichletBC,
-    'NeumannBC': NeumannBC
+    'NeumannBC': NeumannBC,
+    'NeumannBCConcentrated': NeumannBCConcentrated,
+    'NeumannBCDistributed': NeumannBCDistributed
 }
 
 
 def get_bc_data(bc: BC,
                 dof: Dof,
                 mesh_data: MeshData,
                 solver: Solver,
```

### Comparing `pyfem-0.1.0/src/pyfem/elements/BaseElement.py` & `pyfem-0.1.1/src/pyfem/elements/BaseElement.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,49 @@
 # -*- coding: utf-8 -*-
 """
 
 """
 from copy import deepcopy
-from typing import List, Dict
+from typing import List, Dict, Tuple
 
 from numpy import dot, array, ndarray
 from numpy.linalg import det, inv
 
 from pyfem.elements.IsoElementShape import IsoElementShape
 from pyfem.fem.Timer import Timer
 from pyfem.io.Dof import Dof
 from pyfem.io.Material import Material
 from pyfem.io.Section import Section
 from pyfem.materials.BaseMaterial import BaseMaterial
+from pyfem.utils.colors import error_style
 from pyfem.utils.visualization import object_slots_to_string_ndarray
 
 
 class BaseElement:
-    __slots__ = ('element_id', 'iso_element_shape', 'connectivity', 'node_coords', 'assembly_conn', 'dof', 'material',
-                 'section', 'material_data', 'timer', 'dof_names', 'gp_number', 'gp_jacobis', 'gp_jacobi_invs',
+    __slots__ = ('element_id', 'iso_element_shape', 'connectivity', 'node_coords', 'assembly_conn', 'dof', 'materials',
+                 'section', 'material_data_list', 'timer', 'dof_names', 'gp_number', 'gp_jacobis', 'gp_jacobi_invs',
                  'gp_jacobi_dets', 'gp_weight_times_jacobi_dets', 'gp_ddsddes', 'gp_state_variables',
                  'gp_state_variables_new', 'gp_field_variables', 'element_dof_number', 'element_dof_ids',
                  'element_dof_values', 'element_ddof_values', 'element_fint', 'element_stiffness',
-                 'element_average_field_variables')
+                 'element_average_field_variables', 'allowed_material_data_list', 'allowed_material_number')
 
     def __init__(self, element_id: int,
                  iso_element_shape: IsoElementShape,
                  connectivity: ndarray,
                  node_coords: ndarray) -> None:
         self.element_id: int = element_id  # 用户自定义的节点编号
         self.iso_element_shape: IsoElementShape = iso_element_shape
         self.connectivity: ndarray = connectivity  # 对应用户定义的节点编号
         self.node_coords: ndarray = node_coords
         self.assembly_conn: ndarray = None  # type: ignore  # 对应系统组装时的节点序号
 
         self.dof: Dof = None  # type: ignore
-        self.material: Material = None  # type: ignore
+        self.materials: List[Material] = None  # type: ignore
         self.section: Section = None  # type: ignore
-        self.material_data: BaseMaterial = None  # type: ignore
+        self.material_data_list: List[BaseMaterial] = None  # type: ignore
         self.timer: Timer = None  # type: ignore
 
         self.dof_names: List[str] = []
 
         self.gp_number: int = self.iso_element_shape.gp_number
         self.gp_jacobis: ndarray = None  # type: ignore
         self.gp_jacobi_invs: ndarray = None  # type: ignore
@@ -58,14 +59,17 @@
         self.element_dof_ids: List[int] = []  # 对应系统组装时的自由度序号
         self.element_dof_values: ndarray = None  # type: ignore  # 对应系统组装时的自由度的值
         self.element_ddof_values: ndarray = None  # type: ignore  # 对应系统组装时的自由度增量的值
         self.element_fint: ndarray = None  # type: ignore  # 对应系统组装时的内力值
         self.element_stiffness: ndarray = None  # type: ignore
         self.element_average_field_variables: Dict[str, ndarray] = {}
 
+        self.allowed_material_data_list: Tuple = ()
+        self.allowed_material_number: int = 1
+
     def to_string(self, level: int = 1) -> str:
         return object_slots_to_string_ndarray(self, level)
 
     def show(self) -> None:
         print(self.to_string())
 
     def cal_jacobi(self) -> None:
@@ -74,35 +78,45 @@
         """
 
         # 以下代码为采用for循环的计算方法，结构清晰，但计算效率较低
         # self.gp_jacobis = []
         # self.gp_jacobi_invs = []
         # self.gp_jacobi_dets = []
         # for gp_shape_gradient in self.iso_element_shape.gp_shape_gradients:
-        #     jacobi = dot(self.node_coords.transpose(), gp_shape_gradient)
+        #     jacobi = dot(gp_shape_gradient, self.node_coords).transpose()
         #     self.gp_jacobis.append(jacobi)
         #     self.gp_jacobi_invs.append(inv(jacobi))
         #     self.gp_jacobi_dets.append(det(jacobi))
         # self.gp_jacobis = array(self.gp_jacobis)
         # self.gp_jacobi_invs = array(self.gp_jacobi_invs)
         # self.gp_jacobi_dets = array(self.gp_jacobi_dets)
 
         # 以下代码为采用numpy高维矩阵乘法的计算方法，计算效率高，但要注意矩阵维度的变化
-        self.gp_jacobis = dot(self.node_coords.transpose(), self.iso_element_shape.gp_shape_gradients).swapaxes(0, 1)
+        self.gp_jacobis = dot(self.iso_element_shape.gp_shape_gradients, self.node_coords).swapaxes(1, 2)
         self.gp_jacobi_dets = det(self.gp_jacobis)
+
         # gp_jacobi通常为2×2或3×3的方阵，可以直接根据解析式求逆矩阵，计算效率比numpy.linalg.inv()函数更高
-        # self.gp_jacobi_invs = inv(self.gp_jacobis)
         self.gp_jacobi_invs = inverse(self.gp_jacobis, self.gp_jacobi_dets)
         self.gp_weight_times_jacobi_dets = self.iso_element_shape.gp_weights * self.gp_jacobi_dets
 
     def create_element_dof_ids(self) -> None:
         for node_index in self.assembly_conn:
             for dof_id, _ in enumerate(self.dof_names):
                 self.element_dof_ids.append(node_index * len(self.dof_names) + dof_id)
 
+    def check_materials(self) -> None:
+        if len(self.materials) != self.allowed_material_number:
+            error_msg = f'{type(self).__name__} section supports only {self.allowed_material_number} thermal material, please check the definition of {self.section.name}, length of {self.section.material_names} must be {self.allowed_material_number}'
+            raise NotImplementedError(error_style(error_msg))
+        for material_data in self.material_data_list:
+            material_data_class_name = type(material_data).__name__
+            if material_data_class_name not in self.allowed_material_data_list:
+                error_msg = f'{material_data_class_name} is not the supported material of {type(self).__name__} section, the allowed materials are {self.allowed_material_data_list}'
+                raise NotImplementedError(error_style(error_msg))
+
     def create_gp_b_matrices(self) -> None:
         pass
 
     def update_element_dof_values(self, global_dof_values: ndarray) -> None:
         self.element_dof_values = global_dof_values[self.element_dof_ids]
 
     def update_element_ddof_values(self, global_ddof_values: ndarray) -> None:
@@ -125,36 +139,41 @@
 
     def update_element_field_variables(self) -> None:
         pass
 
 
 def inverse(gp_jacobis: ndarray, gp_jacobi_dets: ndarray) -> ndarray:
     """
+    对于2×2和3×3的矩阵求逆直接带入下面的公式，其余的情况则调用np.linalg.inv()函数
+
     对于2×2的矩阵::
 
-        | a11  a12 |
-    A = |          |
-        | a21  a22 |
-
-    A^-1 = (1 / det(A)) * | a22  -a12 |
-                          |           |
-                          |-a21   a11 |
+            | a11  a12 |
+        A = |          |
+            | a21  a22 |
+
+        A^-1 = (1 / det(A)) * | a22  -a12 |
+                              |           |
+                              |-a21   a11 |
 
     对于3×3的矩阵::
-        | a11  a12  a13 |
-    A = |               |
-        | a21  a22  a23 |
-        |               |
-        | a31  a32  a33 |
-
-    A^-1 = (1 / det(A)) * |  A22*A33 - A23*A32   A13*A32 - A12*A33   A12*A23 - A13*A22 |
-                          |                                                            |
-                          |  A23*A31 - A21*A33   A11*A33 - A13*A31   A13*A21 - A11*A23 |
-                          |                                                            |
-                          |  A21*A32 - A22*A31   A12*A31 - A11*A32   A11*A22 - A12*A21 |
+
+            | a11  a12  a13 |
+        A = |               |
+            | a21  a22  a23 |
+            |               |
+            | a31  a32  a33 |
+
+        A^-1 = (1 / det(A)) * |  A22*A33 - A23*A32   A13*A32 - A12*A33   A12*A23 - A13*A22 |
+                              |                                                            |
+                              |  A23*A31 - A21*A33   A11*A33 - A13*A31   A13*A21 - A11*A23 |
+                              |                                                            |
+                              |  A21*A32 - A22*A31   A12*A31 - A11*A32   A11*A22 - A12*A21 |
+
+
     """
     gp_jacobi_invs = []
     for A, det_A in zip(gp_jacobis, gp_jacobi_dets):
         if A.shape == (2, 2):
             gp_jacobi_invs.append(
                 array([[A[1][1], -A[0][1]], [-A[1][0], A[0][0]]]) / det_A)
         elif A.shape == (3, 3):
@@ -170,9 +189,7 @@
         else:
             return inv(gp_jacobis)
     return array(gp_jacobi_invs)
 
 
 if __name__ == "__main__":
     pass
-    # a = array([[0,0],[0.125,0.125]])
-    # inv(a)
```

### Comparing `pyfem-0.1.0/src/pyfem/elements/IsoElementDiagram.py` & `pyfem-0.1.1/src/pyfem/elements/IsoElementDiagram.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.0/src/pyfem/elements/IsoElementShape.py` & `pyfem-0.1.1/src/pyfem/elements/IsoElementShape.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-from typing import Tuple, Callable
+from typing import Tuple, Callable, Dict
 
-from numpy import (empty, meshgrid, outer, column_stack, array, ndarray)
+from numpy import (empty, meshgrid, outer, column_stack, array, ndarray, insert, in1d)
 from numpy.polynomial.legendre import leggauss
 
 from pyfem.elements.IsoElementDiagram import IsoElementDiagram
+from pyfem.fem.constants import DTYPE
 from pyfem.utils.colors import error_style
 from pyfem.utils.visualization import object_dict_to_string_ndarray
 
 
 class IsoElementShape:
     """
     等参单元类，设置等参单元的形函数和积分点等信息
@@ -25,14 +26,22 @@
         self.order: int = 0
         self.shape_function: Callable = get_shape_empty
         self.gp_number = 0
         self.gp_coords: ndarray = empty(0)
         self.gp_weights: ndarray = empty(0)
         self.gp_shape_values: ndarray = empty(0)
         self.gp_shape_gradients: ndarray = empty(0)
+        self.bc_surface_number: int = 0
+        self.bc_surface_nodes_dict: Dict[str, Tuple] = {}
+        self.bc_surface_coord_dict: Dict[str, Tuple] = {}
+        self.bc_gp_coords_dict: Dict[str, ndarray] = {}
+        self.bc_gp_weights: ndarray = empty(0)
+        self.bc_gp_shape_values_dict: Dict[str, ndarray] = {}
+        self.bc_gp_shape_gradients_dict: Dict[str, ndarray] = {}
+        self.nodes_to_surface_dict: Dict[str, ndarray] = {}
 
         if element_type == 'empty':
             self.element_type = element_type
         elif element_type == 'line2':
             self.element_type = element_type
             self.set_line2()
         elif element_type == 'line3':
@@ -114,14 +123,41 @@
         gp_shape_gradients = []
         for gp_coord in self.gp_coords:
             h, dhdxi = self.shape_function(gp_coord)
             gp_shape_values.append(h)
             gp_shape_gradients.append(dhdxi)
         self.gp_shape_values = array(gp_shape_values)
         self.gp_shape_gradients = array(gp_shape_gradients)
+        self.bc_surface_number = 4
+        self.bc_surface_nodes_dict = {'s1': (3, 0),
+                                      's2': (1, 2),
+                                      's3': (0, 1),
+                                      's4': (2, 3)}
+        self.bc_surface_coord_dict = {'s1': (0, -1, 1),
+                                      's2': (0, 1, 1),
+                                      's3': (1, -1, 1),
+                                      's4': (1, 1, 1)}
+        for surface_name, surface_conn in self.bc_surface_nodes_dict.items():
+            self.nodes_to_surface_dict[surface_name] = in1d(range(self.nodes_number), surface_conn)
+        bc_gp_coords, self.bc_gp_weights = get_gauss_points(dimension=self.dimension - 1, order=self.order)
+        self.bc_gp_coords_dict = {'s1': insert(bc_gp_coords, 0, -1, axis=1),
+                                  's2': insert(bc_gp_coords, 0, 1, axis=1),
+                                  's3': insert(bc_gp_coords, 1, -1, axis=1),
+                                  's4': insert(bc_gp_coords, 1, 1, axis=1)}
+        self.bc_gp_shape_values_dict = {}
+        self.bc_gp_shape_gradients_dict = {}
+        for bc_surface_name, bc_surface_gp_coords in self.bc_gp_coords_dict.items():
+            bc_gp_shape_values = []
+            bc_gp_shape_gradients = []
+            for bc_surface_gp_coord in bc_surface_gp_coords:
+                h, dhdxi = self.shape_function(bc_surface_gp_coord)
+                bc_gp_shape_values.append(h)
+                bc_gp_shape_gradients.append(dhdxi)
+            self.bc_gp_shape_values_dict[bc_surface_name] = array(bc_gp_shape_values)
+            self.bc_gp_shape_gradients_dict[bc_surface_name] = array(bc_gp_shape_gradients)
         self.diagram = IsoElementDiagram.quad4
 
     def set_quad8(self) -> None:
         self.dimension = 2
         self.nodes_number = 8
         self.order = 3
         self.gp_coords, self.gp_weights = get_gauss_points(dimension=self.dimension, order=self.order)
@@ -131,14 +167,41 @@
         gp_shape_gradients = []
         for gp_coord in self.gp_coords:
             h, dhdxi = self.shape_function(gp_coord)
             gp_shape_values.append(h)
             gp_shape_gradients.append(dhdxi)
         self.gp_shape_values = array(gp_shape_values)
         self.gp_shape_gradients = array(gp_shape_gradients)
+        self.bc_surface_number = 4
+        self.bc_surface_nodes_dict = {'s1': (3, 0, 7),
+                                      's2': (1, 2, 5),
+                                      's3': (0, 1, 4),
+                                      's4': (2, 3, 6)}
+        self.bc_surface_coord_dict = {'s1': (0, -1, 1),
+                                      's2': (0, 1, 1),
+                                      's3': (1, -1, 1),
+                                      's4': (1, 1, 1)}
+        for surface_name, surface_conn in self.bc_surface_nodes_dict.items():
+            self.nodes_to_surface_dict[surface_name] = in1d(range(self.nodes_number), surface_conn)
+        bc_gp_coords, self.bc_gp_weights = get_gauss_points(dimension=self.dimension - 1, order=self.order)
+        self.bc_gp_coords_dict = {'s1': insert(bc_gp_coords, 0, -1, axis=1),
+                                  's2': insert(bc_gp_coords, 0, 1, axis=1),
+                                  's3': insert(bc_gp_coords, 1, -1, axis=1),
+                                  's4': insert(bc_gp_coords, 1, 1, axis=1)}
+        self.bc_gp_shape_values_dict = {}
+        self.bc_gp_shape_gradients_dict = {}
+        for bc_surface_name, bc_surface_gp_coords in self.bc_gp_coords_dict.items():
+            bc_gp_shape_values = []
+            bc_gp_shape_gradients = []
+            for bc_surface_gp_coord in bc_surface_gp_coords:
+                h, dhdxi = self.shape_function(bc_surface_gp_coord)
+                bc_gp_shape_values.append(h)
+                bc_gp_shape_gradients.append(dhdxi)
+            self.bc_gp_shape_values_dict[bc_surface_name] = array(bc_gp_shape_values)
+            self.bc_gp_shape_gradients_dict[bc_surface_name] = array(bc_gp_shape_gradients)
         self.diagram = IsoElementDiagram.quad8
 
     def set_tria3(self) -> None:
         self.dimension = 2
         self.nodes_number = 3
         self.order = 1
         self.gp_coords, self.gp_weights = get_gauss_points_triangle(order=self.order)
@@ -199,14 +262,47 @@
         gp_shape_gradients = []
         for gp_coord in self.gp_coords:
             h, dhdxi = self.shape_function(gp_coord)
             gp_shape_values.append(h)
             gp_shape_gradients.append(dhdxi)
         self.gp_shape_values = array(gp_shape_values)
         self.gp_shape_gradients = array(gp_shape_gradients)
+        self.bc_surface_number = 6
+        self.bc_surface_nodes_dict = {'s1': (0, 3, 7, 4),
+                                      's2': (1, 2, 6, 5),
+                                      's3': (0, 1, 5, 4),
+                                      's4': (2, 3, 6, 7),
+                                      's5': (0, 1, 2, 3),
+                                      's6': (4, 5, 6, 7)}
+        self.bc_surface_coord_dict = {'s1': (0, -1, 1),
+                                      's2': (0, 1, 1),
+                                      's3': (1, -1, 1),
+                                      's4': (1, 1, 1),
+                                      's5': (2, -1, 1),
+                                      's6': (2, 1, 1)}
+        for surface_name, surface_conn in self.bc_surface_nodes_dict.items():
+            self.nodes_to_surface_dict[surface_name] = in1d(range(self.nodes_number), surface_conn)
+        bc_gp_coords, self.bc_gp_weights = get_gauss_points(dimension=self.dimension - 1, order=self.order)
+        self.bc_gp_coords_dict = {'s1': insert(bc_gp_coords, 0, -1, axis=1),
+                                  's2': insert(bc_gp_coords, 0, 1, axis=1),
+                                  's3': insert(bc_gp_coords, 1, -1, axis=1),
+                                  's4': insert(bc_gp_coords, 1, 1, axis=1),
+                                  's5': insert(bc_gp_coords, 2, -1, axis=1),
+                                  's6': insert(bc_gp_coords, 2, 1, axis=1)}
+        self.bc_gp_shape_values_dict = {}
+        self.bc_gp_shape_gradients_dict = {}
+        for bc_surface_name, bc_surface_gp_coords in self.bc_gp_coords_dict.items():
+            bc_gp_shape_values = []
+            bc_gp_shape_gradients = []
+            for bc_surface_gp_coord in bc_surface_gp_coords:
+                h, dhdxi = self.shape_function(bc_surface_gp_coord)
+                bc_gp_shape_values.append(h)
+                bc_gp_shape_gradients.append(dhdxi)
+            self.bc_gp_shape_values_dict[bc_surface_name] = array(bc_gp_shape_values)
+            self.bc_gp_shape_gradients_dict[bc_surface_name] = array(bc_gp_shape_gradients)
         self.diagram = IsoElementDiagram.hex8
 
     def set_hex20(self) -> None:
         self.dimension = 3
         self.nodes_number = 20
         self.order = 3
         self.gp_coords, self.gp_weights = get_gauss_points(dimension=self.dimension, order=self.order)
@@ -238,21 +334,21 @@
                 +-->x0
 
     """
     if len(xi) != 1:
         raise NotImplementedError(error_style(f'coordinate {xi} must be dimension 1'))
 
     h = empty(2)
-    dhdxi = empty(shape=(2, 1))
+    dhdxi = empty(shape=(1, 2))
 
     h[0] = 0.5 * (1.0 - xi)
     h[1] = 0.5 * (1.0 + xi)
 
     dhdxi[0, 0] = -0.5
-    dhdxi[1, 0] = 0.5
+    dhdxi[0, 1] = 0.5
 
     return h, dhdxi
 
 
 def get_shape_line3(xi: ndarray) -> Tuple[ndarray, ndarray]:
     """
     三节点直线单元，节点序号及局部坐标方向如图所示::
@@ -291,28 +387,28 @@
         0--x0 * * * 1
 
     """
     if len(xi) != 2:
         raise NotImplementedError(error_style(f'coordinate {xi} must be dimension 2'))
 
     h = empty(3)
-    dhdxi = empty(shape=(3, 2))
+    dhdxi = empty(shape=(2, 3))
     xi = xi
 
     h[0] = 1.0 - xi[0] - xi[1]
     h[1] = xi[0]
     h[2] = xi[1]
 
     dhdxi[0, 0] = -1.0
-    dhdxi[1, 0] = 1.0
-    dhdxi[2, 0] = 0.0
+    dhdxi[0, 1] = 1.0
+    dhdxi[0, 2] = 0.0
 
-    dhdxi[0, 1] = -1.0
+    dhdxi[1, 0] = -1.0
     dhdxi[1, 1] = 0.0
-    dhdxi[2, 1] = 1.0
+    dhdxi[1, 2] = 1.0
 
     return h, dhdxi
 
 
 def get_shape_quad4(xi: ndarray) -> Tuple[ndarray, ndarray]:
     """
     四节点四边形单元，节点序号及局部坐标方向如图所示::
@@ -325,31 +421,31 @@
         |               |
         0---------------1
 
     """
     if len(xi) != 2:
         raise NotImplementedError(error_style(f'coordinate {xi} must be dimension 2'))
 
-    h = empty(4, dtype='float32')
-    dhdxi = empty(shape=(4, 2), dtype='float32')
+    h = empty(4, dtype=DTYPE)
+    dhdxi = empty(shape=(2, 4), dtype=DTYPE)
 
     h[0] = 0.25 * (1.0 - xi[0]) * (1.0 - xi[1])
     h[1] = 0.25 * (1.0 + xi[0]) * (1.0 - xi[1])
     h[2] = 0.25 * (1.0 + xi[0]) * (1.0 + xi[1])
     h[3] = 0.25 * (1.0 - xi[0]) * (1.0 + xi[1])
 
     dhdxi[0, 0] = -0.25 * (1.0 - xi[1])
-    dhdxi[1, 0] = 0.25 * (1.0 - xi[1])
-    dhdxi[2, 0] = 0.25 * (1.0 + xi[1])
-    dhdxi[3, 0] = -0.25 * (1.0 + xi[1])
+    dhdxi[0, 1] = 0.25 * (1.0 - xi[1])
+    dhdxi[0, 2] = 0.25 * (1.0 + xi[1])
+    dhdxi[0, 3] = -0.25 * (1.0 + xi[1])
 
-    dhdxi[0, 1] = -0.25 * (1.0 - xi[0])
+    dhdxi[1, 0] = -0.25 * (1.0 - xi[0])
     dhdxi[1, 1] = -0.25 * (1.0 + xi[0])
-    dhdxi[2, 1] = 0.25 * (1.0 + xi[0])
-    dhdxi[3, 1] = 0.25 * (1.0 - xi[0])
+    dhdxi[1, 2] = 0.25 * (1.0 + xi[0])
+    dhdxi[1, 3] = 0.25 * (1.0 - xi[0])
 
     return h, dhdxi
 
 
 def get_shape_quad8(xi: ndarray) -> Tuple[ndarray, ndarray]:
     """
     八节点四边形单元，节点序号及局部坐标方向如图所示::
@@ -363,42 +459,42 @@
         0-------4-------1
 
     """
     if len(xi) != 2:
         raise NotImplementedError(error_style(f'coordinate {xi} must be dimension 2'))
 
     h = empty(8)
-    dhdxi = empty(shape=(8, 2))
+    dhdxi = empty(shape=(2, 8))
 
     h[0] = -0.25 * (1.0 - xi[0]) * (1.0 - xi[1]) * (1.0 + xi[0] + xi[1])
     h[1] = -0.25 * (1.0 + xi[0]) * (1.0 - xi[1]) * (1.0 - xi[0] + xi[1])
     h[2] = -0.25 * (1.0 + xi[0]) * (1.0 + xi[1]) * (1.0 - xi[0] - xi[1])
     h[3] = -0.25 * (1.0 - xi[0]) * (1.0 + xi[1]) * (1.0 + xi[0] - xi[1])
     h[4] = 0.5 * (1.0 - xi[0]) * (1.0 + xi[0]) * (1.0 - xi[1])
     h[5] = 0.5 * (1.0 + xi[0]) * (1.0 + xi[1]) * (1.0 - xi[1])
     h[6] = 0.5 * (1.0 - xi[0]) * (1.0 + xi[0]) * (1.0 + xi[1])
     h[7] = 0.5 * (1.0 - xi[0]) * (1.0 + xi[1]) * (1.0 - xi[1])
 
     dhdxi[0, 0] = -0.25 * (-1.0 + xi[1]) * (2.0 * xi[0] + xi[1])
-    dhdxi[1, 0] = 0.25 * (-1.0 + xi[1]) * (-2.0 * xi[0] + xi[1])
-    dhdxi[2, 0] = 0.25 * (1.0 + xi[1]) * (2.0 * xi[0] + xi[1])
-    dhdxi[3, 0] = -0.25 * (1.0 + xi[1]) * (-2.0 * xi[0] + xi[1])
-    dhdxi[4, 0] = xi[0] * (-1.0 + xi[1])
-    dhdxi[5, 0] = -0.5 * (1.0 + xi[1]) * (-1.0 + xi[1])
-    dhdxi[6, 0] = -xi[0] * (1.0 + xi[1])
-    dhdxi[7, 0] = 0.5 * (1.0 + xi[1]) * (-1.0 + xi[1])
+    dhdxi[0, 1] = 0.25 * (-1.0 + xi[1]) * (-2.0 * xi[0] + xi[1])
+    dhdxi[0, 2] = 0.25 * (1.0 + xi[1]) * (2.0 * xi[0] + xi[1])
+    dhdxi[0, 3] = -0.25 * (1.0 + xi[1]) * (-2.0 * xi[0] + xi[1])
+    dhdxi[0, 4] = xi[0] * (-1.0 + xi[1])
+    dhdxi[0, 5] = -0.5 * (1.0 + xi[1]) * (-1.0 + xi[1])
+    dhdxi[0, 6] = -xi[0] * (1.0 + xi[1])
+    dhdxi[0, 7] = 0.5 * (1.0 + xi[1]) * (-1.0 + xi[1])
 
-    dhdxi[0, 1] = -0.25 * (-1.0 + xi[0]) * (xi[0] + 2.0 * xi[1])
+    dhdxi[1, 0] = -0.25 * (-1.0 + xi[0]) * (xi[0] + 2.0 * xi[1])
     dhdxi[1, 1] = 0.25 * (1.0 + xi[0]) * (-xi[0] + 2.0 * xi[1])
-    dhdxi[2, 1] = 0.25 * (1.0 + xi[0]) * (xi[0] + 2.0 * xi[1])
-    dhdxi[3, 1] = -0.25 * (-1.0 + xi[0]) * (-xi[0] + 2.0 * xi[1])
-    dhdxi[4, 1] = 0.5 * (1.0 + xi[0]) * (-1.0 + xi[0])
-    dhdxi[5, 1] = -xi[1] * (1.0 + xi[0])
-    dhdxi[6, 1] = -0.5 * (1.0 + xi[0]) * (-1.0 + xi[0])
-    dhdxi[7, 1] = xi[1] * (-1.0 + xi[0])
+    dhdxi[1, 2] = 0.25 * (1.0 + xi[0]) * (xi[0] + 2.0 * xi[1])
+    dhdxi[1, 3] = -0.25 * (-1.0 + xi[0]) * (-xi[0] + 2.0 * xi[1])
+    dhdxi[1, 4] = 0.5 * (1.0 + xi[0]) * (-1.0 + xi[0])
+    dhdxi[1, 5] = -xi[1] * (1.0 + xi[0])
+    dhdxi[1, 6] = -0.5 * (1.0 + xi[0]) * (-1.0 + xi[0])
+    dhdxi[1, 7] = xi[1] * (-1.0 + xi[0])
 
     return h, dhdxi
 
 
 def get_shape_tetra4(xi: ndarray) -> Tuple[ndarray, ndarray]:
     """
     四节点四面体单元，节点序号及局部坐标方向如图所示::
@@ -414,35 +510,35 @@
         0--x0 * * * * * 1
 
     """
     if len(xi) != 3:
         raise NotImplementedError(error_style(f'coordinate {xi} must be dimension 3'))
 
     h = empty(4)
-    dhdxi = empty(shape=(4, 3))
+    dhdxi = empty(shape=(3, 4))
 
     h[0] = 1.0 - xi[0] - xi[1] - xi[2]
     h[1] = xi[0]
     h[2] = xi[1]
     h[3] = xi[2]
 
     dhdxi[0, 0] = -1.0
-    dhdxi[1, 0] = 1.0
-    dhdxi[2, 0] = 0.0
-    dhdxi[3, 0] = 0.0
+    dhdxi[0, 1] = 1.0
+    dhdxi[0, 2] = 0.0
+    dhdxi[0, 3] = 0.0
 
-    dhdxi[0, 1] = -1.0
+    dhdxi[1, 0] = -1.0
     dhdxi[1, 1] = 0.0
-    dhdxi[2, 1] = 1.0
-    dhdxi[3, 1] = 0.0
+    dhdxi[1, 2] = 1.0
+    dhdxi[1, 3] = 0.0
 
-    dhdxi[0, 2] = -1.0
-    dhdxi[1, 2] = 0.0
+    dhdxi[2, 0] = -1.0
+    dhdxi[2, 1] = 0.0
     dhdxi[2, 2] = 0.0
-    dhdxi[3, 2] = 1.0
+    dhdxi[2, 3] = 1.0
 
     return h, dhdxi
 
 
 def get_shape_hex8(xi: ndarray) -> Tuple[ndarray, ndarray]:
     """
     八节点六面体单元，节点序号及局部坐标方向如图所示::
@@ -460,51 +556,51 @@
         0---------------1
 
     """
     if len(xi) != 3:
         raise NotImplementedError(error_style(f'coordinate {xi} must be dimension 3'))
 
     h = empty(8)
-    dhdxi = empty(shape=(8, 3))
+    dhdxi = empty(shape=(3, 8))
 
     h[0] = 0.125 * (1.0 - xi[0]) * (1.0 - xi[1]) * (1.0 - xi[2])
     h[1] = 0.125 * (1.0 + xi[0]) * (1.0 - xi[1]) * (1.0 - xi[2])
     h[2] = 0.125 * (1.0 + xi[0]) * (1.0 + xi[1]) * (1.0 - xi[2])
     h[3] = 0.125 * (1.0 - xi[0]) * (1.0 + xi[1]) * (1.0 - xi[2])
     h[4] = 0.125 * (1.0 - xi[0]) * (1.0 - xi[1]) * (1.0 + xi[2])
     h[5] = 0.125 * (1.0 + xi[0]) * (1.0 - xi[1]) * (1.0 + xi[2])
     h[6] = 0.125 * (1.0 + xi[0]) * (1.0 + xi[1]) * (1.0 + xi[2])
     h[7] = 0.125 * (1.0 - xi[0]) * (1.0 + xi[1]) * (1.0 + xi[2])
 
     dhdxi[0, 0] = -0.125 * (1.0 - xi[1]) * (1.0 - xi[2])
-    dhdxi[1, 0] = 0.125 * (1.0 - xi[1]) * (1.0 - xi[2])
-    dhdxi[2, 0] = 0.125 * (1.0 + xi[1]) * (1.0 - xi[2])
-    dhdxi[3, 0] = -0.125 * (1.0 + xi[1]) * (1.0 - xi[2])
-    dhdxi[4, 0] = -0.125 * (1.0 - xi[1]) * (1.0 + xi[2])
-    dhdxi[5, 0] = 0.125 * (1.0 - xi[1]) * (1.0 + xi[2])
-    dhdxi[6, 0] = 0.125 * (1.0 + xi[1]) * (1.0 + xi[2])
-    dhdxi[7, 0] = -0.125 * (1.0 + xi[1]) * (1.0 + xi[2])
+    dhdxi[0, 1] = 0.125 * (1.0 - xi[1]) * (1.0 - xi[2])
+    dhdxi[0, 2] = 0.125 * (1.0 + xi[1]) * (1.0 - xi[2])
+    dhdxi[0, 3] = -0.125 * (1.0 + xi[1]) * (1.0 - xi[2])
+    dhdxi[0, 4] = -0.125 * (1.0 - xi[1]) * (1.0 + xi[2])
+    dhdxi[0, 5] = 0.125 * (1.0 - xi[1]) * (1.0 + xi[2])
+    dhdxi[0, 6] = 0.125 * (1.0 + xi[1]) * (1.0 + xi[2])
+    dhdxi[0, 7] = -0.125 * (1.0 + xi[1]) * (1.0 + xi[2])
+    dhdxi[1, 0] = -0.125 * (1.0 - xi[0]) * (1.0 - xi[2])
 
-    dhdxi[0, 1] = -0.125 * (1.0 - xi[0]) * (1.0 - xi[2])
     dhdxi[1, 1] = -0.125 * (1.0 + xi[0]) * (1.0 - xi[2])
-    dhdxi[2, 1] = 0.125 * (1.0 + xi[0]) * (1.0 - xi[2])
-    dhdxi[3, 1] = 0.125 * (1.0 - xi[0]) * (1.0 - xi[2])
-    dhdxi[4, 1] = -0.125 * (1.0 - xi[0]) * (1.0 + xi[2])
-    dhdxi[5, 1] = -0.125 * (1.0 + xi[0]) * (1.0 + xi[2])
-    dhdxi[6, 1] = 0.125 * (1.0 + xi[0]) * (1.0 + xi[2])
-    dhdxi[7, 1] = 0.125 * (1.0 - xi[0]) * (1.0 + xi[2])
+    dhdxi[1, 2] = 0.125 * (1.0 + xi[0]) * (1.0 - xi[2])
+    dhdxi[1, 3] = 0.125 * (1.0 - xi[0]) * (1.0 - xi[2])
+    dhdxi[1, 4] = -0.125 * (1.0 - xi[0]) * (1.0 + xi[2])
+    dhdxi[1, 5] = -0.125 * (1.0 + xi[0]) * (1.0 + xi[2])
+    dhdxi[1, 6] = 0.125 * (1.0 + xi[0]) * (1.0 + xi[2])
+    dhdxi[1, 7] = 0.125 * (1.0 - xi[0]) * (1.0 + xi[2])
 
-    dhdxi[0, 2] = -0.125 * (1.0 - xi[0]) * (1.0 - xi[1])
-    dhdxi[1, 2] = -0.125 * (1.0 + xi[0]) * (1.0 - xi[1])
+    dhdxi[2, 0] = -0.125 * (1.0 - xi[0]) * (1.0 - xi[1])
+    dhdxi[2, 1] = -0.125 * (1.0 + xi[0]) * (1.0 - xi[1])
     dhdxi[2, 2] = -0.125 * (1.0 + xi[0]) * (1.0 + xi[1])
-    dhdxi[3, 2] = -0.125 * (1.0 - xi[0]) * (1.0 + xi[1])
-    dhdxi[4, 2] = 0.125 * (1.0 - xi[0]) * (1.0 - xi[1])
-    dhdxi[5, 2] = 0.125 * (1.0 + xi[0]) * (1.0 - xi[1])
-    dhdxi[6, 2] = 0.125 * (1.0 + xi[0]) * (1.0 + xi[1])
-    dhdxi[7, 2] = 0.125 * (1.0 - xi[0]) * (1.0 + xi[1])
+    dhdxi[2, 3] = -0.125 * (1.0 - xi[0]) * (1.0 + xi[1])
+    dhdxi[2, 4] = 0.125 * (1.0 - xi[0]) * (1.0 - xi[1])
+    dhdxi[2, 5] = 0.125 * (1.0 + xi[0]) * (1.0 - xi[1])
+    dhdxi[2, 6] = 0.125 * (1.0 + xi[0]) * (1.0 + xi[1])
+    dhdxi[2, 7] = 0.125 * (1.0 - xi[0]) * (1.0 + xi[1])
 
     return h, dhdxi
 
 
 def get_shape_tria6(xi: ndarray) -> Tuple[ndarray, ndarray]:
     """
     六节点三角形单元，节点序号及局部坐标方向如图所示::
@@ -520,37 +616,37 @@
     """
     # u = a0 + a1 * x0 + a2 * x1 + a3 * x0 * x1 + a4 * x0 * x0 +a5 * x1 *x1
     # v = b0 + b1 * x0 + b2 * x1 + b3 * x0 * x1 + b4 * x0 * x0 +b5 * x1 *x1
     if len(xi) != 2:
         raise NotImplementedError(error_style(f'coordinate {xi} must be dimension 2'))
 
     h = empty(6)
-    dhdxi = empty(shape=(6, 2))
+    dhdxi = empty(shape=(2, 6))
     xi = xi
 
     h[0] = - xi[0] + 2.0 * xi[0] * xi[0]
     h[1] = - xi[1] + 2.0 * xi[1] * xi[1]
     h[2] = - (1.0 - xi[0] - xi[1]) + 2.0 * (1.0 - xi[0] - xi[1]) * (1.0 - xi[0] - xi[1])
     h[3] = 4.0 * xi[0] * xi[1]
     h[4] = 4.0 * xi[1] * (1.0 - xi[0] - xi[1])
     h[5] = 4.0 * xi[0] * (1.0 - xi[0] - xi[1])
 
     dhdxi[0, 0] = -1.0 + 4.0 * xi[0]
-    dhdxi[1, 0] = 0.0
-    dhdxi[2, 0] = 1.0 + 4.0 * (-1.0) * (1.0 - xi[0] - xi[1])
-    dhdxi[3, 0] = 4.0 * xi[1]
-    dhdxi[4, 0] = -4.0 * xi[1]
-    dhdxi[5, 0] = 4.0 * (1.0 - xi[0] - xi[1]) - 4.0 * xi[0]
-
     dhdxi[0, 1] = 0.0
+    dhdxi[0, 2] = 1.0 + 4.0 * (-1.0) * (1.0 - xi[0] - xi[1])
+    dhdxi[0, 3] = 4.0 * xi[1]
+    dhdxi[0, 4] = -4.0 * xi[1]
+    dhdxi[0, 5] = 4.0 * (1.0 - xi[0] - xi[1]) - 4.0 * xi[0]
+
+    dhdxi[1, 0] = 0.0
     dhdxi[1, 1] = -1.0 + 4.0 * xi[1]
-    dhdxi[2, 1] = 1.0 + 4.0 * (-1.0) * (1.0 - xi[0] - xi[1])
-    dhdxi[3, 1] = 4.0 * xi[0]
-    dhdxi[4, 1] = 4.0 * (1.0 - xi[0] - xi[1]) - 4.0 * xi[1]
-    dhdxi[5, 1] = -4.0 * xi[0]
+    dhdxi[1, 2] = 1.0 + 4.0 * (-1.0) * (1.0 - xi[0] - xi[1])
+    dhdxi[1, 3] = 4.0 * xi[0]
+    dhdxi[1, 4] = 4.0 * (1.0 - xi[0] - xi[1]) - 4.0 * xi[1]
+    dhdxi[1, 5] = -4.0 * xi[0]
 
     return h, dhdxi
 
 
 def get_shape_hex20(xi: ndarray) -> Tuple[ndarray, ndarray]:
     """
     二十节点六面体单元，节点序号及局部坐标方向如图所示::
@@ -577,15 +673,15 @@
     # w = c0 + c1 * x0 + c2 * x1 + c3 * x2 + c4 * x0 * x0 + c5 * x1 * x1 + c6 * x2 * x2 + c7 * x0 * x1 + c8 * x1 * x2 +
     #     c9 * x2 * x0 + c10 * x0^3 + c11 * x1^3 + c12 * x2^3 + c13 * x0^2 * x1 + c14 * x1^2 * x2 + c15 * x2^2 * x0 +
     #     c16 * x0 * x1^2 + c17 * x1 * x2^2 + c18 * x2 * x0^2 + c19 * x0 * x1 * x2
     if len(xi) != 3:
         raise NotImplementedError(error_style(f'coordinate {xi} must be dimension 3'))
 
     h = empty(20)
-    dhdxi = empty(shape=(20, 3))
+    dhdxi = empty(shape=(3, 20))
 
     h[0] = 0.125 * (1.0 - xi[0]) * (1.0 - xi[1]) * (1.0 - xi[2]) * (- xi[0] - xi[1] - xi[2] - 2)
     h[1] = 0.125 * (1.0 + xi[0]) * (1.0 - xi[1]) * (1.0 - xi[2]) * (xi[0] - xi[1] - xi[2] - 2)
     h[2] = 0.125 * (1.0 + xi[0]) * (1.0 + xi[1]) * (1.0 - xi[2]) * (xi[0] + xi[1] - xi[2] - 2)
     h[3] = 0.125 * (1.0 - xi[0]) * (1.0 + xi[1]) * (1.0 - xi[2]) * (- xi[0] + xi[1] - xi[2] - 2)
     h[4] = 0.125 * (1.0 - xi[0]) * (1.0 - xi[1]) * (1.0 + xi[2]) * (- xi[0] - xi[1] + xi[2] - 2)
     h[5] = 0.125 * (1.0 + xi[0]) * (1.0 - xi[1]) * (1.0 + xi[2]) * (xi[0] - xi[1] + xi[2] - 2)
@@ -601,75 +697,75 @@
     h[15] = 0.25 * (1.0 - xi[0]) * (1.0 - xi[1] * xi[1]) * (1.0 + xi[2])
     h[16] = 0.25 * (1.0 - xi[0]) * (1.0 - xi[1]) * (1.0 - xi[2] * xi[2])
     h[17] = 0.25 * (1.0 + xi[0]) * (1.0 - xi[1]) * (1.0 - xi[2] * xi[2])
     h[18] = 0.25 * (1.0 + xi[0]) * (1.0 + xi[1]) * (1.0 - xi[2] * xi[2])
     h[19] = 0.25 * (1.0 - xi[0]) * (1.0 + xi[1]) * (1.0 - xi[2] * xi[2])
 
     dhdxi[0, 0] = 0.125 * (1.0 - xi[1]) * (1.0 - xi[2])
-    dhdxi[1, 0] = 0.125 * (1.0 - xi[1]) * (1.0 - xi[2])
-    dhdxi[2, 0] = 0.125 * (1.0 + xi[1]) * (1.0 - xi[2])
-    dhdxi[3, 0] = 0.125 * (1.0 + xi[1]) * (1.0 - xi[2])
-    dhdxi[4, 0] = 0.125 * (1.0 - xi[1]) * (1.0 + xi[2])
-    dhdxi[5, 0] = 0.125 * (1.0 - xi[1]) * (1.0 + xi[2])
-    dhdxi[6, 0] = 0.125 * (1.0 + xi[1]) * (1.0 + xi[2])
-    dhdxi[7, 0] = 0.125 * (1.0 + xi[1]) * (1.0 + xi[2])
-    dhdxi[8, 0] = -0.50 * xi[0] * (1.0 - xi[1]) * (1.0 - xi[2])
-    dhdxi[9, 0] = 0.25 * (1.0 - xi[1] * xi[1]) * (1.0 - xi[2])
-    dhdxi[10, 0] = -0.50 * xi[0] * (1.0 + xi[1]) * (1.0 - xi[2])
-    dhdxi[11, 0] = -0.25 * (1.0 - xi[1] * xi[1]) * (1.0 - xi[2])
-    dhdxi[12, 0] = -0.50 * xi[0] * (1.0 - xi[1]) * (1.0 + xi[2])
-    dhdxi[13, 0] = 0.25 * (1.0 - xi[1] * xi[1]) * (1.0 + xi[2])
-    dhdxi[14, 0] = -0.50 * xi[0] * (1.0 + xi[1]) * (1.0 + xi[2])
-    dhdxi[15, 0] = -0.25 * (1.0 - xi[1] * xi[1]) * (1.0 + xi[2])
-    dhdxi[16, 0] = -0.25 * (1.0 - xi[1]) * (1.0 - xi[2] * xi[2])
-    dhdxi[17, 0] = 0.25 * (1.0 - xi[1]) * (1.0 - xi[2] * xi[2])
-    dhdxi[18, 0] = 0.25 * (1.0 + xi[1]) * (1.0 - xi[2] * xi[2])
-    dhdxi[19, 0] = -0.25 * (1.0 + xi[1]) * (1.0 - xi[2] * xi[2])
+    dhdxi[0, 1] = 0.125 * (1.0 - xi[1]) * (1.0 - xi[2])
+    dhdxi[0, 2] = 0.125 * (1.0 + xi[1]) * (1.0 - xi[2])
+    dhdxi[0, 3] = 0.125 * (1.0 + xi[1]) * (1.0 - xi[2])
+    dhdxi[0, 4] = 0.125 * (1.0 - xi[1]) * (1.0 + xi[2])
+    dhdxi[0, 5] = 0.125 * (1.0 - xi[1]) * (1.0 + xi[2])
+    dhdxi[0, 6] = 0.125 * (1.0 + xi[1]) * (1.0 + xi[2])
+    dhdxi[0, 7] = 0.125 * (1.0 + xi[1]) * (1.0 + xi[2])
+    dhdxi[0, 8] = -0.50 * xi[0] * (1.0 - xi[1]) * (1.0 - xi[2])
+    dhdxi[0, 9] = 0.25 * (1.0 - xi[1] * xi[1]) * (1.0 - xi[2])
+    dhdxi[0, 10] = -0.50 * xi[0] * (1.0 + xi[1]) * (1.0 - xi[2])
+    dhdxi[0, 11] = -0.25 * (1.0 - xi[1] * xi[1]) * (1.0 - xi[2])
+    dhdxi[0, 12] = -0.50 * xi[0] * (1.0 - xi[1]) * (1.0 + xi[2])
+    dhdxi[0, 13] = 0.25 * (1.0 - xi[1] * xi[1]) * (1.0 + xi[2])
+    dhdxi[0, 14] = -0.50 * xi[0] * (1.0 + xi[1]) * (1.0 + xi[2])
+    dhdxi[0, 15] = -0.25 * (1.0 - xi[1] * xi[1]) * (1.0 + xi[2])
+    dhdxi[0, 16] = -0.25 * (1.0 - xi[1]) * (1.0 - xi[2] * xi[2])
+    dhdxi[0, 17] = 0.25 * (1.0 - xi[1]) * (1.0 - xi[2] * xi[2])
+    dhdxi[0, 18] = 0.25 * (1.0 + xi[1]) * (1.0 - xi[2] * xi[2])
+    dhdxi[0, 19] = -0.25 * (1.0 + xi[1]) * (1.0 - xi[2] * xi[2])
 
-    dhdxi[0, 1] = 0.125 * (1.0 - xi[0]) * (1.0 - xi[2])
+    dhdxi[1, 0] = 0.125 * (1.0 - xi[0]) * (1.0 - xi[2])
     dhdxi[1, 1] = 0.125 * (1.0 + xi[0]) * (1.0 - xi[2])
-    dhdxi[2, 1] = 0.125 * (1.0 + xi[0]) * (1.0 - xi[2])
-    dhdxi[3, 1] = 0.125 * (1.0 - xi[0]) * (1.0 - xi[2])
-    dhdxi[4, 1] = 0.125 * (1.0 - xi[0]) * (1.0 + xi[2])
-    dhdxi[5, 1] = 0.125 * (1.0 + xi[0]) * (1.0 + xi[2])
-    dhdxi[6, 1] = 0.125 * (1.0 + xi[0]) * (1.0 + xi[2])
-    dhdxi[7, 1] = 0.125 * (1.0 - xi[0]) * (1.0 + xi[2])
-    dhdxi[8, 1] = -0.25 * (1.0 - xi[0] * xi[0]) * (1.0 - xi[2])
-    dhdxi[9, 1] = -0.50 * (1.0 + xi[0]) * xi[1] * (1.0 - xi[2])
-    dhdxi[10, 1] = 0.25 * (1.0 - xi[0] * xi[0]) * (1.0 - xi[2])
-    dhdxi[11, 1] = -0.50 * (1.0 - xi[0]) * xi[1] * (1.0 - xi[2])
-    dhdxi[12, 1] = -0.25 * (1.0 - xi[0] * xi[0]) * (1.0 + xi[2])
-    dhdxi[13, 1] = -0.50 * (1.0 + xi[0]) * xi[1] * (1.0 + xi[2])
-    dhdxi[14, 1] = 0.25 * (1.0 - xi[0] * xi[0]) * (1.0 + xi[2])
-    dhdxi[15, 1] = -0.50 * (1.0 - xi[0]) * (1.0 + xi[2])
-    dhdxi[16, 1] = -0.25 * (1.0 - xi[0]) * (1.0 - xi[2] * xi[2])
-    dhdxi[17, 1] = -0.25 * (1.0 + xi[0]) * (1.0 - xi[2] * xi[2])
-    dhdxi[18, 1] = 0.25 * (1.0 + xi[0]) * (1.0 - xi[2] * xi[2])
-    dhdxi[19, 1] = 0.25 * (1.0 - xi[0]) * (1.0 - xi[2] * xi[2])
+    dhdxi[1, 2] = 0.125 * (1.0 + xi[0]) * (1.0 - xi[2])
+    dhdxi[1, 3] = 0.125 * (1.0 - xi[0]) * (1.0 - xi[2])
+    dhdxi[1, 4] = 0.125 * (1.0 - xi[0]) * (1.0 + xi[2])
+    dhdxi[1, 5] = 0.125 * (1.0 + xi[0]) * (1.0 + xi[2])
+    dhdxi[1, 6] = 0.125 * (1.0 + xi[0]) * (1.0 + xi[2])
+    dhdxi[1, 7] = 0.125 * (1.0 - xi[0]) * (1.0 + xi[2])
+    dhdxi[1, 8] = -0.25 * (1.0 - xi[0] * xi[0]) * (1.0 - xi[2])
+    dhdxi[1, 9] = -0.50 * (1.0 + xi[0]) * xi[1] * (1.0 - xi[2])
+    dhdxi[1, 10] = 0.25 * (1.0 - xi[0] * xi[0]) * (1.0 - xi[2])
+    dhdxi[1, 11] = -0.50 * (1.0 - xi[0]) * xi[1] * (1.0 - xi[2])
+    dhdxi[1, 12] = -0.25 * (1.0 - xi[0] * xi[0]) * (1.0 + xi[2])
+    dhdxi[1, 13] = -0.50 * (1.0 + xi[0]) * xi[1] * (1.0 + xi[2])
+    dhdxi[1, 14] = 0.25 * (1.0 - xi[0] * xi[0]) * (1.0 + xi[2])
+    dhdxi[1, 15] = -0.50 * (1.0 - xi[0]) * (1.0 + xi[2])
+    dhdxi[1, 16] = -0.25 * (1.0 - xi[0]) * (1.0 - xi[2] * xi[2])
+    dhdxi[1, 17] = -0.25 * (1.0 + xi[0]) * (1.0 - xi[2] * xi[2])
+    dhdxi[1, 18] = 0.25 * (1.0 + xi[0]) * (1.0 - xi[2] * xi[2])
+    dhdxi[1, 19] = 0.25 * (1.0 - xi[0]) * (1.0 - xi[2] * xi[2])
 
-    dhdxi[0, 2] = 0.125 * (1.0 - xi[0]) * (1.0 - xi[1])
-    dhdxi[1, 2] = 0.125 * (1.0 + xi[0]) * (1.0 - xi[1])
+    dhdxi[2, 0] = 0.125 * (1.0 - xi[0]) * (1.0 - xi[1])
+    dhdxi[2, 1] = 0.125 * (1.0 + xi[0]) * (1.0 - xi[1])
     dhdxi[2, 2] = 0.125 * (1.0 + xi[0]) * (1.0 + xi[1])
-    dhdxi[3, 2] = 0.125 * (1.0 - xi[0]) * (1.0 + xi[1])
-    dhdxi[4, 2] = 0.125 * (1.0 - xi[0]) * (1.0 - xi[1])
-    dhdxi[5, 2] = 0.125 * (1.0 + xi[0]) * (1.0 - xi[1])
-    dhdxi[6, 2] = 0.125 * (1.0 + xi[0]) * (1.0 + xi[1])
-    dhdxi[7, 2] = 0.125 * (1.0 - xi[0]) * (1.0 + xi[1])
-    dhdxi[8, 2] = -0.25 * (1.0 - xi[0] * xi[0]) * (1.0 - xi[1])
-    dhdxi[9, 2] = -0.25 * (1.0 + xi[0]) * (1.0 - xi[1] * xi[1])
-    dhdxi[10, 2] = -0.25 * (1.0 - xi[0] * xi[0]) * (1.0 + xi[1])
-    dhdxi[11, 2] = -0.25 * (1.0 - xi[0]) * (1.0 - xi[1] * xi[1])
-    dhdxi[12, 2] = 0.25 * (1.0 - xi[0] * xi[0]) * (1.0 - xi[1])
-    dhdxi[13, 2] = 0.25 * (1.0 + xi[0]) * (1.0 - xi[1] * xi[1])
-    dhdxi[14, 2] = 0.25 * (1.0 - xi[0] * xi[0]) * (1.0 + xi[1])
-    dhdxi[15, 2] = 0.25 * (1.0 - xi[0]) * (1.0 - xi[1] * xi[1])
-    dhdxi[16, 2] = -0.50 * (1.0 - xi[0]) * (1.0 - xi[1]) * xi[2]
-    dhdxi[17, 2] = -0.50 * (1.0 + xi[0]) * (1.0 - xi[1]) * xi[2]
-    dhdxi[18, 2] = -0.50 * (1.0 + xi[0]) * (1.0 + xi[1]) * xi[2]
-    dhdxi[19, 2] = -0.50 * (1.0 - xi[0]) * (1.0 + xi[1]) * xi[2]
+    dhdxi[2, 3] = 0.125 * (1.0 - xi[0]) * (1.0 + xi[1])
+    dhdxi[2, 4] = 0.125 * (1.0 - xi[0]) * (1.0 - xi[1])
+    dhdxi[2, 5] = 0.125 * (1.0 + xi[0]) * (1.0 - xi[1])
+    dhdxi[2, 6] = 0.125 * (1.0 + xi[0]) * (1.0 + xi[1])
+    dhdxi[2, 7] = 0.125 * (1.0 - xi[0]) * (1.0 + xi[1])
+    dhdxi[2, 8] = -0.25 * (1.0 - xi[0] * xi[0]) * (1.0 - xi[1])
+    dhdxi[2, 9] = -0.25 * (1.0 + xi[0]) * (1.0 - xi[1] * xi[1])
+    dhdxi[2, 10] = -0.25 * (1.0 - xi[0] * xi[0]) * (1.0 + xi[1])
+    dhdxi[2, 11] = -0.25 * (1.0 - xi[0]) * (1.0 - xi[1] * xi[1])
+    dhdxi[2, 12] = 0.25 * (1.0 - xi[0] * xi[0]) * (1.0 - xi[1])
+    dhdxi[2, 13] = 0.25 * (1.0 + xi[0]) * (1.0 - xi[1] * xi[1])
+    dhdxi[2, 14] = 0.25 * (1.0 - xi[0] * xi[0]) * (1.0 + xi[1])
+    dhdxi[2, 15] = 0.25 * (1.0 - xi[0]) * (1.0 - xi[1] * xi[1])
+    dhdxi[2, 16] = -0.50 * (1.0 - xi[0]) * (1.0 - xi[1]) * xi[2]
+    dhdxi[2, 17] = -0.50 * (1.0 + xi[0]) * (1.0 - xi[1]) * xi[2]
+    dhdxi[2, 18] = -0.50 * (1.0 + xi[0]) * (1.0 + xi[1]) * xi[2]
+    dhdxi[2, 19] = -0.50 * (1.0 - xi[0]) * (1.0 + xi[1]) * xi[2]
 
     return h, dhdxi
 
 
 def get_gauss_points(dimension: int, order: int) -> Tuple[ndarray, ndarray]:
     xi, weight = leggauss(order)
     if dimension == 1:
@@ -689,15 +785,15 @@
         xi1 = xi1.ravel()
         xi2 = xi2.ravel()
         xi3 = xi3.ravel()
         xi = column_stack((xi1, xi2, xi3))
         weight = outer(outer(weight, weight), weight)
         weight = weight.ravel()
 
-    return xi.astype('float32'), weight.astype('float32')
+    return xi.astype(DTYPE), weight.astype(DTYPE)
 
 
 def get_gauss_points_triangle(order: int) -> Tuple[ndarray, ndarray]:
     if order == 1:
         xi = [[1.0 / 3.0, 1.0 / 3.0]]
         weight = [0.5]
 
@@ -719,36 +815,36 @@
         w4 = 0.1323941527885
         w7 = 0.225
         weight = [w1, w1, w1, w4, w4, w4, w7]
 
     else:
         raise NotImplementedError(error_style('Order must be 1, 3 or 7'))
 
-    return array(xi, dtype='float32'), array(weight, dtype='float32')
+    return array(xi, dtype=DTYPE), array(weight, dtype=DTYPE)
 
 
 def get_gauss_points_tetra(order: int) -> Tuple[ndarray, ndarray]:
     if order == 1:
         third = 1.0 / 3.0
         xi = [[third, third, third]]
         weight = [0.5 * third]
     else:
         raise NotImplementedError(error_style('Only order 1 integration implemented'))
 
-    return array(xi, dtype='float32'), array(weight, dtype='float32')
+    return array(xi, dtype=DTYPE), array(weight, dtype=DTYPE)
 
 
 def get_gauss_points_pyramid(order: int) -> Tuple[ndarray, ndarray]:
     if order == 1:
         xi = [[0., 0., -0.5]]
         weight = [128.0 / 27.0]
     else:
         raise NotImplementedError(error_style('Only order 1 integration implemented'))
 
-    return array(xi, dtype='float32'), array(weight, dtype='float32')
+    return array(xi, dtype=DTYPE), array(weight, dtype=DTYPE)
 
 
 def get_default_element_type(node_coords: ndarray) -> str:
     num_element_nodes = node_coords.shape[0]
     dimension = node_coords.shape[1]
 
     if dimension == 1:
@@ -798,9 +894,16 @@
     iso_element_shape = IsoElementShape('quad4')
     # iso_element_shape = IsoElementShape('hex8')
     # iso_element_shape = IsoElementShape('quad8')
     # iso_element_shape = IsoElementShape('tetra4')
     # iso_element_shape = IsoElementShape('line2')
     # iso_element_shape = IsoElementShape('line3')
     # iso_element_shape = IsoElementShape('empty')
+
+    # print(iso_element_shape.bc_gp_coords_dict['s1'])
+    # print(iso_element_shape.bc_gp_weights)
+    # print(iso_element_shape.bc_gp_shape_values_dict['s1'])
+    # print(iso_element_shape.bc_gp_shape_gradients_dict['s1'])
+
     iso_element_shape.show()
-    print(iso_element_shape.gp_weights.dtype)
+
+    # print(iso_element_shape.gp_weights.dtype)
```

### Comparing `pyfem-0.1.0/src/pyfem/elements/SolidPlaneSmallStrain.py` & `pyfem-0.1.1/src/pyfem/elements/SolidPlaneSmallStrain.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,32 +14,36 @@
 from pyfem.io.Material import Material
 from pyfem.io.Section import Section
 from pyfem.materials.BaseMaterial import BaseMaterial
 from pyfem.utils.colors import error_style
 
 
 class SolidPlaneSmallStrain(BaseElement):
-    __slots__ = ('gp_b_matrices', 'gp_b_matrices_transpose', 'gp_strains', 'gp_stresses')
+    __slots__ = BaseElement.__slots__ + ('gp_b_matrices', 'gp_b_matrices_transpose', 'gp_strains', 'gp_stresses')
 
     def __init__(self, element_id: int,
                  iso_element_shape: IsoElementShape,
                  connectivity: ndarray,
                  node_coords: ndarray,
                  dof: Dof,
-                 material: Material,
+                 materials: List[Material],
                  section: Section,
-                 material_data: BaseMaterial,
+                 material_data_list: List[BaseMaterial],
                  timer: Timer) -> None:
 
         super().__init__(element_id, iso_element_shape, connectivity, node_coords)
 
+        self.allowed_material_data_list = ('ElasticIsotropic', 'PlasticKinematicHardening', 'ViscoElasticMaxwell')
+        self.allowed_material_number = 1
+
         self.dof = dof
-        self.material = material
+        self.materials = materials
         self.section = section
-        self.material_data = material_data
+        self.material_data_list = material_data_list
+        self.check_materials()
         self.timer = timer
 
         self.dof_names = ['u1', 'u2']
         if dof.names != self.dof_names:
             error_msg = f'{dof.names} is not the supported dof of {type(self).__name__} element'
             raise NotImplementedError(error_style(error_msg))
 
@@ -58,15 +62,15 @@
         self.create_gp_b_matrices()
 
     def create_gp_b_matrices(self) -> None:
         self.gp_b_matrices = zeros(shape=(self.gp_number, 3, self.element_dof_number), dtype=DTYPE)
 
         for igp, (gp_shape_gradient, gp_jacobi_inv) in \
                 enumerate(zip(self.iso_element_shape.gp_shape_gradients, self.gp_jacobi_invs)):
-            gp_dhdx = dot(gp_shape_gradient, gp_jacobi_inv)
+            gp_dhdx = dot(gp_shape_gradient.transpose(), gp_jacobi_inv)
             for i, val in enumerate(gp_dhdx):
                 self.gp_b_matrices[igp, 0, i * 2] = val[0]
                 self.gp_b_matrices[igp, 1, i * 2 + 1] = val[1]
                 self.gp_b_matrices[igp, 2, i * 2] = val[1]
                 self.gp_b_matrices[igp, 2, i * 2 + 1] = val[0]
 
         self.gp_b_matrices_transpose = array([gp_b_matrix.transpose() for gp_b_matrix in self.gp_b_matrices])
@@ -85,23 +89,23 @@
         gp_strains = []
         gp_stresses = []
 
         for i in range(gp_number):
             gp_strain = dot(gp_b_matrices[i], element_dof_values)
             gp_dstrain = dot(gp_b_matrices[i], element_ddof_values)
             variable = {'strain': gp_strain, 'dstrain': gp_dstrain}
-            gp_ddsdde, gp_output = self.material_data.get_tangent(variable=variable,
-                                                                  state_variable=gp_state_variables[i],
-                                                                  state_variable_new=gp_state_variables_new[i],
-                                                                  element_id=element_id,
-                                                                  igp=i,
-                                                                  ntens=3,
-                                                                  ndi=2,
-                                                                  nshr=1,
-                                                                  timer=timer)
+            gp_ddsdde, gp_output = self.material_data_list[0].get_tangent(variable=variable,
+                                                                          state_variable=gp_state_variables[i],
+                                                                          state_variable_new=gp_state_variables_new[i],
+                                                                          element_id=element_id,
+                                                                          igp=i,
+                                                                          ntens=4,
+                                                                          ndi=3,
+                                                                          nshr=1,
+                                                                          timer=timer)
             gp_stress = gp_output['stress']
             gp_ddsddes.append(gp_ddsdde)
             gp_strains.append(gp_strain)
             gp_stresses.append(gp_stress)
 
         self.gp_ddsddes = gp_ddsddes
         self.gp_strains = gp_strains
@@ -132,23 +136,23 @@
         for i in range(gp_number):
             gp_weight_times_jacobi_det = gp_weight_times_jacobi_dets[i]
             gp_b_matrix_transpose = gp_b_matrices_transpose[i]
             gp_b_matrix = gp_b_matrices[i]
             gp_strain = dot(gp_b_matrix, element_dof_values)
             gp_dstrain = dot(gp_b_matrix, element_ddof_values)
             variable = {'strain': gp_strain, 'dstrain': gp_dstrain}
-            gp_ddsdde, gp_output = self.material_data.get_tangent(variable=variable,
-                                                                  state_variable=gp_state_variables[i],
-                                                                  state_variable_new=gp_state_variables_new[i],
-                                                                  element_id=element_id,
-                                                                  igp=i,
-                                                                  ntens=4,
-                                                                  ndi=3,
-                                                                  nshr=1,
-                                                                  timer=timer)
+            gp_ddsdde, gp_output = self.material_data_list[0].get_tangent(variable=variable,
+                                                                          state_variable=gp_state_variables[i],
+                                                                          state_variable_new=gp_state_variables_new[i],
+                                                                          element_id=element_id,
+                                                                          igp=i,
+                                                                          ntens=4,
+                                                                          ndi=3,
+                                                                          nshr=1,
+                                                                          timer=timer)
             gp_stress = gp_output['stress']
 
             self.element_stiffness += dot(gp_b_matrix_transpose, dot(gp_ddsdde, gp_b_matrix)) * \
                                       gp_weight_times_jacobi_det
 
             self.element_fint += dot(gp_b_matrix_transpose, gp_stress) * gp_weight_times_jacobi_det
 
@@ -198,8 +202,12 @@
         self.element_average_field_variables['E12'] = average_strain[2]
         self.element_average_field_variables['S11'] = average_stress[0]
         self.element_average_field_variables['S22'] = average_stress[1]
         self.element_average_field_variables['S12'] = average_stress[2]
 
 
 if __name__ == "__main__":
-    pass
+    from pyfem.Job import Job
+
+    job = Job(r'F:\Github\pyfem\examples\1element\hex8\Job-1.toml')
+
+    job.assembly.element_data_list[0].show()
```

### Comparing `pyfem-0.1.0/src/pyfem/elements/SolidVolumeSmallStrain.py` & `pyfem-0.1.1/src/pyfem/elements/SolidVolumeSmallStrain.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,32 +14,36 @@
 from pyfem.io.Material import Material
 from pyfem.io.Section import Section
 from pyfem.materials.BaseMaterial import BaseMaterial
 from pyfem.utils.colors import error_style
 
 
 class SolidVolumeSmallStrain(BaseElement):
-    __slots__ = ('gp_b_matrices', 'gp_b_matrices_transpose', 'gp_strains', 'gp_stresses')
+    __slots__ = BaseElement.__slots__ + ('gp_b_matrices', 'gp_b_matrices_transpose', 'gp_strains', 'gp_stresses')
 
     def __init__(self, element_id: int,
                  iso_element_shape: IsoElementShape,
                  connectivity: ndarray,
                  node_coords: ndarray,
                  dof: Dof,
-                 material: Material,
+                 materials: List[Material],
                  section: Section,
-                 material_data: BaseMaterial,
+                 material_data_list: List[BaseMaterial],
                  timer: Timer) -> None:
 
         super().__init__(element_id, iso_element_shape, connectivity, node_coords)
 
+        self.allowed_material_data_list = ('ElasticIsotropic', 'PlasticKinematicHardening', 'ViscoElasticMaxwell')
+        self.allowed_material_number = 1
+
         self.dof = dof
-        self.material = material
+        self.materials = materials
         self.section = section
-        self.material_data = material_data
+        self.material_data_list = material_data_list
+        self.check_materials()
         self.timer = timer
 
         self.dof_names = ['u1', 'u2', 'u3']
         if dof.names != self.dof_names:
             error_msg = f'{dof.names} is not the supported dof of {type(self).__name__} element'
             raise NotImplementedError(error_style(error_msg))
 
@@ -58,15 +62,15 @@
         self.create_gp_b_matrices()
 
     def create_gp_b_matrices(self) -> None:
         self.gp_b_matrices = zeros(shape=(self.iso_element_shape.gp_number, 6, self.element_dof_number))
 
         for igp, (gp_shape_gradient, gp_jacobi_inv) in \
                 enumerate(zip(self.iso_element_shape.gp_shape_gradients, self.gp_jacobi_invs)):
-            gp_dhdx = dot(gp_shape_gradient, gp_jacobi_inv)
+            gp_dhdx = dot(gp_shape_gradient.transpose(), gp_jacobi_inv)
             for i, val in enumerate(gp_dhdx):
                 self.gp_b_matrices[igp, 0, i * 3] = val[0]
                 self.gp_b_matrices[igp, 1, i * 3 + 1] = val[1]
                 self.gp_b_matrices[igp, 2, i * 3 + 2] = val[2]
                 self.gp_b_matrices[igp, 3, i * 3] = val[1]
                 self.gp_b_matrices[igp, 3, i * 3 + 1] = val[0]
                 self.gp_b_matrices[igp, 4, i * 3] = val[2]
@@ -90,23 +94,23 @@
         gp_strains = []
         gp_stresses = []
 
         for i in range(gp_number):
             gp_strain = dot(gp_b_matrices[i], element_dof_values)
             gp_dstrain = dot(gp_b_matrices[i], element_ddof_values)
             variable = {'strain': gp_strain, 'dstrain': gp_dstrain}
-            gp_ddsdde, gp_output = self.material_data.get_tangent(variable=variable,
-                                                                  state_variable=gp_state_variables[i],
-                                                                  state_variable_new=gp_state_variables_new[i],
-                                                                  element_id=element_id,
-                                                                  igp=i,
-                                                                  ntens=6,
-                                                                  ndi=3,
-                                                                  nshr=3,
-                                                                  timer=timer)
+            gp_ddsdde, gp_output = self.material_data_list[0].get_tangent(variable=variable,
+                                                                          state_variable=gp_state_variables[i],
+                                                                          state_variable_new=gp_state_variables_new[i],
+                                                                          element_id=element_id,
+                                                                          igp=i,
+                                                                          ntens=6,
+                                                                          ndi=3,
+                                                                          nshr=3,
+                                                                          timer=timer)
             gp_stress = gp_output['stress']
             gp_ddsddes.append(gp_ddsdde)
             gp_strains.append(gp_strain)
             gp_stresses.append(gp_stress)
 
         self.gp_ddsddes = gp_ddsddes
         self.gp_strains = gp_strains
@@ -137,23 +141,23 @@
         for i in range(gp_number):
             gp_weight_times_jacobi_det = gp_weight_times_jacobi_dets[i]
             gp_b_matrix_transpose = gp_b_matrices_transpose[i]
             gp_b_matrix = gp_b_matrices[i]
             gp_strain = dot(gp_b_matrix, element_dof_values)
             gp_dstrain = dot(gp_b_matrix, element_ddof_values)
             variable = {'strain': gp_strain, 'dstrain': gp_dstrain}
-            gp_ddsdde, gp_output = self.material_data.get_tangent(variable=variable,
-                                                                  state_variable=gp_state_variables[i],
-                                                                  state_variable_new=gp_state_variables_new[i],
-                                                                  element_id=element_id,
-                                                                  igp=i,
-                                                                  ntens=6,
-                                                                  ndi=3,
-                                                                  nshr=3,
-                                                                  timer=timer)
+            gp_ddsdde, gp_output = self.material_data_list[0].get_tangent(variable=variable,
+                                                                          state_variable=gp_state_variables[i],
+                                                                          state_variable_new=gp_state_variables_new[i],
+                                                                          element_id=element_id,
+                                                                          igp=i,
+                                                                          ntens=6,
+                                                                          ndi=3,
+                                                                          nshr=3,
+                                                                          timer=timer)
             gp_stress = gp_output['stress']
 
             self.element_stiffness += dot(gp_b_matrix_transpose, dot(gp_ddsdde, gp_b_matrix)) * \
                                       gp_weight_times_jacobi_det
 
             self.element_fint += dot(gp_b_matrix_transpose, gp_stress) * gp_weight_times_jacobi_det
 
@@ -209,8 +213,12 @@
         self.element_average_field_variables['S33'] = average_stress[2]
         self.element_average_field_variables['S12'] = average_stress[3]
         self.element_average_field_variables['S13'] = average_stress[4]
         self.element_average_field_variables['S23'] = average_stress[5]
 
 
 if __name__ == "__main__":
-    pass
+    from pyfem.Job import Job
+
+    job = Job(r'F:\Github\pyfem\examples\1element\hex8\Job-1.toml')
+
+    job.assembly.element_data_list[0].show()
```

### Comparing `pyfem-0.1.0/src/pyfem/elements/get_element_data.py` & `pyfem-0.1.1/src/pyfem/elements/get_element_data.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,48 +1,58 @@
+# -*- coding: utf-8 -*-
+"""
+
+"""
+from typing import List
+
 from numpy import ndarray
 
 from pyfem.elements.BaseElement import BaseElement
 from pyfem.elements.IsoElementShape import IsoElementShape
 from pyfem.elements.SolidPlaneSmallStrain import SolidPlaneSmallStrain
 from pyfem.elements.SolidVolumeSmallStrain import SolidVolumeSmallStrain
+from pyfem.elements.ThermalStatic import ThermalStatic
+from pyfem.elements.SolidThermalPlaneSmallStrain import SolidThermalPlaneSmallStrain
 from pyfem.fem.Timer import Timer
 from pyfem.io.Dof import Dof
 from pyfem.io.Material import Material
 from pyfem.io.Section import Section
 from pyfem.materials.BaseMaterial import BaseMaterial
 from pyfem.utils.colors import error_style
 
 element_data_dict = {
     'SolidPlaneStressSmallStrain': SolidPlaneSmallStrain,
     'SolidPlaneStrainSmallStrain': SolidPlaneSmallStrain,
-    'SolidVolumeSmallStrain': SolidVolumeSmallStrain
+    'SolidVolumeSmallStrain': SolidVolumeSmallStrain,
+    'SolidThermalPlaneStrainSmallStrain': SolidThermalPlaneSmallStrain,
+    'ThermalStatic': ThermalStatic
 }
 
 
 # @trace_calls
 def get_element_data(element_id: int,
                      iso_element_shape: IsoElementShape,
                      connectivity: ndarray,
                      node_coords: ndarray,
                      dof: Dof,
-                     material: Material,
+                     materials: List[Material],
                      section: Section,
-                     material_data: BaseMaterial,
+                     material_data_list: List[BaseMaterial],
                      timer: Timer) -> BaseElement:
     class_name = f'{section.category}{section.type}{section.option}'.strip().replace(' ', '')
 
     if class_name in element_data_dict:
         return element_data_dict[class_name](element_id=element_id,
                                              iso_element_shape=iso_element_shape,
                                              connectivity=connectivity,
                                              node_coords=node_coords,
                                              dof=dof,
-                                             material=material,
+                                             materials=materials,
                                              section=section,
-                                             material_data=material_data,
+                                             material_data_list=material_data_list,
                                              timer=timer)
     else:
         error_msg = f'{class_name} element is not supported.\n'
         error_msg += f'The allowed element types are {list(element_data_dict.keys())}.'
         raise NotImplementedError(error_style(error_msg))
```

### Comparing `pyfem-0.1.0/src/pyfem/elements/get_iso_element_type.py` & `pyfem-0.1.1/src/pyfem/elements/get_iso_element_type.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.0/src/pyfem/fem/Timer.py` & `pyfem-0.1.1/src/pyfem/fem/Timer.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.0/src/pyfem/io/Amplitude.py` & `pyfem-0.1.1/src/pyfem/io/Amplitude.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.0/src/pyfem/io/BC.py` & `pyfem-0.1.1/src/pyfem/io/BC.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.0/src/pyfem/io/Dof.py` & `pyfem-0.1.1/src/pyfem/io/Dof.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.0/src/pyfem/io/Material.py` & `pyfem-0.1.1/src/pyfem/io/Material.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     当 self.is_read_only = True 时：
         1. Material 类的所有属性在首次被赋非None值后不能再被修改和删除，
         2. 此时许可的属性关键字存储在self.slots中。
     """
     is_read_only: bool = True
     slots: Tuple = ('name', 'category', 'type', 'data')
     allowed_keys_values: Dict = {
-        'category': [None, 'Elastic', 'Plastic', 'ViscoElastic'],
+        'category': [None, 'Elastic', 'Plastic', 'ViscoElastic', 'Thermal'],
         'type': [None, 'Isotropic', 'IsotropicHardening', 'KinematicHardening', 'Maxwell']
     }
 
     def __init__(self) -> None:
         self.name: str = None  # type: ignore
         self.category: str = None  # type: ignore
         self.type: str = None  # type: ignore
```

### Comparing `pyfem-0.1.0/src/pyfem/io/Mesh.py` & `pyfem-0.1.1/src/pyfem/io/Mesh.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.0/src/pyfem/io/Output.py` & `pyfem-0.1.1/src/pyfem/io/Output.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.0/src/pyfem/io/Properties.py` & `pyfem-0.1.1/src/pyfem/io/Properties.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.0/src/pyfem/io/Section.py` & `pyfem-0.1.1/src/pyfem/io/Section.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 class Section:
     def __init__(self) -> None:
         self.name: str = None  # type: ignore
         self.category: str = None  # type: ignore
         self.type: str = None  # type: ignore
         self.option: Optional[str] = None
         self.element_sets: List[str] = None  # type: ignore
-        self.material_name: str = None  # type: ignore
+        self.material_names: List[str] = None  # type: ignore
         self.data: List = None  # type: ignore
 
     def to_string(self, level: int = 1) -> str:
         return object_dict_to_string(self, level)
 
     def show(self) -> None:
         print(self.to_string())
```

### Comparing `pyfem-0.1.0/src/pyfem/io/Solver.py` & `pyfem-0.1.1/src/pyfem/io/Solver.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.0/src/pyfem/io/arguments.py` & `pyfem-0.1.1/src/pyfem/io/arguments.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
     # 添加帮助选项
     parser.add_argument('-h', '--help', action='help', default=SUPPRESS,
                         help='Show this help message and exit.')
 
     # 添加版本选项
     parser.add_argument('-v', '--version', action='version', help='Show program\'s version number and exit.',
-                        version='pyfem 0.1.0')
+                        version='pyfem 0.1.1')
 
     # 解析命令行参数
     args = parser.parse_args()
 
     # 如果未指定程序输入文件，则打印帮助并退出
     if not args.i:
         print('--------------------------------------')
```

### Comparing `pyfem-0.1.0/src/pyfem/io/write_vtk.py` & `pyfem-0.1.1/src/pyfem/io/write_vtk.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,39 +22,44 @@
     piece = SubElement(ugrid, "Piece", {
         "NumberOfPoints": str(len(props.mesh_data.nodes)),
         "NumberOfCells": str(len(props.mesh_data.elements))
     })
 
     # 添加节点数据
     point_data = SubElement(piece, "PointData")
-    temp = SubElement(point_data, "DataArray", {
-        "type": "Float64",
-        "Name": "Temperature",
-        "NumberOfComponents": "1",
-        "format": "ascii"
-    })
-    temp.text = ""
-    for _ in props.mesh_data.nodes:
-        temp.text += "0.0\n"  # 在这里添加具体的场量数值
 
-    disp = SubElement(point_data, "DataArray", {
-        "type": "Float64",
-        "Name": "Displacement",
-        "NumberOfComponents": "3",
-        "format": "ascii"
-    })
-    disp.text = ""
-    if dimension == 2:
-        for u1, u2 in assembly.dof_solution.reshape(-1, 2):
-            disp.text += f"{u1} {u2} 0.0 \n"
-    elif dimension == 3:
-        for u1, u2, u3 in assembly.dof_solution.reshape(-1, 3):
-            disp.text += f"{u1} {u2} {u3} \n"
-    else:
-        raise NotImplementedError
+    if "T" in props.dof.names:
+        temp = SubElement(point_data, "DataArray", {
+            "type": "Float64",
+            "Name": "Temperature",
+            "NumberOfComponents": "1",
+            "format": "ascii"
+        })
+        temp.text = ""
+        col_T = props.dof.names.index("T")
+        dof_T = assembly.dof_solution.reshape(-1, len(props.dof.names))[:, col_T]
+        for T in dof_T:
+            temp.text += f"{T} \n"
+
+    if "u1" in props.dof.names:
+        disp = SubElement(point_data, "DataArray", {
+            "type": "Float64",
+            "Name": "Displacement",
+            "NumberOfComponents": "3",
+            "format": "ascii"
+        })
+        disp.text = ""
+        if dimension == 2:
+            for u1, u2 in assembly.dof_solution.reshape(-1, len(props.dof.names))[:, 0:2]:
+                disp.text += f"{u1} {u2} 0.0 \n"
+        elif dimension == 3:
+            for u1, u2, u3 in assembly.dof_solution.reshape(-1, len(props.dof.names))[:, 0:3]:
+                disp.text += f"{u1} {u2} {u3} \n"
+        else:
+            raise NotImplementedError
 
     for field_name, field_values in assembly.field_variables.items():
         field = SubElement(point_data, "DataArray", {
             "type": "Float64",
             "Name": field_name,
             "NumberOfComponents": "1",
             "format": "ascii"
```

### Comparing `pyfem-0.1.0/src/pyfem/materials/BaseMaterial.py` & `pyfem-0.1.1/src/pyfem/materials/BaseMaterial.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 # -*- coding: utf-8 -*-
 """
 
 """
-from typing import Tuple, Dict, Optional
+from typing import Tuple, Dict
 
 from numpy import ndarray, empty
 
 from pyfem.fem.Timer import Timer
 from pyfem.io.Material import Material
+from pyfem.io.Section import Section
 from pyfem.utils.visualization import object_dict_to_string_ndarray
 
 
 class BaseMaterial:
-    def __init__(self, material: Material, dimension: int, option: Optional[str] = None) -> None:
+    def __init__(self, material: Material, dimension: int, section: Section) -> None:
         self.material: Material = material
         self.dimension: int = dimension
-        self.option: Optional[str] = option
+        self.section: Section = section
+        self.allowed_section_types: Tuple = ()
         self.ddsdde: ndarray = empty(0)
         self.output: Dict[str, ndarray] = {}
 
     def to_string(self, level: int = 1) -> str:
         return object_dict_to_string_ndarray(self, level)
 
     def show(self) -> None:
```

### Comparing `pyfem-0.1.0/src/pyfem/materials/ElasticIsotropic.py` & `pyfem-0.1.1/src/pyfem/materials/ElasticIsotropic.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,35 +5,34 @@
 from typing import Optional, Tuple, Dict
 
 from numpy import array, outer, diag, ndarray, dot
 
 from pyfem.fem.Timer import Timer
 from pyfem.fem.constants import DTYPE
 from pyfem.io.Material import Material
+from pyfem.io.Section import Section
 from pyfem.materials.BaseMaterial import BaseMaterial
 from pyfem.utils.colors import error_style
 
 
 class ElasticIsotropic(BaseMaterial):
-    allowed_option = ['Volume', 'PlaneStress', 'PlaneStrain', None]
 
-    def __init__(self, material: Material, dimension: int, option: Optional[str] = None) -> None:
-        super().__init__(material, dimension, option)
+    def __init__(self, material: Material, dimension: int, section: Section) -> None:
+        super().__init__(material, dimension, section)
+        self.allowed_section_types = ('Volume', 'PlaneStress', 'PlaneStrain', None)
         self.create_tangent()
 
     def create_tangent(self):
         young = self.material.data[0]
         poisson = self.material.data[1]
 
-        if self.option in self.allowed_option:
-            if self.dimension == 3:
-                self.option = None
-            self.ddsdde = get_stiffness_from_young_poisson(self.dimension, young, poisson, self.option)
+        if self.section.type in self.allowed_section_types:
+            self.ddsdde = get_stiffness_from_young_poisson(self.dimension, young, poisson, self.section.type)
         else:
-            error_msg = f'{self.option} is not the allowed options {self.allowed_option}'
+            error_msg = f'{self.section.type} is not the allowed section types {self.allowed_section_types} of the material {type(self).__name__}, please check the definition of the section {self.section.name}'
             raise NotImplementedError(error_style(error_msg))
 
     def get_tangent(self, variable: Dict[str, ndarray],
                     state_variable: Dict[str, ndarray],
                     state_variable_new: Dict[str, ndarray],
                     element_id: int,
                     igp: int,
@@ -194,9 +193,9 @@
 
 if __name__ == "__main__":
     from pyfem.io.Properties import Properties
 
     props = Properties()
     props.read_file(r'F:\Github\pyfem\examples\rectangle\rectangle.toml')
 
-    material_data = ElasticIsotropic(props.materials[0], 3)
+    material_data = ElasticIsotropic(props.materials[0], 3, props.sections[0])
     print(material_data.ddsdde.dtype)
```

### Comparing `pyfem-0.1.0/src/pyfem/materials/PlasticKinematicHardening.py` & `pyfem-0.1.1/src/pyfem/materials/PlasticKinematicHardening.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 # -*- coding: utf-8 -*-
 """
 
 """
 from copy import deepcopy
-from typing import Optional, Dict, Tuple
+from typing import Dict, Tuple
 
 from numpy import zeros, ndarray, dot, sqrt, outer, insert, delete
 
 from pyfem.fem.Timer import Timer
 from pyfem.fem.constants import DTYPE
 from pyfem.io.Material import Material
+from pyfem.io.Section import Section
 from pyfem.materials.BaseMaterial import BaseMaterial
 from pyfem.materials.ElasticIsotropic import get_stiffness_from_young_poisson
 from pyfem.utils.colors import error_style
 
 
 class PlasticKinematicHardening(BaseMaterial):
-    allowed_option = ['PlaneStress', 'PlaneStrain', 'Volume', None]
 
-    def __init__(self, material: Material, dimension: int, option: Optional[str] = None) -> None:
-        super().__init__(material, dimension, option)
+    def __init__(self, material: Material, dimension: int, section: Section) -> None:
+        super().__init__(material, dimension, section)
+        self.allowed_section_types = ('PlaneStress', 'PlaneStrain', 'Volume')
         self.young: float = self.material.data[0]
         self.poisson: float = self.material.data[1]
         self.yield_stress: float = self.material.data[2]
         self.hard: float = self.material.data[3]
         self.EBULK3: float = self.young / (1.0 - 2.0 * self.poisson)
         self.EG2: float = self.young / (1.0 + self.poisson)
         self.EG: float = self.EG2 / 2.0
         self.EG3: float = 3.0 * self.EG
         self.ELAM: float = (self.EBULK3 - self.EG2) / 3.0
         self.tolerance: float = 1.0e-10
         self.create_tangent()
 
     def create_tangent(self):
-        if self.option in self.allowed_option:
-            if self.dimension == 3:
-                self.option = None
-            self.ddsdde = get_stiffness_from_young_poisson(self.dimension, self.young, self.poisson, self.option)
+        if self.section.type in self.allowed_section_types:
+            self.ddsdde = get_stiffness_from_young_poisson(self.dimension, self.young, self.poisson, self.section.type)
         else:
-            error_msg = f'{self.option} is not the allowed options {self.allowed_option}'
+            error_msg = f'{self.section.type} is not the allowed section types {self.allowed_section_types} of the material {type(self).__name__}, please check the definition of the section {self.section.name}'
             raise NotImplementedError(error_style(error_msg))
 
     def get_tangent(self, variable: Dict[str, ndarray],
                     state_variable: Dict[str, ndarray],
                     state_variable_new: Dict[str, ndarray],
                     element_id: int,
                     igp: int,
@@ -63,17 +62,17 @@
         stress = deepcopy(state_variable['stress'])
 
         dstrain = variable['dstrain']
 
         E = self.young
         nu = self.poisson
 
-        if self.option == 'PlaneStrain':
+        if self.section.type == 'PlaneStrain':
             dstrain = insert(dstrain, 2, 0)
-        elif self.option == 'PlaneStress':
+        elif self.section.type == 'PlaneStress':
             dstrain = insert(dstrain, 2, -nu / (1 - nu) * (dstrain[0] + dstrain[1]))
 
         elastic_strain += dstrain
 
         ddsdde = zeros((ntens, ntens), dtype=DTYPE)
 
         lam = E * nu / ((1.0 + nu) * (1.0 - 2.0 * nu))
@@ -137,18 +136,18 @@
         #     print(stress)
 
         state_variable_new['elastic_strain'] = elastic_strain
         state_variable_new['plastic_strain'] = plastic_strain
         state_variable_new['back_stress'] = back_stress
         state_variable_new['stress'] = stress
 
-        if self.option == 'PlaneStrain':
+        if self.section.type == 'PlaneStrain':
             ddsdde = delete(delete(ddsdde, 2, axis=0), 2, axis=1)
             stress = delete(stress, 2)
-        elif self.option == 'PlaneStress':
+        elif self.section.type == 'PlaneStress':
             ddsdde = delete(delete(ddsdde, 2, axis=0), 2, axis=1)
             ddsdde[0, 0] -= lam * lam / (lam + 2 * mu)
             ddsdde[0, 1] -= lam * lam / (lam + 2 * mu)
             ddsdde[1, 0] -= lam * lam / (lam + 2 * mu)
             ddsdde[1, 1] -= lam * lam / (lam + 2 * mu)
             stress = delete(stress, 2)
 
@@ -171,8 +170,8 @@
 
 
 if __name__ == "__main__":
     from pyfem.Job import Job
 
     job = Job(r'F:\Github\pyfem\examples\rectangle\rectangle.toml')
 
-    material_data = PlasticKinematicHardening(job.props.materials[0], 3)
+    material_data = PlasticKinematicHardening(job.props.materials[0], 3, job.props.sections[0])
```

### Comparing `pyfem-0.1.0/src/pyfem/materials/ViscoElasticMaxwell.py` & `pyfem-0.1.1/src/pyfem/materials/ViscoElasticMaxwell.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,49 +1,48 @@
 # -*- coding: utf-8 -*-
 """
 
 """
 from copy import deepcopy
-from typing import Optional, Dict, Tuple
+from typing import Dict, Tuple
 
 from numpy import zeros, ndarray, exp
 
 from pyfem.fem.Timer import Timer
 from pyfem.fem.constants import DTYPE
 from pyfem.io.Material import Material
+from pyfem.io.Section import Section
 from pyfem.materials.BaseMaterial import BaseMaterial
 from pyfem.materials.ElasticIsotropic import get_stiffness_from_young_poisson
 from pyfem.utils.colors import error_style
 
 
 class ViscoElasticMaxwell(BaseMaterial):
-    allowed_option = ['PlaneStress', 'PlaneStrain', 'Volume', None]
 
-    def __init__(self, material: Material, dimension: int, option: Optional[str] = None) -> None:
-        super().__init__(material, dimension, option)
+    def __init__(self, material: Material, dimension: int, section: Section) -> None:
+        super().__init__(material, dimension, section)
+        self.allowed_section_types = ('PlaneStress', 'PlaneStrain', 'Volume')
         self.E0: float = self.material.data[0]
         self.E1: float = self.material.data[1]
         self.E2: float = self.material.data[2]
         self.E3: float = self.material.data[3]
         self.TAU1: float = self.material.data[4]
         self.TAU2: float = self.material.data[5]
         self.TAU3: float = self.material.data[6]
         self.POISSON: float = self.material.data[7]
         self.create_tangent()
 
     def create_tangent(self):
         young = self.material.data[0]
         poisson = self.material.data[1]
 
-        if self.option in self.allowed_option:
-            if self.dimension == 3:
-                self.option = None
-            self.ddsdde = get_stiffness_from_young_poisson(self.dimension, young, poisson, self.option)
+        if self.section.type in self.allowed_section_types:
+            self.ddsdde = get_stiffness_from_young_poisson(self.dimension, young, poisson, self.section.type)
         else:
-            error_msg = f'{self.option} is not the allowed options {self.allowed_option}'
+            error_msg = f'{self.section.type} is not the allowed section types {self.allowed_section_types} of the material {type(self).__name__}, please check the definition of the section {self.section.name}'
             raise NotImplementedError(error_style(error_msg))
 
     def get_tangent(self, variable: Dict[str, ndarray],
                     state_variable: Dict[str, ndarray],
                     state_variable_new: Dict[str, ndarray],
                     element_id: int,
                     igp: int,
@@ -145,9 +144,9 @@
 
 
 if __name__ == "__main__":
     from pyfem.Job import Job
 
     job = Job(r'F:\Github\pyfem\examples\specimen3D\Job-1.toml')
 
-    material_data = ViscoElasticMaxwell(job.props.materials[2], 3)
+    material_data = ViscoElasticMaxwell(job.props.materials[2], 3, job.props.sections[0])
     print(material_data.to_string())
```

### Comparing `pyfem-0.1.0/src/pyfem/materials/get_material_data.py` & `pyfem-0.1.1/src/pyfem/materials/get_material_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 # -*- coding: utf-8 -*-
 """
 
 """
-from typing import Optional
 
 from pyfem.io.Material import Material
+from pyfem.io.Section import Section
 from pyfem.materials.BaseMaterial import BaseMaterial
 from pyfem.materials.ElasticIsotropic import ElasticIsotropic
 from pyfem.materials.PlasticKinematicHardening import PlasticKinematicHardening
+from pyfem.materials.ThermalIsotropic import ThermalIsotropic
 from pyfem.materials.ViscoElasticMaxwell import ViscoElasticMaxwell
 from pyfem.utils.colors import error_style
 
 material_data_dict = {
     'ElasticIsotropic': ElasticIsotropic,
     'PlasticKinematicHardening': PlasticKinematicHardening,
-    'ViscoElasticMaxwell': ViscoElasticMaxwell
+    'ViscoElasticMaxwell': ViscoElasticMaxwell,
+    'ThermalIsotropic': ThermalIsotropic
+
 }
 
 
-def get_material_data(material: Material, dimension: int, option: Optional[str] = None) -> BaseMaterial:
+def get_material_data(material: Material, dimension: int, section: Section) -> BaseMaterial:
     class_name = f'{material.category}{material.type}'.strip().replace(' ', '')
 
     if class_name in material_data_dict:
-        return material_data_dict[class_name](material, dimension, option)
+        return material_data_dict[class_name](material, dimension, section)
     else:
         error_msg = f'{class_name} material is not supported.\n'
         error_msg += f'The allowed material types are {list(material_data_dict.keys())}.'
         raise NotImplementedError(error_style(error_msg))
 
 
 if __name__ == "__main__":
     from pyfem.io.Properties import Properties
 
     props = Properties()
     props.read_file(r'F:\Github\pyfem\examples\rectangle\rectangle.toml')
 
-    material_data = get_material_data(props.materials[0], 3)
+    material_data = get_material_data(props.materials[0], 3, props.sections[0])
 
     print(material_data.to_string())
```

### Comparing `pyfem-0.1.0/src/pyfem/mesh/ElementSet.py` & `pyfem-0.1.1/src/pyfem/mesh/ElementSet.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.0/src/pyfem/mesh/MeshData.py` & `pyfem-0.1.1/src/pyfem/mesh/MeshData.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.0/src/pyfem/mesh/NodeSet.py` & `pyfem-0.1.1/src/pyfem/mesh/NodeSet.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.0/src/pyfem/solvers/BaseSolver.py` & `pyfem-0.1.1/src/pyfem/solvers/BaseSolver.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.0/src/pyfem/solvers/LinearSolver.py` & `pyfem-0.1.1/src/pyfem/solvers/LinearSolver.py`

 * *Files 24% similar despite different names*

```diff
@@ -24,22 +24,27 @@
         self.solve()
 
     def solve(self) -> None:
         A = self.assembly.global_stiffness
         rhs = self.assembly.fext
 
         for bc_data in self.assembly.bc_data_list:
-            for dof_id, dof_value in zip(bc_data.dof_ids, bc_data.dof_values):
-                A[dof_id, dof_id] += self.PENALTY
-                rhs[dof_id] += dof_value * self.PENALTY
+            if bc_data.bc.category == 'DirichletBC':
+                for dof_id, dof_value in zip(bc_data.dof_ids, bc_data.dof_values):
+                    A[dof_id, dof_id] += self.PENALTY
+                    rhs[dof_id] += dof_value * self.PENALTY
+            elif bc_data.bc.category == 'NeumannBC':
+                for dof_id, fext in zip(bc_data.dof_ids, bc_data.bc_fext):
+                    rhs[dof_id] += fext
 
         x = spsolve(A, rhs)
+
         self.dof_solution = x
         self.assembly.dof_solution = x
-        self.assembly.update_element_data_without_stiffness()
+        self.assembly.update_element_data()
         self.assembly.update_element_field_variables()
         self.assembly.assembly_field_variables()
         write_vtk(self.assembly)
 
 
 if __name__ == "__main__":
     pass
```

### Comparing `pyfem-0.1.0/src/pyfem/solvers/NonlinearSolver.py` & `pyfem-0.1.1/src/pyfem/solvers/NonlinearSolver.py`

 * *Files 9% similar despite different names*

```diff
@@ -57,36 +57,42 @@
             is_convergence = False
             for niter in range(self.MAX_NITER):
                 self.assembly.assembly_global_stiffness()
                 fint = self.assembly.fint
                 rhs = deepcopy(self.assembly.fext)
                 if niter == 0:
                     for bc_data in self.assembly.bc_data_list:
-                        for dof_id, dof_value in zip(bc_data.dof_ids, bc_data.dof_values):
-                            self.assembly.global_stiffness[dof_id, dof_id] += self.PENALTY
-                            rhs[dof_id] += dof_value * (bc_data.get_amplitude(timer.time1) - bc_data.get_amplitude(
-                                timer.time0)) * self.PENALTY
+                        amplitude_increment = bc_data.get_amplitude(timer.time1) - bc_data.get_amplitude(timer.time0)
+                        if bc_data.bc.category == 'DirichletBC':
+                            for dof_id, dof_value in zip(bc_data.dof_ids, bc_data.dof_values):
+                                self.assembly.global_stiffness[dof_id, dof_id] += self.PENALTY
+                                rhs[dof_id] += dof_value * self.PENALTY * amplitude_increment
+                        elif bc_data.bc.category == 'NeumannBC':
+                            for dof_id, fext in zip(bc_data.dof_ids, bc_data.bc_fext):
+                                rhs[dof_id] += fext * amplitude_increment
+                                self.assembly.fext[dof_id] += fext * amplitude_increment
                 else:
                     for bc_data in self.assembly.bc_data_list:
-                        for dof_id, dof_value in zip(bc_data.dof_ids, bc_data.dof_values):
-                            self.assembly.global_stiffness[dof_id, dof_id] += self.PENALTY
-                            rhs[dof_id] = 0.0 * self.PENALTY
+                        if bc_data.bc.category == 'DirichletBC':
+                            for dof_id, dof_value in zip(bc_data.dof_ids, bc_data.dof_values):
+                                self.assembly.global_stiffness[dof_id, dof_id] += self.PENALTY
+                                rhs[dof_id] = 0.0 * self.PENALTY
 
                 LU = splu(self.assembly.global_stiffness)
                 da = LU.solve(rhs - fint)
 
                 self.assembly.ddof_solution += da
                 self.assembly.update_element_data()
                 self.assembly.assembly_fint()
 
                 f_residual = self.assembly.fext - self.assembly.fint
                 f_residual[self.assembly.bc_dof_ids] = 0
                 f_residual = norm(f_residual)
 
-                print(f'  niter = {niter}, force residual = {f_residual}')
+                print(f'  niter = {niter}, residual = {f_residual}')
 
                 if f_residual < self.FORCE_TOL:
                     is_convergence = True
                     break
 
             if is_convergence:
                 self.assembly.dof_solution += self.assembly.ddof_solution
@@ -106,14 +112,15 @@
                 write_pvd(self.assembly)
                 break
 
         if not timer.is_done():
             raise NotImplementedError(error_style('maximum increment is reached'))
 
     def initial_tangent_solve(self) -> None:
+        self.MAX_NITER = 1024
         timer = self.assembly.timer
 
         timer.total_time = self.solver.total_time
         timer.dtime = self.solver.initial_dtime
         timer.time0 = self.solver.start_time
         timer.increment = 0
         timer.frame_ids.append(0)
@@ -134,25 +141,31 @@
             is_convergence = False
             for niter in range(self.MAX_NITER):
                 if niter == 0:
                     self.assembly.assembly_global_stiffness()
                     fint = self.assembly.fint
                     rhs = deepcopy(self.assembly.fext)
                     for bc_data in self.assembly.bc_data_list:
-                        for dof_id, dof_value in zip(bc_data.dof_ids, bc_data.dof_values):
-                            self.assembly.global_stiffness[dof_id, dof_id] += self.PENALTY
-                            rhs[dof_id] += dof_value * (bc_data.get_amplitude(timer.time1) - bc_data.get_amplitude(
-                                timer.time0)) * self.PENALTY
+                        amplitude_increment = bc_data.get_amplitude(timer.time1) - bc_data.get_amplitude(timer.time0)
+                        if bc_data.bc.category == 'DirichletBC':
+                            for dof_id, dof_value in zip(bc_data.dof_ids, bc_data.dof_values):
+                                self.assembly.global_stiffness[dof_id, dof_id] += self.PENALTY
+                                rhs[dof_id] += dof_value * self.PENALTY * amplitude_increment
+                        elif bc_data.bc.category == 'NeumannBC':
+                            for dof_id, fext in zip(bc_data.dof_ids, bc_data.bc_fext):
+                                rhs[dof_id] += fext * amplitude_increment
+                                self.assembly.fext[dof_id] += fext * amplitude_increment
                     LU = splu(self.assembly.global_stiffness)
                 else:
                     fint = self.assembly.fint
                     rhs = deepcopy(self.assembly.fext)
                     for bc_data in self.assembly.bc_data_list:
-                        for dof_id, dof_value in zip(bc_data.dof_ids, bc_data.dof_values):
-                            rhs[dof_id] = 0.0 * self.PENALTY
+                        if bc_data.bc.category == 'DirichletBC':
+                            for dof_id, dof_value in zip(bc_data.dof_ids, bc_data.dof_values):
+                                rhs[dof_id] = 0.0 * self.PENALTY
 
                 da = LU.solve(rhs - fint)
 
                 self.assembly.ddof_solution += da
                 self.assembly.update_element_data_without_stiffness()
                 self.assembly.assembly_fint()
```

### Comparing `pyfem-0.1.0/src/pyfem/solvers/get_solver_data.py` & `pyfem-0.1.1/src/pyfem/solvers/get_solver_data.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.0/src/pyfem/utils/IntKeyDict.py` & `pyfem-0.1.1/src/pyfem/utils/IntKeyDict.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.0/src/pyfem/utils/colors.py` & `pyfem-0.1.1/src/pyfem/utils/colors.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.0/src/pyfem/utils/logger.py` & `pyfem-0.1.1/src/pyfem/utils/logger.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.0/src/pyfem/utils/visualization.py` & `pyfem-0.1.1/src/pyfem/utils/visualization.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.0/src/pyfem/utils/wrappers.py` & `pyfem-0.1.1/src/pyfem/utils/wrappers.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.0/src/pyfem.egg-info/SOURCES.txt` & `pyfem-0.1.1/src/pyfem.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -15,21 +15,25 @@
 src/pyfem/amplitude/__init__.py
 src/pyfem/amplitude/get_amplitude_data.py
 src/pyfem/assembly/Assembly.py
 src/pyfem/assembly/__init__.py
 src/pyfem/bc/BaseBC.py
 src/pyfem/bc/DirichletBC.py
 src/pyfem/bc/NeumannBC.py
+src/pyfem/bc/NeumannBCConcentrated.py
+src/pyfem/bc/NeumannBCDistributed.py
 src/pyfem/bc/__init__.py
 src/pyfem/bc/get_bc_data.py
 src/pyfem/elements/BaseElement.py
 src/pyfem/elements/IsoElementDiagram.py
 src/pyfem/elements/IsoElementShape.py
 src/pyfem/elements/SolidPlaneSmallStrain.py
+src/pyfem/elements/SolidThermalPlaneSmallStrain.py
 src/pyfem/elements/SolidVolumeSmallStrain.py
+src/pyfem/elements/ThermalStatic.py
 src/pyfem/elements/__init__.py
 src/pyfem/elements/get_element_data.py
 src/pyfem/elements/get_iso_element_type.py
 src/pyfem/fem/Timer.py
 src/pyfem/fem/__init__.py
 src/pyfem/fem/constants.py
 src/pyfem/io/Amplitude.py
@@ -42,16 +46,16 @@
 src/pyfem/io/Section.py
 src/pyfem/io/Solver.py
 src/pyfem/io/__init__.py
 src/pyfem/io/arguments.py
 src/pyfem/io/write_vtk.py
 src/pyfem/materials/BaseMaterial.py
 src/pyfem/materials/ElasticIsotropic.py
-src/pyfem/materials/PlasticIsotropicHardening.py
 src/pyfem/materials/PlasticKinematicHardening.py
+src/pyfem/materials/ThermalIsotropic.py
 src/pyfem/materials/ViscoElasticMaxwell.py
 src/pyfem/materials/__init__.py
 src/pyfem/materials/get_material_data.py
 src/pyfem/mesh/ElementSet.py
 src/pyfem/mesh/MeshData.py
 src/pyfem/mesh/NodeSet.py
 src/pyfem/mesh/__init__.py
```

