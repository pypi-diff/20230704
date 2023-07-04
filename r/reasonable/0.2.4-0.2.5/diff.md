# Comparing `tmp/reasonable-0.2.4.tar.gz` & `tmp/reasonable-0.2.5.tar.gz`

## Comparing `reasonable-0.2.4.tar` & `reasonable-0.2.5.tar`

### file list

```diff
@@ -1,145 +1,145 @@
--rw-r--r--   0        0        0     1156 1970-01-01 00:00:00.000000 reasonable-0.2.4/Cargo.toml
--rw-r--r--   0      501       20      111 2023-07-04 15:21:07.000000 reasonable-0.2.4/.cargo/config
--rw-r--r--   0      501       20     7144 2023-07-04 15:21:07.000000 reasonable-0.2.4/.github/workflows/Python.yml
--rw-r--r--   0      501       20     2428 2023-07-04 15:21:07.000000 reasonable-0.2.4/.github/workflows/builds.yml
--rw-r--r--   0      501       20      542 2023-07-04 15:21:07.000000 reasonable-0.2.4/.github/workflows/manylinux_build.sh
--rw-r--r--   0      501       20      568 2023-07-04 15:21:07.000000 reasonable-0.2.4/.gitignore
--rw-r--r--   0      501       20    16792 2023-07-04 15:21:14.000000 reasonable-0.2.4/Cargo.lock
--rw-r--r--   0      501       20     1519 2023-07-04 15:21:07.000000 reasonable-0.2.4/LICENSE
--rw-r--r--   0      501       20     1608 2023-07-04 15:21:07.000000 reasonable-0.2.4/Makefile
--rw-r--r--   0      501       20     5360 2023-07-04 15:21:07.000000 reasonable-0.2.4/README.md
--rw-r--r--   0      501       20     4490 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/my_benchmark.rs
--rw-r--r--   0      501       20     3755 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/bench.py
--rw-r--r--   0      501       20   438888 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/ACAD(v1.1).ttl
--rw-r--r--   0      501       20    15738 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/AMRL(v1.1).ttl
--rw-r--r--   0      501       20     4663 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/AOB4(v1.1).ttl
--rw-r--r--   0      501       20     2456 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/AQUA(v1.1).ttl
--rw-r--r--   0      501       20   148837 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/ARC(v1.1).ttl
--rw-r--r--   0      501       20     8626 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/ART(v1.1).ttl
--rw-r--r--   0      501       20    32114 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/ARTX(v1.1).ttl
--rw-r--r--   0      501       20    32336 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/ASMUN(v1.1).ttl
--rw-r--r--   0      501       20     5821 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/BIXB(v1.1).ttl
--rw-r--r--   0      501       20   680383 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/BRIG(v1.1).ttl
--rw-r--r--   0      501       20    52446 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/BWFP(v1.1).ttl
--rw-r--r--   0      501       20   103849 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/Bainer(v1.1).ttl
--rw-r--r--   0      501       20     2740 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/C113(v1.1).ttl
--rw-r--r--   0      501       20   234090 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/CHEM(v1.1).ttl
--rw-r--r--   0      501       20   201232 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/CHEMX(v1.1).ttl
--rw-r--r--   0      501       20    26964 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/CONT(v1.1).ttl
--rw-r--r--   0      501       20    23617 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/COWL(v1.1).ttl
--rw-r--r--   0      501       20    56380 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/CRUS(v1.1).ttl
--rw-r--r--   0      501       20     2785 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/CURR(v1.1).ttl
--rw-r--r--   0      501       20   197473 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/DH(v1.1).ttl
--rw-r--r--   0      501       20   435076 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/EPS(v1.1).ttl
--rw-r--r--   0      501       20    27951 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/FDPD(v1.1).ttl
--rw-r--r--   0      501       20   530501 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/GBSF(v1.1).ttl
--rw-r--r--   0      501       20   210071 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/GHA_ICS(v1.1).ttl
--rw-r--r--   0      501       20    48299 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/GIEDT(v1.1).ttl
--rw-r--r--   0      501       20     5808 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/GILM(v1.1).ttl
--rw-r--r--   0      501       20   304349 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/HART(v1.1).ttl
--rw-r--r--   0      501       20     8128 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/HICK(v1.1).ttl
--rw-r--r--   0      501       20     5628 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/HUNT(v1.1).ttl
--rw-r--r--   0      501       20   303396 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/HUTCH(v1.1).ttl
--rw-r--r--   0      501       20   194712 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/HWC(v1.1).ttl
--rw-r--r--   0      501       20    57424 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/JUNGER(v1.1).ttl
--rw-r--r--   0      501       20     6215 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/KERR(v1.1).ttl
--rw-r--r--   0      501       20     6999 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/KING(v1.1).ttl
--rw-r--r--   0      501       20     6609 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/KLEIBER(v1.1).ttl
--rw-r--r--   0      501       20    18419 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/LFH(v1.1).ttl
--rw-r--r--   0      501       20    19160 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/LSA(v1.1).ttl
--rw-r--r--   0      501       20    84768 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/MADDY(v1.1).ttl
--rw-r--r--   0      501       20    28687 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/MANN(v1.1).ttl
--rw-r--r--   0      501       20    15662 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/MATH(v1.1).ttl
--rw-r--r--   0      501       20   131812 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/MEYR(v1.1).ttl
--rw-r--r--   0      501       20    23894 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/MIWF(v1.1).ttl
--rw-r--r--   0      501       20   164159 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/MRAK(v1.1).ttl
--rw-r--r--   0      501       20    18750 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/MSB(v1.1).ttl
--rw-r--r--   0      501       20    11894 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/MSC(v1.1).ttl
--rw-r--r--   0      501       20     3115 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/MSD(v1.1).ttl
--rw-r--r--   0      501       20    42466 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/MU(v1.1).ttl
--rw-r--r--   0      501       20     8421 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/MUSIC(v1.1).ttl
--rw-r--r--   0      501       20    14105 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/OLS(v1.1).ttl
--rw-r--r--   0      501       20   476097 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/PES_ICS(v1.1).ttl
--rw-r--r--   0      501       20     7860 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/PHSL(v1.1).ttl
--rw-r--r--   0      501       20     2785 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/PINE(v1.1).ttl
--rw-r--r--   0      501       20    86053 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/PRB(v1.1).ttl
--rw-r--r--   0      501       20    20839 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/RECH(v1.1).ttl
--rw-r--r--   0      501       20    42143 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/ROES(v1.1).ttl
--rw-r--r--   0      501       20     2454 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/RPL(v1.1).ttl
--rw-r--r--   0      501       20     5498 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/RYER(v1.1).ttl
--rw-r--r--   0      501       20    47682 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/SCC(v1.1).ttl
--rw-r--r--   0      501       20     6683 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/SCHM(v1.1).ttl
--rw-r--r--   0      501       20     2785 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/SEQU(v1.1).ttl
--rw-r--r--   0      501       20   271074 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/SHIELDS(v1.1).ttl
--rw-r--r--   0      501       20   166666 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/SLAB(v1.1).ttl
--rw-r--r--   0      501       20     6312 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/SLEC(v1.1).ttl
--rw-r--r--   0      501       20    63381 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/SMOA(v1.1).ttl
--rw-r--r--   0      501       20   489384 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/SOCS(v1.1).ttl
--rw-r--r--   0      501       20     4380 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/SPRL(v1.1).ttl
--rw-r--r--   0      501       20   222603 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/STOR(v1.1).ttl
--rw-r--r--   0      501       20    32752 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/SURGE3(v1.1).ttl
--rw-r--r--   0      501       20     3657 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/SWL(v1.1).ttl
--rw-r--r--   0      501       20    73442 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/TAPS(v1.1).ttl
--rw-r--r--   0      501       20     2457 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/THOR(v1.1).ttl
--rw-r--r--   0      501       20    91770 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/THUR(v1.1).ttl
--rw-r--r--   0      501       20    26122 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/TUPP(v1.1).ttl
--rw-r--r--   0      501       20    34129 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/VEIH(v1.1).ttl
--rw-r--r--   0      501       20   137513 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/VM2(v1.1).ttl
--rw-r--r--   0      501       20  1100244 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/VM3A(v1.1).ttl
--rw-r--r--   0      501       20     6920 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/VM3B(v1.1).ttl
--rw-r--r--   0      501       20    37918 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/VMEP(v1.1).ttl
--rw-r--r--   0      501       20   130411 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/VMIF(v1.1).ttl
--rw-r--r--   0      501       20    13294 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/VMLF(v1.1).ttl
--rw-r--r--   0      501       20    55576 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/VMTH(v1.1).ttl
--rw-r--r--   0      501       20     4286 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/VMTHB(v1.1).ttl
--rw-r--r--   0      501       20     4286 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/VMTHC(v1.1).ttl
--rw-r--r--   0      501       20    91018 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/WELL(v1.1).ttl
--rw-r--r--   0      501       20    27797 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/WICK(v1.1).ttl
--rw-r--r--   0      501       20    73670 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/WSRC(v1.1).ttl
--rw-r--r--   0      501       20    23245 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/YOUNG(v1.1).ttl
--rw-r--r--   0      501       20    13281 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/avenal-animal-shelter(v1.1).ttl
--rw-r--r--   0      501       20    39438 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/avenal-movie-theatre(v1.1).ttl
--rw-r--r--   0      501       20    10692 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/avenal-public-works-yard(v1.1).ttl
--rw-r--r--   0      501       20    14596 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/avenal-recreation-center(v1.1).ttl
--rw-r--r--   0      501       20    27336 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/avenal-veterans-hall(v1.1).ttl
--rw-r--r--   0      501       20    29969 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/berkeley-corporate-yard(v1.1).ttl
--rw-r--r--   0      501       20    82637 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/ciee(v1.1).ttl
--rw-r--r--   0      501       20    81292 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/ciee-13-dec-2019(v1.1).ttl
--rw-r--r--   0      501       20   474074 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/csu-dominguez-hills(v1.1).ttl
--rw-r--r--   0      501       20    13557 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/garber(v1.1).ttl
--rw-r--r--   0      501       20    24179 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/hayward-station-1(v1.1).ttl
--rw-r--r--   0      501       20    18716 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/hayward-station-8(v1.1).ttl
--rw-r--r--   0      501       20    76388 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/jesse-turner-center(v1.1).ttl
--rw-r--r--   0      501       20    10088 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/local-butcher-shop(v1.1).ttl
--rw-r--r--   0      501       20    21969 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/north-berkeley-senior-center(v1.1).ttl
--rw-r--r--   0      501       20    58913 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/orinda-community-center(v1.1).ttl
--rw-r--r--   0      501       20    98730 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/orinda-public-library(v1.1).ttl
--rw-r--r--   0      501       20    18839 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/rfs(v1.1).ttl
--rw-r--r--   0      501       20   424960 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/sdh(v1.1).ttl
--rw-r--r--   0      501       20    31717 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/south-berkeley-senior-center(v1.1).ttl
--rw-r--r--   0      501       20    32735 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/buildings/word-of-faith-cc(v1.1).ttl
--rw-r--r--   0      501       20       41 2023-07-04 15:21:07.000000 reasonable-0.2.4/benches/python/requirements.txt
--rw-r--r--   0      501       20  2189973 2023-07-04 15:21:07.000000 reasonable-0.2.4/example_models/ontologies/Brick.n3
--rw-r--r--   0      501       20    64515 2023-07-04 15:21:07.000000 reasonable-0.2.4/example_models/ontologies/owl.n3
--rw-r--r--   0      501       20     3812 2023-07-04 15:21:07.000000 reasonable-0.2.4/example_models/ontologies/rdfs.ttl
--rw-r--r--   0      501       20     2263 2023-07-04 15:21:07.000000 reasonable-0.2.4/example_models/small1.n3
--rw-r--r--   0      501       20   707359 2023-07-04 15:21:07.000000 reasonable-0.2.4/example_models/soda_hall.n3
--rw-r--r--   0      501       20    43207 2023-07-04 15:21:07.000000 reasonable-0.2.4/img/benchmark.png
--rw-r--r--   0      501       20    21479 2023-07-04 15:21:07.000000 reasonable-0.2.4/poetry.lock
--rw-r--r--   0      501       20      597 2023-07-04 15:21:07.000000 reasonable-0.2.4/pyproject.toml
--rw-r--r--   0      501       20       84 2023-07-04 15:21:07.000000 reasonable-0.2.4/reasonable/__init__.py
--rwxr-xr-x   0      501       20     1117 2023-07-04 15:21:07.000000 reasonable-0.2.4/scripts/bench_examples.sh
--rwxr-xr-x   0      501       20      318 2023-07-04 15:21:07.000000 reasonable-0.2.4/scripts/convert_to_n3.py
--rwxr-xr-x   0      501       20      323 2023-07-04 15:21:07.000000 reasonable-0.2.4/scripts/reason_owlrl.py
--rw-r--r--   0      501       20     5741 2023-07-04 15:21:07.000000 reasonable-0.2.4/src/common.rs
--rw-r--r--   0      501       20     4181 2023-07-04 15:21:07.000000 reasonable-0.2.4/src/disjoint_sets.rs
--rw-r--r--   0      501       20     2102 2023-07-04 15:21:07.000000 reasonable-0.2.4/src/error.rs
--rw-r--r--   0      501       20     1034 2023-07-04 15:21:07.000000 reasonable-0.2.4/src/index.rs
--rw-r--r--   0      501       20      795 2023-07-04 15:21:07.000000 reasonable-0.2.4/src/lib.rs
--rw-r--r--   0      501       20      620 2023-07-04 15:21:07.000000 reasonable-0.2.4/src/main.rs
--rw-r--r--   0      501       20     6240 2023-07-04 15:21:07.000000 reasonable-0.2.4/src/pyreason.rs
--rw-r--r--   0      501       20    11950 2023-07-04 15:21:07.000000 reasonable-0.2.4/src/query.rs
--rw-r--r--   0      501       20    61875 2023-07-04 15:21:07.000000 reasonable-0.2.4/src/reasoner.rs
--rw-r--r--   0      501       20    26591 2023-07-04 15:21:07.000000 reasonable-0.2.4/src/tests.rs
--rw-r--r--   0      501       20      350 2023-07-04 15:21:07.000000 reasonable-0.2.4/test.py
--rw-r--r--   0        0        0     5731 1970-01-01 00:00:00.000000 reasonable-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1209 1970-01-01 00:00:00.000000 reasonable-0.2.5/Cargo.toml
+-rw-r--r--   0      501       20      111 2023-07-04 15:24:22.000000 reasonable-0.2.5/.cargo/config
+-rw-r--r--   0      501       20     7144 2023-07-04 15:24:22.000000 reasonable-0.2.5/.github/workflows/Python.yml
+-rw-r--r--   0      501       20     2428 2023-07-04 15:24:22.000000 reasonable-0.2.5/.github/workflows/builds.yml
+-rw-r--r--   0      501       20      542 2023-07-04 15:24:22.000000 reasonable-0.2.5/.github/workflows/manylinux_build.sh
+-rw-r--r--   0      501       20      568 2023-07-04 15:24:22.000000 reasonable-0.2.5/.gitignore
+-rw-r--r--   0      501       20    21815 2023-07-04 15:24:30.000000 reasonable-0.2.5/Cargo.lock
+-rw-r--r--   0      501       20     1519 2023-07-04 15:24:22.000000 reasonable-0.2.5/LICENSE
+-rw-r--r--   0      501       20     1608 2023-07-04 15:24:22.000000 reasonable-0.2.5/Makefile
+-rw-r--r--   0      501       20     5360 2023-07-04 15:24:22.000000 reasonable-0.2.5/README.md
+-rw-r--r--   0      501       20     4490 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/my_benchmark.rs
+-rw-r--r--   0      501       20     3755 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/bench.py
+-rw-r--r--   0      501       20   438888 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/ACAD(v1.1).ttl
+-rw-r--r--   0      501       20    15738 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/AMRL(v1.1).ttl
+-rw-r--r--   0      501       20     4663 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/AOB4(v1.1).ttl
+-rw-r--r--   0      501       20     2456 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/AQUA(v1.1).ttl
+-rw-r--r--   0      501       20   148837 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/ARC(v1.1).ttl
+-rw-r--r--   0      501       20     8626 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/ART(v1.1).ttl
+-rw-r--r--   0      501       20    32114 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/ARTX(v1.1).ttl
+-rw-r--r--   0      501       20    32336 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/ASMUN(v1.1).ttl
+-rw-r--r--   0      501       20     5821 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/BIXB(v1.1).ttl
+-rw-r--r--   0      501       20   680383 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/BRIG(v1.1).ttl
+-rw-r--r--   0      501       20    52446 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/BWFP(v1.1).ttl
+-rw-r--r--   0      501       20   103849 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/Bainer(v1.1).ttl
+-rw-r--r--   0      501       20     2740 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/C113(v1.1).ttl
+-rw-r--r--   0      501       20   234090 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/CHEM(v1.1).ttl
+-rw-r--r--   0      501       20   201232 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/CHEMX(v1.1).ttl
+-rw-r--r--   0      501       20    26964 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/CONT(v1.1).ttl
+-rw-r--r--   0      501       20    23617 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/COWL(v1.1).ttl
+-rw-r--r--   0      501       20    56380 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/CRUS(v1.1).ttl
+-rw-r--r--   0      501       20     2785 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/CURR(v1.1).ttl
+-rw-r--r--   0      501       20   197473 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/DH(v1.1).ttl
+-rw-r--r--   0      501       20   435076 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/EPS(v1.1).ttl
+-rw-r--r--   0      501       20    27951 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/FDPD(v1.1).ttl
+-rw-r--r--   0      501       20   530501 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/GBSF(v1.1).ttl
+-rw-r--r--   0      501       20   210071 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/GHA_ICS(v1.1).ttl
+-rw-r--r--   0      501       20    48299 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/GIEDT(v1.1).ttl
+-rw-r--r--   0      501       20     5808 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/GILM(v1.1).ttl
+-rw-r--r--   0      501       20   304349 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/HART(v1.1).ttl
+-rw-r--r--   0      501       20     8128 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/HICK(v1.1).ttl
+-rw-r--r--   0      501       20     5628 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/HUNT(v1.1).ttl
+-rw-r--r--   0      501       20   303396 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/HUTCH(v1.1).ttl
+-rw-r--r--   0      501       20   194712 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/HWC(v1.1).ttl
+-rw-r--r--   0      501       20    57424 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/JUNGER(v1.1).ttl
+-rw-r--r--   0      501       20     6215 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/KERR(v1.1).ttl
+-rw-r--r--   0      501       20     6999 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/KING(v1.1).ttl
+-rw-r--r--   0      501       20     6609 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/KLEIBER(v1.1).ttl
+-rw-r--r--   0      501       20    18419 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/LFH(v1.1).ttl
+-rw-r--r--   0      501       20    19160 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/LSA(v1.1).ttl
+-rw-r--r--   0      501       20    84768 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/MADDY(v1.1).ttl
+-rw-r--r--   0      501       20    28687 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/MANN(v1.1).ttl
+-rw-r--r--   0      501       20    15662 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/MATH(v1.1).ttl
+-rw-r--r--   0      501       20   131812 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/MEYR(v1.1).ttl
+-rw-r--r--   0      501       20    23894 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/MIWF(v1.1).ttl
+-rw-r--r--   0      501       20   164159 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/MRAK(v1.1).ttl
+-rw-r--r--   0      501       20    18750 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/MSB(v1.1).ttl
+-rw-r--r--   0      501       20    11894 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/MSC(v1.1).ttl
+-rw-r--r--   0      501       20     3115 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/MSD(v1.1).ttl
+-rw-r--r--   0      501       20    42466 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/MU(v1.1).ttl
+-rw-r--r--   0      501       20     8421 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/MUSIC(v1.1).ttl
+-rw-r--r--   0      501       20    14105 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/OLS(v1.1).ttl
+-rw-r--r--   0      501       20   476097 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/PES_ICS(v1.1).ttl
+-rw-r--r--   0      501       20     7860 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/PHSL(v1.1).ttl
+-rw-r--r--   0      501       20     2785 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/PINE(v1.1).ttl
+-rw-r--r--   0      501       20    86053 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/PRB(v1.1).ttl
+-rw-r--r--   0      501       20    20839 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/RECH(v1.1).ttl
+-rw-r--r--   0      501       20    42143 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/ROES(v1.1).ttl
+-rw-r--r--   0      501       20     2454 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/RPL(v1.1).ttl
+-rw-r--r--   0      501       20     5498 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/RYER(v1.1).ttl
+-rw-r--r--   0      501       20    47682 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/SCC(v1.1).ttl
+-rw-r--r--   0      501       20     6683 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/SCHM(v1.1).ttl
+-rw-r--r--   0      501       20     2785 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/SEQU(v1.1).ttl
+-rw-r--r--   0      501       20   271074 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/SHIELDS(v1.1).ttl
+-rw-r--r--   0      501       20   166666 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/SLAB(v1.1).ttl
+-rw-r--r--   0      501       20     6312 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/SLEC(v1.1).ttl
+-rw-r--r--   0      501       20    63381 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/SMOA(v1.1).ttl
+-rw-r--r--   0      501       20   489384 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/SOCS(v1.1).ttl
+-rw-r--r--   0      501       20     4380 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/SPRL(v1.1).ttl
+-rw-r--r--   0      501       20   222603 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/STOR(v1.1).ttl
+-rw-r--r--   0      501       20    32752 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/SURGE3(v1.1).ttl
+-rw-r--r--   0      501       20     3657 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/SWL(v1.1).ttl
+-rw-r--r--   0      501       20    73442 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/TAPS(v1.1).ttl
+-rw-r--r--   0      501       20     2457 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/THOR(v1.1).ttl
+-rw-r--r--   0      501       20    91770 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/THUR(v1.1).ttl
+-rw-r--r--   0      501       20    26122 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/TUPP(v1.1).ttl
+-rw-r--r--   0      501       20    34129 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/VEIH(v1.1).ttl
+-rw-r--r--   0      501       20   137513 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/VM2(v1.1).ttl
+-rw-r--r--   0      501       20  1100244 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/VM3A(v1.1).ttl
+-rw-r--r--   0      501       20     6920 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/VM3B(v1.1).ttl
+-rw-r--r--   0      501       20    37918 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/VMEP(v1.1).ttl
+-rw-r--r--   0      501       20   130411 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/VMIF(v1.1).ttl
+-rw-r--r--   0      501       20    13294 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/VMLF(v1.1).ttl
+-rw-r--r--   0      501       20    55576 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/VMTH(v1.1).ttl
+-rw-r--r--   0      501       20     4286 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/VMTHB(v1.1).ttl
+-rw-r--r--   0      501       20     4286 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/VMTHC(v1.1).ttl
+-rw-r--r--   0      501       20    91018 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/WELL(v1.1).ttl
+-rw-r--r--   0      501       20    27797 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/WICK(v1.1).ttl
+-rw-r--r--   0      501       20    73670 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/WSRC(v1.1).ttl
+-rw-r--r--   0      501       20    23245 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/YOUNG(v1.1).ttl
+-rw-r--r--   0      501       20    13281 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/avenal-animal-shelter(v1.1).ttl
+-rw-r--r--   0      501       20    39438 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/avenal-movie-theatre(v1.1).ttl
+-rw-r--r--   0      501       20    10692 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/avenal-public-works-yard(v1.1).ttl
+-rw-r--r--   0      501       20    14596 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/avenal-recreation-center(v1.1).ttl
+-rw-r--r--   0      501       20    27336 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/avenal-veterans-hall(v1.1).ttl
+-rw-r--r--   0      501       20    29969 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/berkeley-corporate-yard(v1.1).ttl
+-rw-r--r--   0      501       20    82637 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/ciee(v1.1).ttl
+-rw-r--r--   0      501       20    81292 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/ciee-13-dec-2019(v1.1).ttl
+-rw-r--r--   0      501       20   474074 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/csu-dominguez-hills(v1.1).ttl
+-rw-r--r--   0      501       20    13557 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/garber(v1.1).ttl
+-rw-r--r--   0      501       20    24179 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/hayward-station-1(v1.1).ttl
+-rw-r--r--   0      501       20    18716 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/hayward-station-8(v1.1).ttl
+-rw-r--r--   0      501       20    76388 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/jesse-turner-center(v1.1).ttl
+-rw-r--r--   0      501       20    10088 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/local-butcher-shop(v1.1).ttl
+-rw-r--r--   0      501       20    21969 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/north-berkeley-senior-center(v1.1).ttl
+-rw-r--r--   0      501       20    58913 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/orinda-community-center(v1.1).ttl
+-rw-r--r--   0      501       20    98730 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/orinda-public-library(v1.1).ttl
+-rw-r--r--   0      501       20    18839 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/rfs(v1.1).ttl
+-rw-r--r--   0      501       20   424960 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/sdh(v1.1).ttl
+-rw-r--r--   0      501       20    31717 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/south-berkeley-senior-center(v1.1).ttl
+-rw-r--r--   0      501       20    32735 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/buildings/word-of-faith-cc(v1.1).ttl
+-rw-r--r--   0      501       20       41 2023-07-04 15:24:22.000000 reasonable-0.2.5/benches/python/requirements.txt
+-rw-r--r--   0      501       20  2189973 2023-07-04 15:24:22.000000 reasonable-0.2.5/example_models/ontologies/Brick.n3
+-rw-r--r--   0      501       20    64515 2023-07-04 15:24:22.000000 reasonable-0.2.5/example_models/ontologies/owl.n3
+-rw-r--r--   0      501       20     3812 2023-07-04 15:24:22.000000 reasonable-0.2.5/example_models/ontologies/rdfs.ttl
+-rw-r--r--   0      501       20     2263 2023-07-04 15:24:22.000000 reasonable-0.2.5/example_models/small1.n3
+-rw-r--r--   0      501       20   707359 2023-07-04 15:24:22.000000 reasonable-0.2.5/example_models/soda_hall.n3
+-rw-r--r--   0      501       20    43207 2023-07-04 15:24:22.000000 reasonable-0.2.5/img/benchmark.png
+-rw-r--r--   0      501       20    21479 2023-07-04 15:24:22.000000 reasonable-0.2.5/poetry.lock
+-rw-r--r--   0      501       20      597 2023-07-04 15:24:22.000000 reasonable-0.2.5/pyproject.toml
+-rw-r--r--   0      501       20       84 2023-07-04 15:24:22.000000 reasonable-0.2.5/reasonable/__init__.py
+-rwxr-xr-x   0      501       20     1117 2023-07-04 15:24:22.000000 reasonable-0.2.5/scripts/bench_examples.sh
+-rwxr-xr-x   0      501       20      318 2023-07-04 15:24:22.000000 reasonable-0.2.5/scripts/convert_to_n3.py
+-rwxr-xr-x   0      501       20      323 2023-07-04 15:24:22.000000 reasonable-0.2.5/scripts/reason_owlrl.py
+-rw-r--r--   0      501       20     5741 2023-07-04 15:24:22.000000 reasonable-0.2.5/src/common.rs
+-rw-r--r--   0      501       20     4181 2023-07-04 15:24:22.000000 reasonable-0.2.5/src/disjoint_sets.rs
+-rw-r--r--   0      501       20     2102 2023-07-04 15:24:22.000000 reasonable-0.2.5/src/error.rs
+-rw-r--r--   0      501       20     1034 2023-07-04 15:24:22.000000 reasonable-0.2.5/src/index.rs
+-rw-r--r--   0      501       20      795 2023-07-04 15:24:22.000000 reasonable-0.2.5/src/lib.rs
+-rw-r--r--   0      501       20     1128 2023-07-04 15:24:22.000000 reasonable-0.2.5/src/main.rs
+-rw-r--r--   0      501       20     6239 2023-07-04 15:24:22.000000 reasonable-0.2.5/src/pyreason.rs
+-rw-r--r--   0      501       20    11950 2023-07-04 15:24:22.000000 reasonable-0.2.5/src/query.rs
+-rw-r--r--   0      501       20    61832 2023-07-04 15:24:22.000000 reasonable-0.2.5/src/reasoner.rs
+-rw-r--r--   0      501       20    26591 2023-07-04 15:24:22.000000 reasonable-0.2.5/src/tests.rs
+-rw-r--r--   0      501       20      350 2023-07-04 15:24:22.000000 reasonable-0.2.5/test.py
+-rw-r--r--   0        0        0     5731 1970-01-01 00:00:00.000000 reasonable-0.2.5/PKG-INFO
```

