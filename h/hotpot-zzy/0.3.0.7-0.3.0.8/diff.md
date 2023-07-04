# Comparing `tmp/hotpot-zzy-0.3.0.7.tar.gz` & `tmp/hotpot-zzy-0.3.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/zz1/hotpot/dist/.tmp-a053367u/hotpot-zzy-0.3.0.7.tar", last modified: Mon Jul  3 11:32:31 2023, max compression
+gzip compressed data, was "/home/zz1/hotpot/dist/.tmp-qskjt3wf/hotpot-zzy-0.3.0.8.tar", last modified: Tue Jul  4 06:24:40 2023, max compression
```

## Comparing `hotpot-zzy-0.3.0.7.tar` & `hotpot-zzy-0.3.0.8.tar`

### file list

```diff
@@ -1,127 +1,127 @@
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-03 11:32:31.533866 hotpot-zzy-0.3.0.7/
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1070 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/LICENSE
--rw-rw-r--   0 zz1       (1005) zz1       (1008)       17 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/MANIFEST.in
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      382 2023-07-03 11:32:31.533866 hotpot-zzy-0.3.0.7/PKG-INFO
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     6643 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/README.md
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-03 11:32:31.521866 hotpot-zzy-0.3.0.7/hotpot/
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      419 2023-07-03 11:10:43.000000 hotpot-zzy-0.3.0.7/hotpot/__init__.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)    40274 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/_io.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)    22851 2023-07-03 07:20:46.000000 hotpot-zzy-0.3.0.7/hotpot/bundle.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)   113142 2023-07-03 11:06:14.000000 hotpot-zzy-0.3.0.7/hotpot/cheminfo.py
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-03 11:32:31.521866 hotpot-zzy-0.3.0.7/hotpot/data/
--rw-rw-r--   0 zz1       (1005) zz1       (1008)       65 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/atom_single_point.json
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1874 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/deepmd_script.json
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-03 11:32:31.521866 hotpot-zzy-0.3.0.7/hotpot/data/force_field/
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-03 11:32:31.521866 hotpot-zzy-0.3.0.7/hotpot/data/force_field/UFF/
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     4606 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/force_field/UFF/LJ.json
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-03 11:32:31.525866 hotpot-zzy-0.3.0.7/hotpot/data/force_field/aMaterials/
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1701 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/force_field/aMaterials/SiC.tersoff
--rw-rw-r--   0 zz1       (1005) zz1       (1008)       82 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/force_field/contents.json
--rw-rw-r--   0 zz1       (1005) zz1       (1008)   231681 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/periodic_table.json
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-03 11:32:31.533866 hotpot-zzy-0.3.0.7/hotpot/data/solvents/
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      946 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/1,1,1-trichloroethane.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1039 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/1,1,1-trifluroethanol.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      760 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/1,1,2-trichloroethene.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      757 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/1,1-dichloroethene.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     2525 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/1,1-diethoxypropane.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1410 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/1,1-dimethoxymethane.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      943 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/1,2-dichloroethane.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      757 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/1,2-dichloroethene.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1688 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/1,2-dimethoxyethane.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1518 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/1,4-dioxane.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1585 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/1-butanol.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1865 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/1-pentanol.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1307 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/1-propanol.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1968 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/2,2-dimethoxypropane.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1585 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/2-butanol.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1684 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/2-ethoxyethanol.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1406 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/2-methoxyethanol.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1595 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/2-methyl-1-propanol.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1716 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/2-methyltetrahydrofuran.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1873 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/3-methyl-1-butanol.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      649 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/DCM.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1300 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/DMF.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1115 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/DMSO.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1597 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/N,N-dimethylacetamide.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1712 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/N-methylpyrrolidone.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1417 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/THF.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      936 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/acetic_acid.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1118 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/acetone.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      751 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/acetonitrile.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1328 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/benzene.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     2053 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/butylacetate.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      666 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/carbon_tetrachloride.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1334 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/chlorobenzene.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      656 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/chloroform.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     2164 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/cumene.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1890 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/cyclohexane.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1588 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/diethylether.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     2243 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/diisopropylamine.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1025 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/ethanol.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1217 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/ethyl_formate.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1495 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/ethylacetate.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1125 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/ethyleneglycol.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      748 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/formamide.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      657 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/formic_acid.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     2327 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/heptane.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     2047 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/hexane.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     2057 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/isobutyl_acetate.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     2608 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/isooctane.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1308 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/isopropanol.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1778 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/isopropylacetate.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     2148 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/isopropylether.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1890 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/meta-xylene.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      747 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/methanol.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1707 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/methoxybenzene.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1217 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/methylacetate.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1965 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/methylbutylketone.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     2175 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/methylcyclohexane.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1407 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/methylethylketone.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1968 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/methylisobutylketone.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1690 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/methylisopropylketone.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1610 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/morpholine.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      844 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/nitromethane.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1891 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/ortho-xylene.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1890 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/para-xylene.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1769 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/pentane.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1775 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/propylacetate.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1236 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/pyridine.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1609 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/sulfolane.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1873 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/t-butylmethylether.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     2283 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/tetralin.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1607 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/toluene.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      945 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/trichloroacetic_acid.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      945 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/trifluoroacetic_acid.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      465 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/solvents/water.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      182 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/data/units.json
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-03 11:32:31.533866 hotpot-zzy-0.3.0.7/hotpot/tanks/
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      205 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/tanks/__init__.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)    10245 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/tanks/cc.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      306 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/tanks/deepmd.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      149 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/tanks/features.py
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-03 11:32:31.533866 hotpot-zzy-0.3.0.7/hotpot/tanks/lmp/
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      269 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/tanks/lmp/__init__.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     7862 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/tanks/lmp/base.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     8553 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/tanks/lmp/gcmc.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     9158 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/tanks/lmp/materials.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     8896 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/tanks/quantum.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     2838 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/tmo.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     2805 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/tools.py
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-03 11:32:31.533866 hotpot-zzy-0.3.0.7/hotpot/utils/
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      125 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/utils/__init__.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     3979 2023-07-03 10:51:41.000000 hotpot-zzy-0.3.0.7/hotpot/utils/library.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1403 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/utils/manage_machine.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      642 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/hotpot/utils/units_convert.py
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-03 11:32:31.533866 hotpot-zzy-0.3.0.7/hotpot_zzy.egg-info/
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      382 2023-07-03 11:32:31.000000 hotpot-zzy-0.3.0.7/hotpot_zzy.egg-info/PKG-INFO
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     3941 2023-07-03 11:32:31.000000 hotpot-zzy-0.3.0.7/hotpot_zzy.egg-info/SOURCES.txt
--rw-rw-r--   0 zz1       (1005) zz1       (1008)        1 2023-07-03 11:32:31.000000 hotpot-zzy-0.3.0.7/hotpot_zzy.egg-info/dependency_links.txt
--rw-rw-r--   0 zz1       (1005) zz1       (1008)       44 2023-07-03 11:32:31.000000 hotpot-zzy-0.3.0.7/hotpot_zzy.egg-info/requires.txt
--rw-rw-r--   0 zz1       (1005) zz1       (1008)        7 2023-07-03 11:32:31.000000 hotpot-zzy-0.3.0.7/hotpot_zzy.egg-info/top_level.txt
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      656 2023-07-03 11:31:44.000000 hotpot-zzy-0.3.0.7/pyproject.toml
--rw-rw-r--   0 zz1       (1005) zz1       (1008)       38 2023-07-03 11:32:31.533866 hotpot-zzy-0.3.0.7/setup.cfg
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-03 11:32:31.533866 hotpot-zzy-0.3.0.7/test/
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      533 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/test/test_amorphous_maker.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1812 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/test/test_bundle.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     3095 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/test/test_chemif.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     6853 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.7/test/test_lmp.py
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-04 06:24:40.592325 hotpot-zzy-0.3.0.8/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1070 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/LICENSE
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)       17 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/MANIFEST.in
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      382 2023-07-04 06:24:40.592325 hotpot-zzy-0.3.0.8/PKG-INFO
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     6643 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/README.md
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-04 06:24:40.564325 hotpot-zzy-0.3.0.8/hotpot/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      419 2023-07-04 06:17:05.000000 hotpot-zzy-0.3.0.8/hotpot/__init__.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)    36575 2023-07-04 06:09:00.000000 hotpot-zzy-0.3.0.8/hotpot/_io.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)    25799 2023-07-04 06:05:29.000000 hotpot-zzy-0.3.0.8/hotpot/bundle.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)   113273 2023-07-04 04:34:02.000000 hotpot-zzy-0.3.0.8/hotpot/cheminfo.py
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-04 06:24:40.568325 hotpot-zzy-0.3.0.8/hotpot/data/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)       65 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/atom_single_point.json
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1874 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/deepmd_script.json
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-04 06:24:40.568325 hotpot-zzy-0.3.0.8/hotpot/data/force_field/
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-04 06:24:40.568325 hotpot-zzy-0.3.0.8/hotpot/data/force_field/UFF/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     4606 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/force_field/UFF/LJ.json
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-04 06:24:40.568325 hotpot-zzy-0.3.0.8/hotpot/data/force_field/aMaterials/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1701 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/force_field/aMaterials/SiC.tersoff
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)       82 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/force_field/contents.json
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)   231681 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/periodic_table.json
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-04 06:24:40.584325 hotpot-zzy-0.3.0.8/hotpot/data/solvents/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      946 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/1,1,1-trichloroethane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1039 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/1,1,1-trifluroethanol.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      760 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/1,1,2-trichloroethene.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      757 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/1,1-dichloroethene.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2525 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/1,1-diethoxypropane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1410 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/1,1-dimethoxymethane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      943 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/1,2-dichloroethane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      757 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/1,2-dichloroethene.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1688 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/1,2-dimethoxyethane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1518 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/1,4-dioxane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1585 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/1-butanol.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1865 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/1-pentanol.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1307 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/1-propanol.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1968 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/2,2-dimethoxypropane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1585 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/2-butanol.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1684 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/2-ethoxyethanol.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1406 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/2-methoxyethanol.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1595 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/2-methyl-1-propanol.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1716 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/2-methyltetrahydrofuran.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1873 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/3-methyl-1-butanol.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      649 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/DCM.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1300 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/DMF.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1115 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/DMSO.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1597 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/N,N-dimethylacetamide.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1712 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/N-methylpyrrolidone.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1417 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/THF.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      936 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/acetic_acid.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1118 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/acetone.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      751 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/acetonitrile.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1328 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/benzene.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2053 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/butylacetate.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      666 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/carbon_tetrachloride.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1334 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/chlorobenzene.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      656 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/chloroform.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2164 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/cumene.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1890 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/cyclohexane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1588 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/diethylether.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2243 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/diisopropylamine.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1025 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/ethanol.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1217 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/ethyl_formate.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1495 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/ethylacetate.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1125 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/ethyleneglycol.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      748 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/formamide.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      657 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/formic_acid.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2327 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/heptane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2047 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/hexane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2057 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/isobutyl_acetate.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2608 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/isooctane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1308 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/isopropanol.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1778 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/isopropylacetate.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2148 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/isopropylether.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1890 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/meta-xylene.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      747 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/methanol.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1707 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/methoxybenzene.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1217 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/methylacetate.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1965 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/methylbutylketone.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2175 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/methylcyclohexane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1407 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/methylethylketone.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1968 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/methylisobutylketone.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1690 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/methylisopropylketone.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1610 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/morpholine.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      844 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/nitromethane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1891 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/ortho-xylene.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1890 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/para-xylene.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1769 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/pentane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1775 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/propylacetate.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1236 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/pyridine.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1609 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/sulfolane.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1873 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/t-butylmethylether.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2283 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/tetralin.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1607 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/toluene.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      945 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/trichloroacetic_acid.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      945 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/trifluoroacetic_acid.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      465 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/water.mol2
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      182 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/units.json
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-04 06:24:40.584325 hotpot-zzy-0.3.0.8/hotpot/tanks/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      205 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/tanks/__init__.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)    10245 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/tanks/cc.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     8070 2023-07-04 05:01:45.000000 hotpot-zzy-0.3.0.8/hotpot/tanks/deepmd.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      149 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/tanks/features.py
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-04 06:24:40.588325 hotpot-zzy-0.3.0.8/hotpot/tanks/lmp/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      269 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/tanks/lmp/__init__.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     7862 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/tanks/lmp/base.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     8553 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/tanks/lmp/gcmc.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     9158 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/tanks/lmp/materials.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     8896 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/tanks/quantum.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2838 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/tmo.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2805 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/tools.py
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-04 06:24:40.588325 hotpot-zzy-0.3.0.8/hotpot/utils/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      125 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/utils/__init__.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     3979 2023-07-03 10:51:41.000000 hotpot-zzy-0.3.0.8/hotpot/utils/library.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1403 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/utils/manage_machine.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      642 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/utils/units_convert.py
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-04 06:24:40.588325 hotpot-zzy-0.3.0.8/hotpot_zzy.egg-info/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      382 2023-07-04 06:24:40.000000 hotpot-zzy-0.3.0.8/hotpot_zzy.egg-info/PKG-INFO
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     3941 2023-07-04 06:24:40.000000 hotpot-zzy-0.3.0.8/hotpot_zzy.egg-info/SOURCES.txt
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)        1 2023-07-04 06:24:40.000000 hotpot-zzy-0.3.0.8/hotpot_zzy.egg-info/dependency_links.txt
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)       44 2023-07-04 06:24:40.000000 hotpot-zzy-0.3.0.8/hotpot_zzy.egg-info/requires.txt
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)        7 2023-07-04 06:24:40.000000 hotpot-zzy-0.3.0.8/hotpot_zzy.egg-info/top_level.txt
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      656 2023-07-04 06:17:05.000000 hotpot-zzy-0.3.0.8/pyproject.toml
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)       38 2023-07-04 06:24:40.592325 hotpot-zzy-0.3.0.8/setup.cfg
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-04 06:24:40.588325 hotpot-zzy-0.3.0.8/test/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      533 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/test/test_amorphous_maker.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1812 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/test/test_bundle.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     3095 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/test/test_chemif.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     6853 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/test/test_lmp.py
```

### Comparing `hotpot-zzy-0.3.0.7/LICENSE` & `hotpot-zzy-0.3.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/README.md` & `hotpot-zzy-0.3.0.8/README.md`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/_io.py` & `hotpot-zzy-0.3.0.8/hotpot/_io.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,17 @@
 from abc import ABCMeta, abstractmethod
 from copy import copy
 import io
 from io import IOBase
 from openbabel import pybel
 import cclib
 import numpy as np
+
 import hotpot.cheminfo as ci
+from hotpot.tanks.deepmd import DeepSystem
 
 """
 Notes:
 This module contain Classes to IO between the Molecule object and various file formats.
 the main classes are:
     - Reader: from Formatted files to Molecule, called by the Molecule.read() method.
     - Writer: from Molecule to formatted files, called by the Molecule.write() method.
@@ -322,17 +324,17 @@
 
         except IOEarlyStop:
             return None
 
     @abstractmethod
     def _checks(self) -> Dict[str, Any]:
         """
-        This method should be override when definition of new IO class
+        This method should be overriden when definition of new IO class
         The purpose of this class is to check the regulation of initialized arguments.
-        If not any arguments should be check, return None directly.
+        If not any arguments should be checked, return None directly.
         """
         raise NotImplemented()
 
     def _get_pre(self) -> Callable:
         return self.register.pre(self.fmt)
 
     def _get_io(self) -> Callable:
@@ -438,71 +440,15 @@
             self.src.build_3d()
 
         self.src.assign_atoms_formal_charge()
         self.src.identifier = self.src.formula
 
     def _io_dpmd_sys(self):
         """ convert molecule information to numpy arrays """
-        required_items = ['coord', 'type']
-        check_atom_num = ['coord', 'force', 'charge']
-        share_same_conformers = ['type', 'coord', 'energy', 'force', 'charge', 'virial']
-        need_reshape = ['coord', 'force']
-
-        conf_num = len(self.src.all_coordinates)
-        crystal = self.src.crystal()
-        if crystal:
-            box = self.src.crystal().vector  # angstrom
-            is_periodic = True
-        else:
-            box = np.zeros((3, 3))
-            for i in range(3):
-                box[i, i] = 100.
-            is_periodic = False
-        box = box.reshape(-1, 9).repeat(conf_num, axis=0)
-
-        data = {
-            'type': self.src.atomic_numbers_array,
-            'type_map': ['-'] + list(ci.periodic_table.symbols),
-            'nopbc': not is_periodic,
-            'coord': self.src.all_coordinates,  # angstrom,
-            'box': box,
-            'energy': self.src.all_energy,  # eV
-            'force': self.src.all_forces,  # Hartree/Bohr,
-            'charge': self.src.all_atom_charges,  # q
-            'virial': None,
-            'atom_ener': None,
-            'atom_pref': None,
-            'dipole': None,
-            'atom_dipole': None,
-            'polarizability': None,
-            'atomic_polarizability': None
-        }
-
-        for name in required_items:
-            if data.get(name) is None:
-                raise ValueError('the required composition to make the dpmd system is incomplete!')
-
-        # Check whether the number of conformers are matching among data
-        if any(len(data[n]) != conf_num for n in share_same_conformers if data[n] is not None):
-            raise ValueError('the number of conformers is not match')
-
-        # Check whether the number of atoms in data are matching to the molecular atoms
-        if any(data[n].shape[1] != self.src.atom_counts for n in check_atom_num if data[n] is not None):
-            raise ValueError('the number of atoms is not matching the number of atom is the molecule')
-
-        for name in need_reshape:
-            item = data.get(name)
-            if isinstance(item, np.ndarray):
-                shape = item.shape
-
-                assert len(shape) == 3
-
-                data[name] = item.reshape((shape[0], shape[1]*shape[2]))
-
-        return data
+        return DeepSystem(self.src)
 
     def _io_lmpmol(self):
         """
         write a molecule script
         default values: coordinates, velocities, atom IDs and types
         additional attributes for atomic: Bonds
         additional attributes for full: Bonds + molecular + charge
@@ -602,51 +548,14 @@
         elif atom_style == 'full':
             if num_bonds:
                 script += bonds(mol)
             script += charge()
 
         return script
 
-    def _post_dpmd_sys(self, data: Dict[str, Union[List, np.ndarray, None]]):
-        """"""
-        mapping_items = ['type', 'type_map']
-        path_save = self.kwargs.get('path_save')
-        if path_save:
-            if isinstance(path_save, str):
-                path_save = Path(path_save)
-            if path_save.is_file():
-                raise NotADirectoryError('the given path_save to dpmd_sys should be an empty dir, not a existed file')
-
-            if not path_save.exists():
-                path_save.mkdir()
-
-            if [p for p in path_save.glob('*')]:
-                raise IOError('the given path_save should be a empty dir, files or dirs have exist in the dir')
-
-            dir_npy = path_save.joinpath('set.000')
-            dir_npy.mkdir()
-
-            for name, value in data.items():
-                if name == 'nopbc' and value:
-                    with open(path_save.joinpath('nopbc'), 'w') as writer:
-                        writer.write('')
-
-                elif name in mapping_items:
-                    with open(path_save.joinpath(f'{name}.raw'), 'w') as writer:
-                        writer.write('\n'.join(map(str, value)))
-
-                else:
-                    if value is not None:
-                        if not isinstance(value, np.ndarray):
-                            raise ValueError(f'the data to set.*** must be np.ndarray, instead of {type(value)}')
-
-                        np.save(dir_npy.joinpath(f'{name}.npy'), value)
-
-        return data
-
     def _post_gjf(self, script):
         """ postprocess the dumped Gaussian 16 .gjf script to add the link0 and route context """
         # To count the insert lines
         inserted_lines = 0
 
         # separate keyword arguments:
         link0 = self.kwargs['link0']
```

