# Comparing `tmp/ypricemagic-2.5.5.tar.gz` & `tmp/ypricemagic-2.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ypricemagic-2.5.5.tar", last modified: Mon Jul  3 03:06:25 2023, max compression
+gzip compressed data, was "ypricemagic-2.5.6.tar", last modified: Tue Jul  4 11:57:28 2023, max compression
```

## Comparing `ypricemagic-2.5.5.tar` & `ypricemagic-2.5.6.tar`

### file list

```diff
@@ -1,153 +1,154 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 03:06:25.419298 ypricemagic-2.5.5/
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/.env.sample
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 03:06:25.399297 ypricemagic-2.5.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 03:06:25.403298 ypricemagic-2.5.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (122)     3229 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/.github/workflows/pytest.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      632 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      139 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      120 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)      406 2023-07-03 03:06:25.419298 ypricemagic-2.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      776 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)      168 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-07-03 03:06:25.419298 ypricemagic-2.5.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      840 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 03:06:25.403298 ypricemagic-2.5.5/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 03:06:25.403298 ypricemagic-2.5.5/tests/classes/
--rw-r--r--   0 runner    (1001) docker     (122)     3851 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/tests/classes/test_erc20.py
--rw-r--r--   0 runner    (1001) docker     (122)      550 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/tests/classes/test_singleton.py
--rw-r--r--   0 runner    (1001) docker     (122)      144 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     2202 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/tests/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 03:06:25.403298 ypricemagic-2.5.5/tests/prices/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/tests/prices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 03:06:25.403298 ypricemagic-2.5.5/tests/prices/dex/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/tests/prices/dex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      316 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/tests/prices/dex/test_balancer.py
--rw-r--r--   0 runner    (1001) docker     (122)     2918 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/tests/prices/dex/test_uniswap.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 03:06:25.403298 ypricemagic-2.5.5/tests/prices/lending/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/tests/prices/lending/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7133 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/tests/prices/lending/test_aave.py
--rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/tests/prices/lending/test_compound.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 03:06:25.403298 ypricemagic-2.5.5/tests/prices/stable_swap/
--rw-r--r--   0 runner    (1001) docker     (122)      379 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/tests/prices/stable_swap/test_curve.py
--rw-r--r--   0 runner    (1001) docker     (122)     7040 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/tests/prices/test_chainlink.py
--rw-r--r--   0 runner    (1001) docker     (122)      471 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/tests/prices/test_gearbox.py
--rw-r--r--   0 runner    (1001) docker     (122)     4496 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/tests/prices/test_magic.py
--rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/tests/prices/test_popsicle.py
--rw-r--r--   0 runner    (1001) docker     (122)     1116 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/tests/prices/test_synthetix.py
--rw-r--r--   0 runner    (1001) docker     (122)     1017 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/tests/prices/test_yearn.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 03:06:25.403298 ypricemagic-2.5.5/tests/prices/tokenized_fund/
--rw-r--r--   0 runner    (1001) docker     (122)      236 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/tests/prices/tokenized_fund/test_piedao.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 03:06:25.403298 ypricemagic-2.5.5/tests/prices/utils/
--rw-r--r--   0 runner    (1001) docker     (122)     2025 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/tests/prices/utils/test_buckets.py
--rw-r--r--   0 runner    (1001) docker     (122)      492 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/tests/test_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 03:06:25.403298 ypricemagic-2.5.5/y/
--rw-r--r--   0 runner    (1001) docker     (122)     1876 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 03:06:25.407297 ypricemagic-2.5.5/y/classes/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7773 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/classes/common.py
--rw-r--r--   0 runner    (1001) docker     (122)     2406 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/classes/singleton.py
--rw-r--r--   0 runner    (1001) docker     (122)    10017 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    20593 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/contracts.py
--rw-r--r--   0 runner    (1001) docker     (122)      493 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/convert.py
--rw-r--r--   0 runner    (1001) docker     (122)      576 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (122)     1170 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/decorators.py
--rw-r--r--   0 runner    (1001) docker     (122)     3187 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/erc20.py
--rw-r--r--   0 runner    (1001) docker     (122)     2488 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 03:06:25.407297 ypricemagic-2.5.5/y/interfaces/
--rw-r--r--   0 runner    (1001) docker     (122)     6400 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/interfaces/ERC20.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 03:06:25.407297 ypricemagic-2.5.5/y/interfaces/balancer/
--rw-r--r--   0 runner    (1001) docker     (122)    23102 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/interfaces/balancer/WeightedPool.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/interfaces/balancer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 03:06:25.407297 ypricemagic-2.5.5/y/interfaces/compound/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/interfaces/compound/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    32517 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/interfaces/compound/unitroller.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 03:06:25.407297 ypricemagic-2.5.5/y/interfaces/curve/
--rw-r--r--   0 runner    (1001) docker     (122)     7124 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/interfaces/curve/CurveRegistry.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/interfaces/curve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3802 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/interfaces/multicall2.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 03:06:25.407297 ypricemagic-2.5.5/y/interfaces/uniswap/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/interfaces/uniswap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2248 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/interfaces/uniswap/factoryv2.py
--rw-r--r--   0 runner    (1001) docker     (122)     2283 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/interfaces/uniswap/quoterv3.py
--rw-r--r--   0 runner    (1001) docker     (122)     3271 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/networks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 03:06:25.407297 ypricemagic-2.5.5/y/prices/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/prices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2910 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/prices/band.py
--rw-r--r--   0 runner    (1001) docker     (122)    19868 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/prices/chainlink.py
--rw-r--r--   0 runner    (1001) docker     (122)     1073 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/prices/convex.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 03:06:25.407297 ypricemagic-2.5.5/y/prices/dex/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/prices/dex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 03:06:25.411298 ypricemagic-2.5.5/y/prices/dex/balancer/
--rw-r--r--   0 runner    (1001) docker     (122)       64 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/prices/dex/balancer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2905 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/prices/dex/balancer/balancer.py
--rw-r--r--   0 runner    (1001) docker     (122)     6669 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/prices/dex/balancer/v1.py
--rw-r--r--   0 runner    (1001) docker     (122)    10788 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/prices/dex/balancer/v2.py
--rw-r--r--   0 runner    (1001) docker     (122)     2544 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/prices/dex/genericamm.py
--rw-r--r--   0 runner    (1001) docker     (122)     2206 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/prices/dex/mooniswap.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 03:06:25.411298 ypricemagic-2.5.5/y/prices/dex/uniswap/
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/prices/dex/uniswap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6370 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/prices/dex/uniswap/uniswap.py
--rw-r--r--   0 runner    (1001) docker     (122)     2125 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/prices/dex/uniswap/v1.py
--rw-r--r--   0 runner    (1001) docker     (122)    23293 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/prices/dex/uniswap/v2.py
--rw-r--r--   0 runner    (1001) docker     (122)    12588 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/prices/dex/uniswap/v2_forks.py
--rw-r--r--   0 runner    (1001) docker     (122)     3949 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/prices/dex/uniswap/v3.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 03:06:25.411298 ypricemagic-2.5.5/y/prices/eth_derivs/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/prices/eth_derivs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1076 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/prices/eth_derivs/creth.py
--rw-r--r--   0 runner    (1001) docker     (122)     1272 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/prices/eth_derivs/wsteth.py
--rw-r--r--   0 runner    (1001) docker     (122)     2940 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/prices/gearbox.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 03:06:25.411298 ypricemagic-2.5.5/y/prices/lending/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/prices/lending/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10245 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/prices/lending/aave.py
--rw-r--r--   0 runner    (1001) docker     (122)    10528 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/prices/lending/compound.py
--rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/prices/lending/ib.py
--rw-r--r--   0 runner    (1001) docker     (122)    11390 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/prices/magic.py
--rw-r--r--   0 runner    (1001) docker     (122)      815 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/prices/one_to_one.py
--rw-r--r--   0 runner    (1001) docker     (122)     2490 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/prices/popsicle.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 03:06:25.415298 ypricemagic-2.5.5/y/prices/stable_swap/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/prices/stable_swap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/prices/stable_swap/belt.py
--rw-r--r--   0 runner    (1001) docker     (122)    22296 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/prices/stable_swap/curve.py
--rw-r--r--   0 runner    (1001) docker     (122)     1597 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/prices/stable_swap/ellipsis.py
--rw-r--r--   0 runner    (1001) docker     (122)      832 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/prices/stable_swap/froyo.py
--rw-r--r--   0 runner    (1001) docker     (122)     1098 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/prices/stable_swap/mstablefeederpool.py
--rw-r--r--   0 runner    (1001) docker     (122)     3259 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/prices/stable_swap/saddle.py
--rw-r--r--   0 runner    (1001) docker     (122)     3887 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/prices/synthetix.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 03:06:25.415298 ypricemagic-2.5.5/y/prices/tokenized_fund/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/prices/tokenized_fund/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1079 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/prices/tokenized_fund/basketdao.py
--rw-r--r--   0 runner    (1001) docker     (122)     1630 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/prices/tokenized_fund/gelato.py
--rw-r--r--   0 runner    (1001) docker     (122)     2351 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/prices/tokenized_fund/piedao.py
--rw-r--r--   0 runner    (1001) docker     (122)     2257 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/prices/tokenized_fund/tokensets.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 03:06:25.415298 ypricemagic-2.5.5/y/prices/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      100 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/prices/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4756 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/prices/utils/buckets.py
--rw-r--r--   0 runner    (1001) docker     (122)     8741 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/prices/utils/sense_check.py
--rw-r--r--   0 runner    (1001) docker     (122)     8174 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/prices/utils/ypriceapi.py
--rw-r--r--   0 runner    (1001) docker     (122)     5879 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/prices/yearn.py
--rw-r--r--   0 runner    (1001) docker     (122)     5499 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/time.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 03:06:25.419298 ypricemagic-2.5.5/y/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      178 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (122)      864 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/utils/client.py
--rw-r--r--   0 runner    (1001) docker     (122)      113 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/utils/dank_mids.py
--rw-r--r--   0 runner    (1001) docker     (122)     7970 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/utils/events.py
--rw-r--r--   0 runner    (1001) docker     (122)      669 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/utils/fakes.py
--rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (122)     2726 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/utils/middleware.py
--rw-r--r--   0 runner    (1001) docker     (122)    11228 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/utils/multicall.py
--rw-r--r--   0 runner    (1001) docker     (122)    14776 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/y/utils/raw_calls.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 03:06:25.419298 ypricemagic-2.5.5/ypricemagic/
--rw-r--r--   0 runner    (1001) docker     (122)      404 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/ypricemagic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      626 2023-07-03 03:06:10.000000 ypricemagic-2.5.5/ypricemagic/magic.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-03 03:06:25.419298 ypricemagic-2.5.5/ypricemagic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      406 2023-07-03 03:06:25.000000 ypricemagic-2.5.5/ypricemagic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3161 2023-07-03 03:06:25.000000 ypricemagic-2.5.5/ypricemagic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-03 03:06:25.000000 ypricemagic-2.5.5/ypricemagic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      168 2023-07-03 03:06:25.000000 ypricemagic-2.5.5/ypricemagic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-07-03 03:06:25.000000 ypricemagic-2.5.5/ypricemagic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:28.722522 ypricemagic-2.5.6/
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/.env.sample
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:28.698522 ypricemagic-2.5.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:28.702522 ypricemagic-2.5.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     3229 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      632 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      139 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      120 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      406 2023-07-04 11:57:28.722522 ypricemagic-2.5.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      776 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      168 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-07-04 11:57:28.722522 ypricemagic-2.5.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      840 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:28.706522 ypricemagic-2.5.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:28.706522 ypricemagic-2.5.6/tests/classes/
+-rw-r--r--   0 runner    (1001) docker     (122)     3851 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/tests/classes/test_erc20.py
+-rw-r--r--   0 runner    (1001) docker     (122)      550 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/tests/classes/test_singleton.py
+-rw-r--r--   0 runner    (1001) docker     (122)      144 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2248 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/tests/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:28.706522 ypricemagic-2.5.6/tests/prices/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/tests/prices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:28.706522 ypricemagic-2.5.6/tests/prices/dex/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/tests/prices/dex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      586 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/tests/prices/dex/test_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2918 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/tests/prices/dex/test_uniswap.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:28.706522 ypricemagic-2.5.6/tests/prices/lending/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/tests/prices/lending/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7133 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/tests/prices/lending/test_aave.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/tests/prices/lending/test_compound.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:28.706522 ypricemagic-2.5.6/tests/prices/stable_swap/
+-rw-r--r--   0 runner    (1001) docker     (122)      379 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/tests/prices/stable_swap/test_curve.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7040 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/tests/prices/test_chainlink.py
+-rw-r--r--   0 runner    (1001) docker     (122)      471 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/tests/prices/test_gearbox.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4496 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/tests/prices/test_magic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/tests/prices/test_popsicle.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1116 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/tests/prices/test_synthetix.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1017 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/tests/prices/test_yearn.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:28.706522 ypricemagic-2.5.6/tests/prices/tokenized_fund/
+-rw-r--r--   0 runner    (1001) docker     (122)      236 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/tests/prices/tokenized_fund/test_piedao.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:28.706522 ypricemagic-2.5.6/tests/prices/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     2025 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/tests/prices/utils/test_buckets.py
+-rw-r--r--   0 runner    (1001) docker     (122)      492 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/tests/test_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:28.710522 ypricemagic-2.5.6/y/
+-rw-r--r--   0 runner    (1001) docker     (122)      209 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/ENVIRONMENT_VARIABLES.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1876 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:28.710522 ypricemagic-2.5.6/y/classes/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7773 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/classes/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2406 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/classes/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9930 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20712 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/contracts.py
+-rw-r--r--   0 runner    (1001) docker     (122)      493 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/convert.py
+-rw-r--r--   0 runner    (1001) docker     (122)      576 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2130 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3187 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/erc20.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2868 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:28.710522 ypricemagic-2.5.6/y/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (122)     6400 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/interfaces/ERC20.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:28.710522 ypricemagic-2.5.6/y/interfaces/balancer/
+-rw-r--r--   0 runner    (1001) docker     (122)    23102 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/interfaces/balancer/WeightedPool.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/interfaces/balancer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:28.710522 ypricemagic-2.5.6/y/interfaces/compound/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/interfaces/compound/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32517 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/interfaces/compound/unitroller.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:28.710522 ypricemagic-2.5.6/y/interfaces/curve/
+-rw-r--r--   0 runner    (1001) docker     (122)     7124 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/interfaces/curve/CurveRegistry.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/interfaces/curve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3802 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/interfaces/multicall2.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:28.710522 ypricemagic-2.5.6/y/interfaces/uniswap/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/interfaces/uniswap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2248 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/interfaces/uniswap/factoryv2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2283 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/interfaces/uniswap/quoterv3.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3271 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/networks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:28.714522 ypricemagic-2.5.6/y/prices/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2910 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/band.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19907 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/chainlink.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1073 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/convex.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:28.714522 ypricemagic-2.5.6/y/prices/dex/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/dex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:28.714522 ypricemagic-2.5.6/y/prices/dex/balancer/
+-rw-r--r--   0 runner    (1001) docker     (122)       64 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/dex/balancer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2905 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/dex/balancer/balancer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6669 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/dex/balancer/v1.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10463 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/dex/balancer/v2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2544 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/dex/genericamm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2206 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/dex/mooniswap.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:28.714522 ypricemagic-2.5.6/y/prices/dex/uniswap/
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/dex/uniswap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6372 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/dex/uniswap/uniswap.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2125 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/dex/uniswap/v1.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23293 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/dex/uniswap/v2.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12588 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/dex/uniswap/v2_forks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3988 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/dex/uniswap/v3.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:28.714522 ypricemagic-2.5.6/y/prices/eth_derivs/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/eth_derivs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1076 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/eth_derivs/creth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1272 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/eth_derivs/wsteth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2995 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/gearbox.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:28.714522 ypricemagic-2.5.6/y/prices/lending/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/lending/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10245 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/lending/aave.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10530 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/lending/compound.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/lending/ib.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12107 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/magic.py
+-rw-r--r--   0 runner    (1001) docker     (122)      815 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/one_to_one.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2490 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/popsicle.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:28.718522 ypricemagic-2.5.6/y/prices/stable_swap/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/stable_swap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/stable_swap/belt.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22296 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/stable_swap/curve.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1597 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/stable_swap/ellipsis.py
+-rw-r--r--   0 runner    (1001) docker     (122)      832 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/stable_swap/froyo.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1098 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/stable_swap/mstablefeederpool.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3298 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/stable_swap/saddle.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3926 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/synthetix.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:28.718522 ypricemagic-2.5.6/y/prices/tokenized_fund/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/tokenized_fund/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1079 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/tokenized_fund/basketdao.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1630 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/tokenized_fund/gelato.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2351 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/tokenized_fund/piedao.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2257 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/tokenized_fund/tokensets.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:28.718522 ypricemagic-2.5.6/y/prices/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      100 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4756 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/utils/buckets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8741 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/utils/sense_check.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8174 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/utils/ypriceapi.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5879 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/yearn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5511 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/time.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:28.718522 ypricemagic-2.5.6/y/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      178 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)      864 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/utils/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)      113 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/utils/dank_mids.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7970 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/utils/events.py
+-rw-r--r--   0 runner    (1001) docker     (122)      669 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/utils/fakes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1644 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2726 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/utils/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11228 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/utils/multicall.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14776 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/utils/raw_calls.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:28.718522 ypricemagic-2.5.6/ypricemagic/
+-rw-r--r--   0 runner    (1001) docker     (122)      404 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/ypricemagic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      626 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/ypricemagic/magic.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:28.722522 ypricemagic-2.5.6/ypricemagic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      406 2023-07-04 11:57:28.000000 ypricemagic-2.5.6/ypricemagic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3188 2023-07-04 11:57:28.000000 ypricemagic-2.5.6/ypricemagic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-04 11:57:28.000000 ypricemagic-2.5.6/ypricemagic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      168 2023-07-04 11:57:28.000000 ypricemagic-2.5.6/ypricemagic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-07-04 11:57:28.000000 ypricemagic-2.5.6/ypricemagic.egg-info/top_level.txt
```

### Comparing `ypricemagic-2.5.5/.github/workflows/codeql-analysis.yml` & `ypricemagic-2.5.6/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.5/.github/workflows/pytest.yaml` & `ypricemagic-2.5.6/.github/workflows/pytest.yaml`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.5/.github/workflows/release.yaml` & `ypricemagic-2.5.6/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.5/LICENSE.txt` & `ypricemagic-2.5.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.5/README.md` & `ypricemagic-2.5.6/README.md`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.5/setup.py` & `ypricemagic-2.5.6/setup.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.5/tests/classes/test_erc20.py` & `ypricemagic-2.5.6/tests/classes/test_erc20.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.5/tests/classes/test_singleton.py` & `ypricemagic-2.5.6/tests/classes/test_singleton.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.5/tests/fixtures.py` & `ypricemagic-2.5.6/tests/fixtures.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 
 from y.networks import Network
 
 mainnet_only = pytest.mark.skipif(
     chain.id != Network.Mainnet, reason="This test is only applicable on mainnet"
 )
 
