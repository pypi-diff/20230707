# Comparing `tmp/kybra-0.5.0rc0.tar.gz` & `tmp/kybra-0.5.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kybra-0.5.0rc0.tar", last modified: Wed Jul  5 21:21:07 2023, max compression
+gzip compressed data, was "kybra-0.5.0rc1.tar", last modified: Fri Jul  7 18:06:08 2023, max compression
```

## Comparing `kybra-0.5.0rc0.tar` & `kybra-0.5.0rc1.tar`

### file list

```diff
@@ -1,328 +1,321 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.070636 kybra-0.5.0rc0/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-07-05 21:21:07.070636 kybra-0.5.0rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.034636 kybra-0.5.0rc0/kybra/
--rw-r--r--   0 runner    (1001) docker     (123)    17603 2023-07-05 21:20:51.000000 kybra-0.5.0rc0/kybra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16227 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/build_wasm_binary_or_exit.py
--rw-r--r--   0 runner    (1001) docker     (123)     9432 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/candid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.034636 kybra-0.5.0rc0/kybra/canisters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/canisters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.038636 kybra-0.5.0rc0/kybra/canisters/ledger/
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/canisters/ledger/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     9521 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/canisters/ledger/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.038636 kybra-0.5.0rc0/kybra/canisters/management/
--rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/canisters/management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/canisters/management/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/canisters/management/bitcoin.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/canisters/management/http.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/canisters/management/tecdsa.py
--rw-r--r--   0 runner    (1001) docker     (123)    80489 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/cargotoml.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/colors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.038636 kybra-0.5.0rc0/kybra/compiler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.038636 kybra-0.5.0rc0/kybra/compiler/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-05 21:21:06.000000 kybra-0.5.0rc0/kybra/compiler/__pycache__/__init__.cpython-310.pyc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.038636 kybra-0.5.0rc0/kybra/compiler/custom_modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/custom_modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.038636 kybra-0.5.0rc0/kybra/compiler/custom_modules/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-05 21:21:06.000000 kybra-0.5.0rc0/kybra/compiler/custom_modules/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-07-05 21:21:06.000000 kybra-0.5.0rc0/kybra/compiler/custom_modules/__pycache__/principal.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/custom_modules/principal.py
--rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/custom_modules/typing.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2609 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/install_rust_dependencies.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.038636 kybra-0.5.0rc0/kybra/compiler/kybra_deployer/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_deployer/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.038636 kybra-0.5.0rc0/kybra/compiler/kybra_deployer/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_deployer/src/errors.rs
--rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_deployer/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.038636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.038636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.042636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/body/
--rw-r--r--   0 runner    (1001) docker     (123)    24504 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/body/async_result_handler.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/body/call_global_python_function.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/body/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/body/unwrap_rust_python_result.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/body/utils.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.042636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/array.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.042636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/errors/
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/errors/invalid_member.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/errors/invalid_subscriptable.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/errors/invalid_target.rs
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/errors/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/errors/none_cannot_be_a_type.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/errors/not_exactly_one_target.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/errors/unsupported_type.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.042636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/func/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.042636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/func/errors/
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/func/errors/func_call_takes_one_arg.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/func/errors/func_formatting.rs
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/func/errors/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/func/errors/return_type_mode.rs
--rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/func/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/func/rust.rs
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/opt.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/primitive.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.042636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/record/
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/record/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.042636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/record/record_members/
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/record/record_members/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.042636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/service/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.046636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/service/errors/
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/service/errors/missing_decorator_error.rs
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/service/errors/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/service/errors/service_must_have_methods.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/service/errors/service_with_non_function_defs.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/service/errors/too_many_decorators.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/service/errors/wrong_decorator.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/service/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/service/rust.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/to_candid_type.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.046636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/tuple/
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/tuple/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/tuple/tuple_members.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/type_alias.rs
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/type_ref.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.046636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/variant/
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/variant/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.046636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/variant/variants_members/
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/variant/variants_members/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.046636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/warnings/
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/warnings/default_value_ignored.rs
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/warnings/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.046636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.046636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/errors/
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/errors/guard_function_name.rs
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/errors/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/errors/multiple_system_methods.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/errors/return_type_must_be_void.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.046636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/heartbeat_method/
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/heartbeat_method/build.rs
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/heartbeat_method/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/heartbeat_method/rust.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.046636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/init_method/
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/init_method/build.rs
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/init_method/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/init_method/rust.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.046636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/inspect_message_method/
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/inspect_message_method/build.rs
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/inspect_message_method/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/inspect_message_method/rust.rs
--rw-r--r--   0 runner    (1001) docker     (123)     5007 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.046636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/post_upgrade_method/
--rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/post_upgrade_method/build.rs
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/post_upgrade_method/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/post_upgrade_method/rust.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.046636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/pre_upgrade_method/
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/pre_upgrade_method/build.rs
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/pre_upgrade_method/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/pre_upgrade_method/rust.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.050636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/query_or_update/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/query_or_update/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/query_or_update/query_method.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/query_or_update/query_or_update.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/query_or_update/rust.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/query_or_update/update_method.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/rust.rs
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/constants.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.050636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/debug/
--rw-r--r--   0 runner    (1001) docker     (123)    33809 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/debug/analyze.rs
--rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/debug/display_string.rs
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/debug/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/debug/test_error.rs
--rw-r--r--   0 runner    (1001) docker     (123)    14547 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/debug/to_hash_string.rs
--rw-r--r--   0 runner    (1001) docker     (123)    11531 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/debug/what_is_it.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.050636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/errors/
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/errors/collect_results.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/errors/compiler_output.rs
--rw-r--r--   0 runner    (1001) docker     (123)     8753 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/errors/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/errors/unreachable.rs
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/exit_codes.rs
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/get_child_class_of.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/get_name.rs
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/get_subscript_slice.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.050636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/guard_function/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.050636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/guard_function/errors/
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/guard_function/errors/guard_functions_param.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/guard_function/errors/guard_functions_return.rs
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/guard_function/errors/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/guard_function/guard_function.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/guard_function/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.050636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/header/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/header/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/header/ref_cells.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/header/traits.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/header/use_statements.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.050636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.058636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/accept_message.rs
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/arg_data_raw.rs
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/arg_data_raw_size.rs
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/caller.rs
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/candid_decode.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/candid_encode.rs
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/canister_balance.rs
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/canister_balance128.rs
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/clear_timer.rs
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/data_certificate.rs
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/id.rs
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/method_name.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_accept.rs
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_accept128.rs
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_available.rs
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_available128.rs
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_refunded.rs
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_refunded128.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/notify_functions.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/notify_raw.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/notify_with_payment128_functions.rs
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/performance_counter.rs
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/print.rs
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/reject.rs
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/reject_code.rs
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/reject_message.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/reply.rs
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/reply_raw.rs
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/set_certified_data.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/set_timer.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/set_timer_interval.rs
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_grow.rs
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_read.rs
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_size.rs
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_write.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.058636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/contains_key.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/get.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/insert.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/is_empty.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/items.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/keys.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/len.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/remove.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/values.rs
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_bytes.rs
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_grow.rs
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_read.rs
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_size.rs
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_write.rs
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/time.rs
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/trap.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/keywords.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.058636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/kybra_modules_init/
--rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/kybra_modules_init/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/main.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.058636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/method_utils/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.058636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/method_utils/errors/
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/method_utils/errors/dictionary_unpacking_operator_not_supported.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/method_utils/errors/first_parameter_must_be_self.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/method_utils/errors/first_parameter_must_not_be_self.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/method_utils/errors/iterator_unpacking_operator_not_supported.rs
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/method_utils/errors/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/method_utils/errors/param_type_annotation_required.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/method_utils/errors/return_type_annotation_required.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/method_utils/errors/too_many_params.rs
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/method_utils/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/method_utils/params.rs
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/method_utils/returns.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.062636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/py_ast/
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/py_ast/errors.rs
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/py_ast/get_stmt_kinds.rs
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/py_ast/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/py_ast/py_ast.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/py_ast/to_act.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.062636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/source_map/
--rw-r--r--   0 runner    (1001) docker     (123)    22031 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/source_map/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.062636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/source_map/token_length/
--rw-r--r--   0 runner    (1001) docker     (123)    28330 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/source_map/token_length/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.062636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.062636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/invalid_memory_id.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_key_size_missing.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_size_must_be_integer_constant.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_size_must_be_non_negative.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_size_too_big.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_value_size_missing.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_must_be_an_integer.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_must_be_integer_constant.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_must_be_non_negative.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_too_big.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/missing_memory_id.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/stable_b_tree_map_node_format.rs
--rw-r--r--   0 runner    (1001) docker     (123)    10126 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.062636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/bounded_storable_impl.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/ref_cell_ident.rs
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/storable_impl.rs
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/try_into_vm_value_impl.rs
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/wrapper_type.rs
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/tuple.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.062636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.066636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/
--rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/basic.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/generic.rs
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     9041 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/numeric.rs
--rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/vec.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.066636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/
--rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/basic.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/generic.rs
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/numeric.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/vec.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.066636 kybra-0.5.0rc0/kybra/compiler/kybra_modules_init/
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_modules_init/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.066636 kybra-0.5.0rc0/kybra/compiler/kybra_modules_init/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_modules_init/src/main.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.066636 kybra-0.5.0rc0/kybra/compiler/kybra_post_install/
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_post_install/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_post_install/build.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.066636 kybra-0.5.0rc0/kybra/compiler/kybra_post_install/src/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_post_install/src/dfx.rs
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_post_install/src/error.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_post_install/src/install_app_canister.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_post_install/src/main.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_post_install/src/permissions.rs
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_post_install/src/upload_app_canister.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_post_install/src/upload_chunk.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_post_install/src/upload_python_stdlib.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.066636 kybra-0.5.0rc0/kybra/compiler/kybra_vm_value_derive/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_vm_value_derive/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.066636 kybra-0.5.0rc0/kybra/compiler/kybra_vm_value_derive/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.066636 kybra-0.5.0rc0/kybra/compiler/kybra_vm_value_derive/src/derive_try_from_vm_value/
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_vm_value_derive/src/derive_try_from_vm_value/derive_try_from_vm_value_enum.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_vm_value_derive/src/derive_try_from_vm_value/derive_try_from_vm_value_struct.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.066636 kybra-0.5.0rc0/kybra/compiler/kybra_vm_value_derive/src/derive_try_into_vm_value/
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_vm_value_derive/src/derive_try_into_vm_value/derive_try_into_vm_value_enum.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_vm_value_derive/src/derive_try_into_vm_value/derive_try_into_vm_value_struct.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_vm_value_derive/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.066636 kybra-0.5.0rc0/kybra/compiler/shared_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/shared_utils/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.066636 kybra-0.5.0rc0/kybra/compiler/shared_utils/src/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/shared_utils/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.066636 kybra-0.5.0rc0/kybra/compiler/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/module_bundler.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/run_kybra_generate_or_exit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/timed.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.034636 kybra-0.5.0rc0/kybra.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-07-05 21:21:06.000000 kybra-0.5.0rc0/kybra.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16636 2023-07-05 21:21:07.000000 kybra-0.5.0rc0/kybra.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 21:21:06.000000 kybra-0.5.0rc0/kybra.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-05 21:21:06.000000 kybra-0.5.0rc0/kybra.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-05 21:21:06.000000 kybra-0.5.0rc0/kybra.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 21:21:07.070636 kybra-0.5.0rc0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:08.737026 kybra-0.5.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-07-07 18:06:08.737026 kybra-0.5.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:08.701024 kybra-0.5.0rc1/kybra/
+-rw-r--r--   0 runner    (1001) docker     (123)    17601 2023-07-07 18:05:50.000000 kybra-0.5.0rc1/kybra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16096 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/build_wasm_binary_or_exit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9432 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/candid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:08.701024 kybra-0.5.0rc1/kybra/canisters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/canisters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:08.701024 kybra-0.5.0rc1/kybra/canisters/ledger/
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/canisters/ledger/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     9521 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/canisters/ledger/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:08.701024 kybra-0.5.0rc1/kybra/canisters/management/
+-rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/canisters/management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/canisters/management/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/canisters/management/bitcoin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/canisters/management/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/canisters/management/tecdsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80489 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/cargotoml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/colors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:08.701024 kybra-0.5.0rc1/kybra/compiler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:08.701024 kybra-0.5.0rc1/kybra/compiler/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-07 18:06:08.000000 kybra-0.5.0rc1/kybra/compiler/__pycache__/__init__.cpython-310.pyc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:08.701024 kybra-0.5.0rc1/kybra/compiler/custom_modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/custom_modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:08.701024 kybra-0.5.0rc1/kybra/compiler/custom_modules/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-07 18:06:08.000000 kybra-0.5.0rc1/kybra/compiler/custom_modules/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-07-07 18:06:08.000000 kybra-0.5.0rc1/kybra/compiler/custom_modules/__pycache__/principal.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/custom_modules/principal.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2609 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/install_rust_dependencies.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:08.705024 kybra-0.5.0rc1/kybra/compiler/kybra_deployer/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_deployer/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:08.705024 kybra-0.5.0rc1/kybra/compiler/kybra_deployer/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_deployer/src/errors.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     6608 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_deployer/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:08.705024 kybra-0.5.0rc1/kybra/compiler/kybra_generate/
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:08.705024 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:08.705024 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/body/
+-rw-r--r--   0 runner    (1001) docker     (123)    24510 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/body/async_result_handler.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/body/call_global_python_function.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/body/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/body/unwrap_rust_python_result.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/body/utils.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:08.705024 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/array.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:08.709025 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/errors/invalid_member.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/errors/invalid_subscriptable.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/errors/invalid_target.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/errors/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/errors/none_cannot_be_a_type.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/errors/not_exactly_one_target.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/errors/unsupported_type.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:08.709025 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/func/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:08.709025 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/func/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/func/errors/func_call_takes_one_arg.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/func/errors/func_formatting.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/func/errors/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/func/errors/return_type_mode.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/func/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/func/rust.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/opt.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/primitive.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:08.709025 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/record/
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/record/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:08.709025 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/record/record_members/
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/record/record_members/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:08.709025 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/service/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:08.709025 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/service/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/service/errors/missing_decorator_error.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/service/errors/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/service/errors/service_must_have_methods.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/service/errors/service_with_non_function_defs.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/service/errors/too_many_decorators.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/service/errors/wrong_decorator.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/service/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/service/rust.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/to_candid_type.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:08.709025 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/tuple/
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/tuple/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/tuple/tuple_members.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/type_alias.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/type_ref.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:08.709025 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/variant/
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/variant/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:08.713025 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/variant/variants_members/
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/variant/variants_members/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:08.713025 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/warnings/
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/warnings/default_value_ignored.rs
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/warnings/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:08.713025 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/canister_method/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:08.713025 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/canister_method/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/canister_method/errors/guard_function_name.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/canister_method/errors/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/canister_method/errors/multiple_system_methods.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/canister_method/errors/return_type_must_be_void.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:08.713025 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/canister_method/heartbeat_method/
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/canister_method/heartbeat_method/build.rs
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/canister_method/heartbeat_method/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/canister_method/heartbeat_method/rust.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:08.713025 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/canister_method/init_method/
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/canister_method/init_method/build.rs
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/canister_method/init_method/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/canister_method/init_method/rust.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:08.713025 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/canister_method/inspect_message_method/
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/canister_method/inspect_message_method/build.rs
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/canister_method/inspect_message_method/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/canister_method/inspect_message_method/rust.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     5007 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/canister_method/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:08.713025 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/canister_method/post_upgrade_method/
+-rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/canister_method/post_upgrade_method/build.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/canister_method/post_upgrade_method/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/canister_method/post_upgrade_method/rust.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:08.713025 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/canister_method/pre_upgrade_method/
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/canister_method/pre_upgrade_method/build.rs
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/canister_method/pre_upgrade_method/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/canister_method/pre_upgrade_method/rust.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:08.717025 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/canister_method/query_or_update/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/canister_method/query_or_update/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/canister_method/query_or_update/query_method.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/canister_method/query_or_update/query_or_update.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/canister_method/query_or_update/rust.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/canister_method/query_or_update/update_method.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/canister_method/rust.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/constants.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:08.717025 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/debug/
+-rw-r--r--   0 runner    (1001) docker     (123)    33809 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/debug/analyze.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/debug/display_string.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/debug/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/debug/test_error.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    14547 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/debug/to_hash_string.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    11531 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/debug/what_is_it.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:08.717025 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/errors/collect_results.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/errors/compiler_output.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     8753 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/errors/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/errors/unreachable.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/exit_codes.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/get_child_class_of.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/get_name.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/get_subscript_slice.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:08.717025 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/guard_function/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:08.717025 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/guard_function/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/guard_function/errors/guard_functions_param.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/guard_function/errors/guard_functions_return.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/guard_function/errors/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/guard_function/guard_function.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/guard_function/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:08.717025 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/header/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/header/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/header/ref_cells.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/header/traits.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/header/use_statements.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:08.717025 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:08.725025 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/accept_message.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/arg_data_raw.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/arg_data_raw_size.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/caller.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/candid_decode.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/candid_encode.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/canister_balance.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/canister_balance128.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/clear_timer.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/data_certificate.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/id.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/method_name.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_accept.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_accept128.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_available.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_available128.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_refunded.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_refunded128.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/notify_functions.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/notify_raw.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/notify_with_payment128_functions.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/performance_counter.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/print.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/reject.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/reject_code.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/reject_message.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/reply.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/reply_raw.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/set_certified_data.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/set_timer.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/set_timer_interval.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_grow.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_read.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_size.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_write.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:08.725025 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/contains_key.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/get.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/insert.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/is_empty.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/items.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/keys.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/len.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/remove.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/values.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/stable_bytes.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/stable_grow.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/stable_read.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/stable_size.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/stable_write.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/time.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/trap.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/keywords.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/main.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:08.729025 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/method_utils/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:08.729025 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/method_utils/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/method_utils/errors/dictionary_unpacking_operator_not_supported.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/method_utils/errors/first_parameter_must_be_self.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/method_utils/errors/first_parameter_must_not_be_self.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/method_utils/errors/iterator_unpacking_operator_not_supported.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/method_utils/errors/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/method_utils/errors/param_type_annotation_required.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/method_utils/errors/return_type_annotation_required.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/method_utils/errors/too_many_params.rs
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/method_utils/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/method_utils/params.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/method_utils/returns.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:08.729025 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/py_ast/
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/py_ast/errors.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/py_ast/get_stmt_kinds.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/py_ast/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/py_ast/py_ast.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/py_ast/to_act.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:08.729025 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/source_map/
+-rw-r--r--   0 runner    (1001) docker     (123)    22031 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/source_map/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:08.729025 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/source_map/token_length/
+-rw-r--r--   0 runner    (1001) docker     (123)    28330 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/source_map/token_length/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:08.729025 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:08.733026 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/invalid_memory_id.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_key_size_missing.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_size_must_be_integer_constant.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_size_must_be_non_negative.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_size_too_big.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_value_size_missing.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_must_be_an_integer.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_must_be_integer_constant.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_must_be_non_negative.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_too_big.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/missing_memory_id.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/stable_b_tree_map_node_format.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    10126 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:08.733026 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/bounded_storable_impl.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/ref_cell_ident.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/storable_impl.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/try_into_vm_value_impl.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/wrapper_type.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/tuple.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:08.733026 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/vm_value_conversion/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/vm_value_conversion/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:08.733026 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/
+-rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/basic.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/generic.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     9041 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/numeric.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/vec.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:08.733026 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/
+-rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/basic.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/generic.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/numeric.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/vec.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:08.733026 kybra-0.5.0rc1/kybra/compiler/kybra_post_install/
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_post_install/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_post_install/build.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:08.737026 kybra-0.5.0rc1/kybra/compiler/kybra_post_install/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_post_install/src/dfx.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_post_install/src/error.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_post_install/src/install_app_canister.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_post_install/src/main.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_post_install/src/permissions.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_post_install/src/upload_app_canister.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_post_install/src/upload_chunk.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_post_install/src/upload_python_stdlib.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:08.737026 kybra-0.5.0rc1/kybra/compiler/kybra_vm_value_derive/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_vm_value_derive/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:08.737026 kybra-0.5.0rc1/kybra/compiler/kybra_vm_value_derive/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:08.737026 kybra-0.5.0rc1/kybra/compiler/kybra_vm_value_derive/src/derive_try_from_vm_value/
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_vm_value_derive/src/derive_try_from_vm_value/derive_try_from_vm_value_enum.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_vm_value_derive/src/derive_try_from_vm_value/derive_try_from_vm_value_struct.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:08.737026 kybra-0.5.0rc1/kybra/compiler/kybra_vm_value_derive/src/derive_try_into_vm_value/
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_vm_value_derive/src/derive_try_into_vm_value/derive_try_into_vm_value_enum.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_vm_value_derive/src/derive_try_into_vm_value/derive_try_into_vm_value_struct.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/kybra_vm_value_derive/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:08.737026 kybra-0.5.0rc1/kybra/compiler/shared_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/shared_utils/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:08.737026 kybra-0.5.0rc1/kybra/compiler/shared_utils/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/shared_utils/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:08.737026 kybra-0.5.0rc1/kybra/compiler/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/compiler/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/module_bundler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/run_kybra_generate_or_exit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/timed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/kybra/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:06:08.701024 kybra-0.5.0rc1/kybra.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-07-07 18:06:08.000000 kybra-0.5.0rc1/kybra.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16445 2023-07-07 18:06:08.000000 kybra-0.5.0rc1/kybra.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 18:06:08.000000 kybra-0.5.0rc1/kybra.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-07 18:06:08.000000 kybra-0.5.0rc1/kybra.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-07 18:06:08.000000 kybra-0.5.0rc1/kybra.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 18:06:08.737026 kybra-0.5.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-07 18:03:12.000000 kybra-0.5.0rc1/setup.py
```

### Comparing `kybra-0.5.0rc0/LICENSE` & `kybra-0.5.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/NOTICE` & `kybra-0.5.0rc1/NOTICE`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/PKG-INFO` & `kybra-0.5.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kybra
-Version: 0.5.0rc0
+Version: 0.5.0rc1
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 
 <div align="center">
     <a href="https://github.com/demergent-labs/kybra" target="_blank" rel="noopener noreferrer">
         <img height="150" src="https://raw.githubusercontent.com/demergent-labs/kybra/main/logo/logo.svg" alt="kybra logo">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kybra Version: 0.5.0rc0 Description-Content-Type:
+Metadata-Version: 2.1 Name: kybra Version: 0.5.0rc1 Description-Content-Type:
 text/markdown License-File: LICENSE License-File: NOTICE
                                  [kybra_logo]
                        [Coverage_Status] [PyPI_version]
 # Kybra (Beta) Python CDK for the [Internet Computer](https://
 internetcomputer.org/). ## Disclaimer Things to keep in mind: - Kybra does not
 yet have many live, successful, continuously operating applications deployed to
 the IC - Kybra does not yet have extensive automated property tests - Kybra
```