### Comparing `hotpot-zzy-0.3.0.7/hotpot/bundle.py` & `hotpot-zzy-0.3.0.8/hotpot/bundle.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 @Project: hotpot
 @File   : bundle.py
 @Author : Zhiyuan Zhang
 @Date   : 2023/3/22
 @Time   : 3:18
 """
 import copy
+import os
 import random
 import time
 from os import PathLike
 from typing import *
 from pathlib import Path
 import numpy as np
 from tqdm import tqdm
@@ -89,24 +90,32 @@
         """
         return self.__get_all_unique_attrs('atom_counts')
 
     @property
     def atomic_numbers(self):
         return self.__get_all_unique_attrs('atomic_numbers')
 
-    def choice(self, size: int = 1, replace: bool = True, p: Union[Sequence, float, Callable] = None) -> 'MolBundle':
+    def choice(
+            self, size: int = 1, replace: bool = True,
+            p: Union[Sequence, float, Callable] = None,
+            get_remain: bool = False
+    ) -> Union['MolBundle', tuple['MolBundle', 'MolBundle']]:
         """
          Generate new MolBundle with a list of random Molecule objects from the current MolBundle
         Args:
             size: the size of generating MolBundle, that the number of contained Molecule objects
-            replace: whether allow to choice a Molecule object multiply times
+            replace: whether allow to choice a Molecule object multiply times. It must be noted that
+             if this MolBundle is a generator or the get_remain arg has been specified, this arg
+             would not work.
             p: If the current MolBundle is a Generator it should be a float or a Callable object
              which arg is the generated molecule. If the current MolBundle is a Sequence, the p
              should bea sequence with same size as the number of Molecule objects in current
              MolBundle, specify the probability of each Molecule to be chosen.
+            get_remain: whether to get the remain Molecule object, if the current MolBundle is a Generator
+             this arg would not work
 
         Return:
             MolBundle contained specified-number molecules
         """
         def choice_from_generator():
             """ Generator molecule according to specified probability """
             if isinstance(p, float):