+async_test = pytest.mark.asyncio_cooperative
+
 def blocks_for_contract(address: Address, count: int = 5) -> List[Block]:
     address = convert.to_address(address)
     return [int(block) for block in np.linspace(contract_creation_block(address) + 10000, chain.height, count)]
 
 def mutate_address(address: Address) -> Tuple[str,str,str,EthAddress]:
     """
     Returns the same address in various forms for testing.
```

### Comparing `ypricemagic-2.5.5/tests/prices/dex/test_uniswap.py` & `ypricemagic-2.5.6/tests/prices/dex/test_uniswap.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.5/tests/prices/lending/test_aave.py` & `ypricemagic-2.5.6/tests/prices/lending/test_aave.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.5/tests/prices/lending/test_compound.py` & `ypricemagic-2.5.6/tests/prices/lending/test_compound.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.5/tests/prices/test_chainlink.py` & `ypricemagic-2.5.6/tests/prices/test_chainlink.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.5/tests/prices/test_magic.py` & `ypricemagic-2.5.6/tests/prices/test_magic.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.5/tests/prices/test_popsicle.py` & `ypricemagic-2.5.6/tests/prices/test_popsicle.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.5/tests/prices/test_synthetix.py` & `ypricemagic-2.5.6/tests/prices/test_synthetix.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.5/tests/prices/test_yearn.py` & `ypricemagic-2.5.6/tests/prices/test_yearn.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.5/tests/prices/utils/test_buckets.py` & `ypricemagic-2.5.6/tests/prices/utils/test_buckets.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.5/y/__init__.py` & `ypricemagic-2.5.6/y/__init__.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.5/y/classes/common.py` & `ypricemagic-2.5.6/y/classes/common.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.5/y/classes/singleton.py` & `ypricemagic-2.5.6/y/classes/singleton.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.5/y/constants.py` & `ypricemagic-2.5.6/y/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,16 +188,14 @@
     Network.Avalanche:          "0xB31f66AA3C1e785363F0875A1B74E27b85FD66c7",
     Network.Heco:               "0x5545153CCFcA01fbd7Dd11C0b23ba694D9509A6F",
     Network.Harmony:            "0xcF664087a5bB0237a0BAd6742852ec6c8d69A27a",
     Network.Cronos:             "0x5C7F8A570d578ED84E63fdFA7b1eE72dEae1AE23",
     Network.Optimism:           "0x4200000000000000000000000000000000000006",
 }.get(chain.id)
 
-RAM_CACHE_TTL = int(os.environ.get("YPRICEMAGIC_CACHE_TTL", 60*60*24))  # 24h default
-
 thread_pool_executor = PruningThreadPoolExecutor(max_workers = int(os.environ.get("DOP", 128)))
 
 RECURSION_TIMEOUT = int(os.environ.get("YPRICEMAGIC_RECURSION_TIMEOUT", 60))
 recursion_logger_level = os.environ.get("YPRICEMAGIC_RECURSION_LOGGER_LEVEL", "debug").lower()
 log_possible_recursion_err = getattr(logging.getLogger("ypricemagic.recursion_logger"), recursion_logger_level)
 
 SKIP_YPRICEAPI = bool(os.environ.get("SKIP_YPRICEAPI"))
```

### Comparing `ypricemagic-2.5.5/y/contracts.py` & `ypricemagic-2.5.6/y/contracts.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,22 +20,22 @@
 from dank_mids.executor import PruningThreadPoolExecutor
 from dank_mids.semaphore import ThreadsafeSemaphore
 from hexbytes import HexBytes
 from multicall import Call
 
 from y import convert
 from y.datatypes import Address, AnyAddressType, Block
+from y.decorators import stuck_coro_debugger
 from y.exceptions import (ContractNotVerified, NodeNotSynced, call_reverted,
                           contract_not_verified)
 from y.interfaces.ERC20 import ERC20ABI
 from y.networks import Network
 from y.time import check_node, check_node_async
 from y.utils.cache import memory
 from y.utils.dank_mids import dank_w3
-from y.utils.logging import yLazyLogger
 
 logger = logging.getLogger(__name__)
 
 contract_threads = PruningThreadPoolExecutor(16)
 
 # cached Contract instance, saves about 20ms of init time
 _contract_lock = threading.Lock()
@@ -114,14 +114,15 @@
     if hi != height:
         logger.debug(f"contract creation block {address} -> {hi}")
         return hi
     raise ValueError(f"Unable to find deploy block for {address} on {Network.name()}")
 
 
 @a_sync.a_sync(cache_type='memory')
+@stuck_coro_debugger
 async def contract_creation_block_async(address: AnyAddressType, when_no_history_return_0: bool = False) -> int:
     """
     Determine the block when a contract was created using binary search.
     NOTE Requires access to historical state. Doesn't account for CREATE2 or SELFDESTRUCT.
     """
     address = convert.to_address(address)
     logger.debug(f"contract creation block {address}")
@@ -250,14 +251,15 @@
         build = {"abi": abi, "address": _resolve_address(address), "contractName": name, "type": "contract"}
         self.__init_from_abi__(build, owner, persist)
         patch_contract(self, dank_w3)   # Patch the Contract with coroutines for each method.
         _squeeze(self)                  # Get rid of unnecessary memory-hog properties
         return self
     
     @classmethod
+    @stuck_coro_debugger
     async def coroutine(
         cls, 
         address: AnyAddressType, 
         ) -> "Contract":
         # We do this so we don't clog the threadpool with multiple jobs for the same contract.
         async with address_semaphores[address]:
             try:
@@ -269,15 +271,15 @@
         _ContractBase.__init__(self, None, build, {})  # type: ignore
         _DeployedContractBase.__init__(self, build['address'], owner, None)
         if persist:
             _add_deployment(self)
         try:
             self.verified = True
         except AttributeError:
-            logger.warning(f'`Contract("{address}").verified` property will not be usable due to the contract having a `verified` method in its ABI.')
+            logger.warning(f'`Contract("{self.address}").verified` property will not be usable due to the contract having a `verified` method in its ABI.')
         return self
 
     def has_method(self, method: str, return_response: bool = False) -> Union[bool,Any]:
         return has_method(self.address, method, return_response=return_response, sync=False)
 
     async def has_methods(
         self, 
@@ -323,14 +325,15 @@
         return False
     if return_response:
         return response
     return True
 
 
 @a_sync.a_sync(default='sync', cache_type='memory')
+@stuck_coro_debugger
 async def has_methods(
     address: AnyAddressType, 
     methods: Tuple[str],
     _func: Callable = all # Union[any, all]
 ) -> bool:
     '''
     Checks to see if a contract has each view method (with no inputs) in `methods`.
@@ -351,14 +354,15 @@
         # Out of gas error implies one or more method is state-changing.
         # If `_func == all` we return False because `has_methods` is only supposed to work for public view methods with no inputs
         # If `_func == any` maybe one of the methods will work without "out of gas" error
         return False if _func == all else any(await asyncio.gather(*[has_method(address, method, sync=False) for method in methods]))
 
 
 #yLazyLogger(logger)
+@stuck_coro_debugger
 async def probe(
     address: AnyAddressType, 
     methods: List[str],
     block: Optional[Block] = None,
     return_method: bool = False
 ) -> Any:
     address = convert.to_address(address)
@@ -381,14 +385,15 @@
     if not return_method:
         return result
     else:
         return method, result
     
 
 @a_sync.a_sync(default='sync')
+@stuck_coro_debugger
 async def build_name(address: AnyAddressType, return_None_on_failure: bool = False) -> str:
     try:
         contract = await Contract.coroutine(address)
         return contract.__dict__['_build']['contractName']
     except ContractNotVerified:
         if not return_None_on_failure:
             raise
```

### Comparing `ypricemagic-2.5.5/y/datatypes.py` & `ypricemagic-2.5.6/y/datatypes.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.5/y/decorators.py` & `ypricemagic-2.5.6/y/decorators.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 
-import functools
-import os
-from typing import Callable, TypeVar, Union
 import asyncio
+import functools
+import logging
+import time
+from typing import Awaitable, Callable, TypeVar, Union
 
 from typing_extensions import ParamSpec
 
-DEBUG = os.environ.get('YPRICEMAGIC_DEBUG', False)
-
 P = ParamSpec('P')
 T = TypeVar('T')
 
 def continue_on_revert(func: Callable[P, T]) -> Callable[P, T]:
     '''
     Decorates a call-making function. If the call reverts, returns `None`. Raises any other exceptions.
     '''
@@ -30,7 +29,30 @@
             try:
                 return func(*args,**kwargs)
             except Exception as e:
                 continue_if_call_reverted(e)
     else:
         raise NotImplementedError(f"Unable to decorate {func}")
     return continue_on_revert_wrap
+
+def stuck_coro_debugger(fn: Callable[P, Awaitable[T]]) -> Callable[P, Awaitable[T]]:
+    logger = logging.getLogger("y.stuck?")
+    @functools.wraps(fn)
+    async def stuck_coro_wrap(*args: P.args, **kwargs: P.kwargs) -> T:
+        if not logger.isEnabledFor(logging.DEBUG):
+            return await fn(*args, **kwargs)
+        t = asyncio.create_task(_stuck_debug_task(logger, fn, args, kwargs))
+        retval = await fn(*args, **kwargs)
+        t.cancel()
+        return retval
+    return stuck_coro_wrap
+
+async def _stuck_debug_task(logger: logging.Logger, fn: Callable[P, T], *args: P.args, **kwargs: P.kwargs):
+    start = time.time()
+    while True:
+        await asyncio.sleep(300)
+        logger._log(
+            logging.DEBUG, 
+            f"{fn.__module__}.{fn.__name__} still executing after {round(time.time() - start, 2)}s with"
+            + f" args {tuple(str(arg) for arg in args)}"
+             + f" kwargs {dict((k, str(v)) for k, v in kwargs.items())}"
+        )
```

### Comparing `ypricemagic-2.5.5/y/erc20.py` & `ypricemagic-2.5.6/y/erc20.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.5/y/exceptions.py` & `ypricemagic-2.5.6/y/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,26 @@
 import logging
+from typing import Optional
+
 from brownie import Contract as BrownieContract
 from brownie.exceptions import CompilerError
-from y.utils.logging import yLazyLogger
 
 logger = logging.getLogger(__name__)
 
 # General
 
+class yPriceMagicError(ValueError):
+    def __init__(self, exc: Exception, address: str, block: Optional[int], symbol: str):
+        from y import Network
+        self.exception = exc
+        super().__init__(f"{self.exception} while fetching {Network.printable()} {symbol} {address} at block {block}")
+
 class PriceError(Exception):
-    pass
+    def __init__(self, logger: logging.Logger, symbol: str):
+        super().__init__(f"No price found for {symbol} {logger.address} at block {logger.block}")
 
 class UnsupportedNetwork(Exception):
     pass
 
 class NonStandardERC20(Exception):
     pass
 
@@ -42,15 +50,14 @@
             elif "list index out of range" in str(e): pass # didn't work, oh well
             elif "pop from an empty deque" in str(e): pass # didn't work, oh well
             elif "'UsingForDirective' object has no attribute 'typeName'" in str(e): pass # didn't work, oh well
             elif contract_not_verified(e): pass # not verified, won't work
             else: raise
 
 
-#yLazyLogger(logger)
 def contract_not_verified(e: Exception) -> bool:
     triggers = [
         'Contract source code not verified',
         'has not been verified',
     ]
     return any(trigger in str(e) for trigger in triggers)
 
@@ -73,15 +80,14 @@
 class CalldataPreparationError(Exception):
     pass
 
 class CallReverted(Exception):
     pass
 
 
-#yLazyLogger(logger)
 def call_reverted(e: Exception) -> bool:
     triggers = [
         'execution reverted',
         'No data was returned - the call likely reverted',
         'invalid opcode: opcode 0xfe not defined',
         'Tried to read 32 bytes.  Only got 0 bytes',
         'invalid jump destination',
@@ -91,15 +97,14 @@
 
 
 def continue_if_call_reverted(e: Exception) -> None:
     if call_reverted(e): return
     else: raise e
 
 
-#yLazyLogger(logger)
 def out_of_gas(e: Exception) -> bool:
     return 'out of gas' in str(e) 
 
 # Provider Exceptions:
 
 class NodeNotSynced(Exception):
     pass
```

### Comparing `ypricemagic-2.5.5/y/interfaces/ERC20.py` & `ypricemagic-2.5.6/y/interfaces/ERC20.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.5/y/interfaces/balancer/WeightedPool.py` & `ypricemagic-2.5.6/y/interfaces/balancer/WeightedPool.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.5/y/interfaces/compound/unitroller.py` & `ypricemagic-2.5.6/y/interfaces/compound/unitroller.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.5/y/interfaces/curve/CurveRegistry.py` & `ypricemagic-2.5.6/y/interfaces/curve/CurveRegistry.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.5/y/interfaces/multicall2.py` & `ypricemagic-2.5.6/y/interfaces/multicall2.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.5/y/interfaces/uniswap/factoryv2.py` & `ypricemagic-2.5.6/y/interfaces/uniswap/factoryv2.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.5/y/interfaces/uniswap/quoterv3.py` & `ypricemagic-2.5.6/y/interfaces/uniswap/quoterv3.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.5/y/networks.py` & `ypricemagic-2.5.6/y/networks.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.5/y/prices/band.py` & `ypricemagic-2.5.6/y/prices/band.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.5/y/prices/chainlink.py` & `ypricemagic-2.5.6/y/prices/chainlink.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import Dict, NoReturn, Optional, Union
 
 import a_sync
 from async_lru import alru_cache
 from brownie import ZERO_ADDRESS, chain
 from multicall import Call
 
+from y import ENVIRONMENT_VARIABLES as ENVS
 from y import convert
 from y.classes.common import ERC20
 from y.contracts import Contract, contract_creation_block_async
 from y.datatypes import Address, AnyAddressType, Block, UsdPrice
 from y.exceptions import ContractNotVerified, UnsupportedNetwork
 from y.networks import Network
 from y.utils.dank_mids import dank_w3
@@ -235,15 +236,15 @@
         return convert.to_address(asset) in await self.__feeds__(sync=False)
 
     async def get_price(self, asset, block: Optional[Block] = None) -> UsdPrice:
         if block is None:
             block = chain.height
         return await self._get_price(asset, block)
 
-    alru_cache(maxsize=1000, ttl=60*60*24)  # 24h ttl
+    alru_cache(maxsize=1000, ttl=ENVS.CACHE_TTL)
     async def _get_price(self, asset, block: Block) -> Optional[UsdPrice]:
         asset = convert.to_address(asset)
         if asset == ZERO_ADDRESS:
             return None
         feed = await self.get_feed(asset, sync=False)
         if feed is None or (block is not None and block < await contract_creation_block_async(feed.address, True)):
             return None
```

### Comparing `ypricemagic-2.5.5/y/prices/convex.py` & `ypricemagic-2.5.6/y/prices/convex.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.5/y/prices/dex/balancer/balancer.py` & `ypricemagic-2.5.6/y/prices/dex/balancer/balancer.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.5/y/prices/dex/balancer/v1.py` & `ypricemagic-2.5.6/y/prices/dex/balancer/v1.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.5/y/prices/dex/balancer/v2.py` & `ypricemagic-2.5.6/y/prices/dex/balancer/v2.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 
 import a_sync
 from brownie import chain
 from brownie.convert.datatypes import EthAddress
 from hexbytes import HexBytes
 from multicall import Call
 
+from y import ENVIRONMENT_VARIABLES as ENVS
 from y import constants, contracts
 from y.classes.common import ERC20, ContractBase, WeiBalance
 from y.datatypes import Address, AnyAddressType, Block, UsdPrice, UsdValue
 from y.networks import Network
 from y.utils.events import decode_logs, get_logs_asap
+from y.utils.logging import _get_price_logger
 from y.utils.raw_calls import raw_call
 
-logger = logging.getLogger(__name__)
-
 BALANCER_V2_VAULTS = {
     Network.Mainnet: [
         '0xBA12222222228d8Ba445958a75a0704d566BF2C8',
     ],
     Network.Fantom: [
         '0x20dd72Ed959b6147912C2e529F0a0C651c33c9ce',
     ],
@@ -38,64 +38,58 @@
 class BalancerV2Vault(ContractBase):
     def __init__(self, address: AnyAddressType, asynchronous: bool = False) -> None:
         super().__init__(address, asynchronous=asynchronous)
         if not self._is_cached:
             # we need the contract cached so we can decode logs correctly
             self.contract
             
-    @a_sync.a_sync(ram_cache_ttl=60*60)
+    @a_sync.a_sync(ram_cache_ttl=ENVS.CACHE_TTL)
     async def get_pool_tokens(self, pool_id: int, block: Optional[Block] = None):
         return await self.contract.getPoolTokens.coroutine(pool_id, block_identifier = block)
     
-    @a_sync.a_sync(ram_cache_ttl=60*60)
+    @a_sync.a_sync(ram_cache_ttl=ENVS.CACHE_TTL)
     async def list_pools(self, block: Optional[Block] = None) -> Dict[HexBytes,EthAddress]:
         topics = ['0x3c13bc30b8e878c53fd2a36b679409c073afd75950be43d8858768e956fbc20e']
         events = decode_logs(await get_logs_asap(self.address, topics, to_block=block, sync=False))
         return {
             event['poolId'].hex(): event['poolAddress'] for event in events
             # NOTE: For some reason the Balancer fork on Fantom lists "0x3e522051A9B1958Aa1e828AC24Afba4a551DF37d"
             #       as a pool, but it is not a contract. This handler will prevent it and future cases from causing problems.
             if contracts.is_contract(event['poolAddress'])
         }
     
-    @a_sync.a_sync(ram_cache_ttl=60*60)
+    @a_sync.a_sync(ram_cache_ttl=ENVS.CACHE_TTL)
     async def get_pool_info(self, poolids: Tuple[HexBytes,...], block: Optional[Block] = None) -> List[Tuple]:
         return await asyncio.gather(*[
             self.contract.getPoolTokens.coroutine(poolId, block_identifier=block)
             for poolId in poolids
         ])
     
     async def deepest_pool_for(self, token_address: Address, block: Optional[Block] = None) -> Tuple[Optional[EthAddress],int]:
         # sourcery skip: simplify-len-comparison
         pools = await self.list_pools(block=block, sync=False)
-        is_standard_pool = await asyncio.gather(*[_is_standard_pool(pool) for pool in pools.values()])
-        
-        if block is None:
-            poolids = (poolid for (poolid, pool), is_standard in zip(pools.items(), is_standard_pool) if is_standard)
-        else:
-            deploy_blocks = await asyncio.gather(*[contracts.contract_creation_block_async(pool, True) for pool in pools.values()])
-            poolids = (poolid for (poolid, pool), is_standard, deploy_block in zip(pools.items(), is_standard_pool, deploy_blocks) if is_standard and deploy_block <= block)
-
+        poolids = tuple(pools.keys())
         pools_info = await self.get_pool_info(poolids, block=block, sync=False)
         all_pools = await self.list_pools(block=block, sync=False)
         pools_info = {all_pools[poolid]: info for poolid, info in zip(poolids, pools_info) if str(info) != "((), (), 0)"}
         
+        logger = _get_price_logger(token_address, block, 'balancer.v2')
         deepest_pool = {'pool': None, 'balance': 0}
         for pool, info in pools_info.items():
             num_tokens = len(info[0])
             pool_balances = {info[0][i]: info[1][i] for i in range(num_tokens)}
             pool_balance = [balance for token, balance in pool_balances.items() if token == token_address]
             if len(pool_balance) == 0:
                 continue
             assert len(pool_balance) == 1
             pool_balance = pool_balance[0]
             if pool_balance > deepest_pool['balance']:
                 deepest_pool = {'pool': pool, 'balance': pool_balance}
-
-        return deepest_pool['pool'], deepest_pool['balance']
+        logger.debug(f"deepest pool {deepest_pool}")
+        return tuple(deepest_pool.values())
 
 
 class BalancerV2Pool(ERC20):
     def __init__(self, pool_address: AnyAddressType, asynchronous: bool = False) -> None:
         super().__init__(pool_address, asynchronous=asynchronous)
 
     @a_sync.aka.cached_property
@@ -118,15 +112,15 @@
     async def get_tvl(self, block: Optional[Block] = None) -> Awaitable[UsdValue]:
         balances = await self.get_balances(block=block, sync=False)
         return UsdValue(sum(await asyncio.gather(*[
             balance.__value_usd__(sync=False) for balance in balances.values()
             if balance.token.address != self.address  # NOTE: to prevent an infinite loop for tokens that include themselves in the pool (e.g. bb-a-USDC)
         ])))
 
-    @a_sync.a_sync(ram_cache_ttl=60*60)
+    @a_sync.a_sync(ram_cache_ttl=ENVS.CACHE_TTL)
     async def get_balances(self, block: Optional[Block] = None) -> Dict[ERC20, WeiBalance]:
         tokens = await self.tokens(block=block, sync=False)
         return dict(tokens.items())
 
     async def get_token_price(self, token_address: AnyAddressType, block: Optional[Block] = None) -> Optional[UsdPrice]:
         token_balances, weights = await asyncio.gather(
             self.get_balances(block=block, sync=False),
@@ -152,21 +146,21 @@
             paired_token_balance.__value_usd__(sync=False),
             token_balance.__readable__(sync=False),
         ])
         token_value_in_pool /= paired_token_weight * token_weight
         return UsdPrice(token_value_in_pool / token_balance_readable) 
 
     # NOTE: We can't cache this as a cached property because some balancer pool tokens can change. Womp
-    @a_sync.a_sync(ram_cache_ttl=60*60)
+    @a_sync.a_sync(ram_cache_ttl=ENVS.CACHE_TTL)
     async def tokens(self, block: Optional[Block] = None) -> Dict[ERC20, WeiBalance]:
         vault, id = await asyncio.gather(self.__vault__(sync=False), self.__id__(sync=False))
         tokens, balances, lastChangedBlock = await vault.get_pool_tokens(id, block=block, sync=False)
         return {ERC20(token, asynchronous=self.asynchronous): WeiBalance(balance, token, block=block) for token, balance in zip(tokens, balances)}
 
-    @a_sync.a_sync(ram_cache_ttl=60*60)
+    @a_sync.a_sync(ram_cache_ttl=ENVS.CACHE_TTL)
     async def weights(self, block: Optional[Block] = None) -> List[int]:
         try:
             return await self.contract.getNormalizedWeights.coroutine(block_identifier = block)
         except (AttributeError,ValueError):
             tokens = await self.tokens(block=block, sync=False)
             return [1 for _ in tokens.keys()]
```

### Comparing `ypricemagic-2.5.5/y/prices/dex/genericamm.py` & `ypricemagic-2.5.6/y/prices/dex/genericamm.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.5/y/prices/dex/mooniswap.py` & `ypricemagic-2.5.6/y/prices/dex/mooniswap.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.5/y/prices/dex/uniswap/uniswap.py` & `ypricemagic-2.5.6/y/prices/dex/uniswap/uniswap.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from y.datatypes import Address, AnyAddressType, Block, UsdPrice
 from y.exceptions import NonStandardERC20, contract_not_verified
 from y.networks import Network
 from y.prices.dex.uniswap.v1 import UniswapV1
 from y.prices.dex.uniswap.v2 import (NotAUniswapV2Pool, UniswapPoolV2,
                                      UniswapRouterV2)
 from y.prices.dex.uniswap.v2_forks import UNISWAPS
-from y.utils.logging import gh_issue_request
+from y.utils.logging import _gh_issue_request
 
 logger = logging.getLogger(__name__)
 
 # NOTE: If this is failing to pull a price for a token you need, it's likely because that token requires a special swap path.
 #       Please add a viable swap path to ..protocols to fetch price data successfully.
 
 class UniswapMultiplexer(a_sync.ASyncGenericSingleton):
@@ -46,15 +46,15 @@
             return False
         try:
             pool = UniswapPoolV2(token_address, asynchronous=True)
             is_pool = all(await pool.get_pool_details(sync=False))
             if is_pool:
                 factory = await pool.__factory__(sync=False)
                 if factory not in self.factories and factory != ZERO_ADDRESS:
-                    gh_issue_request(f'UniClone Factory {factory} is unknown to ypricemagic.', logger)
+                    _gh_issue_request(f'UniClone Factory {factory} is unknown to ypricemagic.', logger)
                     self.factories.append(factory)
             return is_pool
         except NotAUniswapV2Pool:
             return False
 
     async def get_price_v1(self, token_address: Address, block: Optional[Block] = None) -> UsdPrice:
         return await self.v1.get_price(token_address, block, sync=False)
```

### Comparing `ypricemagic-2.5.5/y/prices/dex/uniswap/v1.py` & `ypricemagic-2.5.6/y/prices/dex/uniswap/v1.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.5/y/prices/dex/uniswap/v2.py` & `ypricemagic-2.5.6/y/prices/dex/uniswap/v2.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.5/y/prices/dex/uniswap/v2_forks.py` & `ypricemagic-2.5.6/y/prices/dex/uniswap/v2_forks.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.5/y/prices/dex/uniswap/v3.py` & `ypricemagic-2.5.6/y/prices/dex/uniswap/v3.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from itertools import cycle
 from typing import Optional
 
 import a_sync
 from brownie import chain
 from eth_abi.packed import encode_abi_packed
 
+from y import ENVIRONMENT_VARIABLES as ENVS
 from y.classes.common import ERC20
 from y.constants import usdc, weth
 from y.contracts import Contract, contract_creation_block_async
 from y.datatypes import Address, Block, UsdPrice
 from y.exceptions import ContractNotVerified, UnsupportedNetwork
 from y.interfaces.uniswap.quoterv3 import UNIV3_QUOTER_ABI
 from y.networks import Network
@@ -73,15 +74,15 @@
         types = [type for _, type in zip(path, cycle(['address', 'uint24']))]
         return encode_abi_packed(types, path)
 
     def _undo_fees(self, path) -> float:
         fees = [1 - fee / FEE_DENOMINATOR for fee in path if isinstance(fee, int)]
         return math.prod(fees)
     
-    @a_sync.a_sync(cache_type='memory', ram_cache_ttl=60*60*24)  # 24h ttl
+    @a_sync.a_sync(cache_type='memory', ram_cache_ttl=ENVS.CACHE_TTL)
     async def get_price(self, token: Address, block: Optional[Block] = None) -> Optional[UsdPrice]:
         if block and block < await contract_creation_block_async(UNISWAP_V3_QUOTER, True):
             return None
 
         paths = [[token, fee, usdc.address] for fee in self.fee_tiers]
         if token != weth:
             paths += [
```

### Comparing `ypricemagic-2.5.5/y/prices/eth_derivs/creth.py` & `ypricemagic-2.5.6/y/prices/eth_derivs/creth.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.5/y/prices/eth_derivs/wsteth.py` & `ypricemagic-2.5.6/y/prices/eth_derivs/wsteth.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.5/y/prices/gearbox.py` & `ypricemagic-2.5.6/y/prices/gearbox.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import asyncio
 from decimal import Decimal
 from typing import List, Dict
 
 import a_sync
 from brownie import chain
 
+from y import ENVIRONMENT_VARIABLES as ENVS
 from y.classes.common import ERC20, ContractBase
 from y.contracts import Contract
 from y.datatypes import Address, Block, UsdPrice
 from y.exceptions import UnsupportedNetwork
 from y.networks import Network
 
 registry = "0xA50d4E7D8946a7c90652339CDBd262c375d54D99"
@@ -48,15 +49,15 @@
         else:
             raise UnsupportedNetwork()
     
     @a_sync.aka.cached_property
     async def registry(self) -> Contract:
         return await Contract.coroutine(registry)
     
-    @a_sync.a_sync(ram_cache_ttl=600)
+    @a_sync.a_sync(ram_cache_ttl=ENVS.CACHE_TTL)
     async def pools(self) -> List[DieselPool]:
         registry = await self.registry
         return [DieselPool(pool, asynchronous=self.asynchronous) for pool in await registry.getPools.coroutine()]
     
     async def diesel_tokens(self) -> Dict[ERC20, DieselPool]:
         pools = await self.pools(sync=False)
         dtokens = await asyncio.gather(*[pool.__diesel_token__(sync=False) for pool in pools])
```

### Comparing `ypricemagic-2.5.5/y/prices/lending/aave.py` & `ypricemagic-2.5.6/y/prices/lending/aave.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.5/y/prices/lending/compound.py` & `ypricemagic-2.5.6/y/prices/lending/compound.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from y.classes.common import ERC20, ContractBase
 from y.constants import EEE_ADDRESS
 from y.contracts import Contract, has_methods
 from y.datatypes import AddressOrContract, AnyAddressType, Block, UsdPrice
 from y.exceptions import call_reverted
 from y.networks import Network
-from y.utils.logging import gh_issue_request
+from y.utils.logging import _gh_issue_request
 from y.utils.raw_calls import raw_call
 
 logger = logging.getLogger(__name__)
 logger.addHandler(logging.StreamHandler())
 logger.setLevel(logging.INFO)
 
 TROLLERS = {
@@ -222,11 +222,11 @@
     async def get_price(self, token_address: AnyAddressType, block: Optional[Block] = None) -> Optional[UsdPrice]:
         troller = await self.get_troller(token_address)
         return await CToken(token_address, comptroller=troller, asynchronous=True).get_price(block=block)
 
     async def __notify_if_unknown_comptroller(self, token_address: AddressOrContract) -> None:
         comptroller = await raw_call(token_address,'comptroller()',output='address', sync=False)
         if comptroller not in self.trollers.values():
-            gh_issue_request(f'Comptroller {comptroller} is unknown to ypricemagic.', logger)
+            _gh_issue_request(f'Comptroller {comptroller} is unknown to ypricemagic.', logger)
 
 
 compound = Compound(asynchronous=True)
```

### Comparing `ypricemagic-2.5.5/y/prices/lending/ib.py` & `ypricemagic-2.5.6/y/prices/lending/ib.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.5/y/prices/magic.py` & `ypricemagic-2.5.6/y/prices/magic.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import asyncio
 import logging
-from typing import Iterable, List, Optional
+from typing import Iterable, List, NoReturn, Optional
 
 import a_sync
 from brownie import ZERO_ADDRESS, chain
 from brownie.exceptions import ContractNotFound
 from multicall.utils import raise_if_exception_in
 
+from y import ENVIRONMENT_VARIABLES as ENVS
 from y import constants, convert
 from y.classes.common import ERC20
 from y.datatypes import AnyAddressType, Block, UsdPrice
-from y.exceptions import NonStandardERC20, PriceError
-from y.networks import Network
+from y.decorators import stuck_coro_debugger
+from y.exceptions import NonStandardERC20, PriceError, yPriceMagicError
 from y.prices import convex, one_to_one, popsicle, yearn
 from y.prices.band import band
 from y.prices.chainlink import chainlink
 from y.prices.dex import mooniswap
 from y.prices.dex.balancer import balancer_multiplexer
 from y.prices.dex.genericamm import generic_amm
 from y.prices.dex.uniswap import uniswap_multiplexer
@@ -30,16 +31,16 @@
                                   saddle)
 from y.prices.stable_swap.curve import curve
 from y.prices.synthetix import synthetix
 from y.prices.tokenized_fund import basketdao, gelato, piedao, tokensets
 from y.prices.utils import ypriceapi
 from y.prices.utils.buckets import check_bucket
 from y.prices.utils.sense_check import _sense_check
-
-logger = logging.getLogger(__name__)
+from y.utils.dank_mids import dank_w3
+from y.utils.logging import _get_price_logger
 
 
 @a_sync.a_sync(default='sync')
 async def get_price(
     token_address: AnyAddressType,
     block: Optional[Block] = None, 
     fail_to_None: bool = False, 
@@ -53,46 +54,42 @@
 
     When `get_price` is unable to find a price:
     - If `silent == True`, ypricemagic will print an error message using standard python logging
     - If `silent == False`, ypricemagic will not log any error
     - If `fail_to_None == True`, ypricemagic will return `None`
     - If `fail_to_None == False`, ypricemagic will raise a PriceError
     '''
-    block = block or chain.height
+    block = block or await dank_w3.eth.block_number
     token_address = convert.to_address(token_address)
-
     try:
         return await _get_price(token_address, block, fail_to_None=fail_to_None, silent=silent)
     except (ContractNotFound, NonStandardERC20, RecursionError, PriceError) as e:
-        if fail_to_None:
-            return None
-        raise PriceError(f'could not fetch price for {await ERC20(token_address, asynchronous=True).symbol} {token_address} on {Network.printable()}') from e
+        symbol = await ERC20(token_address, asynchronous=True).symbol
+        if not fail_to_None:
+            raise yPriceMagicError(e, token_address, block, symbol) from e
 
 @a_sync.a_sync(default='sync')
 async def get_prices(
     token_addresses: Iterable[AnyAddressType],
     block: Optional[Block] = None,
     fail_to_None: bool = False,
     silent: bool = False,
-    dop: int = None
     ) -> List[Optional[float]]:
     '''
     A more optimized way to fetch prices for multiple assets at the same block.
 
     # NOTE silent kwarg is currently disabled.
     In every case:
     - if `silent == True`, tqdm will not be used
     - if `silent == False`, tqdm will be used
 
     When `get_prices` is unable to find a price:
     - if `fail_to_None == True`, ypricemagic will return `None` for that token
-    - if `fail_to_None == False`, ypricemagic will raise a PriceError and prevent you from receiving prices for your other tokens
+    - if `fail_to_None == False`, ypricemagic will raise a yPriceMagicError
     '''
-    if dop:
-        logger.warning('Kwarg `dop` was Optional in an old impmentation and will be removed in a future version. Please remove `dop` from your code.')
 
     if block is None:
         block = chain.height
 
     prices = await asyncio.gather(
         *[
             get_price(convert.to_address(token), block, fail_to_None=fail_to_None, silent=silent, sync=False)
@@ -105,74 +102,90 @@
         raise_if_exception_in(prices)
     else:
         for p in prices:
             if isinstance(p, Exception) and not isinstance(p, PriceError):
                 raise p
     return prices
 
-@a_sync.a_sync(cache_type='memory', ram_cache_ttl=constants.RAM_CACHE_TTL)
+@a_sync.a_sync(cache_type='memory', ram_cache_ttl=ENVS.CACHE_TTL)
+@stuck_coro_debugger
 async def _get_price(
     token: AnyAddressType, 
     block: Block, 
     fail_to_None: bool = False, 
     silent: bool = False
     ) -> Optional[UsdPrice]:  # sourcery skip: remove-redundant-if
 
     try:
+        # We do this to cache the symbol for later, otherwise some repr woudl break
         symbol = await ERC20(token, asynchronous=True).symbol
     except NonStandardERC20:
         symbol = None
-    token_string = f"{symbol} {token}" if symbol else token
+
+    logger = _get_price_logger(token, block, 'magic')
+    logger.debug(f'fetching price for {symbol}')
+    logger._debugger = asyncio.create_task(_debug_tsk(symbol, logger))
+
+    # Helps to detect stuck code
 
     if token == ZERO_ADDRESS:
-        _fail_appropriately(token_string, fail_to_None=fail_to_None, silent=silent)
+        _fail_appropriately(logger, symbol, fail_to_None=fail_to_None, silent=silent)
+        logger._debugger.cancel()
         return None
 
-    logger.debug("-------------[ y ]-------------")
-    logger.debug("Fetching price for...")
-    logger.debug(f"Token: {token_string}")
-    logger.debug(f"Block: {block or 'latest'}") 
-    logger.debug(f"Network: {Network.printable()}")
-
     if ypriceapi.should_use and token not in ypriceapi.skip_tokens:
         price = await ypriceapi.get_price(token, block)
+        logger.debug(f"ypriceapi -> {price}")
         if price is not None:
+            logger.debug(f"{symbol} price: {price}")
+            logger._debugger.cancel()
             return price
 
     price = await _exit_early_for_known_tokens(token, block=block)
+    logger.debug(f"early exit -> {price}")
     if price is not None:
+        logger.debug(f"{symbol} price: {price}")
+        logger._debugger.cancel()
         return price
     
     # TODO We need better logic to determine whether to use univ2, univ3, curve, balancer. For now this works for all known cases.
     # TODO should we use a liuidity-based method to determine this? 
     if price is None and uniswap_v3:
         price = await uniswap_v3.get_price(token, block=block, sync=False)
+        logger.debug(f"uniswap v3 -> {price}")
 
     if price is None:
         price = await uniswap_multiplexer.get_price(token, block=block, sync=False)
+        logger.debug(f"uniswap v2 -> {price}")
         
     # NOTE: We want this to go last, to hopefully prevent issues with recursion, ie sdANGLE.
     #       We previously had this before uniswap v3, but sdANGLE would create a recursion error by trying to price ANGLE via curve instead of viable uniswap v2.
     if price is None and curve: 
         price = await curve.get_price_for_underlying(token, block=block, sync=False)
+        logger.debug(f"curve -> {price}")
 
     # If price is 0, we can at least try to see if balancer gives us a price. If not, its probably a shitcoin.
     if price is None or price == 0:
         new_price = await balancer_multiplexer.get_price(token, block=block, sync=False)
+        logger.debug(f"balancer -> {price}")
         if new_price:
+            logger.debug(f"replacing price {price} with new price {new_price}")
             price = new_price
 
     if price is None:
-        _fail_appropriately(token_string, fail_to_None=fail_to_None, silent=silent)
+        _fail_appropriately(logger, symbol, fail_to_None=fail_to_None, silent=silent)
     if price:
         await _sense_check(token, price)
+
+    logger.debug(f"{symbol} price: {price}")
+    # Don't need this anymore
+    logger._debugger.cancel()
     return price
 
 
-#yLazyLogger(logger)
 async def _exit_early_for_known_tokens(
     token_address: str,
     block: Block
     ) -> Optional[UsdPrice]:  # sourcery skip: low-code-quality
 
     bucket = await check_bucket(token_address, sync=False)
 
@@ -220,26 +233,32 @@
     
     elif bucket == 'yearn or yearn-like':   price = await yearn.get_price(token_address, block, sync=False)
 
     return price
 
          
 def _fail_appropriately(
-    token_string: str, 
+    logger: logging.Logger,
+    symbol: str, 
     fail_to_None: bool = False, 
     silent: bool = False
     ) -> None:
     '''
     dictates how `magic.get_price()` will handle failures
 
     when `get_price` is unable to find a price:
         if `silent == True`, ypricemagic will print an error message using standard python logging
         if `silent == False`, ypricemagic will not log any error
         if `fail_to_None == True`, ypricemagic will return `None`
         if `fail_to_None == False`, ypricemagic will raise a PriceError
     '''
-
     if not silent:
-        logger.warning(f"failed to get price for {token_string} on {Network.printable()}")
+        logger.warning(f"failed to get price for {symbol}")
 
     if not fail_to_None:
-        raise PriceError(f'could not fetch price for {token_string} on {Network.printable()}')
+        raise PriceError(logger, symbol)
+
+async def _debug_tsk(symbol: str, logger: logging.Logger) -> NoReturn:
+    """Prints a log every 1 minute until the creating coro returns"""
+    while True:
+        await asyncio.sleep(60)
+        logger.debug(f"price still fetching for {symbol}")
```

### Comparing `ypricemagic-2.5.5/y/prices/one_to_one.py` & `ypricemagic-2.5.6/y/prices/one_to_one.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.5/y/prices/popsicle.py` & `ypricemagic-2.5.6/y/prices/popsicle.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.5/y/prices/stable_swap/belt.py` & `ypricemagic-2.5.6/y/prices/stable_swap/belt.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.5/y/prices/stable_swap/curve.py` & `ypricemagic-2.5.6/y/prices/stable_swap/curve.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.5/y/prices/stable_swap/ellipsis.py` & `ypricemagic-2.5.6/y/prices/stable_swap/ellipsis.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.5/y/prices/stable_swap/froyo.py` & `ypricemagic-2.5.6/y/prices/stable_swap/froyo.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.5/y/prices/stable_swap/mstablefeederpool.py` & `ypricemagic-2.5.6/y/prices/stable_swap/mstablefeederpool.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.5/y/prices/stable_swap/saddle.py` & `ypricemagic-2.5.6/y/prices/stable_swap/saddle.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import asyncio
 import logging
 from typing import List, Optional
 
 import a_sync
 from brownie import chain
 
+from y import ENVIRONMENT_VARIABLES as ENVS
 from y import convert
 from y.classes.common import ERC20
 from y.contracts import has_method, has_methods
 from y.datatypes import (Address, AddressOrContract, AnyAddressType, Block,
                          UsdPrice, UsdValue)
 from y.networks import Network
 from y.prices import magic
@@ -21,15 +22,15 @@
 
 @a_sync.a_sync(default='sync', cache_type='memory')
 async def is_saddle_lp(token_address: AnyAddressType) -> bool:
     pool = await get_pool(token_address, sync=False)
     if pool:
         return await has_methods(pool, ('getVirtualPrice()(uint)', 'getA()(uint)','getAPrecise()(uint)'), sync=False)
 
-@a_sync.a_sync(default='sync', ram_cache_ttl=60*60*24)  # 24h ttl
+@a_sync.a_sync(default='sync', ram_cache_ttl=ENVS.CACHE_TTL)
 async def get_pool(token_address: AnyAddressType) -> Address:
     convert.to_address(token_address)
     if chain.id == Network.Mainnet:
         if token_address == '0xc9da65931ABf0Ed1b74Ce5ad8c041C4220940368': # saddle aleth doesn't have swap() function
             return '0xa6018520EAACC06C30fF2e1B3ee2c7c22e64196a'
         elif token_address == '0xd48cF4D7FB0824CC8bAe055dF3092584d0a1726A': # saddle d4
             return '0xC69DDcd4DFeF25D8a793241834d4cc4b3668EAD6'
```

### Comparing `ypricemagic-2.5.5/y/prices/synthetix.py` & `ypricemagic-2.5.6/y/prices/synthetix.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import a_sync
 from brownie import chain
 from brownie.convert.datatypes import EthAddress, HexString
 from eth_abi import encode_single
 from multicall import Call
 
 from y import convert
+from y import ENVIRONMENT_VARIABLES as ENVS
 from y.contracts import Contract, has_method
 from y.datatypes import AnyAddressType, Block, UsdPrice
 from y.exceptions import UnsupportedNetwork, call_reverted
 from y.networks import Network
 
 logger = logging.getLogger(__name__)
 
@@ -63,15 +64,15 @@
         if await synthetix.get_currency_key(token, sync=False):
             return True
         if await has_method(token, 'target()(address)', sync=False):
             target = await Call(token, 'target()(address)').coroutine()
             return target in await synthetix.synths and await Call(target, 'proxy()(address)').coroutine() == token
         return False
     
-    @a_sync.a_sync(cache_type='memory', ram_cache_ttl=60*60*24)  # 24h ttl
+    @a_sync.a_sync(cache_type='memory', ram_cache_ttl=ENVS.CACHE_TTL)
     async def get_currency_key(self, token: AnyAddressType) -> Optional[HexString]:
         target = await Call(token, ['target()(address)']).coroutine() if await has_method(token, 'target()(address)', sync=False) else token
         return await Call(target, ['currencyKey()(bytes32)']).coroutine() if await has_method(token, 'currencyKey()(bytes32)', sync=False) else None
     
     async def get_price(self, token: AnyAddressType, block: Optional[Block] = None) -> Optional[UsdPrice]:
         """
         Get a price of a synth in dollars.
