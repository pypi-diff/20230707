# Comparing `tmp/ypricemagic-2.5.6.tar.gz` & `tmp/ypricemagic-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ypricemagic-2.5.6.tar", last modified: Tue Jul  4 11:57:28 2023, max compression
+gzip compressed data, was "ypricemagic-2.6.0.tar", last modified: Thu Jul  6 21:48:18 2023, max compression
```

## Comparing `ypricemagic-2.5.6.tar` & `ypricemagic-2.6.0.tar`

### file list

```diff
@@ -1,154 +1,155 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:28.722522 ypricemagic-2.5.6/
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/.env.sample
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:28.698522 ypricemagic-2.5.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:28.702522 ypricemagic-2.5.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (122)     3229 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/.github/workflows/pytest.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      632 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      139 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      120 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)      406 2023-07-04 11:57:28.722522 ypricemagic-2.5.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      776 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)      168 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-07-04 11:57:28.722522 ypricemagic-2.5.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      840 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:28.706522 ypricemagic-2.5.6/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:28.706522 ypricemagic-2.5.6/tests/classes/
--rw-r--r--   0 runner    (1001) docker     (122)     3851 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/tests/classes/test_erc20.py
--rw-r--r--   0 runner    (1001) docker     (122)      550 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/tests/classes/test_singleton.py
--rw-r--r--   0 runner    (1001) docker     (122)      144 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     2248 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/tests/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:28.706522 ypricemagic-2.5.6/tests/prices/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/tests/prices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:28.706522 ypricemagic-2.5.6/tests/prices/dex/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/tests/prices/dex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      586 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/tests/prices/dex/test_balancer.py
--rw-r--r--   0 runner    (1001) docker     (122)     2918 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/tests/prices/dex/test_uniswap.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:28.706522 ypricemagic-2.5.6/tests/prices/lending/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/tests/prices/lending/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7133 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/tests/prices/lending/test_aave.py
--rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/tests/prices/lending/test_compound.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:28.706522 ypricemagic-2.5.6/tests/prices/stable_swap/
--rw-r--r--   0 runner    (1001) docker     (122)      379 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/tests/prices/stable_swap/test_curve.py
--rw-r--r--   0 runner    (1001) docker     (122)     7040 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/tests/prices/test_chainlink.py
--rw-r--r--   0 runner    (1001) docker     (122)      471 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/tests/prices/test_gearbox.py
--rw-r--r--   0 runner    (1001) docker     (122)     4496 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/tests/prices/test_magic.py
--rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/tests/prices/test_popsicle.py
--rw-r--r--   0 runner    (1001) docker     (122)     1116 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/tests/prices/test_synthetix.py
--rw-r--r--   0 runner    (1001) docker     (122)     1017 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/tests/prices/test_yearn.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:28.706522 ypricemagic-2.5.6/tests/prices/tokenized_fund/
--rw-r--r--   0 runner    (1001) docker     (122)      236 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/tests/prices/tokenized_fund/test_piedao.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:28.706522 ypricemagic-2.5.6/tests/prices/utils/
--rw-r--r--   0 runner    (1001) docker     (122)     2025 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/tests/prices/utils/test_buckets.py
--rw-r--r--   0 runner    (1001) docker     (122)      492 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/tests/test_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:28.710522 ypricemagic-2.5.6/y/
--rw-r--r--   0 runner    (1001) docker     (122)      209 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/ENVIRONMENT_VARIABLES.py
--rw-r--r--   0 runner    (1001) docker     (122)     1876 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:28.710522 ypricemagic-2.5.6/y/classes/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7773 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/classes/common.py
--rw-r--r--   0 runner    (1001) docker     (122)     2406 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/classes/singleton.py
--rw-r--r--   0 runner    (1001) docker     (122)     9930 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    20712 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/contracts.py
--rw-r--r--   0 runner    (1001) docker     (122)      493 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/convert.py
--rw-r--r--   0 runner    (1001) docker     (122)      576 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (122)     2130 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/decorators.py
--rw-r--r--   0 runner    (1001) docker     (122)     3187 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/erc20.py
--rw-r--r--   0 runner    (1001) docker     (122)     2868 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:28.710522 ypricemagic-2.5.6/y/interfaces/
--rw-r--r--   0 runner    (1001) docker     (122)     6400 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/interfaces/ERC20.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:28.710522 ypricemagic-2.5.6/y/interfaces/balancer/
--rw-r--r--   0 runner    (1001) docker     (122)    23102 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/interfaces/balancer/WeightedPool.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/interfaces/balancer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:28.710522 ypricemagic-2.5.6/y/interfaces/compound/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/interfaces/compound/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    32517 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/interfaces/compound/unitroller.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:28.710522 ypricemagic-2.5.6/y/interfaces/curve/
--rw-r--r--   0 runner    (1001) docker     (122)     7124 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/interfaces/curve/CurveRegistry.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/interfaces/curve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3802 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/interfaces/multicall2.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:28.710522 ypricemagic-2.5.6/y/interfaces/uniswap/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/interfaces/uniswap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2248 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/interfaces/uniswap/factoryv2.py
--rw-r--r--   0 runner    (1001) docker     (122)     2283 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/interfaces/uniswap/quoterv3.py
--rw-r--r--   0 runner    (1001) docker     (122)     3271 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/networks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:28.714522 ypricemagic-2.5.6/y/prices/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2910 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/band.py
--rw-r--r--   0 runner    (1001) docker     (122)    19907 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/chainlink.py
--rw-r--r--   0 runner    (1001) docker     (122)     1073 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/convex.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:28.714522 ypricemagic-2.5.6/y/prices/dex/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/dex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:28.714522 ypricemagic-2.5.6/y/prices/dex/balancer/
--rw-r--r--   0 runner    (1001) docker     (122)       64 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/dex/balancer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2905 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/dex/balancer/balancer.py
--rw-r--r--   0 runner    (1001) docker     (122)     6669 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/dex/balancer/v1.py
--rw-r--r--   0 runner    (1001) docker     (122)    10463 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/dex/balancer/v2.py
--rw-r--r--   0 runner    (1001) docker     (122)     2544 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/dex/genericamm.py
--rw-r--r--   0 runner    (1001) docker     (122)     2206 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/dex/mooniswap.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:28.714522 ypricemagic-2.5.6/y/prices/dex/uniswap/
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/dex/uniswap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6372 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/dex/uniswap/uniswap.py
--rw-r--r--   0 runner    (1001) docker     (122)     2125 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/dex/uniswap/v1.py
--rw-r--r--   0 runner    (1001) docker     (122)    23293 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/dex/uniswap/v2.py
--rw-r--r--   0 runner    (1001) docker     (122)    12588 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/dex/uniswap/v2_forks.py
--rw-r--r--   0 runner    (1001) docker     (122)     3988 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/dex/uniswap/v3.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:28.714522 ypricemagic-2.5.6/y/prices/eth_derivs/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/eth_derivs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1076 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/eth_derivs/creth.py
--rw-r--r--   0 runner    (1001) docker     (122)     1272 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/eth_derivs/wsteth.py
--rw-r--r--   0 runner    (1001) docker     (122)     2995 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/gearbox.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:28.714522 ypricemagic-2.5.6/y/prices/lending/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/lending/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10245 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/lending/aave.py
--rw-r--r--   0 runner    (1001) docker     (122)    10530 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/lending/compound.py
--rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/lending/ib.py
--rw-r--r--   0 runner    (1001) docker     (122)    12107 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/magic.py
--rw-r--r--   0 runner    (1001) docker     (122)      815 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/one_to_one.py
--rw-r--r--   0 runner    (1001) docker     (122)     2490 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/popsicle.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:28.718522 ypricemagic-2.5.6/y/prices/stable_swap/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/stable_swap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/stable_swap/belt.py
--rw-r--r--   0 runner    (1001) docker     (122)    22296 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/stable_swap/curve.py
--rw-r--r--   0 runner    (1001) docker     (122)     1597 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/stable_swap/ellipsis.py
--rw-r--r--   0 runner    (1001) docker     (122)      832 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/stable_swap/froyo.py
--rw-r--r--   0 runner    (1001) docker     (122)     1098 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/stable_swap/mstablefeederpool.py
--rw-r--r--   0 runner    (1001) docker     (122)     3298 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/stable_swap/saddle.py
--rw-r--r--   0 runner    (1001) docker     (122)     3926 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/synthetix.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:28.718522 ypricemagic-2.5.6/y/prices/tokenized_fund/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/tokenized_fund/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1079 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/tokenized_fund/basketdao.py
--rw-r--r--   0 runner    (1001) docker     (122)     1630 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/tokenized_fund/gelato.py
--rw-r--r--   0 runner    (1001) docker     (122)     2351 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/tokenized_fund/piedao.py
--rw-r--r--   0 runner    (1001) docker     (122)     2257 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/tokenized_fund/tokensets.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:28.718522 ypricemagic-2.5.6/y/prices/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      100 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4756 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/utils/buckets.py
--rw-r--r--   0 runner    (1001) docker     (122)     8741 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/utils/sense_check.py
--rw-r--r--   0 runner    (1001) docker     (122)     8174 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/utils/ypriceapi.py
--rw-r--r--   0 runner    (1001) docker     (122)     5879 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/prices/yearn.py
--rw-r--r--   0 runner    (1001) docker     (122)     5511 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/time.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:28.718522 ypricemagic-2.5.6/y/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      178 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (122)      864 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/utils/client.py
--rw-r--r--   0 runner    (1001) docker     (122)      113 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/utils/dank_mids.py
--rw-r--r--   0 runner    (1001) docker     (122)     7970 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/utils/events.py
--rw-r--r--   0 runner    (1001) docker     (122)      669 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/utils/fakes.py
--rw-r--r--   0 runner    (1001) docker     (122)     1644 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (122)     2726 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/utils/middleware.py
--rw-r--r--   0 runner    (1001) docker     (122)    11228 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/utils/multicall.py
--rw-r--r--   0 runner    (1001) docker     (122)    14776 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/y/utils/raw_calls.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:28.718522 ypricemagic-2.5.6/ypricemagic/
--rw-r--r--   0 runner    (1001) docker     (122)      404 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/ypricemagic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      626 2023-07-04 11:57:14.000000 ypricemagic-2.5.6/ypricemagic/magic.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-04 11:57:28.722522 ypricemagic-2.5.6/ypricemagic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      406 2023-07-04 11:57:28.000000 ypricemagic-2.5.6/ypricemagic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3188 2023-07-04 11:57:28.000000 ypricemagic-2.5.6/ypricemagic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-04 11:57:28.000000 ypricemagic-2.5.6/ypricemagic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      168 2023-07-04 11:57:28.000000 ypricemagic-2.5.6/ypricemagic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-07-04 11:57:28.000000 ypricemagic-2.5.6/ypricemagic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 21:48:18.295785 ypricemagic-2.6.0/
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/.env.sample
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 21:48:18.279785 ypricemagic-2.6.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 21:48:18.283785 ypricemagic-2.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     3229 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      632 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      139 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      721 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      120 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      406 2023-07-06 21:48:18.295785 ypricemagic-2.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      776 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      168 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-07-06 21:48:18.295785 ypricemagic-2.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      840 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 21:48:18.283785 ypricemagic-2.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 21:48:18.283785 ypricemagic-2.6.0/tests/classes/
+-rw-r--r--   0 runner    (1001) docker     (122)     3851 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/tests/classes/test_erc20.py
+-rw-r--r--   0 runner    (1001) docker     (122)      550 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/tests/classes/test_singleton.py
+-rw-r--r--   0 runner    (1001) docker     (122)      144 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2248 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/tests/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 21:48:18.287785 ypricemagic-2.6.0/tests/prices/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/tests/prices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 21:48:18.287785 ypricemagic-2.6.0/tests/prices/dex/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/tests/prices/dex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      586 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/tests/prices/dex/test_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2918 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/tests/prices/dex/test_uniswap.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 21:48:18.287785 ypricemagic-2.6.0/tests/prices/lending/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/tests/prices/lending/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7133 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/tests/prices/lending/test_aave.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/tests/prices/lending/test_compound.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 21:48:18.287785 ypricemagic-2.6.0/tests/prices/stable_swap/
+-rw-r--r--   0 runner    (1001) docker     (122)      379 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/tests/prices/stable_swap/test_curve.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7040 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/tests/prices/test_chainlink.py
+-rw-r--r--   0 runner    (1001) docker     (122)      471 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/tests/prices/test_gearbox.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4496 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/tests/prices/test_magic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/tests/prices/test_popsicle.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1116 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/tests/prices/test_synthetix.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1017 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/tests/prices/test_yearn.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 21:48:18.287785 ypricemagic-2.6.0/tests/prices/tokenized_fund/
+-rw-r--r--   0 runner    (1001) docker     (122)      236 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/tests/prices/tokenized_fund/test_piedao.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 21:48:18.287785 ypricemagic-2.6.0/tests/prices/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     2025 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/tests/prices/utils/test_buckets.py
+-rw-r--r--   0 runner    (1001) docker     (122)      492 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/tests/test_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 21:48:18.287785 ypricemagic-2.6.0/y/
+-rw-r--r--   0 runner    (1001) docker     (122)      209 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/ENVIRONMENT_VARIABLES.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1876 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 21:48:18.287785 ypricemagic-2.6.0/y/classes/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7773 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/classes/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2406 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/classes/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9930 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20712 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/contracts.py
+-rw-r--r--   0 runner    (1001) docker     (122)      493 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/convert.py
+-rw-r--r--   0 runner    (1001) docker     (122)      576 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2130 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3187 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/erc20.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2868 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 21:48:18.287785 ypricemagic-2.6.0/y/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (122)     6400 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/interfaces/ERC20.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 21:48:18.287785 ypricemagic-2.6.0/y/interfaces/balancer/
+-rw-r--r--   0 runner    (1001) docker     (122)    23102 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/interfaces/balancer/WeightedPool.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/interfaces/balancer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 21:48:18.287785 ypricemagic-2.6.0/y/interfaces/compound/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/interfaces/compound/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32517 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/interfaces/compound/unitroller.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 21:48:18.287785 ypricemagic-2.6.0/y/interfaces/curve/
+-rw-r--r--   0 runner    (1001) docker     (122)     7124 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/interfaces/curve/CurveRegistry.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/interfaces/curve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3802 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/interfaces/multicall2.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 21:48:18.287785 ypricemagic-2.6.0/y/interfaces/uniswap/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/interfaces/uniswap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2248 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/interfaces/uniswap/factoryv2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2283 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/interfaces/uniswap/quoterv3.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3271 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/networks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 21:48:18.291785 ypricemagic-2.6.0/y/prices/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/prices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2910 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/prices/band.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19907 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/prices/chainlink.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1073 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/prices/convex.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 21:48:18.291785 ypricemagic-2.6.0/y/prices/dex/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/prices/dex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 21:48:18.291785 ypricemagic-2.6.0/y/prices/dex/balancer/
+-rw-r--r--   0 runner    (1001) docker     (122)       64 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/prices/dex/balancer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2905 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/prices/dex/balancer/balancer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6669 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/prices/dex/balancer/v1.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10463 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/prices/dex/balancer/v2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2544 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/prices/dex/genericamm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2206 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/prices/dex/mooniswap.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 21:48:18.291785 ypricemagic-2.6.0/y/prices/dex/uniswap/
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/prices/dex/uniswap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6372 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/prices/dex/uniswap/uniswap.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2125 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/prices/dex/uniswap/v1.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23626 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/prices/dex/uniswap/v2.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12731 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/prices/dex/uniswap/v2_forks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3988 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/prices/dex/uniswap/v3.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 21:48:18.291785 ypricemagic-2.6.0/y/prices/eth_derivs/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/prices/eth_derivs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1076 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/prices/eth_derivs/creth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1272 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/prices/eth_derivs/wsteth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2995 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/prices/gearbox.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 21:48:18.291785 ypricemagic-2.6.0/y/prices/lending/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/prices/lending/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10731 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/prices/lending/aave.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10530 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/prices/lending/compound.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/prices/lending/ib.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12380 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/prices/magic.py
+-rw-r--r--   0 runner    (1001) docker     (122)      815 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/prices/one_to_one.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2490 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/prices/popsicle.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 21:48:18.291785 ypricemagic-2.6.0/y/prices/stable_swap/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/prices/stable_swap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/prices/stable_swap/belt.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22296 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/prices/stable_swap/curve.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1597 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/prices/stable_swap/ellipsis.py
+-rw-r--r--   0 runner    (1001) docker     (122)      832 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/prices/stable_swap/froyo.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1098 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/prices/stable_swap/mstablefeederpool.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3298 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/prices/stable_swap/saddle.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3926 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/prices/synthetix.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 21:48:18.291785 ypricemagic-2.6.0/y/prices/tokenized_fund/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/prices/tokenized_fund/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1079 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/prices/tokenized_fund/basketdao.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1630 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/prices/tokenized_fund/gelato.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2351 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/prices/tokenized_fund/piedao.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2257 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/prices/tokenized_fund/tokensets.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 21:48:18.291785 ypricemagic-2.6.0/y/prices/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      100 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/prices/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5126 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/prices/utils/buckets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8741 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/prices/utils/sense_check.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8174 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/prices/utils/ypriceapi.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5879 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/prices/yearn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5511 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/time.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 21:48:18.295785 ypricemagic-2.6.0/y/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      178 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)      864 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/utils/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)      113 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/utils/dank_mids.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7970 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/utils/events.py
+-rw-r--r--   0 runner    (1001) docker     (122)      669 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/utils/fakes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1644 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2726 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/utils/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11228 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/utils/multicall.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14776 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/y/utils/raw_calls.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 21:48:18.295785 ypricemagic-2.6.0/ypricemagic/
+-rw-r--r--   0 runner    (1001) docker     (122)      404 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/ypricemagic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      626 2023-07-06 21:48:07.000000 ypricemagic-2.6.0/ypricemagic/magic.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 21:48:18.295785 ypricemagic-2.6.0/ypricemagic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      406 2023-07-06 21:48:18.000000 ypricemagic-2.6.0/ypricemagic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3204 2023-07-06 21:48:18.000000 ypricemagic-2.6.0/ypricemagic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-06 21:48:18.000000 ypricemagic-2.6.0/ypricemagic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      168 2023-07-06 21:48:18.000000 ypricemagic-2.6.0/ypricemagic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-07-06 21:48:18.000000 ypricemagic-2.6.0/ypricemagic.egg-info/top_level.txt
```

### Comparing `ypricemagic-2.5.6/.github/workflows/codeql-analysis.yml` & `ypricemagic-2.6.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/.github/workflows/pytest.yaml` & `ypricemagic-2.6.0/.github/workflows/pytest.yaml`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/.github/workflows/release.yaml` & `ypricemagic-2.6.0/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/LICENSE.txt` & `ypricemagic-2.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/README.md` & `ypricemagic-2.6.0/README.md`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/setup.py` & `ypricemagic-2.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/tests/classes/test_erc20.py` & `ypricemagic-2.6.0/tests/classes/test_erc20.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/tests/classes/test_singleton.py` & `ypricemagic-2.6.0/tests/classes/test_singleton.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/tests/fixtures.py` & `ypricemagic-2.6.0/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/tests/prices/dex/test_balancer.py` & `ypricemagic-2.6.0/tests/prices/dex/test_balancer.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/tests/prices/dex/test_uniswap.py` & `ypricemagic-2.6.0/tests/prices/dex/test_uniswap.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/tests/prices/lending/test_aave.py` & `ypricemagic-2.6.0/tests/prices/lending/test_aave.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/tests/prices/lending/test_compound.py` & `ypricemagic-2.6.0/tests/prices/lending/test_compound.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/tests/prices/test_chainlink.py` & `ypricemagic-2.6.0/tests/prices/test_chainlink.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/tests/prices/test_magic.py` & `ypricemagic-2.6.0/tests/prices/test_magic.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/tests/prices/test_popsicle.py` & `ypricemagic-2.6.0/tests/prices/test_popsicle.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/tests/prices/test_synthetix.py` & `ypricemagic-2.6.0/tests/prices/test_synthetix.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/tests/prices/test_yearn.py` & `ypricemagic-2.6.0/tests/prices/test_yearn.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/tests/prices/utils/test_buckets.py` & `ypricemagic-2.6.0/tests/prices/utils/test_buckets.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/y/__init__.py` & `ypricemagic-2.6.0/y/__init__.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/y/classes/common.py` & `ypricemagic-2.6.0/y/classes/common.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/y/classes/singleton.py` & `ypricemagic-2.6.0/y/classes/singleton.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/y/constants.py` & `ypricemagic-2.6.0/y/constants.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/y/contracts.py` & `ypricemagic-2.6.0/y/contracts.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/y/datatypes.py` & `ypricemagic-2.6.0/y/datatypes.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/y/decorators.py` & `ypricemagic-2.6.0/y/decorators.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/y/erc20.py` & `ypricemagic-2.6.0/y/erc20.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/y/exceptions.py` & `ypricemagic-2.6.0/y/exceptions.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/y/interfaces/ERC20.py` & `ypricemagic-2.6.0/y/interfaces/ERC20.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/y/interfaces/balancer/WeightedPool.py` & `ypricemagic-2.6.0/y/interfaces/balancer/WeightedPool.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/y/interfaces/compound/unitroller.py` & `ypricemagic-2.6.0/y/interfaces/compound/unitroller.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/y/interfaces/curve/CurveRegistry.py` & `ypricemagic-2.6.0/y/interfaces/curve/CurveRegistry.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/y/interfaces/multicall2.py` & `ypricemagic-2.6.0/y/interfaces/multicall2.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/y/interfaces/uniswap/factoryv2.py` & `ypricemagic-2.6.0/y/interfaces/uniswap/factoryv2.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/y/interfaces/uniswap/quoterv3.py` & `ypricemagic-2.6.0/y/interfaces/uniswap/quoterv3.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/y/networks.py` & `ypricemagic-2.6.0/y/networks.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/y/prices/band.py` & `ypricemagic-2.6.0/y/prices/band.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/y/prices/chainlink.py` & `ypricemagic-2.6.0/y/prices/chainlink.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/y/prices/convex.py` & `ypricemagic-2.6.0/y/prices/convex.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/y/prices/dex/balancer/balancer.py` & `ypricemagic-2.6.0/y/prices/dex/balancer/balancer.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/y/prices/dex/balancer/v1.py` & `ypricemagic-2.6.0/y/prices/dex/balancer/v1.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/y/prices/dex/balancer/v2.py` & `ypricemagic-2.6.0/y/prices/dex/balancer/v2.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/y/prices/dex/genericamm.py` & `ypricemagic-2.6.0/y/prices/dex/genericamm.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/y/prices/dex/mooniswap.py` & `ypricemagic-2.6.0/y/prices/dex/mooniswap.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/y/prices/dex/uniswap/uniswap.py` & `ypricemagic-2.6.0/y/prices/dex/uniswap/uniswap.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/y/prices/dex/uniswap/v1.py` & `ypricemagic-2.6.0/y/prices/dex/uniswap/v1.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/y/prices/dex/uniswap/v2.py` & `ypricemagic-2.6.0/y/prices/dex/uniswap/v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -253,14 +253,18 @@
             amount_out = quote[-1] / out_scale
             return UsdPrice(amount_out / fees)
 
 
     @continue_on_revert
     async def get_quote(self, amount_in: int, path: Path, block: Optional[Block] = None) -> Tuple[int,int]:
         if self._is_cached:
