# Comparing `tmp/raven-hydro-0.2.2.tar.gz` & `tmp/raven-hydro-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raven-hydro-0.2.2.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "raven-hydro-0.2.3.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `raven-hydro-0.2.2.tar` & `raven-hydro-0.2.3.tar`

### file list

```diff
@@ -1,190 +1,191 @@
--rw-r--r--   0        0        0      775 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/CHANGES.md
--rw-r--r--   0        0        0     3806 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/CMakeLists.txt
--rw-r--r--   0        0        0    11357 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/LICENSE
--rw-r--r--   0        0        0     2927 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/README.md
--rw-r--r--   0        0        0    12965 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/Abstraction.cpp
--rw-r--r--   0        0        0    11990 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/Advection.cpp
--rw-r--r--   0        0        0     1746 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/Advection.h
--rw-r--r--   0        0        0     2165 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/Albedo.h
--rw-r--r--   0        0        0     8416 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/Assimilate.cpp
--rw-r--r--   0        0        0    11198 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/Baseflow.cpp
--rw-r--r--   0        0        0      617 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/CMakeLists.txt
--rw-r--r--   0        0        0     7519 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/CapillaryRise.cpp
--rw-r--r--   0        0        0    24490 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/ChannelXSect.cpp
--rw-r--r--   0        0        0     5697 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/ChannelXSect.h
--rw-r--r--   0        0        0    10679 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/ChemEquilibrium.cpp
--rw-r--r--   0        0        0     2395 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/ChemEquilibrium.h
--rw-r--r--   0        0        0    68775 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/CommonFunctions.cpp
--rw-r--r--   0        0        0    71919 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/ConstituentModel.cpp
--rw-r--r--   0        0        0    12185 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/ControlStructures.cpp
--rw-r--r--   0        0        0     5046 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/ControlStructures.h
--rw-r--r--   0        0        0    10145 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/Convolution.cpp
--rw-r--r--   0        0        0     2583 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/Convolution.h
--rw-r--r--   0        0        0     6013 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/CropGrowth.cpp
--rw-r--r--   0        0        0     2050 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/CropGrowth.h
--rw-r--r--   0        0        0    55277 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/CustomOutput.cpp
--rw-r--r--   0        0        0     5910 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/CustomOutput.h
--rw-r--r--   0        0        0     8166 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/DDS.cpp
--rw-r--r--   0        0        0     8645 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/Decay.cpp
--rw-r--r--   0        0        0     4226 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/Decay.h
--rw-r--r--   0        0        0    16629 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/DepressionProcesses.cpp
--rw-r--r--   0        0        0     7273 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/DepressionProcesses.h
--rw-r--r--   0        0        0    44012 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/Diagnostics.cpp
--rw-r--r--   0        0        0     3113 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/Diagnostics.h
--rw-r--r--   0        0        0     9601 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/Drain.cpp
--rw-r--r--   0        0        0    30269 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/EnKF.cpp
--rw-r--r--   0        0        0     5284 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/EnKF.h
--rw-r--r--   0        0        0    42139 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/EnergyTransport.cpp
--rw-r--r--   0        0        0     4187 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/EnergyTransport.h
--rw-r--r--   0        0        0    34784 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/Evaporation.cpp
--rw-r--r--   0        0        0    16920 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/Flush.cpp
--rw-r--r--   0        0        0    96136 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/ForcingGrid.cpp
--rw-r--r--   0        0        0    20420 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/ForcingGrid.h
--rw-r--r--   0        0        0    13931 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/Forcings.cpp
--rw-r--r--   0        0        0      837 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/Forcings.h
--rw-r--r--   0        0        0     8865 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/GWRecharge.cpp
--rw-r--r--   0        0        0     8457 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/GWRiverConnection.cpp
--rw-r--r--   0        0        0     2505 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/GWRiverConnection.h
--rw-r--r--   0        0        0     6035 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/GWSWProcessABC.cpp
--rw-r--r--   0        0        0     7304 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/GWSWProcesses.h
--rw-r--r--   0        0        0    29447 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/Gauge.cpp
--rw-r--r--   0        0        0     4413 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/Gauge.h
--rw-r--r--   0        0        0    19634 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/GlacierProcesses.cpp
--rw-r--r--   0        0        0     5759 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/GlacierProcesses.h
--rw-r--r--   0        0        0    35310 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/GlobalParams.cpp
--rw-r--r--   0        0        0     1515 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/GlobalParams.h
--rw-r--r--   0        0        0    11375 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/GreenAmpt.cpp
--rw-r--r--   0        0        0    26381 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/GroundwaterModel.cpp
--rw-r--r--   0        0        0     7330 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/GroundwaterModel.h
--rw-r--r--   0        0        0     7097 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/HRUGroups.cpp
--rw-r--r--   0        0        0    33976 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/HeatConduction.cpp
--rw-r--r--   0        0        0     2424 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/HeatConduction.h
--rw-r--r--   0        0        0    13285 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/HydroProcessABC.cpp
--rw-r--r--   0        0        0    10650 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/HydroProcessABC.h
--rw-r--r--   0        0        0    26942 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/HydroUnits.cpp
--rw-r--r--   0        0        0    10470 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/HydroUnits.h
--rw-r--r--   0        0        0    30286 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/Infiltration.cpp
--rw-r--r--   0        0        0     5021 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/Infiltration.h
--rw-r--r--   0        0        0     6072 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/Interflow.cpp
--rw-r--r--   0        0        0    12899 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/IrregularTimeSeries.cpp
--rw-r--r--   0        0        0     2826 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/IrregularTimeSeries.h
--rw-r--r--   0        0        0     9560 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/IsotopeTransport.cpp
--rw-r--r--   0        0        0     2107 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/IsotopeTransport.h
--rw-r--r--   0        0        0     8894 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/LICENSE
--rw-r--r--   0        0        0    35963 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/LandUseClass.cpp
--rw-r--r--   0        0        0     8750 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/LatAdvection.cpp
--rw-r--r--   0        0        0     2347 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/LatAdvection.h
--rw-r--r--   0        0        0     8135 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/LatEquilibrate.cpp
--rw-r--r--   0        0        0     7403 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/LatFlush.cpp
--rw-r--r--   0        0        0     5006 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/LateralExchangeABC.cpp
--rw-r--r--   0        0        0     6255 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/LateralExchangeABC.h
--rw-r--r--   0        0        0     2619 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/MFUSGpp.h
--rw-r--r--   0        0        0     1686 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/Makefile
--rw-r--r--   0        0        0     4222 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/MassLoading.cpp
--rw-r--r--   0        0        0     1669 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/MassLoading.h
--rw-r--r--   0        0        0    19552 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/MassRouting.cpp
--rw-r--r--   0        0        0     9887 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/Matrix.cpp
--rw-r--r--   0        0        0     2116 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/Matrix.h
--rw-r--r--   0        0        0    87437 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/Model.cpp
--rw-r--r--   0        0        0    28581 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/Model.h
--rw-r--r--   0        0        0     2239 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/ModelABC.h
--rw-r--r--   0        0        0    11343 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/ModelEnsemble.cpp
--rw-r--r--   0        0        0     5613 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/ModelEnsemble.h
--rw-r--r--   0        0        0    21465 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/ModelForcingGrids.cpp
--rw-r--r--   0        0        0    42327 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/ModelInitialize.cpp
--rw-r--r--   0        0        0    22130 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/ModelParamCheck.cpp
--rw-r--r--   0        0        0     8426 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/NetCDFReading.cpp
--rw-r--r--   0        0        0    13784 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/OpenWaterEvap.cpp
--rw-r--r--   0        0        0     3907 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/OpenWaterEvap.h
--rw-r--r--   0        0        0    16192 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/OrographicCorrections.cpp
--rw-r--r--   0        0        0    21426 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/ParseEnsembleFile.cpp
--rw-r--r--   0        0        0    40256 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/ParseFEWSRunInfo.cpp
--rw-r--r--   0        0        0    24336 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/ParseGWFile.cpp
--rw-r--r--   0        0        0    77416 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/ParseHRUFile.cpp
--rw-r--r--   0        0        0    36988 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/ParseInitialConditionFile.cpp
--rw-r--r--   0        0        0   176245 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/ParseInput.cpp
--rw-r--r--   0        0        0    16151 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/ParseLib.cpp
--rw-r--r--   0        0        0     5360 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/ParseLib.h
--rw-r--r--   0        0        0    10720 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/ParseLiveFile.cpp
--rw-r--r--   0        0        0    85505 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/ParsePropertyFile.cpp
--rw-r--r--   0        0        0    90860 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/ParseTimeSeriesFile.cpp
--rw-r--r--   0        0        0    13942 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/PartitionPrecip.cpp
--rw-r--r--   0        0        0    14242 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/Percolation.cpp
--rw-r--r--   0        0        0    13184 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/PotentialMelt.cpp
--rw-r--r--   0        0        0    34140 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/PrairieSnow.cpp
--rw-r--r--   0        0        0     4125 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/PrairieSnow.h
--rw-r--r--   0        0        0     1689 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/Precipitation.h
--rw-r--r--   0        0        0     7899 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/ProcessGroup.cpp
--rw-r--r--   0        0        0     2155 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/ProcessGroup.h
--rw-r--r--   0        0        0    28673 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/Properties.h
--rw-r--r--   0        0        0      702 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/README_compile_RAVEN_on_ECCC_Pegasus.dat
--rw-r--r--   0        0        0    46280 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/Radiation.cpp
--rw-r--r--   0        0        0     7442 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/Radiation.h
--rw-r--r--   0        0        0     1577 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/Raven.rc
--rw-r--r--   0        0        0     2939 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/Raven.sln
--rw-r--r--   0        0        0    68381 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/Raven.vcxproj
--rw-r--r--   0        0        0    26631 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/Raven.vcxproj.filters
--rw-r--r--   0        0        0     5013 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/Raven.vcxproj.user
--rw-r--r--   0        0        0     8826 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/RavenAlgParams.dat
--rw-r--r--   0        0        0      788 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/RavenIcon.ico
--rw-r--r--   0        0        0    89872 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/RavenInclude.h
--rw-r--r--   0        0        0    17151 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/RavenMain.cpp
--rw-r--r--   0        0        0    10763 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/RavenParameters.dat
--rw-r--r--   0        0        0    10652 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/RavenProcessConnections.dat
--rw-r--r--   0        0        0     7768 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/Recharge.cpp
--rw-r--r--   0        0        0    60879 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/Reservoir.cpp
--rw-r--r--   0        0        0    16067 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/Reservoir.h
--rw-r--r--   0        0        0     2141 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/RiverReach.cpp
--rw-r--r--   0        0        0     2693 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/RiverReach.h
--rw-r--r--   0        0        0    10887 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/SnowAlbedo.cpp
--rw-r--r--   0        0        0    53462 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/SnowBalance.cpp
--rw-r--r--   0        0        0    14916 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/SnowMeltRefreeze.cpp
--rw-r--r--   0        0        0    11769 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/SnowMovers.h
--rw-r--r--   0        0        0     7106 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/SnowParams.cpp
--rw-r--r--   0        0        0     5620 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/SnowTempEvolve.cpp
--rw-r--r--   0        0        0    11922 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/SoilAndLandClasses.h
--rw-r--r--   0        0        0    15711 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/SoilBalance.cpp
--rw-r--r--   0        0        0    34296 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/SoilClass.cpp
--rw-r--r--   0        0        0    28725 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/SoilEvaporation.cpp
--rw-r--r--   0        0        0     2942 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/SoilParams.cpp
--rw-r--r--   0        0        0     8318 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/SoilProfile.cpp
--rw-r--r--   0        0        0     2300 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/SoilProfile.h
--rw-r--r--   0        0        0    17486 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/SoilWaterMovers.h
--rw-r--r--   0        0        0    25666 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/Solvers.cpp
--rw-r--r--   0        0        0    56161 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/SparseMatrix.cpp
--rw-r--r--   0        0        0     6580 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/SparseMatrix.h
--rw-r--r--   0        0        0     6346 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/StageDischargeRelations.cpp
--rw-r--r--   0        0        0     5566 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/StageDischargeRelations.h
--rw-r--r--   0        0        0   116678 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/StandardOutput.cpp
--rw-r--r--   0        0        0    25554 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/StateVariables.cpp
--rw-r--r--   0        0        0     1710 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/StateVariables.h
--rw-r--r--   0        0        0    92302 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/SubBasin.cpp
--rw-r--r--   0        0        0    20286 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/SubBasin.h
--rw-r--r--   0        0        0     7327 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/SubbasinGroups.cpp
--rw-r--r--   0        0        0    10813 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/Sublimation.cpp
--rw-r--r--   0        0        0    12501 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/SurfaceEnergyExchange.cpp
--rw-r--r--   0        0        0     1846 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/SurfaceEnergyExchange.h
--rw-r--r--   0        0        0     8662 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/TerrainClass.cpp
--rw-r--r--   0        0        0    70195 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/TimeSeries.cpp
--rw-r--r--   0        0        0     9410 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/TimeSeries.h
--rw-r--r--   0        0        0     3499 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/TimeSeriesABC.cpp
--rw-r--r--   0        0        0     2716 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/TimeSeriesABC.h
--rw-r--r--   0        0        0     9826 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/Transformation.cpp
--rw-r--r--   0        0        0     3806 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/TransientParam.cpp
--rw-r--r--   0        0        0     1931 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/TransientParam.h
--rw-r--r--   0        0        0    35222 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/Transport.cpp
--rw-r--r--   0        0        0    18604 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/Transport.h
--rw-r--r--   0        0        0    11447 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/UTM_to_LatLong.cpp
--rw-r--r--   0        0        0    23443 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/UnitTesting.cpp
--rw-r--r--   0        0        0      711 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/UnitTesting.h
--rw-r--r--   0        0        0    47103 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/UpdateForcings.cpp
--rw-r--r--   0        0        0    26426 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/VegetationClass.cpp
--rw-r--r--   0        0        0    20293 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/VegetationMovers.cpp
--rw-r--r--   0        0        0     5226 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/VegetationMovers.h
--rw-r--r--   0        0        0    18294 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/VegetationParams.cpp
--rw-r--r--   0        0        0      432 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/build/_deps/raven-src/resource.h
--rw-r--r--   0        0        0     7956 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/helpers/FindNetCDF.cmake
--rw-r--r--   0        0        0     2651 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      459 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/src/main.cpp
--rw-r--r--   0        0        0      727 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/src/raven_hydro/__init__.py
--rw-r--r--   0        0        0    16882 2022-11-09 12:37:21.000000 raven-hydro-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      127 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/AUTHORS.md
+-rw-r--r--   0        0        0      900 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/CHANGES.md
+-rw-r--r--   0        0        0     3821 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/CMakeLists.txt
+-rw-r--r--   0        0        0    11357 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/LICENSE
+-rw-r--r--   0        0        0     3075 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/README.md
+-rw-r--r--   0        0        0    12965 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/Abstraction.cpp
+-rw-r--r--   0        0        0    11990 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/Advection.cpp
+-rw-r--r--   0        0        0     1746 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/Advection.h
+-rw-r--r--   0        0        0     2165 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/Albedo.h
+-rw-r--r--   0        0        0     8416 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/Assimilate.cpp
+-rw-r--r--   0        0        0    11198 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/Baseflow.cpp
+-rw-r--r--   0        0        0      617 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/CMakeLists.txt
+-rw-r--r--   0        0        0     7519 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/CapillaryRise.cpp
+-rw-r--r--   0        0        0    24490 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/ChannelXSect.cpp
+-rw-r--r--   0        0        0     5697 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/ChannelXSect.h
+-rw-r--r--   0        0        0    10679 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/ChemEquilibrium.cpp
+-rw-r--r--   0        0        0     2395 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/ChemEquilibrium.h
+-rw-r--r--   0        0        0    68775 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/CommonFunctions.cpp
+-rw-r--r--   0        0        0    71919 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/ConstituentModel.cpp
+-rw-r--r--   0        0        0    12185 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/ControlStructures.cpp
+-rw-r--r--   0        0        0     5046 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/ControlStructures.h
+-rw-r--r--   0        0        0    10145 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/Convolution.cpp
+-rw-r--r--   0        0        0     2583 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/Convolution.h
+-rw-r--r--   0        0        0     6013 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/CropGrowth.cpp
+-rw-r--r--   0        0        0     2050 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/CropGrowth.h
+-rw-r--r--   0        0        0    55277 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/CustomOutput.cpp
+-rw-r--r--   0        0        0     5910 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/CustomOutput.h
+-rw-r--r--   0        0        0     8166 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/DDS.cpp
+-rw-r--r--   0        0        0     8645 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/Decay.cpp
+-rw-r--r--   0        0        0     4226 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/Decay.h
+-rw-r--r--   0        0        0    16629 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/DepressionProcesses.cpp
+-rw-r--r--   0        0        0     7273 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/DepressionProcesses.h
+-rw-r--r--   0        0        0    44012 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/Diagnostics.cpp
+-rw-r--r--   0        0        0     3113 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/Diagnostics.h
+-rw-r--r--   0        0        0     9601 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/Drain.cpp
+-rw-r--r--   0        0        0    30269 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/EnKF.cpp
+-rw-r--r--   0        0        0     5284 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/EnKF.h
+-rw-r--r--   0        0        0    42139 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/EnergyTransport.cpp
+-rw-r--r--   0        0        0     4187 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/EnergyTransport.h
+-rw-r--r--   0        0        0    34784 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/Evaporation.cpp
+-rw-r--r--   0        0        0    16920 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/Flush.cpp
+-rw-r--r--   0        0        0    96136 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/ForcingGrid.cpp
+-rw-r--r--   0        0        0    20420 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/ForcingGrid.h
+-rw-r--r--   0        0        0    13931 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/Forcings.cpp
+-rw-r--r--   0        0        0      837 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/Forcings.h
+-rw-r--r--   0        0        0     8865 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/GWRecharge.cpp
+-rw-r--r--   0        0        0     8457 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/GWRiverConnection.cpp
+-rw-r--r--   0        0        0     2505 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/GWRiverConnection.h
+-rw-r--r--   0        0        0     6035 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/GWSWProcessABC.cpp
+-rw-r--r--   0        0        0     7304 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/GWSWProcesses.h
+-rw-r--r--   0        0        0    29447 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/Gauge.cpp
+-rw-r--r--   0        0        0     4413 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/Gauge.h
+-rw-r--r--   0        0        0    19634 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/GlacierProcesses.cpp
+-rw-r--r--   0        0        0     5759 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/GlacierProcesses.h
+-rw-r--r--   0        0        0    35310 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/GlobalParams.cpp
+-rw-r--r--   0        0        0     1515 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/GlobalParams.h
+-rw-r--r--   0        0        0    11375 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/GreenAmpt.cpp
+-rw-r--r--   0        0        0    26381 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/GroundwaterModel.cpp
+-rw-r--r--   0        0        0     7330 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/GroundwaterModel.h
+-rw-r--r--   0        0        0     7097 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/HRUGroups.cpp
+-rw-r--r--   0        0        0    33976 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/HeatConduction.cpp
+-rw-r--r--   0        0        0     2424 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/HeatConduction.h
+-rw-r--r--   0        0        0    13285 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/HydroProcessABC.cpp
+-rw-r--r--   0        0        0    10650 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/HydroProcessABC.h
+-rw-r--r--   0        0        0    26942 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/HydroUnits.cpp
+-rw-r--r--   0        0        0    10470 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/HydroUnits.h
+-rw-r--r--   0        0        0    30286 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/Infiltration.cpp
+-rw-r--r--   0        0        0     5021 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/Infiltration.h
+-rw-r--r--   0        0        0     6072 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/Interflow.cpp
+-rw-r--r--   0        0        0    12899 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/IrregularTimeSeries.cpp
+-rw-r--r--   0        0        0     2826 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/IrregularTimeSeries.h
+-rw-r--r--   0        0        0     9560 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/IsotopeTransport.cpp
+-rw-r--r--   0        0        0     2107 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/IsotopeTransport.h
+-rw-r--r--   0        0        0     8894 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/LICENSE
+-rw-r--r--   0        0        0    35963 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/LandUseClass.cpp
+-rw-r--r--   0        0        0     8750 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/LatAdvection.cpp
+-rw-r--r--   0        0        0     2347 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/LatAdvection.h
+-rw-r--r--   0        0        0     8135 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/LatEquilibrate.cpp
+-rw-r--r--   0        0        0     7403 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/LatFlush.cpp
+-rw-r--r--   0        0        0     5006 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/LateralExchangeABC.cpp
+-rw-r--r--   0        0        0     6255 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/LateralExchangeABC.h
+-rw-r--r--   0        0        0     2619 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/MFUSGpp.h
+-rw-r--r--   0        0        0     1686 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/Makefile
+-rw-r--r--   0        0        0     4222 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/MassLoading.cpp
+-rw-r--r--   0        0        0     1669 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/MassLoading.h
+-rw-r--r--   0        0        0    19552 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/MassRouting.cpp
+-rw-r--r--   0        0        0     9887 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/Matrix.cpp
+-rw-r--r--   0        0        0     2116 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/Matrix.h
+-rw-r--r--   0        0        0    87437 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/Model.cpp
+-rw-r--r--   0        0        0    28581 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/Model.h
+-rw-r--r--   0        0        0     2239 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/ModelABC.h
+-rw-r--r--   0        0        0    11343 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/ModelEnsemble.cpp
+-rw-r--r--   0        0        0     5613 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/ModelEnsemble.h
+-rw-r--r--   0        0        0    21465 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/ModelForcingGrids.cpp
+-rw-r--r--   0        0        0    42327 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/ModelInitialize.cpp
+-rw-r--r--   0        0        0    22130 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/ModelParamCheck.cpp
+-rw-r--r--   0        0        0     8426 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/NetCDFReading.cpp
+-rw-r--r--   0        0        0    13784 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/OpenWaterEvap.cpp
+-rw-r--r--   0        0        0     3907 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/OpenWaterEvap.h
+-rw-r--r--   0        0        0    16192 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/OrographicCorrections.cpp
+-rw-r--r--   0        0        0    21426 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/ParseEnsembleFile.cpp
+-rw-r--r--   0        0        0    40256 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/ParseFEWSRunInfo.cpp
+-rw-r--r--   0        0        0    24336 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/ParseGWFile.cpp
+-rw-r--r--   0        0        0    77416 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/ParseHRUFile.cpp
+-rw-r--r--   0        0        0    36988 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/ParseInitialConditionFile.cpp
+-rw-r--r--   0        0        0   176245 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/ParseInput.cpp
+-rw-r--r--   0        0        0    16151 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/ParseLib.cpp
+-rw-r--r--   0        0        0     5360 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/ParseLib.h
+-rw-r--r--   0        0        0    10720 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/ParseLiveFile.cpp
+-rw-r--r--   0        0        0    85505 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/ParsePropertyFile.cpp
+-rw-r--r--   0        0        0    90860 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/ParseTimeSeriesFile.cpp
+-rw-r--r--   0        0        0    13942 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/PartitionPrecip.cpp
+-rw-r--r--   0        0        0    14242 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/Percolation.cpp
+-rw-r--r--   0        0        0    13184 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/PotentialMelt.cpp
+-rw-r--r--   0        0        0    34140 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/PrairieSnow.cpp
+-rw-r--r--   0        0        0     4125 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/PrairieSnow.h
+-rw-r--r--   0        0        0     1689 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/Precipitation.h
+-rw-r--r--   0        0        0     7899 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/ProcessGroup.cpp
+-rw-r--r--   0        0        0     2155 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/ProcessGroup.h
+-rw-r--r--   0        0        0    28673 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/Properties.h
+-rw-r--r--   0        0        0      702 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/README_compile_RAVEN_on_ECCC_Pegasus.dat
+-rw-r--r--   0        0        0    46280 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/Radiation.cpp
+-rw-r--r--   0        0        0     7442 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/Radiation.h
+-rw-r--r--   0        0        0     1577 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/Raven.rc
+-rw-r--r--   0        0        0     2939 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/Raven.sln
+-rw-r--r--   0        0        0    68381 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/Raven.vcxproj
+-rw-r--r--   0        0        0    26631 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/Raven.vcxproj.filters
+-rw-r--r--   0        0        0     5013 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/Raven.vcxproj.user
+-rw-r--r--   0        0        0     8826 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/RavenAlgParams.dat
+-rw-r--r--   0        0        0      788 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/RavenIcon.ico
+-rw-r--r--   0        0        0    89872 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/RavenInclude.h
+-rw-r--r--   0        0        0    17151 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/RavenMain.cpp
+-rw-r--r--   0        0        0    10763 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/RavenParameters.dat
+-rw-r--r--   0        0        0    10652 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/RavenProcessConnections.dat
+-rw-r--r--   0        0        0     7768 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/Recharge.cpp
+-rw-r--r--   0        0        0    60879 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/Reservoir.cpp
+-rw-r--r--   0        0        0    16067 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/Reservoir.h
+-rw-r--r--   0        0        0     2141 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/RiverReach.cpp
+-rw-r--r--   0        0        0     2693 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/RiverReach.h
+-rw-r--r--   0        0        0    10887 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/SnowAlbedo.cpp
+-rw-r--r--   0        0        0    53462 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/SnowBalance.cpp
+-rw-r--r--   0        0        0    14916 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/SnowMeltRefreeze.cpp
+-rw-r--r--   0        0        0    11769 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/SnowMovers.h
+-rw-r--r--   0        0        0     7106 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/SnowParams.cpp
+-rw-r--r--   0        0        0     5620 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/SnowTempEvolve.cpp
+-rw-r--r--   0        0        0    11922 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/SoilAndLandClasses.h
+-rw-r--r--   0        0        0    15711 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/SoilBalance.cpp
+-rw-r--r--   0        0        0    34296 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/SoilClass.cpp
+-rw-r--r--   0        0        0    28725 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/SoilEvaporation.cpp
+-rw-r--r--   0        0        0     2942 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/SoilParams.cpp
+-rw-r--r--   0        0        0     8318 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/SoilProfile.cpp
+-rw-r--r--   0        0        0     2300 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/SoilProfile.h
+-rw-r--r--   0        0        0    17486 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/SoilWaterMovers.h
+-rw-r--r--   0        0        0    25666 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/Solvers.cpp
+-rw-r--r--   0        0        0    56161 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/SparseMatrix.cpp
+-rw-r--r--   0        0        0     6580 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/SparseMatrix.h
+-rw-r--r--   0        0        0     6346 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/StageDischargeRelations.cpp
+-rw-r--r--   0        0        0     5566 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/StageDischargeRelations.h
+-rw-r--r--   0        0        0   116678 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/StandardOutput.cpp
+-rw-r--r--   0        0        0    25554 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/StateVariables.cpp
+-rw-r--r--   0        0        0     1710 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/StateVariables.h
+-rw-r--r--   0        0        0    92302 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/SubBasin.cpp
+-rw-r--r--   0        0        0    20286 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/SubBasin.h
+-rw-r--r--   0        0        0     7327 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/SubbasinGroups.cpp
+-rw-r--r--   0        0        0    10813 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/Sublimation.cpp
+-rw-r--r--   0        0        0    12501 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/SurfaceEnergyExchange.cpp
+-rw-r--r--   0        0        0     1846 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/SurfaceEnergyExchange.h
+-rw-r--r--   0        0        0     8662 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/TerrainClass.cpp
+-rw-r--r--   0        0        0    70195 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/TimeSeries.cpp
+-rw-r--r--   0        0        0     9410 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/TimeSeries.h
+-rw-r--r--   0        0        0     3499 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/TimeSeriesABC.cpp
+-rw-r--r--   0        0        0     2716 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/TimeSeriesABC.h
+-rw-r--r--   0        0        0     9826 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/Transformation.cpp
+-rw-r--r--   0        0        0     3806 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/TransientParam.cpp
+-rw-r--r--   0        0        0     1931 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/TransientParam.h
+-rw-r--r--   0        0        0    35222 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/Transport.cpp
+-rw-r--r--   0        0        0    18604 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/Transport.h
+-rw-r--r--   0        0        0    11447 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/UTM_to_LatLong.cpp
+-rw-r--r--   0        0        0    23443 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/UnitTesting.cpp
+-rw-r--r--   0        0        0      711 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/UnitTesting.h
+-rw-r--r--   0        0        0    47103 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/UpdateForcings.cpp
+-rw-r--r--   0        0        0    26426 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/VegetationClass.cpp
+-rw-r--r--   0        0        0    20293 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/VegetationMovers.cpp
+-rw-r--r--   0        0        0     5226 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/VegetationMovers.h
+-rw-r--r--   0        0        0    18294 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/VegetationParams.cpp
+-rw-r--r--   0        0        0      432 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/build/_deps/raven-src/resource.h
+-rw-r--r--   0        0        0     7956 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/helpers/FindNetCDF.cmake
+-rw-r--r--   0        0        0     2495 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      459 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/src/main.cpp
+-rw-r--r--   0        0        0      727 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/src/raven_hydro/__init__.py
+-rw-r--r--   0        0        0    17030 2022-11-09 12:37:21.000000 raven-hydro-0.2.3/PKG-INFO
```