### Comparing `kybra-0.5.0rc0/README.md` & `kybra-0.5.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/__init__.py` & `kybra-0.5.0rc1/kybra/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     TypeAlias,
     Union,
 )
 
 # TODO I think we can simplify this just like we're doing with canisters
 from .compiler.custom_modules.principal import Principal as PrincipalRenamed
 
-__version__ = "0.5.0-rc.0"
+__version__ = "0.5.0rc1"
 __rust_version__ = "1.68.2"
 
 Principal = PrincipalRenamed
 
 int64 = int
 int32 = int
 int16 = int
@@ -360,15 +360,15 @@
         return _kybra_ic.performance_counter(counter_type)  # type: ignore
 
     @staticmethod
     def print(x: Any):
         _kybra_ic.print(str(x))  # type: ignore
 
     @staticmethod
-    def reject(x: Any):
+    def reject(x: str):
         _kybra_ic.reject(x)  # type: ignore
 
     @staticmethod
     def reject_code() -> RejectionCode:
         return _kybra_ic.reject_code()  # type: ignore
 
     @staticmethod
```

### Comparing `kybra-0.5.0rc0/kybra/__main__.py` & `kybra-0.5.0rc1/kybra/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -343,39 +343,35 @@
         print(
             f'\nPlease open an issue at https://github.com/demergent-labs/kybra/issues/new\nincluding this message and the following error:\n\n {red(rustfmt_result.stderr.decode("utf-8"))}'
         )
         print("💀 Build failed")
         sys.exit(1)
 
 