```

### Comparing `ypricemagic-2.5.5/y/prices/tokenized_fund/basketdao.py` & `ypricemagic-2.5.6/y/prices/tokenized_fund/basketdao.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.5/y/prices/tokenized_fund/gelato.py` & `ypricemagic-2.5.6/y/prices/tokenized_fund/gelato.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.5/y/prices/tokenized_fund/piedao.py` & `ypricemagic-2.5.6/y/prices/tokenized_fund/piedao.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.5/y/prices/tokenized_fund/tokensets.py` & `ypricemagic-2.5.6/y/prices/tokenized_fund/tokensets.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.5/y/prices/utils/buckets.py` & `ypricemagic-2.5.6/y/prices/utils/buckets.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.5/y/prices/utils/sense_check.py` & `ypricemagic-2.5.6/y/prices/utils/sense_check.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.5/y/prices/utils/ypriceapi.py` & `ypricemagic-2.5.6/y/prices/utils/ypriceapi.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.5/y/prices/yearn.py` & `ypricemagic-2.5.6/y/prices/yearn.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.5/y/time.py` & `ypricemagic-2.5.6/y/time.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,19 +4,21 @@
 import time
 from typing import NewType, Union
 
 from a_sync import a_sync
 from async_lru import alru_cache
 from brownie import chain, web3
 from cachetools.func import ttl_cache