### Comparing `raven-hydro-0.2.2/CHANGES.md` & `raven-hydro-0.2.3/CHANGES.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Changes
 
+## 0.2.3 (2023-07-04)
+
+* Raven-hydro now supports building raven model without NetCDF4 support (see README.md for details).
+
 ## 0.2.2 (2023-06-05)
 
 * Building Raven-hydro from sources available on pip within an Anaconda environment is now supported.
 
 ## 0.2.1 (2023-05-25)
 
 * Raven-hydro only offers source distributions until issues arising from library linking/bundling have been resolved.
```

### Comparing `raven-hydro-0.2.2/CMakeLists.txt` & `raven-hydro-0.2.3/CMakeLists.txt`

 * *Files 22% similar despite different names*

```diff
@@ -12,21 +12,21 @@
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 cmake_minimum_required(VERSION 3.24...3.26)
 
 # Setup Raven Project
 PROJECT(${SKBUILD_PROJECT_NAME} LANGUAGES CXX VERSION ${SKBUILD_PROJECT_VERSION})
 
-set(raven_SOURCE_DIR ${CMAKE_CURRENT_BINARY_DIR}/_deps/raven-src)
+SET(raven_SOURCE_DIR ${CMAKE_CURRENT_BINARY_DIR}/_deps/raven-src)
 
 # Remove deprecation warnings for GCC