@@ -115,21 +124,33 @@
                         yield mol
 
             if isinstance(p, Callable):
                 for mol in self:
                     if p(mol):
                         yield mol
 
+        # if the MolBundle is a generator, the derivative one is still generator
         if self.is_generator:
             if isinstance(p, (float, Callable)):
                 return MolBundle(choice_from_generator())
             else:
                 raise TypeError('When the MolBundle is a generator, the p should be a float or Callable object')
+
+        elif get_remain:  # get remain molecules as the second return
+            mol_indices = np.arange(len(self))
+            chosen_idx = np.random.choice(mol_indices, size=int(len(self) * p))
+            remain_idx = np.setdiff1d(mol_indices, chosen_idx)
+
+            chosen_mol = np.array(self.mols)[chosen_idx].tolist()
+            remain_mol = np.array(self.mols)[remain_idx].tolist()
+
+            return self.__class__(chosen_mol), self.__class__(remain_mol)
+
         else:
-            return MolBundle(np.random.choice(self.mols, size=size, replace=replace, p=p))
+            return self.__class__(np.random.choice(self.mols, size=size, replace=replace, p=p))
 
     @property
     def data(self):
         return self._data
 
     @data.setter
     def data(self, data):
@@ -540,29 +561,80 @@
 
         if isinstance(atom_counts, tuple):
             return sum(bundle.mols[1:], start=bundle.mols[0])
         elif isinstance(atom_counts, dict):
             mol_array = np.array(bundle.mols)
             return self.__class__([mol_array[i].sum() for ans, i in atom_counts.items()])
 