### Comparing `reasonable-0.2.4/Cargo.toml` & `reasonable-0.2.5/Cargo.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "reasonable"
-version = "0.2.4"
+version = "0.2.5"
 authors = ["Gabe Fierro <gtfierro@mines.edu>"]
 repository = "https://github.com/gtfierro/reasonable"
 homepage = "https://brickschema.org/"
 license-file = "LICENSE"
 readme = "README.md"
 description = "An OWL 2 RL reasoner with reasonable performance"
 edition = "2018"
@@ -34,14 +34,15 @@
 regex = "1.3.9"
 serde = "1.0"
 serde_json = "1.0"
 serde_derive = "1.0"
 tinytemplate = "1.2.1"
 anyhow = "1.0.60"
 pyo3 = { version = "0.17", features = ["extension-module", "abi3-py37"]}
+clap = { version = "4.3.10", features = ["derive"] }
 
 [profile.release]
 debug = true
 
 [package.metadata.maturin]
 name = "reasonable"
```

### Comparing `reasonable-0.2.4/.github/workflows/Python.yml` & `reasonable-0.2.5/.github/workflows/Python.yml`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/.github/workflows/builds.yml` & `reasonable-0.2.5/.github/workflows/builds.yml`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/.github/workflows/manylinux_build.sh` & `reasonable-0.2.5/.github/workflows/manylinux_build.sh`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/.gitignore` & `reasonable-0.2.5/.gitignore`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/Cargo.lock` & `reasonable-0.2.5/Cargo.lock`

 * *Files 15% similar despite different names*

```diff
@@ -8,26 +8,75 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "43f6cb1bf222025340178f382c426f13757b2960e89779dfcb319c32542a5a41"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
+name = "anstream"
+version = "0.3.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0ca84f3628370c59db74ee214b3263d58f9aadd9b4fe7e711fd87dc452b7f163"
+dependencies = [
+ "anstyle",
+ "anstyle-parse",
+ "anstyle-query",
+ "anstyle-wincon",
+ "colorchoice",
+ "is-terminal",
+ "utf8parse",
+]
+
+[[package]]
+name = "anstyle"
+version = "1.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3a30da5c5f2d5e72842e00bcb57657162cdabef0931f40e2deb9b4140440cecd"
+
+[[package]]
+name = "anstyle-parse"
+version = "0.2.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "938874ff5980b03a87c5524b3ae5b59cf99b1d6bc836848df7bc5ada9643c333"
+dependencies = [
+ "utf8parse",
+]
+
+[[package]]
+name = "anstyle-query"
+version = "1.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5ca11d4be1bab0c8bc8734a9aa7bf4ee8316d462a08c6ac5052f888fef5b494b"
+dependencies = [
+ "windows-sys",
+]
+
+[[package]]
+name = "anstyle-wincon"
+version = "1.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "180abfa45703aebe0093f79badacc01b8fd4ea2e35118747e5811127f926e188"
+dependencies = [
+ "anstyle",
+ "windows-sys",
+]
+
+[[package]]
 name = "anyhow"
 version = "1.0.71"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c7d0618f0e0b7e8ff11427422b64564d5fb0be1940354bfe2e0529b18a9d9b8"
 
 [[package]]
 name = "atty"
 version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d9b39be18770d11421cdb1b9947a45dd3f37e93092cbf377614828a319d5fee8"
 dependencies = [
- "hermit-abi",
+ "hermit-abi 0.1.19",
  "libc",
  "winapi",
 ]
 
 [[package]]
 name = "autocfg"
 version = "1.1.0"