-# TODO working on optimization
 @timed_inline
 def optimize_wasm_binary_or_exit(
     paths: Paths, canister_name: str, cargo_env: dict[str, str], verbose: bool = False
 ):
     optimization_result = subprocess.run(
         [
             f"{paths['global_kybra_rust_bin_dir']}/ic-wasm",
             f"{paths['canister']}/{canister_name}_app.wasm",
             "-o",
             f"{paths['canister']}/{canister_name}_app.wasm",
             "shrink",
-            # "--optimize",
-            # "Oz",
         ],
         capture_output=not verbose,
     )
 
     if optimization_result.returncode != 0:
         print(red("\n💣 Kybra error: optimizing generated Wasm"))
         print(optimization_result.stderr.decode("utf-8"))
         print("💀 Build failed")
         sys.exit(1)
 
-    # TODO we should be able to get rid of this now
     add_metadata_to_wasm_or_exit(paths, canister_name, verbose=verbose)
 
     os.system(f"gzip -9 -f -k {paths['canister']}/{canister_name}_app.wasm")
 
 
 def add_metadata_to_wasm_or_exit(
     paths: Paths, canister_name: str, verbose: bool = False
```

### Comparing `kybra-0.5.0rc0/kybra/build_wasm_binary_or_exit.py` & `kybra-0.5.0rc1/kybra/build_wasm_binary_or_exit.py`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/candid.py` & `kybra-0.5.0rc1/kybra/candid.py`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/canisters/ledger/NOTICE` & `kybra-0.5.0rc1/kybra/canisters/ledger/NOTICE`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/canisters/ledger/__init__.py` & `kybra-0.5.0rc1/kybra/canisters/ledger/__init__.py`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/canisters/management/__init__.py` & `kybra-0.5.0rc1/kybra/canisters/management/__init__.py`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/canisters/management/basic.py` & `kybra-0.5.0rc1/kybra/canisters/management/basic.py`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/canisters/management/bitcoin.py` & `kybra-0.5.0rc1/kybra/canisters/management/bitcoin.py`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/canisters/management/http.py` & `kybra-0.5.0rc1/kybra/canisters/management/http.py`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/canisters/management/tecdsa.py` & `kybra-0.5.0rc1/kybra/canisters/management/tecdsa.py`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/cargotoml.py` & `kybra-0.5.0rc1/kybra/cargotoml.py`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/custom_modules/__pycache__/principal.cpython-310.pyc` & `kybra-0.5.0rc1/kybra/compiler/custom_modules/__pycache__/principal.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Jul  5 21:18:30 2023 UTC, .py size: 4555 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 26de a564 cb11 0000  o.......&..d....
+00000000: 6f0d 0d0a 0000 0000 6053 a864 cb11 0000  o.......`S.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7400 0000 6400  .....@...st...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6402 6c04 6d05 5a05 0100 6400 6403 6c06  d.l.m.Z...d.d.l.
 00000060: 6d07 5a07 0100 6404 5a08 6405 5a09 6406  m.Z...d.Z.d.Z.d.
 00000070: 5a0a 4700 6407 6408 8400 6408 6505 8303  Z.G.d.d...d.e...
```

### Comparing `kybra-0.5.0rc0/kybra/compiler/custom_modules/principal.py` & `kybra-0.5.0rc1/kybra/compiler/custom_modules/principal.py`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/install_rust_dependencies.sh` & `kybra-0.5.0rc1/kybra/compiler/install_rust_dependencies.sh`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_deployer/src/errors.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_deployer/src/errors.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_deployer/src/lib.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_deployer/src/lib.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-// TODO Once we upgrade to ic-cdk 0.8.1 and dfx >= 14 something
-// TODO then I think we can use the new ic_cdk::api::is_controller check
-// TODO and get rid of INSTALLER_REF_CELL
-
 use errors::{
     call_result_error_to_string, rejection_code_to_string, value_error_to_string, UnwrapOrTrap,
 };
 use ic_cdk::{
     api::{call, management_canister},
     export::Principal,
 };
@@ -19,15 +15,14 @@
 use shared_utils::{PYTHON_STDLIB_MEMORY_ID, RANDOMNESS_MEMORY_ID};
 use std::cell::RefCell;
 
 mod errors;
 
 thread_local! {
     static WASM_REF_CELL: RefCell<Vec<u8>> = RefCell::new(vec![]);
-    static INSTALLER_REF_CELL: RefCell<Option<String>> = RefCell::new(None);
     static ARG_DATA_RAW_REF_CELL: RefCell<Vec<u8>> = RefCell::new(vec![]);
     static PYTHON_STDLIB_REF_CELL: RefCell<Vec<u8>> = RefCell::new(vec![]);
 
     static RANDOMNESS_STABLE_REF_CELL: RefCell<Cell<Vec<u8>, VirtualMemory<DefaultMemoryImpl>>>
     = RefCell::new(Cell::init(MEMORY_MANAGER_REF_CELL.with(|m| m.borrow().get(MemoryId::new(RANDOMNESS_MEMORY_ID))), vec![]).unwrap_or_trap());
 
     static PYTHON_STDLIB_STABLE_REF_CELL: RefCell<Cell<Vec<u8>, VirtualMemory<DefaultMemoryImpl>>>
@@ -44,56 +39,51 @@
 
 #[post_upgrade]
 pub fn post_upgrade() {
     initialize()
 }
 
 fn initialize() {
-    INSTALLER_REF_CELL.with(|installer_ref_cell| {
-        let mut installer_ref_mut = installer_ref_cell.borrow_mut();
-        *installer_ref_mut = Some(ic_cdk::caller().to_string());
-    });
-
     ARG_DATA_RAW_REF_CELL.with(|arg_data_raw_ref_cell| {
         let mut arg_data_ref_mut = arg_data_raw_ref_cell.borrow_mut();
         *arg_data_ref_mut = call::arg_data_raw();
     });
 }
 
-#[update(guard = "installer_guard")]
+#[update(guard = "controller_guard")]
 pub fn upload_wasm_chunk(bytes: Vec<u8>) {
     WASM_REF_CELL.with(|wasm_ref_cell| {
         let mut wasm_ref_mut = wasm_ref_cell.borrow_mut();
         wasm_ref_mut.extend(bytes);
     });
 }
 
-#[update(guard = "installer_guard")]
+#[update(guard = "controller_guard")]
 pub fn upload_python_stdlib_chunk(bytes: Vec<u8>) {
     PYTHON_STDLIB_REF_CELL.with(|python_stdlib_ref_cell| {
         let mut python_stdlib_ref_mut = python_stdlib_ref_cell.borrow_mut();
         python_stdlib_ref_mut.extend(bytes);
     });
 }
 
-#[query(guard = "installer_guard")]
+#[query(guard = "controller_guard")]
 pub fn get_python_stdlib_hash() -> String {
     PYTHON_STDLIB_STABLE_REF_CELL.with(|python_stdlib_stable_ref_cell| {
         let python_stdlib_stable_ref = python_stdlib_stable_ref_cell.borrow();
         let python_stdlib_bytes = python_stdlib_stable_ref.get();
 
         if python_stdlib_bytes.len() == 0 {
             "".to_string()
         } else {
             hash(python_stdlib_bytes)
         }
     })
 }
 
-#[update(guard = "installer_guard")]
+#[update(guard = "controller_guard")]
 pub async fn install_wasm() -> Result<(), String> {
     stable_store_randomness().await?;
     stable_store_python_stdlib()?;
     install_code().map_err(|err| rejection_code_to_string(&err))
 
     // let wasm_module = WASM_REF_CELL.with(|wasm_ref_cell| wasm_ref_cell.borrow().clone());
 
@@ -178,22 +168,17 @@
     // If install_code succeeds this will never be reached because
     // the install_code call returns to a different Wasm binary
     // and the callback no longer exists
     // If there is an error in the cross-canister call this will be reached
     // result.map_err(|err| call_result_error_to_string(&err))
 }
 
-fn installer_guard() -> Result<(), String> {
-    let installer_option =
-        INSTALLER_REF_CELL.with(|installer_ref_cell| installer_ref_cell.borrow().clone());
-
-    if let Some(installer) = installer_option {
-        if installer == ic_cdk::caller().to_string() {
-            return Ok(());
-        }
+fn controller_guard() -> Result<(), String> {
+    if ic_cdk::api::is_controller(&ic_cdk::caller()) {
+        return Ok(());
     }
 
     Err("Not authorized".to_string())
 }
 
 fn hash(bytes: &Vec<u8>) -> String {
     let mut hasher = Sha256::new();
```

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/Cargo.toml` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/Cargo.toml`

 * *Files 6% similar despite different names*

```diff
@@ -9,12 +9,12 @@
 proc-macro2 = "1.0.43"
 regex = "1.7.0"
 rustpython-parser = { git = "https://github.com/demergent-labs/RustPython", branch = "kybra_initial", default-features = false, features = [] }
 annotate-snippets = "0.9.1"
 num-bigint = "0.4.3"
 backtrace = "0.3.67" # The package isn't strickly neccesary. std::backtrace::Backtrace might be able to do what we need, but it isn't clonable and backtrace::Backtrace is, so we are using to avoid adding a buch of lifetime code
 # rustpython = { path = "../../../../RustPython", default-features = false, features = [] }
-cdk_framework = { git = "https://github.com/demergent-labs/cdk_framework", rev = "e6023d9d9c58e0042c6e7249a2fe06c6ee0248fa" }
+cdk_framework = { git = "https://github.com/demergent-labs/cdk_framework", rev = "1791111b792829da1a474758c5dfafb5cbe9115a" }
 # cdk_framework = { path = "/home/cdk_framework" }
 # For local rust-analyzer uncomment this line and comment out the line above.
 # Update path/to/local to be the path to your local cdk_framework repo
 shared_utils = { path = "../shared_utils" }
```

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/body/async_result_handler.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/body/async_result_handler.rs`

 * *Files 0% similar despite different names*

```diff
@@ -367,15 +367,15 @@
                             let variable_type = param.to_type_annotation(
                                 &context,
                                 method.create_qualified_name(&service.name),
                             );
                             let actual_index = index + 2;
 
                             quote! {
-                                let #variable_name: #variable_type = args[#actual_index]
+                                let #variable_name: (#variable_type) = args[#actual_index]
                                     .clone()
                                     .try_from_vm_value(vm)
                                     .map_err(|vmc_err| vm.new_type_error(vmc_err.0))?;
                             }
                         })
                         .collect();
 
@@ -448,15 +448,15 @@
                             let variable_type = param.to_type_annotation(
                                 &context,
                                 method.create_qualified_name(&service.name),
                             );
                             let actual_index = index + 2;
 
                             quote! {
-                                let #variable_name: #variable_type = args[#actual_index]
+                                let #variable_name: (#variable_type) = args[#actual_index]
                                     .clone()
                                     .try_from_vm_value(vm)
                                     .map_err(|vmc_err| vm.new_type_error(vmc_err.0))?;
                             }
                         })
                         .collect();
 
@@ -537,15 +537,15 @@
                             let variable_type = param.to_type_annotation(
                                 &context,
                                 method.create_qualified_name(&service.name),
                             );
                             let actual_index = index + 2;
 
                             quote! {
-                                let #variable_name: #variable_type = args[#actual_index]
+                                let #variable_name: (#variable_type) = args[#actual_index]
                                     .clone()
                                     .try_from_vm_value(vm)
                                     .map_err(|vmc_err| vm.new_type_error(vmc_err.0))?;
                             }
                         })
                         .collect();
```

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/body/call_global_python_function.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/body/call_global_python_function.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/body/mod.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/body/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/body/unwrap_rust_python_result.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/body/unwrap_rust_python_result.rs`

 * *Files 12% similar despite different names*

```diff
@@ -57,14 +57,32 @@
                 match self {
                     Ok(ok) => ok,
                     Err(err) => ic_cdk::trap(&init_error_to_string(&err)),
                 }
             }
         }
 
+        impl<T> UnwrapOrTrap<T> for candid::Result<T> {
+            fn unwrap_or_trap(self) -> T {
+                match self {
+                    Ok(ok) => ok,
+                    Err(err) => ic_cdk::trap(&format!("CandidError: {}", err.to_string())),
+                }
+            }
+        }
+
+        impl<T> UnwrapOrTrap<T> for Result<T, String> {
+            fn unwrap_or_trap(self) -> T {
+                match self {
+                    Ok(ok) => ok,
+                    Err(err) => ic_cdk::trap(&err),
+                }
+            }
+        }
+
         pub trait UnwrapOrTrapWithVm<T> {
             fn unwrap_or_trap(self, vm: &rustpython::vm::VirtualMachine) -> T;
         }
 
         impl<T> UnwrapOrTrapWithVm<T> for Result<T, rustpython::vm::PyRef<rustpython_vm::builtins::PyBaseException>> {
             fn unwrap_or_trap(self, vm: &rustpython::vm::VirtualMachine) -> T {
                 match self {
```

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/body/utils.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/body/utils.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/array.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/array.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/errors/invalid_member.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/errors/invalid_member.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/errors/invalid_subscriptable.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/errors/invalid_subscriptable.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/errors/invalid_target.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/errors/invalid_target.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/errors/none_cannot_be_a_type.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/errors/none_cannot_be_a_type.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/errors/not_exactly_one_target.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/errors/not_exactly_one_target.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/errors/unsupported_type.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/errors/unsupported_type.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/func/errors/func_call_takes_one_arg.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/func/errors/func_call_takes_one_arg.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/func/errors/func_formatting.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/func/errors/func_formatting.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/func/errors/return_type_mode.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/func/errors/return_type_mode.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/func/mod.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/func/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/func/rust.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/func/rust.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/opt.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/opt.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/primitive.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/primitive.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/record/mod.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/record/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/record/record_members/mod.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/record/record_members/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/service/errors/missing_decorator_error.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/service/errors/missing_decorator_error.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/service/errors/service_must_have_methods.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/service/errors/service_must_have_methods.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/service/errors/service_with_non_function_defs.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/service/errors/service_with_non_function_defs.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/service/errors/too_many_decorators.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/service/errors/too_many_decorators.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/service/errors/wrong_decorator.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/service/errors/wrong_decorator.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/service/mod.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/service/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/service/rust.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/service/rust.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/to_candid_type.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/to_candid_type.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/tuple/mod.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/tuple/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/type_alias.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/type_alias.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/type_ref.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/type_ref.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/variant/mod.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/variant/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/variant/variants_members/mod.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/variant/variants_members/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/warnings/default_value_ignored.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/candid_type/warnings/default_value_ignored.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/errors/guard_function_name.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/canister_method/errors/guard_function_name.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/errors/multiple_system_methods.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/canister_method/errors/multiple_system_methods.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/errors/return_type_must_be_void.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/canister_method/errors/return_type_must_be_void.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/heartbeat_method/build.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/canister_method/heartbeat_method/build.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/heartbeat_method/rust.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/canister_method/heartbeat_method/rust.rs`

 * *Files 18% similar despite different names*

```diff
@@ -7,13 +7,13 @@
 pub fn generate(
     heartbeat_function_def: &SourceMapped<&Located<StmtKind>>,
 ) -> Result<TokenStream, Error> {
     let function_name = heartbeat_function_def.get_name_or_err()?;
 
     Ok(quote! {
         ic_cdk::spawn(async {
-            call_global_python_function(#function_name, ())
+            call_global_python_function::<()>(#function_name, ())
                 .await
-                .unwrap_or_else(|err| ic_cdk::trap(err.as_str()));
+                .unwrap_or_trap();
         });
     })
 }
```

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/init_method/build.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/canister_method/init_method/build.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/inspect_message_method/build.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/canister_method/inspect_message_method/build.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/mod.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/canister_method/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/post_upgrade_method/build.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/canister_method/post_upgrade_method/build.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/post_upgrade_method/rust.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/canister_method/post_upgrade_method/rust.rs`

 * *Files 15% similar despite different names*

```diff
@@ -23,28 +23,40 @@
     let code_init = generate_code_init(entry_module_name);
     let save_global_interpreter = generate_save_global_interpreter();
     let call_to_user_init_or_post_upgrade = generate_call_to_user_init_or_post_upgrade(
         &call_to_init_py_function,
         &call_to_post_upgrade_py_function,
     );
 
+    // TODO the set_timer below is here to allow the developer to see error messages
+    // TODO in their local replica during development. For some reason without
+    // TODO this the error messages can't be seen, I believe because they are part of
+    // TODO the cross-canister call from the kybra_deployer. We can't get that response
+    // TODO currently because the Wasm binary changes before the response returns
+    // TODO and calling the respone callback causes undefined behavior
+    // TODO two possible solutions are coming to these issues, named/default callbacks
+    // TODO and dfx chunk uploading. dfx chunk uploading should allow us to remove the
+    // TODO kybra_deployer entirely, get rid of the post_install process hopefully
+    // TODO and return to regular init/post_upgrade semantics
     Ok(quote! {
-        #randomness
+        ic_cdk_timers::set_timer(std::time::Duration::from_secs(0), move || {
+            #randomness
 
-        unsafe { ic_wasi_polyfill::init(&randomness); };
+            unsafe { ic_wasi_polyfill::init(&randomness); };
 
-        #interpreter_init
+            #interpreter_init
 
-        #ic_object_init
+            #ic_object_init
 
-        #code_init
+            #code_init
 
-        #save_global_interpreter
+            #save_global_interpreter
 
-        #call_to_user_init_or_post_upgrade
+            #call_to_user_init_or_post_upgrade
+        });
     })
 }
 
 fn generate_randomness() -> TokenStream {
     quote! {
         let randomness = RANDOMNESS_STABLE_REF_CELL.with(|randomness_stable_ref_cell| randomness_stable_ref_cell.borrow().get().clone());
```

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/pre_upgrade_method/build.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/canister_method/pre_upgrade_method/build.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/query_or_update/query_method.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/canister_method/query_or_update/query_method.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/query_or_update/query_or_update.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/canister_method/query_or_update/query_or_update.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/query_or_update/rust.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/canister_method/rust.rs`

 * *Files 23% similar despite different names*

```diff
@@ -1,77 +1,43 @@
-use cdk_framework::{
-    act::node::{candid::Primitive, CandidType},
-    traits::CollectResults,
-};
+use cdk_framework::traits::CollectResults;
 use proc_macro2::TokenStream;
 use quote::{format_ident, quote};
-use rustpython_parser::ast::{Located, StmtKind};
-
-use crate::{method_utils::params::InternalOrExternal, source_map::SourceMapped, tuple, Error};
+use rustpython_parser::ast::Located;
+use rustpython_parser::ast::StmtKind;
 
-pub fn generate_body(
-    source_mapped_located_stmtkind: &SourceMapped<&Located<StmtKind>>,
-) -> Result<TokenStream, Vec<Error>> {
-    let (params, return_expression) = (
-        source_mapped_located_stmtkind.build_params(InternalOrExternal::Internal),
-        generate_return_expression(source_mapped_located_stmtkind),
-    )
-        .collect_results()?;
-
-    let name = source_mapped_located_stmtkind.get_name_or_err()?;
+use crate::{
+    kybra_unreachable, method_utils::params::InternalOrExternal, source_map::SourceMapped, tuple,
+    Error,
+};
 
-    let param_conversions = params
-        .iter()
-        .map(|param| {
-            let name = format_ident!("{}", param.get_prefixed_name());
-            quote! {
-                #name.try_into_vm_value(vm).unwrap_or_trap()
+impl SourceMapped<&Located<StmtKind>> {
+    pub fn generate_call_to_py_function(&self) -> Result<TokenStream, Vec<Error>> {
+        match self.node {
+            StmtKind::FunctionDef { .. } => {
+                let (function_name, params) = (
+                    self.get_name_or_err().map_err(Error::into),
+                    self.build_params(InternalOrExternal::Internal),
+                )
+                    .collect_results()?;
+
+                let param_conversions = params
+                    .iter()
+                    .map(|param| {
+                        let name = format_ident!("{}", param.get_prefixed_name());
+                        quote! {
+                            #name.try_into_vm_value(vm).unwrap_or_trap()
+                        }
+                    })
+                    .collect();
+                let params = tuple::generate_tuple(&param_conversions);
+
+                Ok(quote! {
+                    let params = #params;
+
+                    call_global_python_function_sync(#function_name, params)
+                        .unwrap_or_trap()
+                })
             }
-        })
-        .collect();
-
-    let params = tuple::generate_tuple(&param_conversions);
-
-    Ok(quote! {
-        let interpreter = unsafe { INTERPRETER_OPTION.as_mut() }
-            .unwrap_or_trap("SystemError: missing python interpreter");
-        let vm = &interpreter.vm;
-        let params = #params;
-
-        let final_return_value = call_global_python_function(#name, params)
-            .await
-            .unwrap_or_else(|err| ic_cdk::trap(err.as_str()));
-
-        #return_expression
-    })
-}
-
-fn generate_return_expression(
-    kybra_statement: &SourceMapped<&Located<StmtKind>>,
-) -> Result<TokenStream, Vec<Error>> {
-    if kybra_statement.is_manual() {
-        return Ok(quote! {
-            ic_cdk::api::call::ManualReply::empty()
-        });
-    }
-
-    if type_is_null_or_void(kybra_statement.build_return_type()?) {
-        return Ok(quote! {
-            return;
-        });
-    }
-
-    Ok(quote! {
-        final_return_value
-    })
-}
-
-fn type_is_null_or_void(candid_type: CandidType) -> bool {
-    match candid_type {
-        CandidType::Primitive(primitive) => match primitive {
-            Primitive::Null => true,
-            Primitive::Void => true,
-            _ => false,
-        },
-        _ => false,
+            _ => kybra_unreachable!(),
+        }
     }
 }
```

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/query_or_update/update_method.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/canister_method/query_or_update/update_method.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/constants.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/constants.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/debug/analyze.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/debug/analyze.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/debug/display_string.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/debug/display_string.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/debug/test_error.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/debug/test_error.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/debug/to_hash_string.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/debug/to_hash_string.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/debug/what_is_it.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/debug/what_is_it.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/errors/collect_results.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/errors/collect_results.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/errors/compiler_output.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/errors/compiler_output.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/errors/mod.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/errors/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/errors/unreachable.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/errors/unreachable.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/get_child_class_of.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/get_child_class_of.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/get_name.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/get_name.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/guard_function/errors/guard_functions_param.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/guard_function/errors/guard_functions_param.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/guard_function/errors/guard_functions_return.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/guard_function/errors/guard_functions_return.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/guard_function/mod.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/guard_function/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/header/mod.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/header/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/header/ref_cells.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/header/ref_cells.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/header/traits.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/header/traits.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/header/use_statements.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/header/use_statements.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/candid_decode.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/candid_decode.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/candid_encode.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/candid_encode.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/clear_timer.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/clear_timer.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/mod.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_accept.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_accept.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_accept128.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_accept128.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/notify_functions.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/notify_functions.rs`

 * *Files 5% similar despite different names*

```diff
@@ -76,15 +76,15 @@
                 cdk_name: "kybra".to_string(),
             };
             let variable_type =
                 param.to_type_annotation(&context, method.create_qualified_name(canister_name));
             let actual_index = index + 2;
 
             quote! {
-                let #variable_name: #variable_type = args_py_object_refs[#actual_index]
+                let #variable_name: (#variable_type) = args_py_object_refs[#actual_index]
                     .clone()
                     .try_from_vm_value(vm)
                     .map_err(|vmc_err| vm.new_type_error(vmc_err.0))?;
             }
         })
         .collect()
 }
```

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/notify_raw.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/notify_raw.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/notify_with_payment128_functions.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/notify_with_payment128_functions.rs`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
                 cdk_name: "kybra".to_string(),
             };
             let variable_type =
                 param.to_type_annotation(&context, method.create_qualified_name(canister_name));
             let actual_index = index + 2;
 
             quote! {
-                let #variable_name: #variable_type = args_py_object_refs[#actual_index]
+                let #variable_name: (#variable_type) = args_py_object_refs[#actual_index]
                     .clone()
                     .try_from_vm_value(vm)
                     .map_err(|vmc_err| vm.new_type_error(vmc_err.0))?;
             }
         })
         .collect()
 }