+            # NOTE: This could be cleaner but is makes it easiest wrt adding modified uni forks
+            if self.contract.getAmountsOut.abi['inputs'][1].get('internalType') == "struct Router.route[]": # Velo router
+                routes = [[path[i], path[i+1], False] for i in range(len(path) - 1)]
+                path = routes
             try:
                 return await self.contract.getAmountsOut.coroutine(amount_in, path, block_identifier=block)
             # TODO figure out how to best handle uni forks with slight modifications.
             # Sometimes the below "else" code will not work with modified methods. Brownie works for now.
             except Exception as e:
                 strings = [
                     "INSUFFICIENT_INPUT_AMOUNT",
```

### Comparing `ypricemagic-2.5.6/y/prices/dex/uniswap/v2_forks.py` & `ypricemagic-2.6.0/y/prices/dex/uniswap/v2_forks.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,14 +91,15 @@
         "trisolaris":       {"factory": "0xc66F594268041dB60507F00703b152492fb176E7", "router": "0x2CB45Edb4517d5947aFdE3BEAbF95A582506858B"},
     },
     Network.OKEx: {
         "dfyn":             {"factory": "0xE7Fb3e833eFE5F9c441105EB65Ef8b261266423B", "router": "0x34686CBF7229ed0bff2Fbe7ED2CFC916317764f6"},
     },
     Network.Optimism: {
         "zipswap":          {"factory": "0x8BCeDD62DD46F1A76F8A1633d4f5B76e0CDa521E", "router": "0xE6Df0BB08e5A97b40B21950a0A51b94c4DbA0Ff6"},
+        "velodrome":        {"factory": "0x25CbdDb98b35ab1FF77413456B31EC81A6B6B746", "router": "0x9c12939390052919aF3155f41Bf4160Fd3666A6f"},
     },
     Network.xDai: {
         "sushiswap":        {"factory": "0xc35DADB65012eC5796536bD9864eD8773aBc74C4", "router": "0x1b02dA8Cb0d097eB8D57A175b88c7D8b47997506"},
     },
 }.get(chain.id, {})