+
 try:
     from dank_mids.ENVIRONMENT_VARIABLES import GANACHE_FORK
 except ImportError:
     from dank_mids._config import GANACHE_FORK
 
+from y import ENVIRONMENT_VARIABLES as ENVS
 from y.exceptions import NoBlockFound, NodeNotSynced
 from y.networks import Network
 from y.utils.cache import memory
 from y.utils.client import get_ethereum_client, get_ethereum_client_async
 from y.utils.dank_mids import dank_w3
 from y.utils.logging import yLazyLogger
 
@@ -28,40 +30,39 @@
     client = get_ethereum_client()
     if client in ['tg', 'erigon']:
         header = web3.manager.request_blocking(f"{client}_getHeaderByNumber", [height])
         return int(header.timestamp, 16)
     else:
         return chain[height].timestamp
 
-@a_sync(cache_type='memory', ram_cache_ttl=60*60*24)  # 24h ttl
+@a_sync(cache_type='memory', ram_cache_ttl=ENVS.CACHE_TTL)
 async def get_block_timestamp_async(height: int) -> int:
     client = await get_ethereum_client_async()
     if client in ['tg', 'erigon']:
         header = await dank_w3.manager.coro_request(f"{client}_getHeaderByNumber", [height])
         return int(header.timestamp, 16)
     else:
         block = await dank_w3.eth.get_block(height)
         return block.timestamp
 
 @memory.cache()