```

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/performance_counter.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/performance_counter.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/print.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/print.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/reject.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/reject.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/reply.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/reply.rs`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         cdk_name: "kybra".to_string(),
     };
     let return_type = update_method
         .return_type
         .to_type_annotation(&context, update_method.name.clone());
     quote!(
         #name => {
-            let reply_value: #return_type = reply_value_py_object_ref
+            let reply_value: (#return_type) = reply_value_py_object_ref
                 .try_from_vm_value(vm)
                 .map_err(|vmc_err| vm.new_type_error(vmc_err.0))?;
             ic_cdk::api::call::reply((reply_value,))
                 .try_into_vm_value(vm)
                 .map_err(|vmc_err| vm.new_type_error(vmc_err.0))
         }
     )
@@ -86,15 +86,15 @@
         cdk_name: "kybra".to_string(),
     };
     let return_type = query_method
         .return_type
         .to_type_annotation(&context, query_method.name.clone());
     quote!(
         #name => {
-            let reply_value: #return_type = reply_value_py_object_ref
+            let reply_value: (#return_type) = reply_value_py_object_ref
                 .try_from_vm_value(vm)
                 .map_err(|vmc_err| vm.new_type_error(vmc_err.0))?;
             ic_cdk::api::call::reply((reply_value,))
                 .try_into_vm_value(vm)
                 .map_err(|vmc_err| vm.new_type_error(vmc_err.0))
         }
     )