```

### Comparing `ypricemagic-2.5.6/y/prices/dex/uniswap/v3.py` & `ypricemagic-2.6.0/y/prices/dex/uniswap/v3.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/y/prices/eth_derivs/creth.py` & `ypricemagic-2.6.0/y/prices/eth_derivs/creth.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/y/prices/eth_derivs/wsteth.py` & `ypricemagic-2.6.0/y/prices/eth_derivs/wsteth.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/y/prices/gearbox.py` & `ypricemagic-2.6.0/y/prices/gearbox.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/y/prices/lending/aave.py` & `ypricemagic-2.6.0/y/prices/lending/aave.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 from y import convert
 from y.classes.common import ERC20, ContractBase
 from y.contracts import Contract
 from y.datatypes import AddressOrContract, AnyAddressType, Block, UsdPrice
 from y.exceptions import ContractNotVerified
 from y.networks import Network
+from y.utils.logging import _get_price_logger
 from y.utils.multicall import fetch_multicall
 from y.utils.raw_calls import raw_call
 
 logger = logging.getLogger(__name__)
 
 
 v1_pools = {
@@ -69,15 +70,17 @@
     def __contains__(self, __o: object) -> bool:
         if not self.asynchronous:
             cls = self.__class__.__name__
             raise RuntimeError(f"'self.asynchronous' must be False to use {cls}.__contains__.\nYou may wish to use {cls}.is_atoken instead.")
         return convert.to_address(__o) in self.atokens
     
     async def contains(self, __o: object) -> bool:
-        return convert.to_address(__o) in await self.__atokens__(sync=False)
+        contains = convert.to_address(__o) in await self.__atokens__(sync=False)
+        logger.debug(f'{self} contains {__o}: {contains}')
+        return contains
 
 
 class AaveMarketV1(AaveMarketBase):
     @a_sync.a_sync(ram_cache_maxsize=256)
     async def underlying(self, token_address: AddressOrContract) -> ERC20:
         underlying = await raw_call(token_address, 'underlyingAssetAddress()',output='address', sync=False)
         return ERC20(underlying)
@@ -155,38 +158,47 @@
             self.__pools_v2__(sync=False), 
             self.__pools_v3__(sync=False),
         )
         return v1 + v2 + v3
     
     @a_sync.aka.cached_property
     async def pools_v1(self) -> List[AaveMarketV1]:
-        return [AaveMarketV1(pool, asynchronous=self.asynchronous) for pool in v1_pools]
+        pools = [AaveMarketV1(pool, asynchronous=self.asynchronous) for pool in v1_pools]
+        logger.debug(f"{self} v1 pools {pools}")
+        return pools
     
     @a_sync.aka.cached_property
     async def pools_v2(self) -> List[AaveMarketV2]:
-        return [AaveMarketV2(pool, asynchronous=self.asynchronous) for pool in v2_pools]
+        pools = [AaveMarketV2(pool, asynchronous=self.asynchronous) for pool in v2_pools]
+        logger.debug(f"{self} v2 pools {pools}")
+        return pools
     
     @a_sync.aka.cached_property
     async def pools_v3(self) -> List[AaveMarketV2]:
-        return [AaveMarketV3(pool, asynchronous=self.asynchronous) for pool in v3_pools]
+        pools = [AaveMarketV3(pool, asynchronous=self.asynchronous) for pool in v3_pools]
+        logger.debug(f"{self} v3 pools {pools}")
+        return pools
     
     async def pool_for_atoken(self, token_address: AnyAddressType) -> Optional[Union[AaveMarketV1, AaveMarketV2]]:
         pools = await self.__pools__(sync=False)
         for pool in pools:
             if await pool.contains(token_address, sync=False):
                 return pool
 
     def __contains__(self, __o: object) -> bool:
         if self.asynchronous:
             raise RuntimeError(f"'self.asynchronous' must be False to use AaveRegistry.__contains__.\nYou may wish to use AaveRegistry.is_atoken instead.")
         return any(__o in pool for pool in self.pools)
 
     @a_sync.a_sync(cache_type='memory')
     async def is_atoken(self, token_address: AnyAddressType) -> bool:
-        return any(await asyncio.gather(*[pool.contains(token_address, sync=False) for pool in await self.__pools__(sync=False)]))
+        logger = _get_price_logger(token_address, block=None)
+        is_atoken = any(await asyncio.gather(*[pool.contains(token_address, sync=False) for pool in await self.__pools__(sync=False)]))
+        logger.debug(f"is_atoken: {is_atoken}")
+        return is_atoken
     
     async def is_wrapped_atoken_v2(self, token_address: AnyAddressType) -> bool:
         # NOTE: Not sure if this wrapped version is actually related to aave but this works for pricing purposes.
         try:
             contract = await Contract.coroutine(token_address)
             attrs = "ATOKEN", "STATIC_ATOKEN_LM_REVISION", "staticToDynamicAmount"
             return all(hasattr(contract, attr) for attr in attrs)
```

### Comparing `ypricemagic-2.5.6/y/prices/lending/compound.py` & `ypricemagic-2.6.0/y/prices/lending/compound.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/y/prices/lending/ib.py` & `ypricemagic-2.6.0/y/prices/lending/ib.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/y/prices/magic.py` & `ypricemagic-2.6.0/y/prices/magic.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,68 +122,71 @@
         symbol = None
 
     logger = _get_price_logger(token, block, 'magic')
     logger.debug(f'fetching price for {symbol}')
     logger._debugger = asyncio.create_task(_debug_tsk(symbol, logger))
 
     # Helps to detect stuck code