-    def to_dpmd_sys(self, dataset_root, mode: Literal['std', 'att'] = 'std'):
+    def to_dpmd_sys(
+            self, system_dir: Union[str, os.PathLike],
+            validate_ratio: float,
+            mode: Literal['std', 'att'] = 'std',
+            split_mode: Optional[Literal['inside', 'outside']] = None
+    ):
         """"""
+        def to_files(mb: MolBundle, save_root: Path):
+            for c, m in enumerate(mb):  # c: counts, m: molecule
+                mol_save_root = \
+                    save_root.joinpath(str(m.atom_counts)) if mode == 'att' else system_dir.joinpath(str(c))
+                if not mol_save_root.exists():
+                    mol_save_root.mkdir()
+
+                m.to_dpmd_sys(mol_save_root, mode)
+
+
+        if split_mode and split_mode not in ['inside', 'outside']:
+            raise ValueError("the split_mode must be 'inside' or 'outside'")
+
+        if not 0.0 < validate_ratio < 1.0:
+            raise ValueError('the validate_ratio must be from 0.0 to 1.0')
+
+        # Organize dirs
+        if not isinstance(system_dir, Path):
+            system_dir = Path(system_dir)
+        training_dir = system_dir.joinpath('training_dir')
+        validate_dir = system_dir.joinpath('validate_dir')
+        if not training_dir.exists():
+            training_dir.mkdir()
+        if not validate_dir.exists():
+            validate_dir.mkdir()
+
         if mode == 'att':
             bundle = self.merge_atoms_same_mols()
