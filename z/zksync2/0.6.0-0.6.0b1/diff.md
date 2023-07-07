# Comparing `tmp/zksync2-0.6.0.tar.gz` & `tmp/zksync2-0.6.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zksync2-0.6.0.tar", last modified: Fri Jul  7 11:36:38 2023, max compression
+gzip compressed data, was "zksync2-0.6.0b1.tar", last modified: Fri Jun 30 00:43:28 2023, max compression
```

## Comparing `zksync2-0.6.0.tar` & `zksync2-0.6.0b1.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:36:38.247201 zksync2-0.6.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:36:38.219200 zksync2-0.6.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:36:38.223200 zksync2-0.6.0/.github/workflows/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1162 2023-07-07 11:36:18.000000 zksync2-0.6.0/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-07-07 11:36:18.000000 zksync2-0.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-07 11:36:18.000000 zksync2-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    16281 2023-07-07 11:36:38.247201 zksync2-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15696 2023-07-07 11:36:18.000000 zksync2-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:36:38.227200 zksync2-0.6.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-07-07 11:36:18.000000 zksync2-0.6.0/examples/01_deposit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-07-07 11:36:18.000000 zksync2-0.6.0/examples/02_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-07-07 11:36:18.000000 zksync2-0.6.0/examples/03_transfer_erc20_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-07-07 11:36:18.000000 zksync2-0.6.0/examples/04_deploy_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     6901 2023-07-07 11:36:18.000000 zksync2-0.6.0/examples/05_deploy_create_with_constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-07-07 11:36:18.000000 zksync2-0.6.0/examples/06_deploy_create_with_deps.py
--rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-07-07 11:36:18.000000 zksync2-0.6.0/examples/07_deploy_create2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-07-07 11:36:18.000000 zksync2-0.6.0/examples/08_deploy_create2_deps.py
--rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-07-07 11:36:18.000000 zksync2-0.6.0/examples/09_withdrawal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-07-07 11:36:18.000000 zksync2-0.6.0/examples/10_finalize_withdrawal.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-07 11:36:18.000000 zksync2-0.6.0/examples/11_check_balance.py
--rw-r--r--   0 runner    (1001) docker     (123)     5305 2023-07-07 11:36:18.000000 zksync2-0.6.0/examples/12_deploy_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     4700 2023-07-07 11:36:18.000000 zksync2-0.6.0/examples/13_deploy_account_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     5369 2023-07-07 11:36:18.000000 zksync2-0.6.0/examples/14_deploy_account_create2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6980 2023-07-07 11:36:18.000000 zksync2-0.6.0/examples/15_use_paymaster.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-07-07 11:36:18.000000 zksync2-0.6.0/examples/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:36:38.223200 zksync2-0.6.0/examples/solidity/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:36:38.227200 zksync2-0.6.0/examples/solidity/custom_paymaster/
--rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-07-07 11:36:18.000000 zksync2-0.6.0/examples/solidity/custom_paymaster/Paymaster.sol
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-07 11:36:18.000000 zksync2-0.6.0/examples/solidity/custom_paymaster/Token.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:36:38.227200 zksync2-0.6.0/examples/solidity/custom_paymaster/build/
--rw-r--r--   0 runner    (1001) docker     (123)    42342 2023-07-07 11:36:18.000000 zksync2-0.6.0/examples/solidity/custom_paymaster/build/Paymaster.json
--rw-r--r--   0 runner    (1001) docker     (123)    65416 2023-07-07 11:36:18.000000 zksync2-0.6.0/examples/solidity/custom_paymaster/build/Token.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:36:38.231201 zksync2-0.6.0/examples/solidity/demo/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-07 11:36:18.000000 zksync2-0.6.0/examples/solidity/demo/Demo.sol
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-07 11:36:18.000000 zksync2-0.6.0/examples/solidity/demo/Foo.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:36:38.231201 zksync2-0.6.0/examples/solidity/demo/build/
--rw-r--r--   0 runner    (1001) docker     (123)    11955 2023-07-07 11:36:18.000000 zksync2-0.6.0/examples/solidity/demo/build/combined.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:36:38.231201 zksync2-0.6.0/examples/solidity/incrementer/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-07 11:36:18.000000 zksync2-0.6.0/examples/solidity/incrementer/Incrementer.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:36:38.231201 zksync2-0.6.0/examples/solidity/incrementer/build/
--rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-07-07 11:36:18.000000 zksync2-0.6.0/examples/solidity/incrementer/build/combined.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:36:38.231201 zksync2-0.6.0/examples/solidity/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-07 11:36:18.000000 zksync2-0.6.0/examples/solidity/storage/Storage.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:36:38.231201 zksync2-0.6.0/examples/solidity/storage/build/
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-07 11:36:18.000000 zksync2-0.6.0/examples/solidity/storage/build/combined.json
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-07 11:36:18.000000 zksync2-0.6.0/examples/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-07 11:36:18.000000 zksync2-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-07 11:36:18.000000 zksync2-0.6.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-07 11:36:38.247201 zksync2-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-07 11:36:18.000000 zksync2-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:36:38.231201 zksync2-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 11:36:18.000000 zksync2-0.6.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:36:38.231201 zksync2-0.6.0/tests/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)     9467 2023-07-07 11:36:18.000000 zksync2-0.6.0/tests/contracts/Counter.json
--rw-r--r--   0 runner    (1001) docker     (123)   103076 2023-07-07 11:36:18.000000 zksync2-0.6.0/tests/contracts/CustomAccount.json
--rw-r--r--   0 runner    (1001) docker     (123)    48494 2023-07-07 11:36:18.000000 zksync2-0.6.0/tests/contracts/CustomPaymaster.json
--rw-r--r--   0 runner    (1001) docker     (123)     8303 2023-07-07 11:36:18.000000 zksync2-0.6.0/tests/contracts/Foo.json
--rw-r--r--   0 runner    (1001) docker     (123)    15075 2023-07-07 11:36:18.000000 zksync2-0.6.0/tests/contracts/Import.json
--rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-07-07 11:36:18.000000 zksync2-0.6.0/tests/contracts/SimpleConstructor.json
--rw-r--r--   0 runner    (1001) docker     (123)    50646 2023-07-07 11:36:18.000000 zksync2-0.6.0/tests/contracts/SomeERC20.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 11:36:18.000000 zksync2-0.6.0/tests/contracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-07 11:36:18.000000 zksync2-0.6.0/tests/contracts/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:36:38.235201 zksync2-0.6.0/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 11:36:18.000000 zksync2-0.6.0/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-07 11:36:18.000000 zksync2-0.6.0/tests/integration/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-07-07 11:36:18.000000 zksync2-0.6.0/tests/integration/test_deposit.py
--rw-r--r--   0 runner    (1001) docker     (123)     9344 2023-07-07 11:36:18.000000 zksync2-0.6.0/tests/integration/test_paymaster.py
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-07-07 11:36:18.000000 zksync2-0.6.0/tests/integration/test_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-07-07 11:36:18.000000 zksync2-0.6.0/tests/integration/test_withdraw.py
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-07-07 11:36:18.000000 zksync2-0.6.0/tests/integration/test_zksync_contract.py
--rw-r--r--   0 runner    (1001) docker     (123)    42460 2023-07-07 11:36:18.000000 zksync2-0.6.0/tests/integration/test_zksync_web3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:36:38.235201 zksync2-0.6.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 11:36:18.000000 zksync2-0.6.0/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-07 11:36:18.000000 zksync2-0.6.0/tests/unit/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-07-07 11:36:18.000000 zksync2-0.6.0/tests/unit/test_contract_deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-07-07 11:36:18.000000 zksync2-0.6.0/tests/unit/test_eip712.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-07-07 11:36:18.000000 zksync2-0.6.0/tests/unit/test_eth_signer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-07-07 11:36:18.000000 zksync2-0.6.0/tests/unit/test_transaction712.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:36:38.235201 zksync2-0.6.0/zksync2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 11:36:18.000000 zksync2-0.6.0/zksync2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:36:38.239201 zksync2-0.6.0/zksync2/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 11:36:18.000000 zksync2-0.6.0/zksync2/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-07-07 11:36:18.000000 zksync2-0.6.0/zksync2/core/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-07 11:36:18.000000 zksync2-0.6.0/zksync2/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:36:38.239201 zksync2-0.6.0/zksync2/manage_contracts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 11:36:18.000000 zksync2-0.6.0/zksync2/manage_contracts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:36:38.243201 zksync2-0.6.0/zksync2/manage_contracts/contract_abi/
--rw-r--r--   0 runner    (1001) docker     (123)     9537 2023-07-07 11:36:18.000000 zksync2-0.6.0/zksync2/manage_contracts/contract_abi/ContractDeployer.json
--rw-r--r--   0 runner    (1001) docker     (123)     6220 2023-07-07 11:36:18.000000 zksync2-0.6.0/zksync2/manage_contracts/contract_abi/IAllowList.json
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-07 11:36:18.000000 zksync2-0.6.0/zksync2/manage_contracts/contract_abi/IERC1271.json
--rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-07-07 11:36:18.000000 zksync2-0.6.0/zksync2/manage_contracts/contract_abi/IERC20.json
--rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-07-07 11:36:18.000000 zksync2-0.6.0/zksync2/manage_contracts/contract_abi/IEthToken.json
--rw-r--r--   0 runner    (1001) docker     (123)     5847 2023-07-07 11:36:18.000000 zksync2-0.6.0/zksync2/manage_contracts/contract_abi/IL1Bridge.json
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-07 11:36:18.000000 zksync2-0.6.0/zksync2/manage_contracts/contract_abi/IL1Messenger.json
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-07-07 11:36:18.000000 zksync2-0.6.0/zksync2/manage_contracts/contract_abi/IL2Bridge.json
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-07-07 11:36:18.000000 zksync2-0.6.0/zksync2/manage_contracts/contract_abi/INonceHolder.json
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-07 11:36:18.000000 zksync2-0.6.0/zksync2/manage_contracts/contract_abi/IPaymasterFlow.json
--rw-r--r--   0 runner    (1001) docker     (123)    49698 2023-07-07 11:36:18.000000 zksync2-0.6.0/zksync2/manage_contracts/contract_abi/IZkSync.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 11:36:18.000000 zksync2-0.6.0/zksync2/manage_contracts/contract_abi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-07-07 11:36:18.000000 zksync2-0.6.0/zksync2/manage_contracts/contract_encoder_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6301 2023-07-07 11:36:18.000000 zksync2-0.6.0/zksync2/manage_contracts/contract_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-07 11:36:18.000000 zksync2-0.6.0/zksync2/manage_contracts/deploy_addresses.py
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-07-07 11:36:18.000000 zksync2-0.6.0/zksync2/manage_contracts/erc20_contract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-07-07 11:36:18.000000 zksync2-0.6.0/zksync2/manage_contracts/eth_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-07-07 11:36:18.000000 zksync2-0.6.0/zksync2/manage_contracts/l1_bridge.py
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-07-07 11:36:18.000000 zksync2-0.6.0/zksync2/manage_contracts/l2_bridge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-07 11:36:18.000000 zksync2-0.6.0/zksync2/manage_contracts/nonce_holder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-07 11:36:18.000000 zksync2-0.6.0/zksync2/manage_contracts/paymaster_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-07-07 11:36:18.000000 zksync2-0.6.0/zksync2/manage_contracts/precompute_contract_deployer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14931 2023-07-07 11:36:18.000000 zksync2-0.6.0/zksync2/manage_contracts/zksync_contract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:36:38.243201 zksync2-0.6.0/zksync2/module/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 11:36:18.000000 zksync2-0.6.0/zksync2/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-07 11:36:18.000000 zksync2-0.6.0/zksync2/module/middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-07 11:36:18.000000 zksync2-0.6.0/zksync2/module/module_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-07 11:36:18.000000 zksync2-0.6.0/zksync2/module/request_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-07 11:36:18.000000 zksync2-0.6.0/zksync2/module/response_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    14805 2023-07-07 11:36:18.000000 zksync2-0.6.0/zksync2/module/zksync_module.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-07 11:36:18.000000 zksync2-0.6.0/zksync2/module/zksync_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:36:38.243201 zksync2-0.6.0/zksync2/provider/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 11:36:18.000000 zksync2-0.6.0/zksync2/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13089 2023-07-07 11:36:18.000000 zksync2-0.6.0/zksync2/provider/eth_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:36:38.243201 zksync2-0.6.0/zksync2/signer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 11:36:18.000000 zksync2-0.6.0/zksync2/signer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-07-07 11:36:18.000000 zksync2-0.6.0/zksync2/signer/eth_signer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:36:38.247201 zksync2-0.6.0/zksync2/transaction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 11:36:18.000000 zksync2-0.6.0/zksync2/transaction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-07-07 11:36:18.000000 zksync2-0.6.0/zksync2/transaction/transaction712.py
--rw-r--r--   0 runner    (1001) docker     (123)    11491 2023-07-07 11:36:18.000000 zksync2-0.6.0/zksync2/transaction/transaction_builders.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:36:38.235201 zksync2-0.6.0/zksync2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16281 2023-07-07 11:36:38.000000 zksync2-0.6.0/zksync2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-07-07 11:36:38.000000 zksync2-0.6.0/zksync2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 11:36:38.000000 zksync2-0.6.0/zksync2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-07 11:36:38.000000 zksync2-0.6.0/zksync2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-07 11:36:38.000000 zksync2-0.6.0/zksync2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:28.903181 zksync2-0.6.0b1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:28.887180 zksync2-0.6.0b1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:28.891181 zksync2-0.6.0b1/.github/workflows/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1162 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    16283 2023-06-30 00:43:28.903181 zksync2-0.6.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15696 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:28.891181 zksync2-0.6.0b1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/examples/01_deposit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/examples/02_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/examples/03_transfer_erc20_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/examples/04_deploy_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6901 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/examples/05_deploy_create_with_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/examples/06_deploy_create_with_deps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/examples/07_deploy_create2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/examples/08_deploy_create2_deps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/examples/09_withdrawal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/examples/10_finalize_withdrawal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/examples/11_check_balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5305 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/examples/12_deploy_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4700 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/examples/13_deploy_account_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5369 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/examples/14_deploy_account_create2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6980 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/examples/15_use_paymaster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/examples/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:28.887180 zksync2-0.6.0b1/examples/solidity/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:28.891181 zksync2-0.6.0b1/examples/solidity/custom_paymaster/
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/examples/solidity/custom_paymaster/Paymaster.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/examples/solidity/custom_paymaster/Token.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:28.891181 zksync2-0.6.0b1/examples/solidity/custom_paymaster/build/
+-rw-r--r--   0 runner    (1001) docker     (123)    42342 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/examples/solidity/custom_paymaster/build/Paymaster.json
+-rw-r--r--   0 runner    (1001) docker     (123)    65416 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/examples/solidity/custom_paymaster/build/Token.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:28.891181 zksync2-0.6.0b1/examples/solidity/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/examples/solidity/demo/Demo.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/examples/solidity/demo/Foo.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:28.895181 zksync2-0.6.0b1/examples/solidity/demo/build/
+-rw-r--r--   0 runner    (1001) docker     (123)    11955 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/examples/solidity/demo/build/combined.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:28.895181 zksync2-0.6.0b1/examples/solidity/incrementer/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/examples/solidity/incrementer/Incrementer.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:28.895181 zksync2-0.6.0b1/examples/solidity/incrementer/build/
+-rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/examples/solidity/incrementer/build/combined.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:28.895181 zksync2-0.6.0b1/examples/solidity/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/examples/solidity/storage/Storage.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:28.895181 zksync2-0.6.0b1/examples/solidity/storage/build/
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/examples/solidity/storage/build/combined.json
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/examples/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-30 00:43:28.907182 zksync2-0.6.0b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:28.895181 zksync2-0.6.0b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:28.895181 zksync2-0.6.0b1/tests/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)     9467 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/tests/contracts/Counter.json
+-rw-r--r--   0 runner    (1001) docker     (123)   103076 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/tests/contracts/CustomAccount.json
+-rw-r--r--   0 runner    (1001) docker     (123)    48494 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/tests/contracts/CustomPaymaster.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8303 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/tests/contracts/Foo.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15075 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/tests/contracts/Import.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/tests/contracts/SimpleConstructor.json
+-rw-r--r--   0 runner    (1001) docker     (123)    50646 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/tests/contracts/SomeERC20.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/tests/contracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/tests/contracts/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:28.895181 zksync2-0.6.0b1/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/tests/integration/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/tests/integration/test_deposit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9344 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/tests/integration/test_paymaster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/tests/integration/test_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/tests/integration/test_withdraw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/tests/integration/test_zksync_contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42460 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/tests/integration/test_zksync_web3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:28.899181 zksync2-0.6.0b1/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/tests/unit/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/tests/unit/test_contract_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/tests/unit/test_eip712.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/tests/unit/test_eth_signer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/tests/unit/test_transaction712.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:28.899181 zksync2-0.6.0b1/zksync2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:28.899181 zksync2-0.6.0b1/zksync2/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/core/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:28.899181 zksync2-0.6.0b1/zksync2/manage_contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/manage_contracts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:28.903181 zksync2-0.6.0b1/zksync2/manage_contracts/contract_abi/
+-rw-r--r--   0 runner    (1001) docker     (123)     9537 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/manage_contracts/contract_abi/ContractDeployer.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6220 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/manage_contracts/contract_abi/IAllowList.json
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/manage_contracts/contract_abi/IERC1271.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/manage_contracts/contract_abi/IERC20.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/manage_contracts/contract_abi/IEthToken.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5847 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/manage_contracts/contract_abi/IL1Bridge.json
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/manage_contracts/contract_abi/IL1Messenger.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/manage_contracts/contract_abi/IL2Bridge.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/manage_contracts/contract_abi/INonceHolder.json
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/manage_contracts/contract_abi/IPaymasterFlow.json
+-rw-r--r--   0 runner    (1001) docker     (123)    49698 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/manage_contracts/contract_abi/IZkSync.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/manage_contracts/contract_abi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/manage_contracts/contract_encoder_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6301 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/manage_contracts/contract_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/manage_contracts/deploy_addresses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/manage_contracts/erc20_contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/manage_contracts/eth_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/manage_contracts/l1_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/manage_contracts/l2_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/manage_contracts/nonce_holder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/manage_contracts/paymaster_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/manage_contracts/precompute_contract_deployer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14931 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/manage_contracts/zksync_contract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:28.903181 zksync2-0.6.0b1/zksync2/module/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/module/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/module/module_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/module/request_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/module/response_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14805 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/module/zksync_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/module/zksync_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:28.903181 zksync2-0.6.0b1/zksync2/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13089 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/provider/eth_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:28.903181 zksync2-0.6.0b1/zksync2/signer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/signer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/signer/eth_signer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:28.903181 zksync2-0.6.0b1/zksync2/transaction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/transaction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/transaction/transaction712.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11491 2023-06-30 00:43:09.000000 zksync2-0.6.0b1/zksync2/transaction/transaction_builders.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 00:43:28.899181 zksync2-0.6.0b1/zksync2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16283 2023-06-30 00:43:28.000000 zksync2-0.6.0b1/zksync2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-06-30 00:43:28.000000 zksync2-0.6.0b1/zksync2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 00:43:28.000000 zksync2-0.6.0b1/zksync2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-30 00:43:28.000000 zksync2-0.6.0b1/zksync2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-30 00:43:28.000000 zksync2-0.6.0b1/zksync2.egg-info/top_level.txt
```

### Comparing `zksync2-0.6.0/.github/workflows/release.yaml` & `zksync2-0.6.0b1/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/.gitignore` & `zksync2-0.6.0b1/.gitignore`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/PKG-INFO` & `zksync2-0.6.0b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zksync2
-Version: 0.6.0
+Version: 0.6.0b1
 Summary: zkSync2 python client sdk
 Home-page: https://zksync.io
 Author: Danijel Radakovic
 Author-email: Danijel Radakovic <danijel@txfusion.io>
 License: MIT
 Project-URL: Homepage, https://github.com/zksync-sdk/zksync2-python
 Project-URL: Bug Tracker, https://github.com/zksync-sdk/zksync2-python/issues
```