+    try:
+        if token == ZERO_ADDRESS:
+            _fail_appropriately(logger, symbol, fail_to_None=fail_to_None, silent=silent)
+            logger._debugger.cancel()
+            return None
 
-    if token == ZERO_ADDRESS:
-        _fail_appropriately(logger, symbol, fail_to_None=fail_to_None, silent=silent)
-        logger._debugger.cancel()
-        return None
+        if ypriceapi.should_use and token not in ypriceapi.skip_tokens:
+            price = await ypriceapi.get_price(token, block)
+            logger.debug(f"ypriceapi -> {price}")
+            if price is not None:
+                logger.debug(f"{symbol} price: {price}")
+                logger._debugger.cancel()
+                return price
 
-    if ypriceapi.should_use and token not in ypriceapi.skip_tokens:
-        price = await ypriceapi.get_price(token, block)
-        logger.debug(f"ypriceapi -> {price}")
+        price = await _exit_early_for_known_tokens(token, block=block)
+        logger.debug(f"early exit -> {price}")
         if price is not None:
             logger.debug(f"{symbol} price: {price}")
             logger._debugger.cancel()
             return price
+        
+        # TODO We need better logic to determine whether to use univ2, univ3, curve, balancer. For now this works for all known cases.
+        # TODO should we use a liuidity-based method to determine this? 
+        if price is None and uniswap_v3:
+            price = await uniswap_v3.get_price(token, block=block, sync=False)
+            logger.debug(f"uniswap v3 -> {price}")
+
+        if price is None:
+            price = await uniswap_multiplexer.get_price(token, block=block, sync=False)
+            logger.debug(f"uniswap v2 -> {price}")
+            
+        # NOTE: We want this to go last, to hopefully prevent issues with recursion, ie sdANGLE.
+        #       We previously had this before uniswap v3, but sdANGLE would create a recursion error by trying to price ANGLE via curve instead of viable uniswap v2.
+        if price is None and curve: 
+            price = await curve.get_price_for_underlying(token, block=block, sync=False)
+            logger.debug(f"curve -> {price}")
+
+        # If price is 0, we can at least try to see if balancer gives us a price. If not, its probably a shitcoin.
+        if price is None or price == 0:
+            new_price = await balancer_multiplexer.get_price(token, block=block, sync=False)
+            logger.debug(f"balancer -> {price}")
+            if new_price:
+                logger.debug(f"replacing price {price} with new price {new_price}")
+                price = new_price
+
+        if price is None:
+            _fail_appropriately(logger, symbol, fail_to_None=fail_to_None, silent=silent)
+        if price:
+            await _sense_check(token, price)
 
-    price = await _exit_early_for_known_tokens(token, block=block)
-    logger.debug(f"early exit -> {price}")
-    if price is not None:
         logger.debug(f"{symbol} price: {price}")
+        # Don't need this anymore
         logger._debugger.cancel()
         return price
-    
-    # TODO We need better logic to determine whether to use univ2, univ3, curve, balancer. For now this works for all known cases.
-    # TODO should we use a liuidity-based method to determine this? 
-    if price is None and uniswap_v3:
-        price = await uniswap_v3.get_price(token, block=block, sync=False)
-        logger.debug(f"uniswap v3 -> {price}")
-
-    if price is None:
-        price = await uniswap_multiplexer.get_price(token, block=block, sync=False)
-        logger.debug(f"uniswap v2 -> {price}")
-        
-    # NOTE: We want this to go last, to hopefully prevent issues with recursion, ie sdANGLE.
-    #       We previously had this before uniswap v3, but sdANGLE would create a recursion error by trying to price ANGLE via curve instead of viable uniswap v2.
-    if price is None and curve: 
-        price = await curve.get_price_for_underlying(token, block=block, sync=False)
-        logger.debug(f"curve -> {price}")
-
-    # If price is 0, we can at least try to see if balancer gives us a price. If not, its probably a shitcoin.
-    if price is None or price == 0:
-        new_price = await balancer_multiplexer.get_price(token, block=block, sync=False)
-        logger.debug(f"balancer -> {price}")
-        if new_price:
-            logger.debug(f"replacing price {price} with new price {new_price}")
-            price = new_price
-
-    if price is None:
-        _fail_appropriately(logger, symbol, fail_to_None=fail_to_None, silent=silent)
-    if price:
-        await _sense_check(token, price)
-
-    logger.debug(f"{symbol} price: {price}")
-    # Don't need this anymore
-    logger._debugger.cancel()
-    return price
+    except Exception as e:
+        logger._debugger.cancel()
+        raise e
 
 
 async def _exit_early_for_known_tokens(
     token_address: str,
     block: Block
     ) -> Optional[UsdPrice]:  # sourcery skip: low-code-quality