+            if not split_mode:
+                split_mode = 'inside'
+
         elif mode == 'std':
             bundle = copy.copy(self)
+            if not split_mode:
+                split_mode = 'outside'
+
         else:
             raise ValueError("the mode is only allowed to be 'att' or 'std'!")
 
-        for mol in bundle:
-            sys_root = dataset_root.joinpath(str(mol.atom_counts)) \
-                if mode == 'att' else dataset_root.joinpath(mol.identifier)
-            if not sys_root.exists():
-                sys_root.mkdir()
-            mol.to_dpmd_sys(sys_root, mode=mode)
+        if split_mode == 'inside':
+            for i, mol in enumerate(bundle):
+                mol_training_dir = \
+                    training_dir.joinpath(str(mol.atom_counts)) if mode == 'att' else system_dir.joinpath(str(i))
+                mol_validate_dir = \
+                    validate_dir.joinpath(str(mol.atom_counts)) if mode == 'att' else system_dir.joinpath(str(i))
+
+                if not mol_training_dir.exists():
+                    mol_training_dir.mkdir()
+                if not mol_validate_dir.exists():
+                    mol_validate_dir.mkdir()
+
+                mol.to_dpmd_sys(mol_training_dir, mode, validate_ratio, mol_validate_dir)
+
+        elif split_mode == 'outside':
+            validate_bundle, training_bundle = bundle.choice(p=validate_ratio, get_remain=True)
+
+            # Save to files
+            to_files(training_bundle, training_dir)
+            to_files(validate_bundle, validate_dir)
 
     def to_mix_mols(self):
         """
         Return a new MolBundle, in which Molecule objects in container are converted to MixSameAtomMol
         Returns:
             MolBundle(MixSameAtomMol)
         """