-#yLazyLogger(logger)
 def last_block_on_date(date: Union[str, datetime.date]) -> int:
     """ Returns the last block on a given `date`. You can pass either a `datetime.date` object or a date string formatted as 'YYYY-MM-DD'. """
     if isinstance(date, datetime.datetime):
         raise TypeError(
             "You can not pass in a `datetime.datetime` object. Please call date() on your input before passing it to this funciton."
         )
     if not isinstance(date, datetime.date):
         date = datetime.datetime.strptime(date, "%Y-%m-%d").date()
-    
+
     height = chain.height
     lo, hi = 0, height
     while hi - lo > 1:
         mid = lo + (hi - lo) // 2
-        logger.debug('block: ' + str(mid))
+        logger.debug(f'block: {str(mid)}')
         mid_ts = get_block_timestamp(mid)
         mid_date = datetime.date.fromtimestamp(mid_ts)
         logger.debug(f'mid: {mid_date}')
         logger.debug(date)
         if mid_date > date:
             hi = mid
         else:
@@ -92,15 +93,15 @@
         except NoBlockFound:
             time.sleep(.2)
     check_node()
     block = _closest_block_after_timestamp_cached(timestamp)
     logger.debug(f'closest {Network.name()} block after timestamp {timestamp} -> {block}')
     return block
 