```

### Comparing `ypricemagic-2.5.6/y/prices/one_to_one.py` & `ypricemagic-2.6.0/y/prices/one_to_one.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/y/prices/popsicle.py` & `ypricemagic-2.6.0/y/prices/popsicle.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/y/prices/stable_swap/belt.py` & `ypricemagic-2.6.0/y/prices/stable_swap/belt.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/y/prices/stable_swap/curve.py` & `ypricemagic-2.6.0/y/prices/stable_swap/curve.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/y/prices/stable_swap/ellipsis.py` & `ypricemagic-2.6.0/y/prices/stable_swap/ellipsis.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/y/prices/stable_swap/froyo.py` & `ypricemagic-2.6.0/y/prices/stable_swap/froyo.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/y/prices/stable_swap/mstablefeederpool.py` & `ypricemagic-2.6.0/y/prices/stable_swap/mstablefeederpool.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/y/prices/stable_swap/saddle.py` & `ypricemagic-2.6.0/y/prices/stable_swap/saddle.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/y/prices/synthetix.py` & `ypricemagic-2.6.0/y/prices/synthetix.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/y/prices/tokenized_fund/basketdao.py` & `ypricemagic-2.6.0/y/prices/tokenized_fund/basketdao.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/y/prices/tokenized_fund/gelato.py` & `ypricemagic-2.6.0/y/prices/tokenized_fund/gelato.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/y/prices/tokenized_fund/piedao.py` & `ypricemagic-2.6.0/y/prices/tokenized_fund/piedao.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/y/prices/tokenized_fund/tokensets.py` & `ypricemagic-2.6.0/y/prices/tokenized_fund/tokensets.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/y/prices/utils/buckets.py` & `ypricemagic-2.6.0/y/prices/utils/buckets.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,82 +1,120 @@
+import asyncio
 import logging
+from typing import Awaitable, Callable, Tuple
 
 import a_sync
 
 from y import convert
 from y.constants import STABLECOINS
-from y.datatypes import AnyAddressType
+from y.datatypes import Address, AnyAddressType
 from y.prices import convex, one_to_one, popsicle, yearn
 from y.prices.band import band
 from y.prices.chainlink import chainlink
-from y.prices.gearbox import gearbox
 from y.prices.dex import mooniswap
 from y.prices.dex.balancer import balancer_multiplexer
 from y.prices.dex.genericamm import generic_amm
 from y.prices.dex.uniswap import uniswap_multiplexer
 from y.prices.eth_derivs import creth, wsteth
+from y.prices.gearbox import gearbox
 from y.prices.lending import ib
 from y.prices.lending.aave import aave
 from y.prices.lending.compound import compound
 from y.prices.stable_swap import (belt, ellipsis, froyo, mstablefeederpool,
                                   saddle)
 from y.prices.stable_swap.curve import curve
 from y.prices.synthetix import synthetix
 from y.prices.tokenized_fund import basketdao, gelato, piedao, tokensets
+from y.utils.logging import _get_price_logger
 
 logger = logging.getLogger(__name__)
 
-
 @a_sync.a_sync(default='sync', cache_type='memory')
 async def check_bucket(
     token: AnyAddressType
     ) -> str:
 
     token_address = convert.to_address(token)
+    logger = _get_price_logger(token_address, block=None)
 
-    # these require neither calls to the chain nor contract initialization
-    if token_address == "0xEeeeeEeeeEeEeeEeEeEeeEEEeeeeEeeeeeeeEEeE":       return 'wrapped gas coin'
-    elif token_address in STABLECOINS:                                      return 'stable usd'
-    elif one_to_one.is_one_to_one_token(token_address):                     return 'one to one'
-    
-    elif wsteth.is_wsteth(token_address):                                   return 'wsteth'
-    elif creth.is_creth(token_address):                                     return 'creth'
-    elif belt.is_belt_lp(token_address):                                    return 'belt lp'
-
-    elif froyo.is_froyo(token_address):                                     return 'froyo'
-    elif await aave.is_atoken(token_address, sync=False):                   return 'atoken'
-    elif convex.is_convex_lp(token_address):                                return 'convex'
-
-    # these just require calls
-    elif await balancer_multiplexer.is_balancer_pool(token_address, sync=False):  return 'balancer pool'
-    elif await ib.is_ib_token(token_address, sync=False):                         return 'ib token'
-
-    elif await gelato.is_gelato_pool(token_address, sync=False):                        return 'gelato'
-    elif await piedao.is_pie(token_address, sync=False):                          return 'piedao lp'
-    elif await tokensets.is_token_set(token_address, sync=False):           return 'token set'
-
-    elif await ellipsis.is_eps_rewards_pool(token_address, sync=False):           return 'ellipsis lp'
-    elif await mstablefeederpool.is_mstable_feeder_pool(token_address, sync=False):     return 'mstable feeder pool'
-    elif await saddle.is_saddle_lp(token_address, sync=False):                    return 'saddle'
-
-    elif await basketdao.is_basketdao_index(token_address, sync=False):     return 'basketdao'
-    elif await popsicle.is_popsicle_lp(token_address, sync=False):                return 'popsicle'
+    # these require neither calls to the chain nor contract initialization, just string comparisons (pretty sure)
+    for bucket, check in string_matchers.items():
+        if check(token):
+            logger.debug(f"{token_address} is {bucket}")
+            return bucket
+        else:
+            logger.debug(f"{token_address} is not {bucket}")
+
+    # check these first, these just require calls
+    coros = [_check_bucket_helper(bucket, check, token_address) for bucket, check in calls_only.items()]
+    for fut in asyncio.as_completed(coros):
+        bucket, is_member = await fut
+        logger.debug(f"{token_address} is {'' if is_member else 'not '}{bucket}")
+        if is_member:
+            return bucket
+        else:
+            bucket = None
 
+    # TODO: Refactor the below like the above
     # these require both calls and contract initializations