```

### Comparing `hotpot-zzy-0.3.0.7/hotpot/cheminfo.py` & `hotpot-zzy-0.3.0.8/hotpot/cheminfo.py`

 * *Files 1% similar despite different names*

```diff
@@ -1245,30 +1245,30 @@
 
         if cell_data:
             ob_unit_cell = ob.toUnitCell(cell_data)
             return Crystal(ob_unit_cell, molecule=self)
         else:
             return None
 
-    def dump(self, fmt: str, *args, **kwargs) -> Union[str, bytes, dict]:
+    def dump(self, fmt: str, *args, **kwargs) -> Union[str, bytes, dict, 'DeepSystem']:
         """"""
         dumper = Dumper(fmt=fmt, source=self, *args, **kwargs)
         return dumper()
 
     @property
     def elements(self) -> list[str]:
         return re.findall(r'[A-Z][a-z]*', self.formula)
 
     @property
     def energy(self):
         """ Return energy with kcal/mol as default """
         return self.ob_mol.GetEnergy()
 
     def feature_matrix(self, *feature_names: Sequence) -> np.ndarray:
-        """ Retrieve the feature matrix (collections of feature vector for every atoms),
+        """ Retrieve the feature matrix (collections of feature vector for atoms),
          The default feature is `atomic_orbital`, if the feature names not be specified, the `atomic_orbital` will be
          retrieved.
          Args:
              feature_names: the feature names are offered in hotpot/data/periodic_table.json
          """
         if not feature_names:
             feature_names = ('atomic_orbital',)
@@ -2064,80 +2064,74 @@
 
         """
         clone = self.copy()
         clone.build_2d()
         return Draw.MolToImage(clone.to_rdmol(), **kwargs)
 
     def to_dpmd_sys(
-            self, dpmd_sys_root: Union[str, os.PathLike],
+            self, system_dir: Union[str, os.PathLike],
             mode: Literal['std', 'att'] = 'std',
-            valid_ratio: float = 0.1
+            validate_ratio: float = None,
+            validate_dir: Union[str, Path] = None
     ):
         """
         convert to DeePMD-Kit System, there are two system mode, that `standard` (std) and `attention` (att)
             1) standard: https://docs.deepmodeling.com/projects/deepmd/en/master/data/system.html
             2) attention: https://docs.deepmodeling.com/projects/deepmd/en/master/model/train-se-atten.html#data-format
 
         Args:
-            dpmd_sys_root: the dir for all system data store
+            system_dir: the dir for all system data store, if the validate_dir has been given, this is the dir of
+             training system
             mode: the system mode, choose from att or std
-            valid_ratio(float): the ratio of validate data set.
+            validate_ratio(float): the ratio of validate data set.
+            validate_dir(str|Path): if validate_ratio has been specified, this must be given
         """