-if(CMAKE_COMPILER_IS_GNUCXX)
-    set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -Wno-deprecated")
-    message(STATUS "Modified compile flags: ${CMAKE_CXX_FLAGS}")
-endif(CMAKE_COMPILER_IS_GNUCXX)
+IF(CMAKE_COMPILER_IS_GNUCXX)
+    add_compile_options(-Wno-deprecated)
+    message(STATUS "Modified compile flags with '-Wno-deprecated'")
+ENDIF(CMAKE_COMPILER_IS_GNUCXX)
 
 IF(NOT EXISTS ${raven_SOURCE_DIR} OR ${ALWAYS_DOWNLOAD})
     IF(NOT EXISTS ${raven_SOURCE_DIR})
         message(STATUS "Sources ${raven_SOURCE_DIR} not found: fetching Raven source files from remote")
     ENDIF()
     IF(${ALWAYS_DOWNLOAD})
         message(STATUS "ALWAYS_DOWNLOAD set as True: Forcing download verification")
@@ -41,38 +41,37 @@
         )
     # Fetch remote source files without building them
     FetchContent_Populate(raven)
 ELSE()
     message(STATUS "Sources found: ${raven_SOURCE_DIR}")
 ENDIF()
 
-# Find Anaconda environment library path
-# if(DEFINED ENV{CONDA_PREFIX})
-#     set(CONDA_LIBRARY_PATH $ENV{CONDA_PREFIX}/lib)
-# else()
-#     set(CONDA_LIBRARY_PATH "")
-# endif()
+IF(USE_NETCDF)
+    # Add NetCDF support flag
+    add_compile_options(-Dnetcdf)
+    message(STATUS "Modified compile flags with '-Dnetcdf'")
+
+    # Find NetCDF library
+    list(APPEND CMAKE_MODULE_PATH ${HELPERS})
+    find_package(NetCDF REQUIRED)
 