### Comparing `zksync2-0.6.0/README.md` & `zksync2-0.6.0b1/README.md`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/examples/01_deposit.py` & `zksync2-0.6.0b1/examples/01_deposit.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/examples/02_transfer.py` & `zksync2-0.6.0b1/examples/02_transfer.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/examples/03_transfer_erc20_token.py` & `zksync2-0.6.0b1/examples/03_transfer_erc20_token.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 def transfer_erc20(
         token_contract,
         account: LocalAccount,
         address: HexAddress,
         amount: float) -> HexStr:
     """
-       Transfer ERC20 token to a desired address on zkSync network
+       Transfer ETH to a desired address on zkSync network
 
        :param token_contract:
            Instance of ERC20 contract
 
        :param account:
            From which account the transfer will be made
 
@@ -52,27 +52,29 @@
     print(f"Tx status: {tx_receipt['status']}")
 
     return tx_hash
 
 
 if __name__ == "__main__":
     # Byte-format private key
-    PRIVATE_KEY = bytes.fromhex(os.environ.get("PRIVATE_KEY"))
+    # PRIVATE_KEY = bytes.fromhex(os.environ.get("PRIVATE_KEY"))
+    PRIVATE_KEY = bytes.fromhex("7726827caac94a7f9e1b160f7ea819f172f7b6f9d2a97f992c38edeab82d4110")
 
     # Set a provider
-    PROVIDER = "https://testnet.era.zksync.dev"
+    # PROVIDER = "https://testnet.era.zksync.dev"
+    PROVIDER = "http://127.0.0.1:3050"
 
     # Connect to zkSync network
     zk_web3 = ZkSyncBuilder.build(PROVIDER)
 
     # Get account object by providing from private key
     account1: LocalAccount = Account.from_key(PRIVATE_KEY)
-    account2_address = zk_web3.to_checksum_address("0x81E9D85b65E9CC8618D85A1110e4b1DF63fA30d9")
+    account2_address = zk_web3.to_checksum_address("0xa61464658AfeAf65CccaaFD3a512b69A83B77618")
 
-    token_address = zk_web3.to_checksum_address("0xCd9BDa1d0FC539043D4C80103bdF4f9cb108931B")
+    token_address = zk_web3.to_checksum_address("0x2Ed5EfAB90d161DdCC65693bd77c3344200c9a00")
     token_contract = zk_web3.zksync.contract(token_address, abi=get_erc20_abi())
 
     # Show balance before token transfer
     print(f"Account1 Crown balance before transfer: {token_contract.functions.balanceOf(account1.address).call()}")
     print(f"Account2 Crown balance before transfer: {token_contract.functions.balanceOf(account2_address).call()}")
 
     # Perform the ETH transfer
```

### Comparing `zksync2-0.6.0/examples/04_deploy_create.py` & `zksync2-0.6.0b1/examples/04_deploy_create.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/examples/05_deploy_create_with_constructor.py` & `zksync2-0.6.0b1/examples/05_deploy_create_with_constructor.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/examples/06_deploy_create_with_deps.py` & `zksync2-0.6.0b1/examples/06_deploy_create_with_deps.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/examples/07_deploy_create2.py` & `zksync2-0.6.0b1/examples/07_deploy_create2.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/examples/08_deploy_create2_deps.py` & `zksync2-0.6.0b1/examples/08_deploy_create2_deps.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/examples/09_withdrawal.py` & `zksync2-0.6.0b1/examples/09_withdrawal.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/examples/10_finalize_withdrawal.py` & `zksync2-0.6.0b1/examples/10_finalize_withdrawal.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/examples/11_check_balance.py` & `zksync2-0.6.0b1/examples/11_check_balance.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/examples/12_deploy_token.py` & `zksync2-0.6.0b1/examples/12_deploy_token.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/examples/13_deploy_account_create.py` & `zksync2-0.6.0b1/examples/13_deploy_account_create.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/examples/14_deploy_account_create2.py` & `zksync2-0.6.0b1/examples/14_deploy_account_create2.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/examples/15_use_paymaster.py` & `zksync2-0.6.0b1/examples/15_use_paymaster.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/examples/README.md` & `zksync2-0.6.0b1/examples/README.md`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/examples/solidity/custom_paymaster/Paymaster.sol` & `zksync2-0.6.0b1/examples/solidity/custom_paymaster/Paymaster.sol`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/examples/solidity/custom_paymaster/Token.sol` & `zksync2-0.6.0b1/examples/solidity/custom_paymaster/Token.sol`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/examples/solidity/custom_paymaster/build/Paymaster.json` & `zksync2-0.6.0b1/examples/solidity/custom_paymaster/build/Paymaster.json`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/examples/solidity/custom_paymaster/build/Token.json` & `zksync2-0.6.0b1/examples/solidity/custom_paymaster/build/Token.json`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/examples/solidity/demo/build/combined.json` & `zksync2-0.6.0b1/examples/solidity/demo/build/combined.json`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/examples/solidity/incrementer/build/combined.json` & `zksync2-0.6.0b1/examples/solidity/incrementer/build/combined.json`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/examples/solidity/storage/build/combined.json` & `zksync2-0.6.0b1/examples/solidity/storage/build/combined.json`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/pyproject.toml` & `zksync2-0.6.0b1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "zksync2"
-version = "0.6.0"
+version = "0.6.0-beta.1"
 authors = [
   { name="Danijel Radakovic", email="danijel@txfusion.io" },
 ]
 description = "zkSync2 python client sdk"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `zksync2-0.6.0/setup.cfg` & `zksync2-0.6.0b1/setup.cfg`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/tests/contracts/Counter.json` & `zksync2-0.6.0b1/tests/contracts/Counter.json`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/tests/contracts/CustomAccount.json` & `zksync2-0.6.0b1/tests/contracts/CustomAccount.json`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/tests/contracts/CustomPaymaster.json` & `zksync2-0.6.0b1/tests/contracts/CustomPaymaster.json`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/tests/contracts/Foo.json` & `zksync2-0.6.0b1/tests/contracts/Foo.json`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/tests/contracts/Import.json` & `zksync2-0.6.0b1/tests/contracts/Import.json`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/tests/contracts/SimpleConstructor.json` & `zksync2-0.6.0b1/tests/contracts/SimpleConstructor.json`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/tests/contracts/SomeERC20.json` & `zksync2-0.6.0b1/tests/contracts/SomeERC20.json`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/tests/integration/test_config.py` & `zksync2-0.6.0b1/tests/integration/test_config.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/tests/integration/test_deposit.py` & `zksync2-0.6.0b1/tests/integration/test_deposit.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/tests/integration/test_paymaster.py` & `zksync2-0.6.0b1/tests/integration/test_paymaster.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/tests/integration/test_transfer.py` & `zksync2-0.6.0b1/tests/integration/test_transfer.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/tests/integration/test_withdraw.py` & `zksync2-0.6.0b1/tests/integration/test_withdraw.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/tests/integration/test_zksync_contract.py` & `zksync2-0.6.0b1/tests/integration/test_zksync_contract.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/tests/integration/test_zksync_web3.py` & `zksync2-0.6.0b1/tests/integration/test_zksync_web3.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/tests/unit/test_config.py` & `zksync2-0.6.0b1/tests/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/tests/unit/test_contract_deploy.py` & `zksync2-0.6.0b1/tests/unit/test_contract_deploy.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/tests/unit/test_eip712.py` & `zksync2-0.6.0b1/tests/unit/test_eip712.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/tests/unit/test_eth_signer.py` & `zksync2-0.6.0b1/tests/unit/test_eth_signer.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/tests/unit/test_transaction712.py` & `zksync2-0.6.0b1/tests/unit/test_transaction712.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/zksync2/core/types.py` & `zksync2-0.6.0b1/zksync2/core/types.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/zksync2/core/utils.py` & `zksync2-0.6.0b1/zksync2/core/utils.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/zksync2/manage_contracts/contract_abi/ContractDeployer.json` & `zksync2-0.6.0b1/zksync2/manage_contracts/contract_abi/ContractDeployer.json`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/zksync2/manage_contracts/contract_abi/IAllowList.json` & `zksync2-0.6.0b1/zksync2/manage_contracts/contract_abi/IAllowList.json`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/zksync2/manage_contracts/contract_abi/IERC1271.json` & `zksync2-0.6.0b1/zksync2/manage_contracts/contract_abi/IERC1271.json`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/zksync2/manage_contracts/contract_abi/IERC20.json` & `zksync2-0.6.0b1/zksync2/manage_contracts/contract_abi/IERC20.json`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/zksync2/manage_contracts/contract_abi/IEthToken.json` & `zksync2-0.6.0b1/zksync2/manage_contracts/contract_abi/IEthToken.json`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/zksync2/manage_contracts/contract_abi/IL1Bridge.json` & `zksync2-0.6.0b1/zksync2/manage_contracts/contract_abi/IL1Bridge.json`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/zksync2/manage_contracts/contract_abi/IL1Messenger.json` & `zksync2-0.6.0b1/zksync2/manage_contracts/contract_abi/IL1Messenger.json`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/zksync2/manage_contracts/contract_abi/IL2Bridge.json` & `zksync2-0.6.0b1/zksync2/manage_contracts/contract_abi/IL2Bridge.json`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/zksync2/manage_contracts/contract_abi/INonceHolder.json` & `zksync2-0.6.0b1/zksync2/manage_contracts/contract_abi/INonceHolder.json`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/zksync2/manage_contracts/contract_abi/IPaymasterFlow.json` & `zksync2-0.6.0b1/zksync2/manage_contracts/contract_abi/IPaymasterFlow.json`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/zksync2/manage_contracts/contract_abi/IZkSync.json` & `zksync2-0.6.0b1/zksync2/manage_contracts/contract_abi/IZkSync.json`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/zksync2/manage_contracts/contract_encoder_base.py` & `zksync2-0.6.0b1/zksync2/manage_contracts/contract_encoder_base.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/zksync2/manage_contracts/contract_factory.py` & `zksync2-0.6.0b1/zksync2/manage_contracts/contract_factory.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/zksync2/manage_contracts/erc20_contract.py` & `zksync2-0.6.0b1/zksync2/manage_contracts/erc20_contract.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/zksync2/manage_contracts/eth_token.py` & `zksync2-0.6.0b1/zksync2/manage_contracts/eth_token.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/zksync2/manage_contracts/l1_bridge.py` & `zksync2-0.6.0b1/zksync2/manage_contracts/l1_bridge.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/zksync2/manage_contracts/l2_bridge.py` & `zksync2-0.6.0b1/zksync2/manage_contracts/l2_bridge.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/zksync2/manage_contracts/nonce_holder.py` & `zksync2-0.6.0b1/zksync2/manage_contracts/nonce_holder.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/zksync2/manage_contracts/paymaster_utils.py` & `zksync2-0.6.0b1/zksync2/manage_contracts/paymaster_utils.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/zksync2/manage_contracts/precompute_contract_deployer.py` & `zksync2-0.6.0b1/zksync2/manage_contracts/precompute_contract_deployer.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/zksync2/manage_contracts/zksync_contract.py` & `zksync2-0.6.0b1/zksync2/manage_contracts/zksync_contract.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/zksync2/module/middleware.py` & `zksync2-0.6.0b1/zksync2/module/middleware.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/zksync2/module/module_builder.py` & `zksync2-0.6.0b1/zksync2/module/module_builder.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/zksync2/module/request_types.py` & `zksync2-0.6.0b1/zksync2/module/request_types.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/zksync2/module/response_types.py` & `zksync2-0.6.0b1/zksync2/module/response_types.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/zksync2/module/zksync_module.py` & `zksync2-0.6.0b1/zksync2/module/zksync_module.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/zksync2/module/zksync_provider.py` & `zksync2-0.6.0b1/zksync2/module/zksync_provider.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/zksync2/provider/eth_provider.py` & `zksync2-0.6.0b1/zksync2/provider/eth_provider.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/zksync2/signer/eth_signer.py` & `zksync2-0.6.0b1/zksync2/signer/eth_signer.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/zksync2/transaction/transaction712.py` & `zksync2-0.6.0b1/zksync2/transaction/transaction712.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/zksync2/transaction/transaction_builders.py` & `zksync2-0.6.0b1/zksync2/transaction/transaction_builders.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.6.0/zksync2.egg-info/PKG-INFO` & `zksync2-0.6.0b1/zksync2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zksync2
-Version: 0.6.0
+Version: 0.6.0b1
 Summary: zkSync2 python client sdk
 Home-page: https://zksync.io
 Author: Danijel Radakovic
 Author-email: Danijel Radakovic <danijel@txfusion.io>
 License: MIT
 Project-URL: Homepage, https://github.com/zksync-sdk/zksync2-python
 Project-URL: Bug Tracker, https://github.com/zksync-sdk/zksync2-python/issues
```

### Comparing `zksync2-0.6.0/zksync2.egg-info/SOURCES.txt` & `zksync2-0.6.0b1/zksync2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