-        dpmd_sys_root = Path(dpmd_sys_root)
-        if not dpmd_sys_root.exists():
-            dpmd_sys_root.mkdir()
-
-        # Make the training and validate sets
-        training_path = dpmd_sys_root.joinpath('training_data')
-        validate_path = dpmd_sys_root.joinpath('validate_data')
-        if not training_path:
-            training_path.mkdir()
-        if not validate_path:
-            validate_path.mkdir()
-
-        tv_paths = [training_path, validate_path]
-
-        # the dir of set data
-        set_root = dpmd_sys_root.joinpath('set.000')
-        if not set_root.exists():
-            set_root.mkdir()
-
-        data = self.dump('dpmd_sys')
-
-        for name, value in data.items():
-
-            # if the value is None, go to next
-            if value is None:
-                continue
-
-            # Write the type raw
-            if name == 'type':
-                if mode == 'std':
-                    type_raw = value[0]
-                elif mode == 'att':
-                    type_raw = np.zeros(value[0].shape, dtype=int)
-                    np.save(set_root.joinpath("real_atom_types.npy"), value)
-                else:
-                    raise ValueError('the mode just allows to be "std" or "att"')
-
-                with open(dpmd_sys_root.joinpath('type.raw'), 'w') as writer:
-                    writer.write('\n'.join([str(i) for i in type_raw]))
-
-            elif name == 'type_map':
-                with open(dpmd_sys_root.joinpath('type_map.raw'), 'w') as writer:
-                    writer.write('\n'.join([str(i) for i in value]))
-
-            # Create an empty 'nopbc', when the system is not periodical
-            elif name == 'nopbc' and value is True:
-                with open(dpmd_sys_root.joinpath('nopbc'), 'w') as writer:
-                    writer.write('')
-
-            # Save the numpy format data
-            elif isinstance(value, np.ndarray):
-                np.save(str(set_root.joinpath(f'{name}.npy')), value)
+        # dpmd_sys_root = Path(dpmd_sys_root)
+        # if not dpmd_sys_root.exists():
+        #     dpmd_sys_root.mkdir()
+        #
+        # # the dir of set data
+        # set_root = dpmd_sys_root.joinpath('set.000')
+        # if not set_root.exists():
+        #     set_root.mkdir()
+
+        system: DeepSystem = self.dump('dpmd_sys')
+        system(system_dir, mode, validate_ratio, validate_dir)
+
+        # for name, value in data.items():
+        #
+        #     # if the value is None, go to next
+        #     if value is None:
+        #         continue
+        #
+        #     # Write the type raw
+        #     if name == 'type':
+        #         if mode == 'std':
+        #             type_raw = value[0]
+        #         elif mode == 'att':
+        #             type_raw = np.zeros(value[0].shape, dtype=int)
+        #             np.save(set_root.joinpath("real_atom_types.npy"), value)
+        #         else:
+        #             raise ValueError('the mode just allows to be "std" or "att"')
+        #
+        #         with open(dpmd_sys_root.joinpath('type.raw'), 'w') as writer:
+        #             writer.write('\n'.join([str(i) for i in type_raw]))
+        #
+        #     elif name == 'type_map':
+        #         with open(dpmd_sys_root.joinpath('type_map.raw'), 'w') as writer:
+        #             writer.write('\n'.join([str(i) for i in value]))
+        #
+        #     # Create an empty 'nopbc', when the system is not periodical
+        #     elif name == 'nopbc' and value is True:
+        #         with open(dpmd_sys_root.joinpath('nopbc'), 'w') as writer:
+        #             writer.write('')
+        #
+        #     # Save the numpy format data
+        #     elif isinstance(value, np.ndarray):
+        #         np.save(str(set_root.joinpath(f'{name}.npy')), value)
 
     def to_mix_mol(self):
         """ Convert this Molecule object to MixSaveAtomMol """
         return MixSameAtomMol(_data=self._data)
 
     def to_rdmol(self):
         """ convert hotpot Molecule object to RdKit mol object """
@@ -3081,7 +3075,8 @@
     def zeo_plus_plus(self):
         """ TODO: complete the method after define the Crystal and ZeoPlusPlus tank """
 
 
 import hotpot.bundle as bd
 from hotpot._io import Dumper, Parser
 from hotpot.tanks.cc import PairBundle