```

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/reply_raw.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/reply_raw.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/set_certified_data.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/set_certified_data.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/set_timer.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/set_timer.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/set_timer_interval.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/set_timer_interval.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_grow.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_grow.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_read.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_read.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_write.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_write.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/contains_key.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/contains_key.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/get.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/get.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/insert.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/insert.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/is_empty.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/is_empty.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/items.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/items.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/keys.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/keys.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/len.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/len.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/mod.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/remove.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/remove.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/values.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/values.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_grow.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/stable_grow.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_read.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/stable_read.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_write.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/stable_write.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/trap.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/functions/trap.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/mod.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/ic_object/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/lib.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/lib.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/main.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/main.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/method_utils/errors/dictionary_unpacking_operator_not_supported.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/method_utils/errors/dictionary_unpacking_operator_not_supported.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/method_utils/errors/first_parameter_must_be_self.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/method_utils/errors/first_parameter_must_be_self.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/method_utils/errors/first_parameter_must_not_be_self.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/method_utils/errors/first_parameter_must_not_be_self.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/method_utils/errors/iterator_unpacking_operator_not_supported.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/method_utils/errors/iterator_unpacking_operator_not_supported.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/method_utils/errors/mod.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/method_utils/errors/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/method_utils/errors/param_type_annotation_required.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/method_utils/errors/param_type_annotation_required.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/method_utils/errors/return_type_annotation_required.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/method_utils/errors/return_type_annotation_required.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/method_utils/errors/too_many_params.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/method_utils/errors/too_many_params.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/method_utils/params.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/method_utils/params.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/method_utils/returns.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/method_utils/returns.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/py_ast/get_stmt_kinds.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/py_ast/get_stmt_kinds.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/py_ast/py_ast.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/py_ast/py_ast.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/py_ast/to_act.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/py_ast/to_act.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/source_map/mod.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/source_map/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/source_map/token_length/mod.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/source_map/token_length/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/invalid_memory_id.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/invalid_memory_id.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_key_size_missing.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_key_size_missing.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_size_must_be_integer_constant.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_size_must_be_integer_constant.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_size_must_be_non_negative.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_size_must_be_non_negative.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_size_too_big.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_size_too_big.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_value_size_missing.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_value_size_missing.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_must_be_an_integer.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_must_be_an_integer.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_must_be_integer_constant.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_must_be_integer_constant.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_must_be_non_negative.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_must_be_non_negative.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_too_big.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_too_big.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/missing_memory_id.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/missing_memory_id.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/mod.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/stable_b_tree_map_node_format.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/stable_b_tree_map_node_format.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/mod.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/mod.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/wrapper_type.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/wrapper_type.rs`

 * *Files 2% similar despite different names*