-# Find NetCDF library
-list(APPEND CMAKE_MODULE_PATH ${HELPERS})
-find_package(NetCDF REQUIRED)
-
-# Find ZLib library
-find_package(ZLIB REQUIRED)
+    # Find ZLib library
+    find_package(ZLIB REQUIRED)
+ENDIF()
 
 # Add Python files
-set(PYBIND11_NEWPYTHON ON)
+SET(PYBIND11_NEWPYTHON ON)
 find_package(pybind11 CONFIG REQUIRED)
 pybind11_add_module(_core MODULE src/main.cpp)
 target_compile_definitions(_core PRIVATE RAVEN_VERSION_INFO=${RAVEN_VERSION} REQUIRED)
 target_compile_definitions(_core PRIVATE VERSION_INFO=${PROJECT_VERSION})
 
 # Find header & source
-file(GLOB HEADER "${raven_SOURCE_DIR}/*.h")
-file(GLOB SOURCE "${raven_SOURCE_DIR}/*.cpp")
+FILE(GLOB HEADER "${raven_SOURCE_DIR}/*.h")
+FILE(GLOB SOURCE "${raven_SOURCE_DIR}/*.cpp")
 
 # Add source files to build
 add_executable(raven
   ${SOURCE}
   ${HEADER}
 )
 source_group("Header Files" FILES ${HEADER})