-@a_sync(cache_type='memory', ram_cache_ttl=60*60*24)  # 24h ttl
+@a_sync(cache_type='memory', ram_cache_ttl=ENVS.CACHE_TTL)
 async def closest_block_after_timestamp_async(timestamp: Timestamp, wait_for_block_if_needed: bool = False) -> int:
     timestamp = _parse_timestamp(timestamp)
     while wait_for_block_if_needed:
         try:
             return await closest_block_after_timestamp_async(timestamp)
         except NoBlockFound:
             await asyncio.sleep(0.2)
@@ -131,24 +132,24 @@
         else:
             lo = mid
     if hi == height:
         raise NoBlockFound(f"No block found after timestamp {timestamp}")
     return hi
 
 
-@ttl_cache(ttl=60)
+@ttl_cache(ttl=300)
 def check_node() -> None:
     if GANACHE_FORK:
         return
     current_time = time.time()
     node_timestamp = web3.eth.get_block('latest').timestamp
     if current_time - node_timestamp > 5 * 60:
         raise NodeNotSynced(f"current time: {current_time}  latest block time: {node_timestamp}  discrepancy: {round((current_time - node_timestamp) / 60, 2)} minutes")
 
-@alru_cache(ttl=60)
+@alru_cache(ttl=300)
 async def check_node_async() -> None:
     if GANACHE_FORK:
         return
     current_time = time.time()
     latest = await dank_w3.eth.get_block('latest')
     node_timestamp = latest.timestamp
     if current_time - node_timestamp > 5 * 60:
```

### Comparing `ypricemagic-2.5.5/y/utils/client.py` & `ypricemagic-2.5.6/y/utils/client.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.5/y/utils/events.py` & `ypricemagic-2.5.6/y/utils/events.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.5/y/utils/fakes.py` & `ypricemagic-2.5.6/y/utils/fakes.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.5/y/utils/logging.py` & `ypricemagic-2.5.6/y/utils/logging.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,40 @@
-
 import logging
-from typing import List, Union
+from typing import List, TypeVar, Union
 
 from brownie import chain
+from cachetools.func import ttl_cache
 from lazy_logging import LazyLoggerFactory
+from typing_extensions import ParamSpec
 
+from y.datatypes import AnyAddressType, Block
 from y.networks import Network
 
+T = TypeVar('T')
+P = ParamSpec('P')
+
 yLazyLogger = LazyLoggerFactory("YPRICEMAGIC")
 
 logger = logging.getLogger(__name__)
 
+@ttl_cache(ttl=10*60)
+def _get_price_logger(token_address: AnyAddressType, block: Block, extra: str = '') -> logging.Logger:
+    address = str(token_address)
+    name = f"y.prices.{Network.label()}.{address}.{block}"
+    if extra: 
+        name += f".{extra}"
+    logger = logging.getLogger(name)
+    logger.setLevel(logger.parent.level)
+    logger.address = address
+    logger.block = block
+    return logger
+
 NETWORK_DESCRIPTOR_FOR_ISSUE_REQ =f'name ({Network.name()})' if Network.name() else f'chainid ({chain.id})'
 