```diff
@@ -24,11 +24,11 @@
     let key_type = &candid_type.to_type_annotation(&context, wrapper_struct_name.clone());
     let wrapper_struct_name_ident = wrapper_struct_name.to_ident();
 
     (
         wrapper_struct_name_ident.clone(),
         quote! {
             #[derive(candid::CandidType, candid::Deserialize, CdkActTryFromVmValue, Ord, PartialOrd, Eq, PartialEq, Clone)]
-            struct #wrapper_struct_name_ident(#key_type);
+            struct #wrapper_struct_name_ident((#key_type));
         },
     )
 }
```

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/basic.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/basic.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/generic.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/generic.rs`

 * *Files 19% similar despite different names*

```diff
@@ -38,9 +38,18 @@
                     match self.try_from_vm_value(vm) {
                         Ok(value) => Ok(Some(value)),
                         Err(err) => Err(err)
                     }
                 }
             }
         }
+
+        impl<T> CdkActTryFromVmValue<ic_cdk::api::call::ManualReply<T>, &rustpython::vm::VirtualMachine> for rustpython::vm::PyObjectRef
+        where
+            rustpython::vm::PyObjectRef: for<'a> CdkActTryFromVmValue<T, &'a rustpython::vm::VirtualMachine>
+        {
+            fn try_from_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<ic_cdk::api::call::ManualReply<T>, CdkActTryFromVmValueError> {
+                Ok(ic_cdk::api::call::ManualReply::empty())
+            }
+        }
     }
 }