@@ -81,33 +80,36 @@
 # Link Anaconda environment libraries if available, otherwise use system libraries
 # if(NOT "${CONDA_LIBRARY_PATH}" STREQUAL "")
 #     include_directories(${CONDA_LIBRARY_PATH})
 # else()
 #     include_directories(${NetCDF_INCLUDE_DIRS})
 # endif()
 
-# Link relevant libraries to build
-include_directories(${NetCDF_INCLUDE_DIRS})
-target_link_libraries(raven PUBLIC ${NetCDF_LIBRARIES})
+IF(USE_NETCDF)
+    # Link relevant NetCDF libraries to build
+    include_directories(${NetCDF_INCLUDE_DIRS})
+    target_link_libraries(raven PUBLIC ${NetCDF_LIBRARIES})
+ENDIF()
+
 target_compile_features(raven PUBLIC cxx_std_11)
 set_target_properties(raven PROPERTIES LINKER_LANGUAGE CXX)
 
 # Install library to environment Python /lib
-install(TARGETS _core LIBRARY DESTINATION ${SKBUILD_PROJECT_NAME})
+INSTALL(TARGETS _core LIBRARY DESTINATION ${SKBUILD_PROJECT_NAME})
 
 # Install binary to environment /bin
-if(WIN32)
+IF(WIN32)
   install(TARGETS raven DESTINATION ${SKBUILD_SCRIPTS_DIR})
-else()
+ELSE()
   add_custom_command(
           TARGET raven POST_BUILD
           COMMAND ${CMAKE_COMMAND} -E copy
                   ${CMAKE_CURRENT_BINARY_DIR}/raven
                   ${SKBUILD_SCRIPTS_DIR}/raven)