@@ -37,26 +86,85 @@
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
+name = "bitflags"
+version = "2.3.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "630be753d4e58660abd17930c71b647fe46c27ea6b63cc59e1e3851406972e42"
+
+[[package]]
 name = "byteorder"
 version = "0.5.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0fc10e8cc6b2580fda3f36eb6dc5316657f812a3df879a44a66fc9f0fdbc4855"
 
 [[package]]
+name = "cc"
+version = "1.0.79"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "50d30906286121d95be3d479533b458f87493b30a4b5f79a607db8f5d11aa91f"
+
+[[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
+name = "clap"
+version = "4.3.10"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "384e169cc618c613d5e3ca6404dda77a8685a63e08660dcc64abaf7da7cb0c7a"
+dependencies = [
+ "clap_builder",
+ "clap_derive",
+ "once_cell",
+]
+
+[[package]]
+name = "clap_builder"
+version = "4.3.10"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ef137bbe35aab78bdb468ccfba75a5f4d8321ae011d34063770780545176af2d"
+dependencies = [
+ "anstream",
+ "anstyle",
+ "clap_lex",
+ "strsim",
+]
+
+[[package]]
+name = "clap_derive"
+version = "4.3.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b8cd2b2a819ad6eec39e8f1d6b53001af1e5469f8c177579cdaeb313115b825f"
+dependencies = [
+ "heck",
+ "proc-macro2",
+ "quote",
+ "syn 2.0.23",
+]
+
+[[package]]
+name = "clap_lex"
+version = "0.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2da6da31387c7e4ef160ffab6d5e7f00c42626fe39aea70a7b0f1773f7dd6c1b"
+
+[[package]]
+name = "colorchoice"
+version = "1.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "acbf1af155f9b9ef647e42cdc158db4b64a1b61f743629225fde6f3e0be2a7c7"
+
+[[package]]
 name = "datafrog"
 version = "2.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a0afaad2b26fa326569eb264b1363e8ae3357618c43982b3f285f0774ce76b69"
 
 [[package]]
 name = "disjoint-sets"
@@ -80,14 +188,35 @@
  "humantime",
  "log",
  "regex",
  "termcolor",
 ]
 
 [[package]]
+name = "errno"
+version = "0.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4bcfec3a70f97c962c307b2d2c56e358cf1d00b558d74262b5f929ee8cc7e73a"
+dependencies = [
+ "errno-dragonfly",
+ "libc",
+ "windows-sys",
+]
+
+[[package]]
+name = "errno-dragonfly"
+version = "0.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "aa68f1b12764fab894d2755d2518754e71b4fd80ecfb822714a1206c2aab39bf"
+dependencies = [
+ "cc",
+ "libc",
+]
+
+[[package]]
 name = "farmhash"
 version = "1.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f35ce9c8fb9891c75ceadbc330752951a4e369b50af10775955aeb9af3eee34b"
 
 [[package]]
 name = "getrandom"
@@ -97,23 +226,35 @@
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
+name = "heck"
+version = "0.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
+
+[[package]]
 name = "hermit-abi"
 version = "0.1.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "62b467343b94ba476dcb2500d242dadbb39557df889310ac77c5d99100aaac33"
 dependencies = [
  "libc",
 ]
 
 [[package]]
+name = "hermit-abi"
+version = "0.3.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "443144c8cdadd93ebf52ddb4056d257f5b52c04d3c804e657d19eb73fc33668b"
+
+[[package]]
 name = "humantime"
 version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "df004cfca50ef23c36850aaaa59ad52cc70d0e90243c3c7737a4dd32dc7a3c4f"
 dependencies = [
  "quick-error",
 ]
@@ -121,14 +262,25 @@
 [[package]]
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
+name = "is-terminal"
+version = "0.4.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "24fddda5af7e54bf7da53067d6e802dbcc381d0a8eef629df528e3ebf68755cb"
+dependencies = [
+ "hermit-abi 0.3.2",
+ "rustix",
+ "windows-sys",
+]
+
+[[package]]
 name = "itertools"
 version = "0.8.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f56a2d0bc861f9165be4eb3442afd3c236d8a98afd426f65d92324ae1091a484"
 dependencies = [
  "either",
 ]
@@ -142,14 +294,20 @@
 [[package]]
 name = "libc"
 version = "0.2.147"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b4668fb0ea861c1df094127ac5f1da3409a82116a4ba74fca2e58ef927159bb3"
 
 [[package]]
+name = "linux-raw-sys"
+version = "0.4.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "09fc20d2ca12cb9f044c93e3bd6d32d523e6e2ec3db4f7b2939cd99026ecd3f0"
+
+[[package]]
 name = "lock_api"
 version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
 dependencies = [
  "autocfg",
  "scopeguard",
@@ -352,17 +510,18 @@
 name = "rdf"
 version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bb1725bf0133fe4a3279e18efd6d69f952cb8356bf8b835023042e1b98d4c646"
 
 [[package]]
 name = "reasonable"
-version = "0.2.4"
+version = "0.2.5"
 dependencies = [
  "anyhow",
+ "clap",
  "datafrog",
  "disjoint-sets",
  "env_logger",
  "farmhash",
  "itertools",
  "log",
  "oxrdf",
@@ -380,15 +539,15 @@
 
 [[package]]
 name = "redox_syscall"
 version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
 dependencies = [
- "bitflags",
+ "bitflags 1.3.2",
 ]
 
 [[package]]
 name = "regex"
 version = "1.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d0ab3ca65655bb1e41f2a8c8cd662eb4fb035e67c3f78da1d61dffe89d07300f"
@@ -427,14 +586,27 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4af20e5d3e44732a57489fa297768ca29361b54fbc3b20cdeb738fa6932cc22d"
 dependencies = [
  "byteorder",
 ]
 
 [[package]]
+name = "rustix"
+version = "0.38.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "aabcb0461ebd01d6b79945797c27f8529082226cb630a9865a71870ff63532a4"
+dependencies = [
+ "bitflags 2.3.3",
+ "errno",
+ "libc",
+ "linux-raw-sys",
+ "windows-sys",
+]
+
+[[package]]
 name = "ryu"
 version = "1.0.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fe232bdf6be8c8de797b22184ee71118d63780ea42ac85b61d1baa6d3b782ae9"
 
 [[package]]
 name = "scopeguard"
@@ -473,14 +645,20 @@
 [[package]]
 name = "smallvec"
 version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
 
 [[package]]
+name = "strsim"
+version = "0.10.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "73473c0e59e6d5812c5dfe2a064a6444949f089e20eec9a2e5506596494e4623"
+
+[[package]]
 name = "syn"
 version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
 dependencies = [
  "proc-macro2",
  "quote",
@@ -532,14 +710,20 @@
 [[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
 [[package]]
+name = "utf8parse"
+version = "0.2.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "711b9620af191e0cdc7468a8d14e709c3dcdb115b36f838e601583af800a370a"
+
+[[package]]
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "winapi"
@@ -569,14 +753,23 @@
 [[package]]
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
+name = "windows-sys"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
+dependencies = [
+ "windows-targets",
+]
+
+[[package]]
 name = "windows-targets"
 version = "0.48.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "05d4b17490f70499f20b9e791dcf6a299785ce8af4d709018206dc5b4953e95f"
 dependencies = [
  "windows_aarch64_gnullvm",
  "windows_aarch64_msvc",
```

### Comparing `reasonable-0.2.4/LICENSE` & `reasonable-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/Makefile` & `reasonable-0.2.5/Makefile`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/README.md` & `reasonable-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/my_benchmark.rs` & `reasonable-0.2.5/benches/my_benchmark.rs`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/bench.py` & `reasonable-0.2.5/benches/python/bench.py`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/ACAD(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/ACAD(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/AMRL(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/AMRL(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/AOB4(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/AOB4(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/AQUA(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/AQUA(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/ARC(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/ARC(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/ART(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/ART(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/ARTX(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/ARTX(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/ASMUN(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/ASMUN(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/BIXB(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/BIXB(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/BRIG(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/BRIG(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/BWFP(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/BWFP(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/Bainer(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/Bainer(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/C113(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/C113(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/CHEM(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/CHEM(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/CHEMX(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/CHEMX(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/CONT(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/CONT(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/COWL(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/COWL(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/CRUS(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/CRUS(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/CURR(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/CURR(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/DH(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/DH(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/EPS(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/EPS(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/FDPD(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/FDPD(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/GBSF(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/GBSF(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/GHA_ICS(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/GHA_ICS(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/GIEDT(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/GIEDT(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/GILM(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/GILM(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/HART(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/HART(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/HICK(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/HICK(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/HUNT(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/HUNT(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/HUTCH(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/HUTCH(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/HWC(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/HWC(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/JUNGER(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/JUNGER(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/KERR(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/KERR(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/KING(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/KING(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/KLEIBER(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/KLEIBER(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/LFH(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/LFH(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/LSA(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/LSA(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/MADDY(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/MADDY(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/MANN(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/MANN(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/MATH(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/MATH(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/MEYR(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/MEYR(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/MIWF(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/MIWF(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/MRAK(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/MRAK(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/MSB(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/MSB(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/MSC(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/MSC(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/MSD(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/MSD(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/MU(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/MU(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/MUSIC(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/MUSIC(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/OLS(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/OLS(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/PES_ICS(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/PES_ICS(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/PHSL(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/PHSL(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/PINE(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/PINE(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/PRB(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/PRB(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/RECH(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/RECH(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/ROES(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/ROES(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/RPL(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/RPL(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/RYER(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/RYER(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/SCC(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/SCC(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/SCHM(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/SCHM(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/SEQU(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/SEQU(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/SHIELDS(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/SHIELDS(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/SLAB(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/SLAB(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/SLEC(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/SLEC(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/SMOA(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/SMOA(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/SOCS(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/SOCS(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/SPRL(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/SPRL(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/STOR(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/STOR(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/SURGE3(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/SURGE3(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/SWL(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/SWL(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/TAPS(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/TAPS(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/THOR(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/THOR(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/THUR(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/THUR(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/TUPP(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/TUPP(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/VEIH(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/VEIH(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/VM2(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/VM2(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/VM3A(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/VM3A(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/VM3B(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/VM3B(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/VMEP(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/VMEP(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/VMIF(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/VMIF(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/VMLF(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/VMLF(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/VMTH(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/VMTH(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/VMTHB(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/VMTHB(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/VMTHC(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/VMTHC(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/WELL(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/WELL(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/WICK(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/WICK(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/WSRC(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/WSRC(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/YOUNG(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/YOUNG(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/avenal-animal-shelter(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/avenal-animal-shelter(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/avenal-movie-theatre(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/avenal-movie-theatre(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/avenal-public-works-yard(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/avenal-public-works-yard(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/avenal-recreation-center(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/avenal-recreation-center(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/avenal-veterans-hall(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/avenal-veterans-hall(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/berkeley-corporate-yard(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/berkeley-corporate-yard(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/ciee(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/ciee(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/ciee-13-dec-2019(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/ciee-13-dec-2019(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/csu-dominguez-hills(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/csu-dominguez-hills(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/garber(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/garber(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/hayward-station-1(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/hayward-station-1(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/hayward-station-8(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/hayward-station-8(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/jesse-turner-center(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/jesse-turner-center(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/local-butcher-shop(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/local-butcher-shop(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/north-berkeley-senior-center(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/north-berkeley-senior-center(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/orinda-community-center(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/orinda-community-center(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/orinda-public-library(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/orinda-public-library(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/rfs(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/rfs(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/sdh(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/sdh(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/south-berkeley-senior-center(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/south-berkeley-senior-center(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/benches/python/buildings/word-of-faith-cc(v1.1).ttl` & `reasonable-0.2.5/benches/python/buildings/word-of-faith-cc(v1.1).ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/example_models/ontologies/Brick.n3` & `reasonable-0.2.5/example_models/ontologies/Brick.n3`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/example_models/ontologies/owl.n3` & `reasonable-0.2.5/example_models/ontologies/owl.n3`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/example_models/ontologies/rdfs.ttl` & `reasonable-0.2.5/example_models/ontologies/rdfs.ttl`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/example_models/small1.n3` & `reasonable-0.2.5/example_models/small1.n3`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/example_models/soda_hall.n3` & `reasonable-0.2.5/example_models/soda_hall.n3`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/img/benchmark.png` & `reasonable-0.2.5/img/benchmark.png`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/poetry.lock` & `reasonable-0.2.5/poetry.lock`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/pyproject.toml` & `reasonable-0.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/scripts/bench_examples.sh` & `reasonable-0.2.5/scripts/bench_examples.sh`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/src/common.rs` & `reasonable-0.2.5/src/common.rs`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/src/disjoint_sets.rs` & `reasonable-0.2.5/src/disjoint_sets.rs`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/src/error.rs` & `reasonable-0.2.5/src/error.rs`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/src/index.rs` & `reasonable-0.2.5/src/index.rs`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/src/lib.rs` & `reasonable-0.2.5/src/lib.rs`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/src/pyreason.rs` & `reasonable-0.2.5/src/pyreason.rs`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,14 @@
                 }
                 (None, None) => rdflib.getattr("Literal")?.call1((literal.value(),))?,
             }
         }
         Term::BlankNode(id) => rdflib
             .getattr("BNode")?
             .call1((id.clone().into_string(),))?,
-
     };
     Ok(res)
 }
 
 #[pyclass(unsendable)]
 pub struct PyReasoner {
     reasoner: reasoner::Reasoner,
```

### Comparing `reasonable-0.2.4/src/query.rs` & `reasonable-0.2.5/src/query.rs`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/src/reasoner.rs` & `reasonable-0.2.5/src/reasoner.rs`

 * *Files 1% similar despite different names*

```diff
@@ -289,15 +289,14 @@
             })?;
         } else {
             return Err(Error::new(
                 ErrorKind::Other,
                 "no parser for file (only ttl and n3)",
             ));
         }
-        println!("filename {}", filename);
 
         //let graph = parser.read_triples(f)?.collect::<Result<Vec<_>,_>>()?;
 
         let mut triples: Vec<(URI, (URI, URI))> = graph
             .iter()
             .map(|_triple| {
                 let triple = _triple;
```

### Comparing `reasonable-0.2.4/src/tests.rs` & `reasonable-0.2.5/src/tests.rs`

 * *Files identical despite different names*

### Comparing `reasonable-0.2.4/PKG-INFO` & `reasonable-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reasonable
-Version: 0.2.4
+Version: 0.2.5
 Summary: An OWL 2 RL reasoner with reasonable performance
 Home-Page: https://brickschema.org/
 Author: Gabe Fierro <gtfierro@mines.edu>
 Author-email: Gabe Fierro <gtfierro@mines.edu>
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Source Code, https://github.com/gtfierro/reasonable
```