```

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/numeric.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/numeric.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/vec.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/vec.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/basic.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/basic.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/generic.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/generic.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/numeric.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/numeric.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/vec.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/vec.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_post_install/Cargo.toml` & `kybra-0.5.0rc1/kybra/compiler/kybra_post_install/Cargo.toml`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_post_install/build.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_post_install/build.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_post_install/src/dfx.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_post_install/src/dfx.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_post_install/src/install_app_canister.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_post_install/src/install_app_canister.rs`

 * *Files 10% similar despite different names*

```diff
@@ -21,15 +21,14 @@
     if !install_output.status.success() {
         handle_install_app_canister_failure(&install_output)?;
     }
 
     Ok(())
 }
 
-// TODO this should be printing the error out
 fn handle_install_app_canister_failure(
     install_output: &std::process::Output,
 ) -> Result<(), String> {
     let error_message = String::from_utf8_lossy(&install_output.stderr);
 
     if !error_message.contains("did not reply to the call")
         && !error_message.contains("function invocation does not match its signature")
```

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_post_install/src/main.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_post_install/src/main.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_post_install/src/permissions.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_post_install/src/permissions.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_post_install/src/upload_app_canister.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_post_install/src/upload_app_canister.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_post_install/src/upload_chunk.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_post_install/src/upload_chunk.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_post_install/src/upload_python_stdlib.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_post_install/src/upload_python_stdlib.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_vm_value_derive/src/derive_try_from_vm_value/derive_try_from_vm_value_enum.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_vm_value_derive/src/derive_try_from_vm_value/derive_try_from_vm_value_enum.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_vm_value_derive/src/derive_try_from_vm_value/derive_try_from_vm_value_struct.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_vm_value_derive/src/derive_try_from_vm_value/derive_try_from_vm_value_struct.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_vm_value_derive/src/derive_try_into_vm_value/derive_try_into_vm_value_enum.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_vm_value_derive/src/derive_try_into_vm_value/derive_try_into_vm_value_enum.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_vm_value_derive/src/derive_try_into_vm_value/derive_try_into_vm_value_struct.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_vm_value_derive/src/derive_try_into_vm_value/derive_try_into_vm_value_struct.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/compiler/kybra_vm_value_derive/src/lib.rs` & `kybra-0.5.0rc1/kybra/compiler/kybra_vm_value_derive/src/lib.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/module_bundler.py` & `kybra-0.5.0rc1/kybra/module_bundler.py`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/run_kybra_generate_or_exit.py` & `kybra-0.5.0rc1/kybra/run_kybra_generate_or_exit.py`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/timed.py` & `kybra-0.5.0rc1/kybra/timed.py`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra/types.py` & `kybra-0.5.0rc1/kybra/types.py`

 * *Files identical despite different names*

### Comparing `kybra-0.5.0rc0/kybra.egg-info/PKG-INFO` & `kybra-0.5.0rc1/kybra.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kybra
-Version: 0.5.0rc0
+Version: 0.5.0rc1
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 
 <div align="center">
     <a href="https://github.com/demergent-labs/kybra" target="_blank" rel="noopener noreferrer">
         <img height="150" src="https://raw.githubusercontent.com/demergent-labs/kybra/main/logo/logo.svg" alt="kybra logo">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kybra Version: 0.5.0rc0 Description-Content-Type:
+Metadata-Version: 2.1 Name: kybra Version: 0.5.0rc1 Description-Content-Type:
 text/markdown License-File: LICENSE License-File: NOTICE
                                  [kybra_logo]
                        [Coverage_Status] [PyPI_version]
 # Kybra (Beta) Python CDK for the [Internet Computer](https://
 internetcomputer.org/). ## Disclaimer Things to keep in mind: - Kybra does not
 yet have many live, successful, continuously operating applications deployed to
 the IC - Kybra does not yet have extensive automated property tests - Kybra