-endif()
+ENDIF()
 
 # Add License for Raven after building library
 add_custom_command(
         TARGET raven POST_BUILD
         COMMAND ${CMAKE_COMMAND} -E copy
                 ${raven_SOURCE_DIR}/LICENSE
                 ${SKBUILD_SCRIPTS_DIR}/raven_COPYING)
```

### Comparing `raven-hydro-0.2.2/LICENSE` & `raven-hydro-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/README.md` & `raven-hydro-0.2.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -22,26 +22,32 @@
 
 - Download and/or compile the Raven hydrological model with `pip`
 - Multiplatform support (macOS, Linux, Windows, BSD, etc.)
 
 ### Installation
 
 > **Warning**
-> This build of Raven requires that NetCDF4 libraries are installed on the system, exposed on the `$PATH`, and discoverable using the `FindNetCDF.cmake` helper script.
+> By default, this build of Raven requires that NetCDF4 libraries are installed on the system, exposed on the `$PATH`, and discoverable using the `FindNetCDF.cmake` helper script.
 >
 > On Linux, this can be provided by the `libnetcdf-dev` system library; On macOS by the `netcdf` homebrew package; And on Windows by using UNIDATA's [pre-built binaries](https://docs.unidata.ucar.edu/netcdf-c/current/winbin.html).
 >
 > This can also be provided by the `libnetcdf` package available at [conda-forge](https://anaconda.org/conda-forge/libnetcdf), though this is not guaranteed to work on macOS at time of writing (further research required).
 
 `raven-hydro` can be installed from PyPI using the following command:
 
 ```shell
 $ pip install raven-hydro
 ```
 
+To install `raven-hydro` from PyPI **without NetCDF support**:
+
+```shell
+$ pip install raven-hydro -Ccmake.define.USE_NETCDF=false
+```
+
 For development purposes, we recommend cloning the repository and performing an `--editable` installation:
 
 ```shell
 $ git clone git@github.com:Ouranosinc/raven-hydro
 $ cd raven-hydro
 $ pip install --editable .
 ```
```

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/Abstraction.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/Abstraction.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/Advection.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/Advection.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/Advection.h` & `raven-hydro-0.2.3/build/_deps/raven-src/Advection.h`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/Albedo.h` & `raven-hydro-0.2.3/build/_deps/raven-src/Albedo.h`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/Assimilate.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/Assimilate.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/Baseflow.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/Baseflow.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/CMakeLists.txt` & `raven-hydro-0.2.3/build/_deps/raven-src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/CapillaryRise.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/CapillaryRise.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/ChannelXSect.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/ChannelXSect.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/ChannelXSect.h` & `raven-hydro-0.2.3/build/_deps/raven-src/ChannelXSect.h`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/ChemEquilibrium.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/ChemEquilibrium.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/ChemEquilibrium.h` & `raven-hydro-0.2.3/build/_deps/raven-src/ChemEquilibrium.h`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/CommonFunctions.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/CommonFunctions.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/ConstituentModel.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/ConstituentModel.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/ControlStructures.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/ControlStructures.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/ControlStructures.h` & `raven-hydro-0.2.3/build/_deps/raven-src/ControlStructures.h`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/Convolution.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/Convolution.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/Convolution.h` & `raven-hydro-0.2.3/build/_deps/raven-src/Convolution.h`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/CropGrowth.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/CropGrowth.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/CropGrowth.h` & `raven-hydro-0.2.3/build/_deps/raven-src/CropGrowth.h`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/CustomOutput.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/CustomOutput.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/CustomOutput.h` & `raven-hydro-0.2.3/build/_deps/raven-src/CustomOutput.h`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/DDS.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/DDS.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/Decay.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/Decay.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/Decay.h` & `raven-hydro-0.2.3/build/_deps/raven-src/Decay.h`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/DepressionProcesses.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/DepressionProcesses.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/DepressionProcesses.h` & `raven-hydro-0.2.3/build/_deps/raven-src/DepressionProcesses.h`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/Diagnostics.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/Diagnostics.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/Diagnostics.h` & `raven-hydro-0.2.3/build/_deps/raven-src/Diagnostics.h`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/Drain.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/Drain.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/EnKF.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/EnKF.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/EnKF.h` & `raven-hydro-0.2.3/build/_deps/raven-src/EnKF.h`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/EnergyTransport.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/EnergyTransport.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/EnergyTransport.h` & `raven-hydro-0.2.3/build/_deps/raven-src/EnergyTransport.h`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/Evaporation.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/Evaporation.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/Flush.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/Flush.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/ForcingGrid.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/ForcingGrid.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/ForcingGrid.h` & `raven-hydro-0.2.3/build/_deps/raven-src/ForcingGrid.h`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/Forcings.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/Forcings.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/Forcings.h` & `raven-hydro-0.2.3/build/_deps/raven-src/Forcings.h`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/GWRecharge.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/GWRecharge.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/GWRiverConnection.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/GWRiverConnection.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/GWRiverConnection.h` & `raven-hydro-0.2.3/build/_deps/raven-src/GWRiverConnection.h`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/GWSWProcessABC.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/GWSWProcessABC.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/GWSWProcesses.h` & `raven-hydro-0.2.3/build/_deps/raven-src/GWSWProcesses.h`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/Gauge.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/Gauge.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/Gauge.h` & `raven-hydro-0.2.3/build/_deps/raven-src/Gauge.h`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/GlacierProcesses.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/GlacierProcesses.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/GlacierProcesses.h` & `raven-hydro-0.2.3/build/_deps/raven-src/GlacierProcesses.h`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/GlobalParams.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/GlobalParams.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/GlobalParams.h` & `raven-hydro-0.2.3/build/_deps/raven-src/GlobalParams.h`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/GreenAmpt.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/GreenAmpt.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/GroundwaterModel.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/GroundwaterModel.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/GroundwaterModel.h` & `raven-hydro-0.2.3/build/_deps/raven-src/GroundwaterModel.h`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/HRUGroups.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/HRUGroups.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/HeatConduction.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/HeatConduction.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/HeatConduction.h` & `raven-hydro-0.2.3/build/_deps/raven-src/HeatConduction.h`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/HydroProcessABC.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/HydroProcessABC.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/HydroProcessABC.h` & `raven-hydro-0.2.3/build/_deps/raven-src/HydroProcessABC.h`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/HydroUnits.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/HydroUnits.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/HydroUnits.h` & `raven-hydro-0.2.3/build/_deps/raven-src/HydroUnits.h`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/Infiltration.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/Infiltration.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/Infiltration.h` & `raven-hydro-0.2.3/build/_deps/raven-src/Infiltration.h`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/Interflow.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/Interflow.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/IrregularTimeSeries.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/IrregularTimeSeries.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/IrregularTimeSeries.h` & `raven-hydro-0.2.3/build/_deps/raven-src/IrregularTimeSeries.h`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/IsotopeTransport.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/IsotopeTransport.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/IsotopeTransport.h` & `raven-hydro-0.2.3/build/_deps/raven-src/IsotopeTransport.h`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/LICENSE` & `raven-hydro-0.2.3/build/_deps/raven-src/LICENSE`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/LandUseClass.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/LandUseClass.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/LatAdvection.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/LatAdvection.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/LatAdvection.h` & `raven-hydro-0.2.3/build/_deps/raven-src/LatAdvection.h`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/LatEquilibrate.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/LatEquilibrate.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/LatFlush.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/LatFlush.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/LateralExchangeABC.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/LateralExchangeABC.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/LateralExchangeABC.h` & `raven-hydro-0.2.3/build/_deps/raven-src/LateralExchangeABC.h`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/MFUSGpp.h` & `raven-hydro-0.2.3/build/_deps/raven-src/MFUSGpp.h`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/Makefile` & `raven-hydro-0.2.3/build/_deps/raven-src/Makefile`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ###
 # appname := raven_rev$(shell svnversion -n . | sed -e 's/:/-/g')_$(shell uname -o).exe
 appname := Raven.exe
 
 CXX      := g++
 CXXFLAGS := -Wno-deprecated
 # some compilers require the c++11 flag, some may not
-CXXFLAGS += std=-c++11
+CXXFLAGS += -std=c++11
 
 srcfiles := $(shell find . -name "*.cpp")
 objects  := $(patsubst %.cpp, %.o, $(srcfiles))
 
 # include netcdf
 CXXFLAGS += -Dnetcdf                # if netcdf is installed use "CXXFLAGS += -Dnetcdf",                    else "CXXFLAGS += "
 LDLIBS   := -L/usr/local -lnetcdf   # if netcdf is installed give first path "-L<PATH>"and then "-lnetcdf", else "LDLIBS   := "
```

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/MassLoading.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/MassLoading.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/MassLoading.h` & `raven-hydro-0.2.3/build/_deps/raven-src/MassLoading.h`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/MassRouting.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/MassRouting.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/Matrix.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/Matrix.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/Matrix.h` & `raven-hydro-0.2.3/build/_deps/raven-src/Matrix.h`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/Model.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/Model.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/Model.h` & `raven-hydro-0.2.3/build/_deps/raven-src/Model.h`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/ModelABC.h` & `raven-hydro-0.2.3/build/_deps/raven-src/ModelABC.h`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/ModelEnsemble.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/ModelEnsemble.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/ModelEnsemble.h` & `raven-hydro-0.2.3/build/_deps/raven-src/ModelEnsemble.h`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/ModelForcingGrids.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/ModelForcingGrids.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/ModelInitialize.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/ModelInitialize.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/ModelParamCheck.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/ModelParamCheck.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/NetCDFReading.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/NetCDFReading.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/OpenWaterEvap.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/OpenWaterEvap.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/OpenWaterEvap.h` & `raven-hydro-0.2.3/build/_deps/raven-src/OpenWaterEvap.h`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/OrographicCorrections.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/OrographicCorrections.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/ParseEnsembleFile.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/ParseEnsembleFile.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/ParseFEWSRunInfo.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/ParseFEWSRunInfo.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/ParseGWFile.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/ParseGWFile.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/ParseHRUFile.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/ParseHRUFile.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/ParseInitialConditionFile.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/ParseInitialConditionFile.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/ParseInput.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/ParseInput.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/ParseLib.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/ParseLib.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/ParseLib.h` & `raven-hydro-0.2.3/build/_deps/raven-src/ParseLib.h`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/ParseLiveFile.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/ParseLiveFile.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/ParsePropertyFile.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/ParsePropertyFile.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/ParseTimeSeriesFile.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/ParseTimeSeriesFile.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/PartitionPrecip.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/PartitionPrecip.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/Percolation.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/Percolation.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/PotentialMelt.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/PotentialMelt.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/PrairieSnow.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/PrairieSnow.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/PrairieSnow.h` & `raven-hydro-0.2.3/build/_deps/raven-src/PrairieSnow.h`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/Precipitation.h` & `raven-hydro-0.2.3/build/_deps/raven-src/Precipitation.h`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/ProcessGroup.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/ProcessGroup.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/ProcessGroup.h` & `raven-hydro-0.2.3/build/_deps/raven-src/ProcessGroup.h`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/Properties.h` & `raven-hydro-0.2.3/build/_deps/raven-src/Properties.h`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/README_compile_RAVEN_on_ECCC_Pegasus.dat` & `raven-hydro-0.2.3/build/_deps/raven-src/README_compile_RAVEN_on_ECCC_Pegasus.dat`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/Radiation.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/Radiation.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/Radiation.h` & `raven-hydro-0.2.3/build/_deps/raven-src/Radiation.h`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/Raven.rc` & `raven-hydro-0.2.3/build/_deps/raven-src/Raven.rc`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/Raven.sln` & `raven-hydro-0.2.3/build/_deps/raven-src/Raven.sln`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/Raven.vcxproj` & `raven-hydro-0.2.3/build/_deps/raven-src/Raven.vcxproj`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/Raven.vcxproj.filters` & `raven-hydro-0.2.3/build/_deps/raven-src/Raven.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/Raven.vcxproj.user` & `raven-hydro-0.2.3/build/_deps/raven-src/Raven.vcxproj.user`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/RavenAlgParams.dat` & `raven-hydro-0.2.3/build/_deps/raven-src/RavenAlgParams.dat`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/RavenIcon.ico` & `raven-hydro-0.2.3/build/_deps/raven-src/RavenIcon.ico`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/RavenInclude.h` & `raven-hydro-0.2.3/build/_deps/raven-src/RavenInclude.h`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/RavenMain.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/RavenMain.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 int main(int argc, char* argv[])
 {
   double      t;
   clock_t     t0, t1;          //computational time markers
   time_struct tt;
   int         nEnsembleMembers;
   
-  Options.version="3.6";
+  Options.version="3.7";
 #ifdef _NETCDF_ 
   Options.version+=" w/ netCDF";
 #endif
   
   ProcessExecutableArguments(argc,argv,Options);
   PrepareOutputdirectory(Options);
```

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/RavenParameters.dat` & `raven-hydro-0.2.3/build/_deps/raven-src/RavenParameters.dat`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/RavenProcessConnections.dat` & `raven-hydro-0.2.3/build/_deps/raven-src/RavenProcessConnections.dat`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/Recharge.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/Recharge.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/Reservoir.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/Reservoir.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/Reservoir.h` & `raven-hydro-0.2.3/build/_deps/raven-src/Reservoir.h`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/RiverReach.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/RiverReach.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/RiverReach.h` & `raven-hydro-0.2.3/build/_deps/raven-src/RiverReach.h`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/SnowAlbedo.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/SnowAlbedo.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/SnowBalance.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/SnowBalance.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/SnowMeltRefreeze.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/SnowMeltRefreeze.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/SnowMovers.h` & `raven-hydro-0.2.3/build/_deps/raven-src/SnowMovers.h`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/SnowParams.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/SnowParams.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/SnowTempEvolve.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/SnowTempEvolve.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/SoilAndLandClasses.h` & `raven-hydro-0.2.3/build/_deps/raven-src/SoilAndLandClasses.h`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/SoilBalance.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/SoilBalance.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/SoilClass.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/SoilClass.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/SoilEvaporation.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/SoilEvaporation.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/SoilParams.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/SoilParams.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/SoilProfile.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/SoilProfile.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/SoilProfile.h` & `raven-hydro-0.2.3/build/_deps/raven-src/SoilProfile.h`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/SoilWaterMovers.h` & `raven-hydro-0.2.3/build/_deps/raven-src/SoilWaterMovers.h`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/Solvers.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/Solvers.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/SparseMatrix.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/SparseMatrix.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/SparseMatrix.h` & `raven-hydro-0.2.3/build/_deps/raven-src/SparseMatrix.h`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/StageDischargeRelations.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/StageDischargeRelations.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/StageDischargeRelations.h` & `raven-hydro-0.2.3/build/_deps/raven-src/StageDischargeRelations.h`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/StandardOutput.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/StandardOutput.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/StateVariables.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/StateVariables.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/StateVariables.h` & `raven-hydro-0.2.3/build/_deps/raven-src/StateVariables.h`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/SubBasin.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/SubBasin.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/SubBasin.h` & `raven-hydro-0.2.3/build/_deps/raven-src/SubBasin.h`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/SubbasinGroups.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/SubbasinGroups.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/Sublimation.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/Sublimation.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/SurfaceEnergyExchange.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/SurfaceEnergyExchange.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/SurfaceEnergyExchange.h` & `raven-hydro-0.2.3/build/_deps/raven-src/SurfaceEnergyExchange.h`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/TerrainClass.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/TerrainClass.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/TimeSeries.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/TimeSeries.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/TimeSeries.h` & `raven-hydro-0.2.3/build/_deps/raven-src/TimeSeries.h`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/TimeSeriesABC.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/TimeSeriesABC.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/TimeSeriesABC.h` & `raven-hydro-0.2.3/build/_deps/raven-src/TimeSeriesABC.h`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/Transformation.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/Transformation.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/TransientParam.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/TransientParam.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/TransientParam.h` & `raven-hydro-0.2.3/build/_deps/raven-src/TransientParam.h`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/Transport.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/Transport.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/Transport.h` & `raven-hydro-0.2.3/build/_deps/raven-src/Transport.h`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/UTM_to_LatLong.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/UTM_to_LatLong.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/UnitTesting.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/UnitTesting.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/UnitTesting.h` & `raven-hydro-0.2.3/build/_deps/raven-src/UnitTesting.h`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/UpdateForcings.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/UpdateForcings.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/VegetationClass.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/VegetationClass.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/VegetationMovers.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/VegetationMovers.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/VegetationMovers.h` & `raven-hydro-0.2.3/build/_deps/raven-src/VegetationMovers.h`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/build/_deps/raven-src/VegetationParams.cpp` & `raven-hydro-0.2.3/build/_deps/raven-src/VegetationParams.cpp`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/helpers/FindNetCDF.cmake` & `raven-hydro-0.2.3/helpers/FindNetCDF.cmake`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/pyproject.toml` & `raven-hydro-0.2.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python",
   "Topic :: Scientific/Engineering :: Hydrology"
 ]
 keywords = ["raven", "hydrologic", "model", "cmake"]
 dynamic = ["readme"]
-version = "0.2.2"
+version = "0.2.3"
 dependencies = []
 
 [project.urls]
 "About Ouranos" = "https://www.ouranos.ca/en"
 "About Raven" = "http://raven.uwaterloo.ca/About.html"
 "Homepage" = "https://github.com/Ouranosinc/raven-hydro"
 "Issue tracker" = "https://github.com/Ouranosinc/raven-hydro/issues"
@@ -49,34 +49,31 @@
 [tool.scikit-build]
 build-dir = "build"
 experimental = true
 
 [tool.scikit-build.cmake]
 minimum-version = "3.24"
 build-type = "Release"
-args = [
-  "-DCMAKE_CXX_FLAGS='-Dnetcdf'"
-]
 verbose = true
 
 [tool.scikit-build.cmake.define]
+USE_NETCDF = true
 HELPERS = "helpers"
 ALWAYS_DOWNLOAD = false
 RAVEN_VERSION = 3.7
 RAVEN_URL = "https://www.civil.uwaterloo.ca/raven/files/v3.7/RavenSource_v3.7.zip"
-# The following build is broken for macOS at time of writing:
-# RAVEN_SHA256 = "7aabf0295e0e28ffee424ff29cabc14301d95b27ad1fc3971bad634bc9fa08f4"
-RAVEN_SHA256 = "5fce9688f1c1004ee36d607b226dac856fb8d35d58a6caeb663bdbf177231f07"
+RAVEN_SHA256 = "1460658be8d47d9d1f3a25ffde881c0c2be72b5ad3b048811142d45b01c62bdb"
 
 [tool.scikit-build.metadata]
 readme.provider = "scikit_build_core.metadata.fancy_pypi_readme"
 
 [tool.scikit-build.sdist]
 include = [
   "./CMakeLists.txt",
+  "AUTHORS.md",
   "CHANGES.md",
   "LICENSE",
   "README.md",
   "build/_deps/raven-src",
   "helpers/FindNetCDF.cmake",
   "src/main.cpp",
   "src/raven_hydro/__init__.py",
```

### Comparing `raven-hydro-0.2.2/src/raven_hydro/__init__.py` & `raven-hydro-0.2.3/src/raven_hydro/__init__.py`

 * *Files identical despite different names*

### Comparing `raven-hydro-0.2.2/PKG-INFO` & `raven-hydro-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raven-hydro
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Python wrapper to set-up and build the hydrologic modelling framework Raven.
 Keywords: raven hydrologic model cmake
 Author-Email: Trevor James Smith <smith.trevorj@ouranos.ca>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -243,26 +243,32 @@
 
 - Download and/or compile the Raven hydrological model with `pip`
 - Multiplatform support (macOS, Linux, Windows, BSD, etc.)
 
 ### Installation
 
 > **Warning**
-> This build of Raven requires that NetCDF4 libraries are installed on the system, exposed on the `$PATH`, and discoverable using the `FindNetCDF.cmake` helper script.
+> By default, this build of Raven requires that NetCDF4 libraries are installed on the system, exposed on the `$PATH`, and discoverable using the `FindNetCDF.cmake` helper script.
 >
 > On Linux, this can be provided by the `libnetcdf-dev` system library; On macOS by the `netcdf` homebrew package; And on Windows by using UNIDATA's [pre-built binaries](https://docs.unidata.ucar.edu/netcdf-c/current/winbin.html).
 >
 > This can also be provided by the `libnetcdf` package available at [conda-forge](https://anaconda.org/conda-forge/libnetcdf), though this is not guaranteed to work on macOS at time of writing (further research required).
 
 `raven-hydro` can be installed from PyPI using the following command:
 
 ```shell
 $ pip install raven-hydro
 ```
 
+To install `raven-hydro` from PyPI **without NetCDF support**:
+
+```shell
+$ pip install raven-hydro -Ccmake.define.USE_NETCDF=false
+```
+
 For development purposes, we recommend cloning the repository and performing an `--editable` installation:
 
 ```shell
 $ git clone git@github.com:Ouranosinc/raven-hydro
 $ cd raven-hydro
 $ pip install --editable .
 ```
```