+from hotpot.tanks.deepmd import DeepSystem
```

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/deepmd_script.json` & `hotpot-zzy-0.3.0.8/hotpot/data/deepmd_script.json`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/force_field/UFF/LJ.json` & `hotpot-zzy-0.3.0.8/hotpot/data/force_field/UFF/LJ.json`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/force_field/aMaterials/SiC.tersoff` & `hotpot-zzy-0.3.0.8/hotpot/data/force_field/aMaterials/SiC.tersoff`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/periodic_table.json` & `hotpot-zzy-0.3.0.8/hotpot/data/periodic_table.json`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/1,1,1-trichloroethane.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/1,1,1-trichloroethane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/1,1,1-trifluroethanol.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/1,1,1-trifluroethanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/1,1,2-trichloroethene.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/1,1,2-trichloroethene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/1,1-dichloroethene.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/1,1-dichloroethene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/1,1-diethoxypropane.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/1,1-diethoxypropane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/1,1-dimethoxymethane.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/1,1-dimethoxymethane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/1,2-dichloroethane.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/1,2-dichloroethane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/1,2-dichloroethene.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/1,2-dichloroethene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/1,2-dimethoxyethane.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/1,2-dimethoxyethane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/1,4-dioxane.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/1,4-dioxane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/1-butanol.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/1-butanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/1-pentanol.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/1-pentanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/1-propanol.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/1-propanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/2,2-dimethoxypropane.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/2,2-dimethoxypropane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/2-butanol.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/2-butanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/2-ethoxyethanol.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/2-ethoxyethanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/2-methoxyethanol.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/2-methoxyethanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/2-methyl-1-propanol.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/2-methyl-1-propanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/2-methyltetrahydrofuran.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/2-methyltetrahydrofuran.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/3-methyl-1-butanol.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/3-methyl-1-butanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/DCM.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/DCM.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/DMF.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/DMF.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/DMSO.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/DMSO.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/N,N-dimethylacetamide.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/N,N-dimethylacetamide.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/N-methylpyrrolidone.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/N-methylpyrrolidone.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/THF.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/THF.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/acetic_acid.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/acetic_acid.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/acetone.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/acetone.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/acetonitrile.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/acetonitrile.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/benzene.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/benzene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/butylacetate.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/butylacetate.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/carbon_tetrachloride.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/carbon_tetrachloride.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/chlorobenzene.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/chlorobenzene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/chloroform.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/chloroform.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/cumene.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/cumene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/cyclohexane.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/cyclohexane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/diethylether.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/diethylether.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/diisopropylamine.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/diisopropylamine.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/ethanol.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/ethanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/ethyl_formate.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/ethyl_formate.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/ethylacetate.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/ethylacetate.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/ethyleneglycol.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/ethyleneglycol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/formamide.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/formamide.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/formic_acid.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/formic_acid.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/heptane.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/heptane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/hexane.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/hexane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/isobutyl_acetate.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/isobutyl_acetate.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/isooctane.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/isooctane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/isopropanol.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/isopropanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/isopropylacetate.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/isopropylacetate.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/isopropylether.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/isopropylether.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/meta-xylene.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/meta-xylene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/methanol.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/methanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/methoxybenzene.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/methoxybenzene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/methylacetate.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/methylacetate.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/methylbutylketone.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/methylbutylketone.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/methylcyclohexane.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/methylcyclohexane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/methylethylketone.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/methylethylketone.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/methylisobutylketone.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/methylisobutylketone.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/methylisopropylketone.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/methylisopropylketone.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/morpholine.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/morpholine.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/nitromethane.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/nitromethane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/ortho-xylene.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/ortho-xylene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/para-xylene.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/para-xylene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/pentane.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/pentane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/propylacetate.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/propylacetate.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/pyridine.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/pyridine.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/sulfolane.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/sulfolane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/t-butylmethylether.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/t-butylmethylether.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/tetralin.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/tetralin.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/toluene.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/toluene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/trichloroacetic_acid.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/trichloroacetic_acid.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/data/solvents/trifluoroacetic_acid.mol2` & `hotpot-zzy-0.3.0.8/hotpot/data/solvents/trifluoroacetic_acid.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/tanks/cc.py` & `hotpot-zzy-0.3.0.8/hotpot/tanks/cc.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/tanks/lmp/base.py` & `hotpot-zzy-0.3.0.8/hotpot/tanks/lmp/base.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/tanks/lmp/gcmc.py` & `hotpot-zzy-0.3.0.8/hotpot/tanks/lmp/gcmc.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/tanks/lmp/materials.py` & `hotpot-zzy-0.3.0.8/hotpot/tanks/lmp/materials.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/tanks/quantum.py` & `hotpot-zzy-0.3.0.8/hotpot/tanks/quantum.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/tmo.py` & `hotpot-zzy-0.3.0.8/hotpot/tmo.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/tools.py` & `hotpot-zzy-0.3.0.8/hotpot/tools.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/utils/library.py` & `hotpot-zzy-0.3.0.8/hotpot/utils/library.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/utils/manage_machine.py` & `hotpot-zzy-0.3.0.8/hotpot/utils/manage_machine.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot/utils/units_convert.py` & `hotpot-zzy-0.3.0.8/hotpot/utils/units_convert.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/hotpot_zzy.egg-info/SOURCES.txt` & `hotpot-zzy-0.3.0.8/hotpot_zzy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/pyproject.toml` & `hotpot-zzy-0.3.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hotpot-zzy"
-version = "0.3.0.7"
+version = "0.3.0.8"
 readme = "RAEDME.md"
 authors = [
     { name = "Zhiyuan Zhang", email = "ZhiyuanZhang_scu@163.com" },
     { name = "Yue Dong", email = "1320801310@qq.com" },
     { name = "Yuqing Qiu", email = "2022223070045@stu.scu.edu.cn" },
 ]
 classifiers = [
```

### Comparing `hotpot-zzy-0.3.0.7/test/test_amorphous_maker.py` & `hotpot-zzy-0.3.0.8/test/test_amorphous_maker.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/test/test_bundle.py` & `hotpot-zzy-0.3.0.8/test/test_bundle.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/test/test_chemif.py` & `hotpot-zzy-0.3.0.8/test/test_chemif.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.7/test/test_lmp.py` & `hotpot-zzy-0.3.0.8/test/test_lmp.py`

 * *Files identical despite different names*