```

### Comparing `kybra-0.5.0rc0/kybra.egg-info/SOURCES.txt` & `kybra-0.5.0rc1/kybra.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 kybra/canisters/management/http.py
 kybra/canisters/management/tecdsa.py
 kybra/compiler/__init__.py
 kybra/compiler/install_rust_dependencies.sh
 kybra/compiler/__pycache__/__init__.cpython-310.pyc
 kybra/compiler/custom_modules/__init__.py
 kybra/compiler/custom_modules/principal.py
-kybra/compiler/custom_modules/typing.py
 kybra/compiler/custom_modules/__pycache__/__init__.cpython-310.pyc
 kybra/compiler/custom_modules/__pycache__/principal.cpython-310.pyc
 kybra/compiler/kybra_deployer/Cargo.toml
 kybra/compiler/kybra_deployer/src/errors.rs
 kybra/compiler/kybra_deployer/src/lib.rs
 kybra/compiler/kybra_generate/Cargo.toml
 kybra/compiler/kybra_generate/src/constants.rs
@@ -183,15 +182,14 @@
 kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/is_empty.rs
 kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/items.rs
 kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/keys.rs
 kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/len.rs
 kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/mod.rs
 kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/remove.rs
 kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/values.rs
-kybra/compiler/kybra_generate/src/kybra_modules_init/mod.rs
 kybra/compiler/kybra_generate/src/method_utils/mod.rs
 kybra/compiler/kybra_generate/src/method_utils/params.rs
 kybra/compiler/kybra_generate/src/method_utils/returns.rs
 kybra/compiler/kybra_generate/src/method_utils/errors/dictionary_unpacking_operator_not_supported.rs
 kybra/compiler/kybra_generate/src/method_utils/errors/first_parameter_must_be_self.rs
 kybra/compiler/kybra_generate/src/method_utils/errors/first_parameter_must_not_be_self.rs
 kybra/compiler/kybra_generate/src/method_utils/errors/iterator_unpacking_operator_not_supported.rs
@@ -233,16 +231,14 @@
 kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/numeric.rs
 kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/vec.rs
 kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/basic.rs
 kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/generic.rs
 kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/mod.rs
 kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/numeric.rs
 kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/vec.rs
-kybra/compiler/kybra_modules_init/Cargo.toml
-kybra/compiler/kybra_modules_init/src/main.rs
 kybra/compiler/kybra_post_install/Cargo.toml
 kybra/compiler/kybra_post_install/build.rs
 kybra/compiler/kybra_post_install/src/dfx.rs
 kybra/compiler/kybra_post_install/src/error.rs
 kybra/compiler/kybra_post_install/src/install_app_canister.rs
 kybra/compiler/kybra_post_install/src/main.rs
 kybra/compiler/kybra_post_install/src/permissions.rs
```

### Comparing `kybra-0.5.0rc0/setup.py` & `kybra-0.5.0rc1/setup.py`

 * *Files identical despite different names*