-    elif await uniswap_multiplexer.is_uniswap_pool(token_address, sync=False):    return 'uni or uni-like lp'
-    elif gearbox and await gearbox.is_diesel_token(token_address, sync=False):    return 'gearbox'
+    if await uniswap_multiplexer.is_uniswap_pool(token_address, sync=False):
+        bucket = 'uni or uni-like lp'
+    elif gearbox and await gearbox.is_diesel_token(token_address, sync=False):
+        bucket = 'gearbox'
 
     # this just requires contract initialization but should go behind uniswap
-    elif await aave.is_wrapped_atoken_v2(token_address, sync=False):        return 'wrapped atoken v2'
-    elif await aave.is_wrapped_atoken_v3(token_address, sync=False):        return 'wrapped atoken v3'
-    elif token_address in generic_amm:                                      return 'generic amm'
-    elif await mooniswap.is_mooniswap_pool(token_address, sync=False):      return 'mooniswap lp'
-    elif await compound.is_compound_market(token_address, sync=False):      return 'compound'
-    elif await _chainlink_and_band(token_address):                          return 'chainlink and band'
-    elif chainlink and await chainlink.has_feed(token_address, sync=False): return 'chainlink feed'
-    elif synthetix and await synthetix.is_synth(token_address, sync=False): return 'synthetix'
-    elif await yearn.is_yearn_vault(token_address, sync=False):             return 'yearn or yearn-like'
-    elif await curve.get_pool(token_address, sync=False):                   return 'curve lp'
+    elif await aave.is_wrapped_atoken_v2(token_address, sync=False):
+        bucket = 'wrapped atoken v2'
+    elif await aave.is_wrapped_atoken_v3(token_address, sync=False):
+        bucket = 'wrapped atoken v3'
+    elif token_address in generic_amm:                                      
+        bucket = 'generic amm'
+    elif await mooniswap.is_mooniswap_pool(token_address, sync=False):      
+        bucket = 'mooniswap lp'
+    elif await compound.is_compound_market(token_address, sync=False):      
+        bucket = 'compound'
+    elif await _chainlink_and_band(token_address):                          
+        bucket = 'chainlink and band'
+    elif chainlink and await chainlink.has_feed(token_address, sync=False): 
+        bucket = 'chainlink feed'
+    elif synthetix and await synthetix.is_synth(token_address, sync=False): 
+        bucket = 'synthetix'
+    elif await yearn.is_yearn_vault(token_address, sync=False):             
+        bucket = 'yearn or yearn-like'
+    elif await curve.get_pool(token_address, sync=False):                   
+        bucket = 'curve lp'
+    logger.debug(f"{token_address} bucket is {bucket}")
+    return bucket
+
+# these require neither calls to the chain nor contract initialization, just string comparisons (pretty sure)
+string_matchers = {
+    'wrapped gas coin': lambda address: address == "0xEeeeeEeeeEeEeeEeEeEeeEEEeeeeEeeeeeeeEEeE",
+    'stable usd': lambda address: address in STABLECOINS,
+    'one to one': one_to_one.is_one_to_one_token,
+    'wsteth': wsteth.is_wsteth,
+    'creth': creth.is_creth,
+    'belt lp': belt.is_belt_lp,
+    'froyo': froyo.is_froyo,
+    'convex': convex.is_convex_lp,
+}
+
+# these just require calls
+calls_only = {
+    'atoken': aave.is_atoken,
+    'balancer pool': balancer_multiplexer.is_balancer_pool,
+    'ib token': ib.is_ib_token,
+    'gelato': gelato.is_gelato_pool,
+    'piedao lp': piedao.is_pie,
+    'token set': tokensets.is_token_set,
+    'ellipsis lp': ellipsis.is_eps_rewards_pool,
+    'mstable feeder pool': mstablefeederpool.is_mstable_feeder_pool,
+    'saddle': saddle.is_saddle_lp,
+    'basketdao': basketdao.is_basketdao_index,
+    'popsicle': popsicle.is_popsicle_lp,
+}
 
 async def _chainlink_and_band(token_address) -> bool:
     """ We only really need band for a short period in the beginning of fantom's history, and then we will default to chainlink once available. """
-    return chainlink and await chainlink.has_feed(token_address, sync=False) and token_address in band
+    return chainlink and await chainlink.has_feed(token_address, sync=False) and token_address in band
+
+async def _check_bucket_helper(bucket: str, check: Callable[[Address], Awaitable[bool]], address: Address) -> Tuple[str, bool]:
+    return bucket, await check(address, sync=False)
```

### Comparing `ypricemagic-2.5.6/y/prices/utils/sense_check.py` & `ypricemagic-2.6.0/y/prices/utils/sense_check.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/y/prices/utils/ypriceapi.py` & `ypricemagic-2.6.0/y/prices/utils/ypriceapi.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/y/prices/yearn.py` & `ypricemagic-2.6.0/y/prices/yearn.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/y/time.py` & `ypricemagic-2.6.0/y/time.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/y/utils/client.py` & `ypricemagic-2.6.0/y/utils/client.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/y/utils/events.py` & `ypricemagic-2.6.0/y/utils/events.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/y/utils/fakes.py` & `ypricemagic-2.6.0/y/utils/fakes.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/y/utils/logging.py` & `ypricemagic-2.6.0/y/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/y/utils/middleware.py` & `ypricemagic-2.6.0/y/utils/middleware.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/y/utils/multicall.py` & `ypricemagic-2.6.0/y/utils/multicall.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/y/utils/raw_calls.py` & `ypricemagic-2.6.0/y/utils/raw_calls.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/ypricemagic/magic.py` & `ypricemagic-2.6.0/ypricemagic/magic.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.5.6/ypricemagic.egg-info/SOURCES.txt` & `ypricemagic-2.6.0/ypricemagic.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 .env.sample
 .gitignore
+CONTRIBUTING.md
 LICENSE.txt
 Makefile
 README.md
 requirements-dev.txt
 requirements.txt
 setup.cfg
 setup.py
```