-def gh_issue_request(issue_request_details: Union[str, List[str]], _logger = None) -> None:
+def _gh_issue_request(issue_request_details: Union[str, List[str]], _logger = None) -> None:
 
     if _logger is None: _logger = logger
 
     if type(issue_request_details) == str:
         _logger.warning(issue_request_details)
 
     elif type(issue_request_details) == list:
```

### Comparing `ypricemagic-2.5.5/y/utils/middleware.py` & `ypricemagic-2.5.6/y/utils/middleware.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.5/y/utils/multicall.py` & `ypricemagic-2.5.6/y/utils/multicall.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.5/y/utils/raw_calls.py` & `ypricemagic-2.5.6/y/utils/raw_calls.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.5/ypricemagic/magic.py` & `ypricemagic-2.5.6/ypricemagic/magic.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.5/ypricemagic.egg-info/SOURCES.txt` & `ypricemagic-2.5.6/ypricemagic.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 tests/prices/dex/test_uniswap.py
 tests/prices/lending/__init__.py
 tests/prices/lending/test_aave.py
 tests/prices/lending/test_compound.py
 tests/prices/stable_swap/test_curve.py
 tests/prices/tokenized_fund/test_piedao.py
 tests/prices/utils/test_buckets.py
+y/ENVIRONMENT_VARIABLES.py
 y/__init__.py
 y/constants.py
 y/contracts.py
 y/convert.py
 y/datatypes.py
 y/decorators.py
 y/erc20.py
```

