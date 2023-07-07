# Comparing `tmp/netqasm-0.9.0.tar.gz` & `tmp/netqasm-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netqasm-0.9.0.tar", last modified: Thu Mar  3 14:44:35 2022, max compression
+gzip compressed data, was "netqasm-0.9.1.tar", last modified: Thu Apr  7 14:53:27 2022, max compression
```

## Comparing `netqasm-0.9.0.tar` & `netqasm-0.9.1.tar`

### file list

```diff
@@ -1,624 +1,624 @@
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:35.732219 netqasm-0.9.0/
--rw-rw-r--   0 bart      (1000) bart      (1000)      186 2022-01-17 15:35:34.000000 netqasm-0.9.0/.flake8
--rw-rw-r--   0 bart      (1000) bart      (1000)    11644 2022-02-28 14:01:35.000000 netqasm-0.9.0/CHANGELOG.md
--rw-rw-r--   0 bart      (1000) bart      (1000)     1063 2022-02-28 13:02:08.000000 netqasm-0.9.0/LICENSE
--rw-rw-r--   0 bart      (1000) bart      (1000)      210 2022-01-17 15:40:12.000000 netqasm-0.9.0/MANIFEST.in
--rw-rw-r--   0 bart      (1000) bart      (1000)     2736 2022-02-28 13:02:08.000000 netqasm-0.9.0/Makefile
--rw-rw-r--   0 bart      (1000) bart      (1000)     5201 2022-03-03 14:44:35.732219 netqasm-0.9.0/PKG-INFO
--rw-rw-r--   0 bart      (1000) bart      (1000)     4841 2022-02-28 14:01:35.000000 netqasm-0.9.0/README.md
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:34.832208 netqasm-0.9.0/docs/
--rw-rw-r--   0 bart      (1000) bart      (1000)      912 2021-05-19 15:28:08.000000 netqasm-0.9.0/docs/Makefile
--rw-rw-r--   0 bart      (1000) bart      (1000)      504 2022-01-17 15:35:34.000000 netqasm-0.9.0/docs/README.md
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:34.836208 netqasm-0.9.0/docs/api_backend/
--rw-rw-r--   0 bart      (1000) bart      (1000)      174 2022-01-17 15:35:34.000000 netqasm-0.9.0/docs/api_backend/netqasm.backend.executor.rst
--rw-rw-r--   0 bart      (1000) bart      (1000)      174 2022-01-17 15:35:34.000000 netqasm-0.9.0/docs/api_backend/netqasm.backend.messages.rst
--rw-rw-r--   0 bart      (1000) bart      (1000)      188 2022-01-17 15:35:34.000000 netqasm-0.9.0/docs/api_backend/netqasm.backend.network_stack.rst
--rw-rw-r--   0 bart      (1000) bart      (1000)      172 2022-01-17 15:35:34.000000 netqasm-0.9.0/docs/api_backend/netqasm.backend.qnodeos.rst
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:34.848208 netqasm-0.9.0/docs/api_lang/
--rw-rw-r--   0 bart      (1000) bart      (1000)      168 2022-01-17 15:35:34.000000 netqasm-0.9.0/docs/api_lang/netqasm.lang.encoding.rst
--rw-rw-r--   0 bart      (1000) bart      (1000)      816 2022-01-17 15:35:34.000000 netqasm-0.9.0/docs/api_lang/netqasm.lang.instr.rst
--rw-rw-r--   0 bart      (1000) bart      (1000)      156 2022-01-17 15:35:34.000000 netqasm-0.9.0/docs/api_lang/netqasm.lang.ir.rst
--rw-rw-r--   0 bart      (1000) bart      (1000)      166 2022-01-17 15:35:34.000000 netqasm-0.9.0/docs/api_lang/netqasm.lang.operand.rst
--rw-rw-r--   0 bart      (1000) bart      (1000)      366 2022-01-17 15:35:34.000000 netqasm-0.9.0/docs/api_lang/netqasm.lang.parsing.rst
--rw-rw-r--   0 bart      (1000) bart      (1000)      172 2022-01-17 15:35:34.000000 netqasm-0.9.0/docs/api_lang/netqasm.lang.subroutine.rst
--rw-rw-r--   0 bart      (1000) bart      (1000)      166 2022-01-17 15:35:34.000000 netqasm-0.9.0/docs/api_lang/netqasm.lang.symbols.rst
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:34.852208 netqasm-0.9.0/docs/api_logging/
--rw-rw-r--   0 bart      (1000) bart      (1000)      170 2022-01-17 15:35:34.000000 netqasm-0.9.0/docs/api_logging/netqasm.logging.glob.rst
--rw-rw-r--   0 bart      (1000) bart      (1000)      166 2022-01-17 15:35:34.000000 netqasm-0.9.0/docs/api_logging/netqasm.logging.output.rst
--rw-rw-r--   0 bart      (1000) bart      (1000)      176 2022-02-28 13:02:08.000000 netqasm-0.9.0/docs/api_root.rst
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:34.868208 netqasm-0.9.0/docs/api_runtime/
--rw-rw-r--   0 bart      (1000) bart      (1000)      179 2022-02-28 13:02:08.000000 netqasm-0.9.0/docs/api_runtime/netqasm.runtime.app_config.rst
--rw-rw-r--   0 bart      (1000) bart      (1000)      182 2022-02-28 13:02:08.000000 netqasm-0.9.0/docs/api_runtime/netqasm.runtime.application.rst
--rw-rw-r--   0 bart      (1000) bart      (1000)      164 2022-01-17 15:35:34.000000 netqasm-0.9.0/docs/api_runtime/netqasm.runtime.cli.rst
--rw-rw-r--   0 bart      (1000) bart      (1000)      168 2022-01-17 15:35:34.000000 netqasm-0.9.0/docs/api_runtime/netqasm.runtime.debug.rst
--rw-rw-r--   0 bart      (1000) bart      (1000)      164 2022-01-17 15:35:34.000000 netqasm-0.9.0/docs/api_runtime/netqasm.runtime.env.rst
--rw-rw-r--   0 bart      (1000) bart      (1000)      174 2022-01-17 15:35:34.000000 netqasm-0.9.0/docs/api_runtime/netqasm.runtime.hardware.rst
--rw-rw-r--   0 bart      (1000) bart      (1000)      593 2022-02-28 13:02:08.000000 netqasm-0.9.0/docs/api_runtime/netqasm.runtime.interface.rst
--rw-rw-r--   0 bart      (1000) bart      (1000)      185 2022-02-28 13:02:08.000000 netqasm-0.9.0/docs/api_runtime/netqasm.runtime.process_logs.rst
--rw-rw-r--   0 bart      (1000) bart      (1000)      174 2022-01-17 15:35:34.000000 netqasm-0.9.0/docs/api_runtime/netqasm.runtime.settings.rst
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:34.892208 netqasm-0.9.0/docs/api_sdk/
--rw-rw-r--   0 bart      (1000) bart      (1000)      164 2022-01-17 15:35:34.000000 netqasm-0.9.0/docs/api_sdk/netqasm.sdk.builder.rst
--rw-rw-r--   0 bart      (1000) bart      (1000)     1493 2022-02-28 13:02:08.000000 netqasm-0.9.0/docs/api_sdk/netqasm.sdk.classical_communication.rst
--rw-rw-r--   0 bart      (1000) bart      (1000)      168 2022-01-17 15:35:34.000000 netqasm-0.9.0/docs/api_sdk/netqasm.sdk.compiling.rst
--rw-rw-r--   0 bart      (1000) bart      (1000)      162 2022-01-17 15:35:34.000000 netqasm-0.9.0/docs/api_sdk/netqasm.sdk.config.rst
--rw-rw-r--   0 bart      (1000) bart      (1000)      170 2022-01-17 15:35:34.000000 netqasm-0.9.0/docs/api_sdk/netqasm.sdk.connection.rst
--rw-rw-r--   0 bart      (1000) bart      (1000)      170 2022-01-17 15:35:34.000000 netqasm-0.9.0/docs/api_sdk/netqasm.sdk.epr_socket.rst
--rw-rw-r--   0 bart      (1000) bart      (1000)      166 2022-01-17 15:35:34.000000 netqasm-0.9.0/docs/api_sdk/netqasm.sdk.external.rst
--rw-rw-r--   0 bart      (1000) bart      (1000)      164 2022-01-17 15:35:34.000000 netqasm-0.9.0/docs/api_sdk/netqasm.sdk.futures.rst
--rw-rw-r--   0 bart      (1000) bart      (1000)      164 2022-01-17 15:35:34.000000 netqasm-0.9.0/docs/api_sdk/netqasm.sdk.network.rst
--rw-rw-r--   0 bart      (1000) bart      (1000)      174 2022-01-17 15:35:34.000000 netqasm-0.9.0/docs/api_sdk/netqasm.sdk.progress_bar.rst
--rw-rw-r--   0 bart      (1000) bart      (1000)      160 2022-01-17 15:35:34.000000 netqasm-0.9.0/docs/api_sdk/netqasm.sdk.qubit.rst
--rw-rw-r--   0 bart      (1000) bart      (1000)      176 2022-01-17 15:35:34.000000 netqasm-0.9.0/docs/api_sdk/netqasm.sdk.shared_memory.rst
--rw-rw-r--   0 bart      (1000) bart      (1000)      994 2022-01-17 15:35:34.000000 netqasm-0.9.0/docs/api_sdk/netqasm.sdk.toolbox.rst
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:34.892208 netqasm-0.9.0/docs/api_util/
--rw-rw-r--   0 bart      (1000) bart      (1000)      162 2022-01-17 15:35:34.000000 netqasm-0.9.0/docs/api_util/netqasm.util.error.rst
--rw-rw-r--   0 bart      (1000) bart      (1000)      158 2022-01-17 15:35:34.000000 netqasm-0.9.0/docs/api_util/netqasm.util.log.rst
--rw-rw-r--   0 bart      (1000) bart      (1000)      179 2022-01-17 15:35:34.000000 netqasm-0.9.0/docs/api_util/netqasm.util.quantum_gates.rst
--rw-rw-r--   0 bart      (1000) bart      (1000)      164 2022-01-17 15:35:34.000000 netqasm-0.9.0/docs/api_util/netqasm.util.states.rst
--rw-rw-r--   0 bart      (1000) bart      (1000)      164 2022-01-17 15:35:34.000000 netqasm-0.9.0/docs/api_util/netqasm.util.string.rst
--rw-rw-r--   0 bart      (1000) bart      (1000)      164 2022-01-17 15:35:34.000000 netqasm-0.9.0/docs/api_util/netqasm.util.thread.rst
--rw-rw-r--   0 bart      (1000) bart      (1000)      160 2022-01-17 15:35:34.000000 netqasm-0.9.0/docs/api_util/netqasm.util.yaml.rst
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:34.736207 netqasm-0.9.0/docs/build/
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:34.924209 netqasm-0.9.0/docs/build/doctrees/
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:34.932209 netqasm-0.9.0/docs/build/doctrees/api_backend/
--rw-rw-r--   0 bart      (1000) bart      (1000)    82242 2021-11-25 15:03:24.000000 netqasm-0.9.0/docs/build/doctrees/api_backend/netqasm.backend.executor.doctree
--rw-rw-r--   0 bart      (1000) bart      (1000)   139066 2021-11-25 15:03:25.000000 netqasm-0.9.0/docs/build/doctrees/api_backend/netqasm.backend.messages.doctree
--rw-rw-r--   0 bart      (1000) bart      (1000)    28783 2021-11-25 15:03:25.000000 netqasm-0.9.0/docs/build/doctrees/api_backend/netqasm.backend.network_stack.doctree
--rw-rw-r--   0 bart      (1000) bart      (1000)    33566 2021-11-25 15:03:25.000000 netqasm-0.9.0/docs/build/doctrees/api_backend/netqasm.backend.qnodeos.doctree
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:34.956209 netqasm-0.9.0/docs/build/doctrees/api_lang/
--rw-rw-r--   0 bart      (1000) bart      (1000)   171040 2021-11-25 15:03:26.000000 netqasm-0.9.0/docs/build/doctrees/api_lang/netqasm.lang.encoding.doctree
--rw-rw-r--   0 bart      (1000) bart      (1000)  1273221 2021-11-25 15:03:28.000000 netqasm-0.9.0/docs/build/doctrees/api_lang/netqasm.lang.instr.doctree
--rw-rw-r--   0 bart      (1000) bart      (1000)    95126 2021-11-25 15:03:28.000000 netqasm-0.9.0/docs/build/doctrees/api_lang/netqasm.lang.ir.doctree
--rw-rw-r--   0 bart      (1000) bart      (1000)    54066 2021-11-25 15:03:28.000000 netqasm-0.9.0/docs/build/doctrees/api_lang/netqasm.lang.operand.doctree
--rw-rw-r--   0 bart      (1000) bart      (1000)    49063 2021-11-25 15:03:29.000000 netqasm-0.9.0/docs/build/doctrees/api_lang/netqasm.lang.parsing.doctree
--rw-rw-r--   0 bart      (1000) bart      (1000)    16479 2021-11-25 15:03:29.000000 netqasm-0.9.0/docs/build/doctrees/api_lang/netqasm.lang.subroutine.doctree
--rw-rw-r--   0 bart      (1000) bart      (1000)    17646 2021-11-25 15:03:29.000000 netqasm-0.9.0/docs/build/doctrees/api_lang/netqasm.lang.symbols.doctree
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:34.960209 netqasm-0.9.0/docs/build/doctrees/api_logging/
--rw-rw-r--   0 bart      (1000) bart      (1000)    35023 2021-11-25 15:03:29.000000 netqasm-0.9.0/docs/build/doctrees/api_logging/netqasm.logging.glob.doctree
--rw-rw-r--   0 bart      (1000) bart      (1000)    12936 2021-11-25 15:03:29.000000 netqasm-0.9.0/docs/build/doctrees/api_logging/netqasm.logging.output.doctree
--rw-rw-r--   0 bart      (1000) bart      (1000)     2764 2021-11-25 15:03:29.000000 netqasm-0.9.0/docs/build/doctrees/api_root.doctree
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:34.976209 netqasm-0.9.0/docs/build/doctrees/api_runtime/
--rw-rw-r--   0 bart      (1000) bart      (1000)    22045 2021-11-25 15:03:29.000000 netqasm-0.9.0/docs/build/doctrees/api_runtime/netqasm.runtime.app_config.doctree
--rw-rw-r--   0 bart      (1000) bart      (1000)    87474 2021-11-25 15:03:29.000000 netqasm-0.9.0/docs/build/doctrees/api_runtime/netqasm.runtime.application.doctree
--rw-rw-r--   0 bart      (1000) bart      (1000)     3904 2021-11-25 15:03:30.000000 netqasm-0.9.0/docs/build/doctrees/api_runtime/netqasm.runtime.cli.doctree
--rw-rw-r--   0 bart      (1000) bart      (1000)     8798 2021-11-25 15:03:30.000000 netqasm-0.9.0/docs/build/doctrees/api_runtime/netqasm.runtime.debug.doctree
--rw-rw-r--   0 bart      (1000) bart      (1000)    27798 2021-11-25 15:03:30.000000 netqasm-0.9.0/docs/build/doctrees/api_runtime/netqasm.runtime.env.doctree
--rw-rw-r--   0 bart      (1000) bart      (1000)     9841 2021-11-25 15:03:30.000000 netqasm-0.9.0/docs/build/doctrees/api_runtime/netqasm.runtime.hardware.doctree
--rw-rw-r--   0 bart      (1000) bart      (1000)   211388 2021-11-25 15:03:30.000000 netqasm-0.9.0/docs/build/doctrees/api_runtime/netqasm.runtime.interface.doctree
--rw-rw-r--   0 bart      (1000) bart      (1000)     5378 2021-11-26 13:17:03.000000 netqasm-0.9.0/docs/build/doctrees/api_runtime/netqasm.runtime.process_logs.doctree
--rw-rw-r--   0 bart      (1000) bart      (1000)    22712 2021-11-25 15:03:30.000000 netqasm-0.9.0/docs/build/doctrees/api_runtime/netqasm.runtime.settings.doctree
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:35.008210 netqasm-0.9.0/docs/build/doctrees/api_sdk/
--rw-rw-r--   0 bart      (1000) bart      (1000)   194990 2021-11-26 13:17:04.000000 netqasm-0.9.0/docs/build/doctrees/api_sdk/netqasm.sdk.builder.doctree
--rw-rw-r--   0 bart      (1000) bart      (1000)   224332 2021-11-25 15:03:31.000000 netqasm-0.9.0/docs/build/doctrees/api_sdk/netqasm.sdk.classical_communication.doctree
--rw-rw-r--   0 bart      (1000) bart      (1000)    31842 2021-11-25 15:03:32.000000 netqasm-0.9.0/docs/build/doctrees/api_sdk/netqasm.sdk.compiling.doctree
--rw-rw-r--   0 bart      (1000) bart      (1000)    26587 2021-11-25 15:03:32.000000 netqasm-0.9.0/docs/build/doctrees/api_sdk/netqasm.sdk.config.doctree
--rw-rw-r--   0 bart      (1000) bart      (1000)   352590 2021-11-26 13:17:05.000000 netqasm-0.9.0/docs/build/doctrees/api_sdk/netqasm.sdk.connection.doctree
--rw-rw-r--   0 bart      (1000) bart      (1000)   106762 2021-11-26 13:17:05.000000 netqasm-0.9.0/docs/build/doctrees/api_sdk/netqasm.sdk.epr_socket.doctree
--rw-rw-r--   0 bart      (1000) bart      (1000)     5791 2021-11-26 13:17:05.000000 netqasm-0.9.0/docs/build/doctrees/api_sdk/netqasm.sdk.external.doctree
--rw-rw-r--   0 bart      (1000) bart      (1000)   232150 2021-11-26 13:17:06.000000 netqasm-0.9.0/docs/build/doctrees/api_sdk/netqasm.sdk.futures.doctree
--rw-rw-r--   0 bart      (1000) bart      (1000)    12254 2021-11-25 15:03:33.000000 netqasm-0.9.0/docs/build/doctrees/api_sdk/netqasm.sdk.network.doctree
--rw-rw-r--   0 bart      (1000) bart      (1000)    10804 2021-11-25 15:03:33.000000 netqasm-0.9.0/docs/build/doctrees/api_sdk/netqasm.sdk.progress_bar.doctree
--rw-rw-r--   0 bart      (1000) bart      (1000)   167266 2021-11-26 13:17:06.000000 netqasm-0.9.0/docs/build/doctrees/api_sdk/netqasm.sdk.qubit.doctree
--rw-rw-r--   0 bart      (1000) bart      (1000)    64515 2021-11-25 15:03:34.000000 netqasm-0.9.0/docs/build/doctrees/api_sdk/netqasm.sdk.shared_memory.doctree
--rw-rw-r--   0 bart      (1000) bart      (1000)    62171 2021-11-26 13:17:06.000000 netqasm-0.9.0/docs/build/doctrees/api_sdk/netqasm.sdk.toolbox.doctree
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:35.020210 netqasm-0.9.0/docs/build/doctrees/api_util/
--rw-rw-r--   0 bart      (1000) bart      (1000)    26943 2021-11-25 15:03:34.000000 netqasm-0.9.0/docs/build/doctrees/api_util/netqasm.util.error.doctree
--rw-rw-r--   0 bart      (1000) bart      (1000)    10895 2021-11-25 15:03:34.000000 netqasm-0.9.0/docs/build/doctrees/api_util/netqasm.util.log.doctree
--rw-rw-r--   0 bart      (1000) bart      (1000)    10783 2021-11-25 15:03:34.000000 netqasm-0.9.0/docs/build/doctrees/api_util/netqasm.util.quantum_gates.doctree
--rw-rw-r--   0 bart      (1000) bart      (1000)     6777 2021-11-25 15:03:34.000000 netqasm-0.9.0/docs/build/doctrees/api_util/netqasm.util.states.doctree
--rw-rw-r--   0 bart      (1000) bart      (1000)    12193 2021-11-25 15:03:34.000000 netqasm-0.9.0/docs/build/doctrees/api_util/netqasm.util.string.doctree
--rw-rw-r--   0 bart      (1000) bart      (1000)     4896 2021-11-25 15:03:34.000000 netqasm-0.9.0/docs/build/doctrees/api_util/netqasm.util.thread.doctree
--rw-rw-r--   0 bart      (1000) bart      (1000)     5239 2021-11-25 15:03:34.000000 netqasm-0.9.0/docs/build/doctrees/api_util/netqasm.util.yaml.doctree
--rw-rw-r--   0 bart      (1000) bart      (1000)   366848 2021-11-26 13:17:14.000000 netqasm-0.9.0/docs/build/doctrees/environment.pickle
--rw-rw-r--   0 bart      (1000) bart      (1000)     3929 2021-11-26 13:17:06.000000 netqasm-0.9.0/docs/build/doctrees/index.doctree
--rw-rw-r--   0 bart      (1000) bart      (1000)    11959 2021-11-26 13:17:06.000000 netqasm-0.9.0/docs/build/doctrees/installation.doctree
--rw-rw-r--   0 bart      (1000) bart      (1000)     3593 2021-11-26 13:17:06.000000 netqasm-0.9.0/docs/build/doctrees/known_issues.doctree
--rw-rw-r--   0 bart      (1000) bart      (1000)     2842 2021-11-25 15:03:34.000000 netqasm-0.9.0/docs/build/doctrees/netqasm.backend.doctree
--rw-rw-r--   0 bart      (1000) bart      (1000)     4180 2021-11-26 13:17:14.000000 netqasm-0.9.0/docs/build/doctrees/netqasm.examples.doctree
--rw-rw-r--   0 bart      (1000) bart      (1000)     2897 2021-11-25 15:03:34.000000 netqasm-0.9.0/docs/build/doctrees/netqasm.lang.doctree
--rw-rw-r--   0 bart      (1000) bart      (1000)     2744 2021-11-25 15:03:34.000000 netqasm-0.9.0/docs/build/doctrees/netqasm.logging.doctree
--rw-rw-r--   0 bart      (1000) bart      (1000)     3055 2021-11-25 15:03:34.000000 netqasm-0.9.0/docs/build/doctrees/netqasm.runtime.doctree
--rw-rw-r--   0 bart      (1000) bart      (1000)     3122 2021-11-25 15:03:34.000000 netqasm-0.9.0/docs/build/doctrees/netqasm.sdk.doctree
--rw-rw-r--   0 bart      (1000) bart      (1000)     2894 2021-11-25 15:03:34.000000 netqasm-0.9.0/docs/build/doctrees/netqasm.util.doctree
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:35.048210 netqasm-0.9.0/docs/build/doctrees/quickstart/
--rw-rw-r--   0 bart      (1000) bart      (1000)    37590 2021-11-26 13:17:06.000000 netqasm-0.9.0/docs/build/doctrees/quickstart/file_structure.doctree
--rw-rw-r--   0 bart      (1000) bart      (1000)    24910 2021-11-26 13:17:06.000000 netqasm-0.9.0/docs/build/doctrees/quickstart/first-app.doctree
--rw-rw-r--   0 bart      (1000) bart      (1000)   503162 2021-11-26 13:17:07.000000 netqasm-0.9.0/docs/build/doctrees/quickstart/modules.doctree
--rw-rw-r--   0 bart      (1000) bart      (1000)    71705 2021-11-26 13:17:07.000000 netqasm-0.9.0/docs/build/doctrees/quickstart/using-sdk.doctree
--rw-rw-r--   0 bart      (1000) bart      (1000)     5490 2021-11-26 13:17:06.000000 netqasm-0.9.0/docs/build/doctrees/quickstart.doctree
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:35.080211 netqasm-0.9.0/docs/build/html/
--rw-rw-r--   0 bart      (1000) bart      (1000)      230 2021-11-26 13:17:15.000000 netqasm-0.9.0/docs/build/html/.buildinfo
--rw-rw-r--   0 bart      (1000) bart      (1000)        0 2021-11-26 13:17:14.000000 netqasm-0.9.0/docs/build/html/.nojekyll
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:35.092211 netqasm-0.9.0/docs/build/html/_sources/
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:35.100211 netqasm-0.9.0/docs/build/html/_sources/api_backend/
--rw-rw-r--   0 bart      (1000) bart      (1000)      174 2021-11-09 12:09:06.000000 netqasm-0.9.0/docs/build/html/_sources/api_backend/netqasm.backend.executor.rst.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)      174 2021-11-09 12:09:06.000000 netqasm-0.9.0/docs/build/html/_sources/api_backend/netqasm.backend.messages.rst.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)      188 2021-11-09 12:09:06.000000 netqasm-0.9.0/docs/build/html/_sources/api_backend/netqasm.backend.network_stack.rst.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)      172 2021-11-09 12:09:06.000000 netqasm-0.9.0/docs/build/html/_sources/api_backend/netqasm.backend.qnodeos.rst.txt
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:35.112211 netqasm-0.9.0/docs/build/html/_sources/api_lang/
--rw-rw-r--   0 bart      (1000) bart      (1000)      168 2021-11-09 12:09:06.000000 netqasm-0.9.0/docs/build/html/_sources/api_lang/netqasm.lang.encoding.rst.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)      816 2021-11-09 12:09:06.000000 netqasm-0.9.0/docs/build/html/_sources/api_lang/netqasm.lang.instr.rst.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)      156 2021-11-09 12:09:06.000000 netqasm-0.9.0/docs/build/html/_sources/api_lang/netqasm.lang.ir.rst.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)      166 2021-11-09 12:09:06.000000 netqasm-0.9.0/docs/build/html/_sources/api_lang/netqasm.lang.operand.rst.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)      366 2021-11-09 12:09:06.000000 netqasm-0.9.0/docs/build/html/_sources/api_lang/netqasm.lang.parsing.rst.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)      172 2021-11-09 12:09:06.000000 netqasm-0.9.0/docs/build/html/_sources/api_lang/netqasm.lang.subroutine.rst.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)      166 2021-11-09 12:09:06.000000 netqasm-0.9.0/docs/build/html/_sources/api_lang/netqasm.lang.symbols.rst.txt
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:35.120211 netqasm-0.9.0/docs/build/html/_sources/api_logging/
--rw-rw-r--   0 bart      (1000) bart      (1000)      170 2021-11-09 12:09:06.000000 netqasm-0.9.0/docs/build/html/_sources/api_logging/netqasm.logging.glob.rst.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)      166 2021-11-09 12:09:06.000000 netqasm-0.9.0/docs/build/html/_sources/api_logging/netqasm.logging.output.rst.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)      176 2021-11-09 15:38:36.000000 netqasm-0.9.0/docs/build/html/_sources/api_root.rst.txt
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:35.136211 netqasm-0.9.0/docs/build/html/_sources/api_runtime/
--rw-rw-r--   0 bart      (1000) bart      (1000)      179 2021-11-09 15:39:26.000000 netqasm-0.9.0/docs/build/html/_sources/api_runtime/netqasm.runtime.app_config.rst.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)      182 2021-11-09 15:39:31.000000 netqasm-0.9.0/docs/build/html/_sources/api_runtime/netqasm.runtime.application.rst.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)      164 2021-11-09 12:09:06.000000 netqasm-0.9.0/docs/build/html/_sources/api_runtime/netqasm.runtime.cli.rst.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)      168 2021-11-09 12:09:06.000000 netqasm-0.9.0/docs/build/html/_sources/api_runtime/netqasm.runtime.debug.rst.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)      164 2021-11-09 12:09:06.000000 netqasm-0.9.0/docs/build/html/_sources/api_runtime/netqasm.runtime.env.rst.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)      174 2021-11-09 12:09:06.000000 netqasm-0.9.0/docs/build/html/_sources/api_runtime/netqasm.runtime.hardware.rst.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)      593 2021-11-09 15:41:50.000000 netqasm-0.9.0/docs/build/html/_sources/api_runtime/netqasm.runtime.interface.rst.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)      185 2021-11-09 15:39:35.000000 netqasm-0.9.0/docs/build/html/_sources/api_runtime/netqasm.runtime.process_logs.rst.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)      174 2021-11-09 12:09:06.000000 netqasm-0.9.0/docs/build/html/_sources/api_runtime/netqasm.runtime.settings.rst.txt
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:35.148212 netqasm-0.9.0/docs/build/html/_sources/api_sdk/
--rw-rw-r--   0 bart      (1000) bart      (1000)      164 2021-11-09 12:09:06.000000 netqasm-0.9.0/docs/build/html/_sources/api_sdk/netqasm.sdk.builder.rst.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)     1493 2021-11-09 15:40:16.000000 netqasm-0.9.0/docs/build/html/_sources/api_sdk/netqasm.sdk.classical_communication.rst.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)      168 2021-11-09 12:09:06.000000 netqasm-0.9.0/docs/build/html/_sources/api_sdk/netqasm.sdk.compiling.rst.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)      162 2021-11-09 12:09:06.000000 netqasm-0.9.0/docs/build/html/_sources/api_sdk/netqasm.sdk.config.rst.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)      170 2021-11-09 12:09:06.000000 netqasm-0.9.0/docs/build/html/_sources/api_sdk/netqasm.sdk.connection.rst.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)      170 2021-11-09 12:09:06.000000 netqasm-0.9.0/docs/build/html/_sources/api_sdk/netqasm.sdk.epr_socket.rst.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)      166 2021-11-09 12:09:06.000000 netqasm-0.9.0/docs/build/html/_sources/api_sdk/netqasm.sdk.external.rst.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)      164 2021-11-09 12:09:06.000000 netqasm-0.9.0/docs/build/html/_sources/api_sdk/netqasm.sdk.futures.rst.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)      164 2021-11-09 12:09:06.000000 netqasm-0.9.0/docs/build/html/_sources/api_sdk/netqasm.sdk.network.rst.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)      174 2021-11-09 12:09:06.000000 netqasm-0.9.0/docs/build/html/_sources/api_sdk/netqasm.sdk.progress_bar.rst.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)      160 2021-11-09 12:09:06.000000 netqasm-0.9.0/docs/build/html/_sources/api_sdk/netqasm.sdk.qubit.rst.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)      176 2021-11-09 12:09:06.000000 netqasm-0.9.0/docs/build/html/_sources/api_sdk/netqasm.sdk.shared_memory.rst.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)      994 2021-11-09 12:09:06.000000 netqasm-0.9.0/docs/build/html/_sources/api_sdk/netqasm.sdk.toolbox.rst.txt
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:35.156212 netqasm-0.9.0/docs/build/html/_sources/api_util/
--rw-rw-r--   0 bart      (1000) bart      (1000)      162 2021-11-09 12:09:06.000000 netqasm-0.9.0/docs/build/html/_sources/api_util/netqasm.util.error.rst.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)      158 2021-11-09 12:09:06.000000 netqasm-0.9.0/docs/build/html/_sources/api_util/netqasm.util.log.rst.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)      179 2021-11-09 12:09:06.000000 netqasm-0.9.0/docs/build/html/_sources/api_util/netqasm.util.quantum_gates.rst.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)      164 2021-11-09 12:09:06.000000 netqasm-0.9.0/docs/build/html/_sources/api_util/netqasm.util.states.rst.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)      164 2021-11-09 12:09:06.000000 netqasm-0.9.0/docs/build/html/_sources/api_util/netqasm.util.string.rst.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)      164 2021-11-09 12:09:06.000000 netqasm-0.9.0/docs/build/html/_sources/api_util/netqasm.util.thread.rst.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)      160 2021-11-09 12:09:06.000000 netqasm-0.9.0/docs/build/html/_sources/api_util/netqasm.util.yaml.rst.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)      606 2021-11-26 13:15:04.000000 netqasm-0.9.0/docs/build/html/_sources/index.rst.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)     1591 2021-11-25 15:27:32.000000 netqasm-0.9.0/docs/build/html/_sources/installation.rst.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)      356 2021-11-26 13:16:56.000000 netqasm-0.9.0/docs/build/html/_sources/known_issues.rst.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)      249 2021-11-09 12:09:06.000000 netqasm-0.9.0/docs/build/html/_sources/netqasm.backend.rst.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)      255 2021-11-09 12:09:06.000000 netqasm-0.9.0/docs/build/html/_sources/netqasm.examples.rst.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)      310 2021-11-09 12:09:06.000000 netqasm-0.9.0/docs/build/html/_sources/netqasm.lang.rst.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)      159 2021-11-09 12:09:06.000000 netqasm-0.9.0/docs/build/html/_sources/netqasm.logging.rst.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)      442 2021-11-09 12:09:06.000000 netqasm-0.9.0/docs/build/html/_sources/netqasm.runtime.rst.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)      517 2021-11-09 12:09:06.000000 netqasm-0.9.0/docs/build/html/_sources/netqasm.sdk.rst.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)      307 2021-11-09 12:09:06.000000 netqasm-0.9.0/docs/build/html/_sources/netqasm.util.rst.txt
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:35.160212 netqasm-0.9.0/docs/build/html/_sources/quickstart/
--rw-rw-r--   0 bart      (1000) bart      (1000)     6364 2021-11-26 13:12:18.000000 netqasm-0.9.0/docs/build/html/_sources/quickstart/file_structure.rst.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)     4854 2021-11-25 15:31:56.000000 netqasm-0.9.0/docs/build/html/_sources/quickstart/first-app.rst.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)     2996 2021-11-09 12:09:06.000000 netqasm-0.9.0/docs/build/html/_sources/quickstart/modules.rst.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)    19303 2021-11-26 13:15:49.000000 netqasm-0.9.0/docs/build/html/_sources/quickstart/using-sdk.rst.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)      677 2021-11-25 14:54:59.000000 netqasm-0.9.0/docs/build/html/_sources/quickstart.rst.txt
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:35.180212 netqasm-0.9.0/docs/build/html/_static/
--rw-rw-r--   0 bart      (1000) bart      (1000)    13877 2021-11-26 13:17:15.000000 netqasm-0.9.0/docs/build/html/_static/basic.css
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:35.180212 netqasm-0.9.0/docs/build/html/_static/css/
--rw-rw-r--   0 bart      (1000) bart      (1000)     3275 2021-04-07 12:13:34.000000 netqasm-0.9.0/docs/build/html/_static/css/badge_only.css
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:35.232213 netqasm-0.9.0/docs/build/html/_static/css/fonts/
--rw-rw-r--   0 bart      (1000) bart      (1000)    87624 2021-04-07 12:13:34.000000 netqasm-0.9.0/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff
--rw-rw-r--   0 bart      (1000) bart      (1000)    67312 2021-04-07 12:13:34.000000 netqasm-0.9.0/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
--rw-rw-r--   0 bart      (1000) bart      (1000)    86288 2021-04-07 12:13:34.000000 netqasm-0.9.0/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff
--rw-rw-r--   0 bart      (1000) bart      (1000)    66444 2021-04-07 12:13:34.000000 netqasm-0.9.0/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
--rw-rw-r--   0 bart      (1000) bart      (1000)   165742 2021-04-07 12:13:34.000000 netqasm-0.9.0/docs/build/html/_static/css/fonts/fontawesome-webfont.eot
--rw-rw-r--   0 bart      (1000) bart      (1000)   444379 2021-04-07 12:13:34.000000 netqasm-0.9.0/docs/build/html/_static/css/fonts/fontawesome-webfont.svg
--rw-rw-r--   0 bart      (1000) bart      (1000)   165548 2021-04-07 12:13:34.000000 netqasm-0.9.0/docs/build/html/_static/css/fonts/fontawesome-webfont.ttf
--rw-rw-r--   0 bart      (1000) bart      (1000)    98024 2021-04-07 12:13:34.000000 netqasm-0.9.0/docs/build/html/_static/css/fonts/fontawesome-webfont.woff
--rw-rw-r--   0 bart      (1000) bart      (1000)    77160 2021-04-07 12:13:34.000000 netqasm-0.9.0/docs/build/html/_static/css/fonts/fontawesome-webfont.woff2
--rw-rw-r--   0 bart      (1000) bart      (1000)   323344 2021-04-07 12:13:34.000000 netqasm-0.9.0/docs/build/html/_static/css/fonts/lato-bold-italic.woff
--rw-rw-r--   0 bart      (1000) bart      (1000)   193308 2021-04-07 12:13:34.000000 netqasm-0.9.0/docs/build/html/_static/css/fonts/lato-bold-italic.woff2
--rw-rw-r--   0 bart      (1000) bart      (1000)   309728 2021-04-07 12:13:34.000000 netqasm-0.9.0/docs/build/html/_static/css/fonts/lato-bold.woff
--rw-rw-r--   0 bart      (1000) bart      (1000)   184912 2021-04-07 12:13:34.000000 netqasm-0.9.0/docs/build/html/_static/css/fonts/lato-bold.woff2
--rw-rw-r--   0 bart      (1000) bart      (1000)   328412 2021-04-07 12:13:34.000000 netqasm-0.9.0/docs/build/html/_static/css/fonts/lato-normal-italic.woff
--rw-rw-r--   0 bart      (1000) bart      (1000)   195704 2021-04-07 12:13:34.000000 netqasm-0.9.0/docs/build/html/_static/css/fonts/lato-normal-italic.woff2
--rw-rw-r--   0 bart      (1000) bart      (1000)   309192 2021-04-07 12:13:34.000000 netqasm-0.9.0/docs/build/html/_static/css/fonts/lato-normal.woff
--rw-rw-r--   0 bart      (1000) bart      (1000)   182708 2021-04-07 12:13:34.000000 netqasm-0.9.0/docs/build/html/_static/css/fonts/lato-normal.woff2
--rw-rw-r--   0 bart      (1000) bart      (1000)   123687 2021-04-07 12:13:34.000000 netqasm-0.9.0/docs/build/html/_static/css/theme.css
--rw-rw-r--   0 bart      (1000) bart      (1000)     9592 2021-11-09 15:36:03.000000 netqasm-0.9.0/docs/build/html/_static/doctools.js
--rw-rw-r--   0 bart      (1000) bart      (1000)      355 2021-11-26 13:17:15.000000 netqasm-0.9.0/docs/build/html/_static/documentation_options.js
--rw-rw-r--   0 bart      (1000) bart      (1000)      286 2021-11-09 15:36:03.000000 netqasm-0.9.0/docs/build/html/_static/file.png
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:35.272213 netqasm-0.9.0/docs/build/html/_static/fonts/
--rw-rw-r--   0 bart      (1000) bart      (1000)   109948 2021-04-07 12:13:34.000000 netqasm-0.9.0/docs/build/html/_static/fonts/Inconsolata-Bold.ttf
--rw-rw-r--   0 bart      (1000) bart      (1000)    96964 2021-04-07 12:13:34.000000 netqasm-0.9.0/docs/build/html/_static/fonts/Inconsolata-Regular.ttf
--rw-rw-r--   0 bart      (1000) bart      (1000)    63184 2021-04-07 12:13:34.000000 netqasm-0.9.0/docs/build/html/_static/fonts/Inconsolata.ttf
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:35.376214 netqasm-0.9.0/docs/build/html/_static/fonts/Lato/
--rw-rw-r--   0 bart      (1000) bart      (1000)   256056 2021-04-07 12:13:34.000000 netqasm-0.9.0/docs/build/html/_static/fonts/Lato/lato-bold.eot
--rw-rw-r--   0 bart      (1000) bart      (1000)   600856 2021-04-07 12:13:34.000000 netqasm-0.9.0/docs/build/html/_static/fonts/Lato/lato-bold.ttf
--rw-rw-r--   0 bart      (1000) bart      (1000)   309728 2021-04-07 12:13:34.000000 netqasm-0.9.0/docs/build/html/_static/fonts/Lato/lato-bold.woff
--rw-rw-r--   0 bart      (1000) bart      (1000)   184912 2021-04-07 12:13:34.000000 netqasm-0.9.0/docs/build/html/_static/fonts/Lato/lato-bold.woff2
--rw-rw-r--   0 bart      (1000) bart      (1000)   266158 2021-04-07 12:13:34.000000 netqasm-0.9.0/docs/build/html/_static/fonts/Lato/lato-bolditalic.eot
--rw-rw-r--   0 bart      (1000) bart      (1000)   622572 2021-04-07 12:13:34.000000 netqasm-0.9.0/docs/build/html/_static/fonts/Lato/lato-bolditalic.ttf
--rw-rw-r--   0 bart      (1000) bart      (1000)   323344 2021-04-07 12:13:34.000000 netqasm-0.9.0/docs/build/html/_static/fonts/Lato/lato-bolditalic.woff
--rw-rw-r--   0 bart      (1000) bart      (1000)   193308 2021-04-07 12:13:34.000000 netqasm-0.9.0/docs/build/html/_static/fonts/Lato/lato-bolditalic.woff2
--rw-rw-r--   0 bart      (1000) bart      (1000)   268604 2021-04-07 12:13:34.000000 netqasm-0.9.0/docs/build/html/_static/fonts/Lato/lato-italic.eot
--rw-rw-r--   0 bart      (1000) bart      (1000)   639388 2021-04-07 12:13:34.000000 netqasm-0.9.0/docs/build/html/_static/fonts/Lato/lato-italic.ttf
--rw-rw-r--   0 bart      (1000) bart      (1000)   328412 2021-04-07 12:13:34.000000 netqasm-0.9.0/docs/build/html/_static/fonts/Lato/lato-italic.woff
--rw-rw-r--   0 bart      (1000) bart      (1000)   195704 2021-04-07 12:13:34.000000 netqasm-0.9.0/docs/build/html/_static/fonts/Lato/lato-italic.woff2
--rw-rw-r--   0 bart      (1000) bart      (1000)   253461 2021-04-07 12:13:34.000000 netqasm-0.9.0/docs/build/html/_static/fonts/Lato/lato-regular.eot
--rw-rw-r--   0 bart      (1000) bart      (1000)   607720 2021-04-07 12:13:34.000000 netqasm-0.9.0/docs/build/html/_static/fonts/Lato/lato-regular.ttf
--rw-rw-r--   0 bart      (1000) bart      (1000)   309192 2021-04-07 12:13:34.000000 netqasm-0.9.0/docs/build/html/_static/fonts/Lato/lato-regular.woff
--rw-rw-r--   0 bart      (1000) bart      (1000)   182708 2021-04-07 12:13:34.000000 netqasm-0.9.0/docs/build/html/_static/fonts/Lato/lato-regular.woff2
--rw-rw-r--   0 bart      (1000) bart      (1000)   656544 2021-04-07 12:13:34.000000 netqasm-0.9.0/docs/build/html/_static/fonts/Lato-Bold.ttf
--rw-rw-r--   0 bart      (1000) bart      (1000)   656568 2021-04-07 12:13:34.000000 netqasm-0.9.0/docs/build/html/_static/fonts/Lato-Regular.ttf
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:35.400215 netqasm-0.9.0/docs/build/html/_static/fonts/RobotoSlab/
--rw-rw-r--   0 bart      (1000) bart      (1000)    79520 2021-04-07 12:13:34.000000 netqasm-0.9.0/docs/build/html/_static/fonts/RobotoSlab/roboto-slab-v7-bold.eot
--rw-rw-r--   0 bart      (1000) bart      (1000)   170616 2021-04-07 12:13:34.000000 netqasm-0.9.0/docs/build/html/_static/fonts/RobotoSlab/roboto-slab-v7-bold.ttf
--rw-rw-r--   0 bart      (1000) bart      (1000)    87624 2021-04-07 12:13:34.000000 netqasm-0.9.0/docs/build/html/_static/fonts/RobotoSlab/roboto-slab-v7-bold.woff
--rw-rw-r--   0 bart      (1000) bart      (1000)    67312 2021-04-07 12:13:34.000000 netqasm-0.9.0/docs/build/html/_static/fonts/RobotoSlab/roboto-slab-v7-bold.woff2
--rw-rw-r--   0 bart      (1000) bart      (1000)    78331 2021-04-07 12:13:34.000000 netqasm-0.9.0/docs/build/html/_static/fonts/RobotoSlab/roboto-slab-v7-regular.eot
--rw-rw-r--   0 bart      (1000) bart      (1000)   169064 2021-04-07 12:13:34.000000 netqasm-0.9.0/docs/build/html/_static/fonts/RobotoSlab/roboto-slab-v7-regular.ttf
--rw-rw-r--   0 bart      (1000) bart      (1000)    86288 2021-04-07 12:13:34.000000 netqasm-0.9.0/docs/build/html/_static/fonts/RobotoSlab/roboto-slab-v7-regular.woff
--rw-rw-r--   0 bart      (1000) bart      (1000)    66444 2021-04-07 12:13:34.000000 netqasm-0.9.0/docs/build/html/_static/fonts/RobotoSlab/roboto-slab-v7-regular.woff2
--rw-rw-r--   0 bart      (1000) bart      (1000)   170616 2021-04-07 12:13:34.000000 netqasm-0.9.0/docs/build/html/_static/fonts/RobotoSlab-Bold.ttf
--rw-rw-r--   0 bart      (1000) bart      (1000)   169064 2021-04-07 12:13:34.000000 netqasm-0.9.0/docs/build/html/_static/fonts/RobotoSlab-Regular.ttf
--rw-rw-r--   0 bart      (1000) bart      (1000)   165742 2021-04-07 12:13:34.000000 netqasm-0.9.0/docs/build/html/_static/fonts/fontawesome-webfont.eot
--rw-rw-r--   0 bart      (1000) bart      (1000)   444379 2021-04-07 12:13:34.000000 netqasm-0.9.0/docs/build/html/_static/fonts/fontawesome-webfont.svg
--rw-rw-r--   0 bart      (1000) bart      (1000)   165548 2021-04-07 12:13:34.000000 netqasm-0.9.0/docs/build/html/_static/fonts/fontawesome-webfont.ttf
--rw-rw-r--   0 bart      (1000) bart      (1000)    98024 2021-04-07 12:13:34.000000 netqasm-0.9.0/docs/build/html/_static/fonts/fontawesome-webfont.woff
--rw-rw-r--   0 bart      (1000) bart      (1000)    77160 2021-04-07 12:13:34.000000 netqasm-0.9.0/docs/build/html/_static/fonts/fontawesome-webfont.woff2
--rw-rw-r--   0 bart      (1000) bart      (1000)   287630 2021-11-09 15:36:03.000000 netqasm-0.9.0/docs/build/html/_static/jquery-3.5.1.js
--rw-rw-r--   0 bart      (1000) bart      (1000)    89476 2021-11-09 15:36:03.000000 netqasm-0.9.0/docs/build/html/_static/jquery.js
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:35.408215 netqasm-0.9.0/docs/build/html/_static/js/
--rw-rw-r--   0 bart      (1000) bart      (1000)      934 2021-04-07 12:13:34.000000 netqasm-0.9.0/docs/build/html/_static/js/badge_only.js
--rw-rw-r--   0 bart      (1000) bart      (1000)     4370 2021-04-07 12:13:34.000000 netqasm-0.9.0/docs/build/html/_static/js/html5shiv-printshiv.min.js
--rw-rw-r--   0 bart      (1000) bart      (1000)     2734 2021-04-07 12:13:34.000000 netqasm-0.9.0/docs/build/html/_static/js/html5shiv.min.js
--rw-rw-r--   0 bart      (1000) bart      (1000)    15414 2021-04-07 12:13:34.000000 netqasm-0.9.0/docs/build/html/_static/js/modernizr.min.js
--rw-rw-r--   0 bart      (1000) bart      (1000)     4916 2021-04-07 12:13:34.000000 netqasm-0.9.0/docs/build/html/_static/js/theme.js
--rw-rw-r--   0 bart      (1000) bart      (1000)    10854 2021-11-26 13:17:15.000000 netqasm-0.9.0/docs/build/html/_static/language_data.js
--rw-rw-r--   0 bart      (1000) bart      (1000)       90 2021-11-09 15:36:03.000000 netqasm-0.9.0/docs/build/html/_static/minus.png
--rw-rw-r--   0 bart      (1000) bart      (1000)       90 2021-11-09 15:36:03.000000 netqasm-0.9.0/docs/build/html/_static/plus.png
--rw-rw-r--   0 bart      (1000) bart      (1000)     4368 2021-11-26 13:17:15.000000 netqasm-0.9.0/docs/build/html/_static/pygments.css
--rw-rw-r--   0 bart      (1000) bart      (1000)    16582 2021-11-09 15:36:03.000000 netqasm-0.9.0/docs/build/html/_static/searchtools.js
--rw-rw-r--   0 bart      (1000) bart      (1000)    67692 2021-11-09 15:36:03.000000 netqasm-0.9.0/docs/build/html/_static/underscore-1.12.0.js
--rw-rw-r--   0 bart      (1000) bart      (1000)    19358 2021-11-09 15:36:03.000000 netqasm-0.9.0/docs/build/html/_static/underscore.js
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:35.424215 netqasm-0.9.0/docs/build/html/api_backend/
--rw-rw-r--   0 bart      (1000) bart      (1000)    30383 2021-11-25 15:03:36.000000 netqasm-0.9.0/docs/build/html/api_backend/netqasm.backend.executor.html
--rw-rw-r--   0 bart      (1000) bart      (1000)    54015 2021-11-25 15:03:36.000000 netqasm-0.9.0/docs/build/html/api_backend/netqasm.backend.messages.html
--rw-rw-r--   0 bart      (1000) bart      (1000)    14197 2021-11-25 15:03:36.000000 netqasm-0.9.0/docs/build/html/api_backend/netqasm.backend.network_stack.html
--rw-rw-r--   0 bart      (1000) bart      (1000)    16641 2021-11-25 15:03:36.000000 netqasm-0.9.0/docs/build/html/api_backend/netqasm.backend.qnodeos.html
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:35.436215 netqasm-0.9.0/docs/build/html/api_lang/
--rw-rw-r--   0 bart      (1000) bart      (1000)    68663 2021-11-25 15:03:36.000000 netqasm-0.9.0/docs/build/html/api_lang/netqasm.lang.encoding.html
--rw-rw-r--   0 bart      (1000) bart      (1000)   465784 2021-11-25 15:03:37.000000 netqasm-0.9.0/docs/build/html/api_lang/netqasm.lang.instr.html
--rw-rw-r--   0 bart      (1000) bart      (1000)    40953 2021-11-25 15:03:37.000000 netqasm-0.9.0/docs/build/html/api_lang/netqasm.lang.ir.html
--rw-rw-r--   0 bart      (1000) bart      (1000)    26633 2021-11-25 15:03:37.000000 netqasm-0.9.0/docs/build/html/api_lang/netqasm.lang.operand.html
--rw-rw-r--   0 bart      (1000) bart      (1000)    25406 2021-11-25 15:03:37.000000 netqasm-0.9.0/docs/build/html/api_lang/netqasm.lang.parsing.html
--rw-rw-r--   0 bart      (1000) bart      (1000)    12733 2021-11-25 15:03:37.000000 netqasm-0.9.0/docs/build/html/api_lang/netqasm.lang.subroutine.html
--rw-rw-r--   0 bart      (1000) bart      (1000)    13385 2021-11-25 15:03:37.000000 netqasm-0.9.0/docs/build/html/api_lang/netqasm.lang.symbols.html
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:35.436215 netqasm-0.9.0/docs/build/html/api_logging/
--rw-rw-r--   0 bart      (1000) bart      (1000)    19497 2021-11-25 15:03:37.000000 netqasm-0.9.0/docs/build/html/api_logging/netqasm.logging.glob.html
--rw-rw-r--   0 bart      (1000) bart      (1000)     9623 2021-11-25 15:03:37.000000 netqasm-0.9.0/docs/build/html/api_logging/netqasm.logging.output.html
--rw-rw-r--   0 bart      (1000) bart      (1000)    15793 2021-11-25 15:03:37.000000 netqasm-0.9.0/docs/build/html/api_root.html
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:35.456215 netqasm-0.9.0/docs/build/html/api_runtime/
--rw-rw-r--   0 bart      (1000) bart      (1000)    13847 2021-11-25 15:03:37.000000 netqasm-0.9.0/docs/build/html/api_runtime/netqasm.runtime.app_config.html
--rw-rw-r--   0 bart      (1000) bart      (1000)    34669 2021-11-25 15:03:37.000000 netqasm-0.9.0/docs/build/html/api_runtime/netqasm.runtime.application.html
--rw-rw-r--   0 bart      (1000) bart      (1000)     7965 2021-11-25 15:03:37.000000 netqasm-0.9.0/docs/build/html/api_runtime/netqasm.runtime.cli.html
--rw-rw-r--   0 bart      (1000) bart      (1000)    10206 2021-11-25 15:03:38.000000 netqasm-0.9.0/docs/build/html/api_runtime/netqasm.runtime.debug.html
--rw-rw-r--   0 bart      (1000) bart      (1000)    16787 2021-11-25 15:03:38.000000 netqasm-0.9.0/docs/build/html/api_runtime/netqasm.runtime.env.html
--rw-rw-r--   0 bart      (1000) bart      (1000)    10348 2021-11-25 15:03:38.000000 netqasm-0.9.0/docs/build/html/api_runtime/netqasm.runtime.hardware.html
--rw-rw-r--   0 bart      (1000) bart      (1000)    74476 2021-11-25 15:03:38.000000 netqasm-0.9.0/docs/build/html/api_runtime/netqasm.runtime.interface.html
--rw-rw-r--   0 bart      (1000) bart      (1000)     9048 2021-11-26 13:17:07.000000 netqasm-0.9.0/docs/build/html/api_runtime/netqasm.runtime.process_logs.html
--rw-rw-r--   0 bart      (1000) bart      (1000)    15215 2021-11-25 15:03:38.000000 netqasm-0.9.0/docs/build/html/api_runtime/netqasm.runtime.settings.html
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:35.472216 netqasm-0.9.0/docs/build/html/api_sdk/
--rw-rw-r--   0 bart      (1000) bart      (1000)    71598 2021-11-26 13:17:07.000000 netqasm-0.9.0/docs/build/html/api_sdk/netqasm.sdk.builder.html
--rw-rw-r--   0 bart      (1000) bart      (1000)    78245 2021-11-25 15:03:38.000000 netqasm-0.9.0/docs/build/html/api_sdk/netqasm.sdk.classical_communication.html
--rw-rw-r--   0 bart      (1000) bart      (1000)    21092 2021-11-25 15:03:38.000000 netqasm-0.9.0/docs/build/html/api_sdk/netqasm.sdk.compiling.html
--rw-rw-r--   0 bart      (1000) bart      (1000)    17467 2021-11-25 15:03:38.000000 netqasm-0.9.0/docs/build/html/api_sdk/netqasm.sdk.config.html
--rw-rw-r--   0 bart      (1000) bart      (1000)   117484 2021-11-26 13:17:08.000000 netqasm-0.9.0/docs/build/html/api_sdk/netqasm.sdk.connection.html
--rw-rw-r--   0 bart      (1000) bart      (1000)    44288 2021-11-26 13:17:08.000000 netqasm-0.9.0/docs/build/html/api_sdk/netqasm.sdk.epr_socket.html
--rw-rw-r--   0 bart      (1000) bart      (1000)    10889 2021-11-26 13:17:08.000000 netqasm-0.9.0/docs/build/html/api_sdk/netqasm.sdk.external.html
--rw-rw-r--   0 bart      (1000) bart      (1000)    87852 2021-11-26 13:17:08.000000 netqasm-0.9.0/docs/build/html/api_sdk/netqasm.sdk.futures.html
--rw-rw-r--   0 bart      (1000) bart      (1000)    12813 2021-11-25 15:03:39.000000 netqasm-0.9.0/docs/build/html/api_sdk/netqasm.sdk.network.html
--rw-rw-r--   0 bart      (1000) bart      (1000)    12378 2021-11-25 15:03:39.000000 netqasm-0.9.0/docs/build/html/api_sdk/netqasm.sdk.progress_bar.html
--rw-rw-r--   0 bart      (1000) bart      (1000)    60622 2021-11-26 13:17:08.000000 netqasm-0.9.0/docs/build/html/api_sdk/netqasm.sdk.qubit.html
--rw-rw-r--   0 bart      (1000) bart      (1000)    29496 2021-11-25 15:03:39.000000 netqasm-0.9.0/docs/build/html/api_sdk/netqasm.sdk.shared_memory.html
--rw-rw-r--   0 bart      (1000) bart      (1000)    28186 2021-11-26 13:17:08.000000 netqasm-0.9.0/docs/build/html/api_sdk/netqasm.sdk.toolbox.html
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:35.480216 netqasm-0.9.0/docs/build/html/api_util/
--rw-rw-r--   0 bart      (1000) bart      (1000)    15286 2021-11-25 15:03:39.000000 netqasm-0.9.0/docs/build/html/api_util/netqasm.util.error.html
--rw-rw-r--   0 bart      (1000) bart      (1000)     9833 2021-11-25 15:03:39.000000 netqasm-0.9.0/docs/build/html/api_util/netqasm.util.log.html
--rw-rw-r--   0 bart      (1000) bart      (1000)     9918 2021-11-25 15:03:39.000000 netqasm-0.9.0/docs/build/html/api_util/netqasm.util.quantum_gates.html
--rw-rw-r--   0 bart      (1000) bart      (1000)     7859 2021-11-25 15:03:39.000000 netqasm-0.9.0/docs/build/html/api_util/netqasm.util.states.html
--rw-rw-r--   0 bart      (1000) bart      (1000)    10553 2021-11-25 15:03:39.000000 netqasm-0.9.0/docs/build/html/api_util/netqasm.util.string.html
--rw-rw-r--   0 bart      (1000) bart      (1000)     7744 2021-11-25 15:03:39.000000 netqasm-0.9.0/docs/build/html/api_util/netqasm.util.thread.html
--rw-rw-r--   0 bart      (1000) bart      (1000)     7622 2021-11-25 15:03:40.000000 netqasm-0.9.0/docs/build/html/api_util/netqasm.util.yaml.html
--rw-rw-r--   0 bart      (1000) bart      (1000)   256777 2021-11-26 13:17:15.000000 netqasm-0.9.0/docs/build/html/genindex.html
--rw-rw-r--   0 bart      (1000) bart      (1000)     7038 2021-11-26 13:17:15.000000 netqasm-0.9.0/docs/build/html/index.html
--rw-rw-r--   0 bart      (1000) bart      (1000)     8450 2021-11-26 13:17:08.000000 netqasm-0.9.0/docs/build/html/installation.html
--rw-rw-r--   0 bart      (1000) bart      (1000)     5527 2021-11-26 13:17:08.000000 netqasm-0.9.0/docs/build/html/known_issues.html
--rw-rw-r--   0 bart      (1000) bart      (1000)     7025 2021-11-25 15:03:40.000000 netqasm-0.9.0/docs/build/html/netqasm.backend.html
--rw-rw-r--   0 bart      (1000) bart      (1000)     4582 2021-11-26 13:17:15.000000 netqasm-0.9.0/docs/build/html/netqasm.examples.html
--rw-rw-r--   0 bart      (1000) bart      (1000)     9942 2021-11-25 15:03:40.000000 netqasm-0.9.0/docs/build/html/netqasm.lang.html
--rw-rw-r--   0 bart      (1000) bart      (1000)     6481 2021-11-25 15:03:40.000000 netqasm-0.9.0/docs/build/html/netqasm.logging.html
--rw-rw-r--   0 bart      (1000) bart      (1000)     9726 2021-11-26 13:17:08.000000 netqasm-0.9.0/docs/build/html/netqasm.runtime.html
--rw-rw-r--   0 bart      (1000) bart      (1000)    13938 2021-11-26 13:17:08.000000 netqasm-0.9.0/docs/build/html/netqasm.sdk.html
--rw-rw-r--   0 bart      (1000) bart      (1000)     7648 2021-11-25 15:03:40.000000 netqasm-0.9.0/docs/build/html/netqasm.util.html
--rw-rw-r--   0 bart      (1000) bart      (1000)     9657 2021-11-26 13:17:15.000000 netqasm-0.9.0/docs/build/html/objects.inv
--rw-rw-r--   0 bart      (1000) bart      (1000)    19451 2021-11-26 13:17:15.000000 netqasm-0.9.0/docs/build/html/py-modindex.html
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:35.480216 netqasm-0.9.0/docs/build/html/quickstart/
--rw-rw-r--   0 bart      (1000) bart      (1000)    20367 2021-11-26 13:17:09.000000 netqasm-0.9.0/docs/build/html/quickstart/file_structure.html
--rw-rw-r--   0 bart      (1000) bart      (1000)    15255 2021-11-26 13:17:09.000000 netqasm-0.9.0/docs/build/html/quickstart/first-app.html
--rw-rw-r--   0 bart      (1000) bart      (1000)   158293 2021-11-26 13:17:09.000000 netqasm-0.9.0/docs/build/html/quickstart/modules.html
--rw-rw-r--   0 bart      (1000) bart      (1000)    67594 2021-11-26 13:17:09.000000 netqasm-0.9.0/docs/build/html/quickstart/using-sdk.html
--rw-rw-r--   0 bart      (1000) bart      (1000)     9774 2021-11-26 13:17:08.000000 netqasm-0.9.0/docs/build/html/quickstart.html
--rw-rw-r--   0 bart      (1000) bart      (1000)     4770 2021-11-26 13:17:15.000000 netqasm-0.9.0/docs/build/html/search.html
--rw-rw-r--   0 bart      (1000) bart      (1000)    79169 2021-11-26 13:17:15.000000 netqasm-0.9.0/docs/build/html/searchindex.js
--rw-rw-r--   0 bart      (1000) bart      (1000)     2873 2022-02-28 14:01:35.000000 netqasm-0.9.0/docs/conf.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      606 2022-02-28 13:02:08.000000 netqasm-0.9.0/docs/index.rst
--rw-rw-r--   0 bart      (1000) bart      (1000)     1591 2022-02-28 13:02:08.000000 netqasm-0.9.0/docs/installation.rst
--rw-rw-r--   0 bart      (1000) bart      (1000)      356 2022-02-28 13:02:08.000000 netqasm-0.9.0/docs/known_issues.rst
--rw-rw-r--   0 bart      (1000) bart      (1000)      760 2020-05-04 09:19:07.000000 netqasm-0.9.0/docs/make.bat
--rw-rw-r--   0 bart      (1000) bart      (1000)      249 2022-01-17 15:35:34.000000 netqasm-0.9.0/docs/netqasm.backend.rst
--rw-rw-r--   0 bart      (1000) bart      (1000)      255 2022-01-17 15:35:34.000000 netqasm-0.9.0/docs/netqasm.examples.rst
--rw-rw-r--   0 bart      (1000) bart      (1000)      310 2022-01-17 15:35:34.000000 netqasm-0.9.0/docs/netqasm.lang.rst
--rw-rw-r--   0 bart      (1000) bart      (1000)      159 2022-01-17 15:35:34.000000 netqasm-0.9.0/docs/netqasm.logging.rst
--rw-rw-r--   0 bart      (1000) bart      (1000)      442 2022-01-17 15:35:34.000000 netqasm-0.9.0/docs/netqasm.runtime.rst
--rw-rw-r--   0 bart      (1000) bart      (1000)      517 2022-01-17 15:35:34.000000 netqasm-0.9.0/docs/netqasm.sdk.rst
--rw-rw-r--   0 bart      (1000) bart      (1000)      307 2022-01-17 15:35:34.000000 netqasm-0.9.0/docs/netqasm.util.rst
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:35.484216 netqasm-0.9.0/docs/quickstart/
--rw-rw-r--   0 bart      (1000) bart      (1000)     6364 2022-02-28 13:02:08.000000 netqasm-0.9.0/docs/quickstart/file_structure.rst
--rw-rw-r--   0 bart      (1000) bart      (1000)     4854 2022-02-28 13:02:08.000000 netqasm-0.9.0/docs/quickstart/first-app.rst
--rw-rw-r--   0 bart      (1000) bart      (1000)     2996 2022-01-17 15:35:34.000000 netqasm-0.9.0/docs/quickstart/modules.rst
--rw-rw-r--   0 bart      (1000) bart      (1000)    19303 2022-02-28 13:02:08.000000 netqasm-0.9.0/docs/quickstart/using-sdk.rst
--rw-rw-r--   0 bart      (1000) bart      (1000)      677 2022-02-28 13:02:08.000000 netqasm-0.9.0/docs/quickstart.rst
--rw-rw-r--   0 bart      (1000) bart      (1000)       92 2022-01-17 15:35:34.000000 netqasm-0.9.0/docs/requirements.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)       87 2021-05-19 15:28:08.000000 netqasm-0.9.0/mypy.ini
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:35.492216 netqasm-0.9.0/netqasm/
--rw-rw-r--   0 bart      (1000) bart      (1000)       99 2022-02-28 14:01:35.000000 netqasm-0.9.0/netqasm/__init__.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:35.496216 netqasm-0.9.0/netqasm/backend/
--rw-rw-r--   0 bart      (1000) bart      (1000)        0 2021-05-19 15:28:08.000000 netqasm-0.9.0/netqasm/backend/__init__.py
--rw-rw-r--   0 bart      (1000) bart      (1000)    66890 2022-02-28 13:02:08.000000 netqasm-0.9.0/netqasm/backend/executor.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     9606 2022-01-17 15:35:34.000000 netqasm-0.9.0/netqasm/backend/messages.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     1561 2022-01-17 15:35:34.000000 netqasm-0.9.0/netqasm/backend/network_stack.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     6404 2022-01-17 15:40:12.000000 netqasm-0.9.0/netqasm/backend/qnodeos.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:35.496216 netqasm-0.9.0/netqasm/examples/
--rw-rw-r--   0 bart      (1000) bart      (1000)        0 2021-05-19 15:28:08.000000 netqasm-0.9.0/netqasm/examples/__init__.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:35.496216 netqasm-0.9.0/netqasm/examples/apps/
--rw-rw-r--   0 bart      (1000) bart      (1000)        0 2021-05-19 15:28:08.000000 netqasm-0.9.0/netqasm/examples/apps/__init__.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:35.512216 netqasm-0.9.0/netqasm/examples/apps/anonymous_transmission/
--rw-rw-r--   0 bart      (1000) bart      (1000)      508 2021-05-19 15:28:08.000000 netqasm-0.9.0/netqasm/examples/apps/anonymous_transmission/README.md
--rw-rw-r--   0 bart      (1000) bart      (1000)        0 2021-05-19 15:28:08.000000 netqasm-0.9.0/netqasm/examples/apps/anonymous_transmission/__init__.py
--rw-rw-r--   0 bart      (1000) bart      (1000)       49 2021-05-19 15:28:08.000000 netqasm-0.9.0/netqasm/examples/apps/anonymous_transmission/alice.yaml
--rw-rw-r--   0 bart      (1000) bart      (1000)      377 2022-01-17 15:35:34.000000 netqasm-0.9.0/netqasm/examples/apps/anonymous_transmission/app_alice.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      375 2022-01-17 15:35:34.000000 netqasm-0.9.0/netqasm/examples/apps/anonymous_transmission/app_bob.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      379 2022-01-17 15:35:34.000000 netqasm-0.9.0/netqasm/examples/apps/anonymous_transmission/app_charlie.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      377 2022-01-17 15:35:34.000000 netqasm-0.9.0/netqasm/examples/apps/anonymous_transmission/app_david.py
--rw-rw-r--   0 bart      (1000) bart      (1000)        0 2021-05-19 15:28:08.000000 netqasm-0.9.0/netqasm/examples/apps/anonymous_transmission/bob.yaml
--rw-rw-r--   0 bart      (1000) bart      (1000)        0 2021-05-19 15:28:08.000000 netqasm-0.9.0/netqasm/examples/apps/anonymous_transmission/charlie.yaml
--rw-rw-r--   0 bart      (1000) bart      (1000)       29 2021-05-19 15:28:08.000000 netqasm-0.9.0/netqasm/examples/apps/anonymous_transmission/david.yaml
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:35.512216 netqasm-0.9.0/netqasm/examples/apps/anonymous_transmission/src/
--rw-rw-r--   0 bart      (1000) bart      (1000)        0 2021-05-19 15:28:08.000000 netqasm-0.9.0/netqasm/examples/apps/anonymous_transmission/src/__init__.py
--rw-rw-r--   0 bart      (1000) bart      (1000)       44 2022-01-17 15:35:34.000000 netqasm-0.9.0/netqasm/examples/apps/anonymous_transmission/src/conf.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     1480 2022-01-17 15:40:12.000000 netqasm-0.9.0/netqasm/examples/apps/anonymous_transmission/src/protocol.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     5655 2022-01-17 15:35:34.000000 netqasm-0.9.0/netqasm/examples/apps/anonymous_transmission/src/sub_protocols.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:35.516216 netqasm-0.9.0/netqasm/examples/apps/bb84/
--rw-rw-r--   0 bart      (1000) bart      (1000)      571 2022-01-17 15:40:37.000000 netqasm-0.9.0/netqasm/examples/apps/bb84/README.md
--rw-rw-r--   0 bart      (1000) bart      (1000)        0 2022-01-17 15:40:37.000000 netqasm-0.9.0/netqasm/examples/apps/bb84/__init__.py
--rw-rw-r--   0 bart      (1000) bart      (1000)       12 2022-01-17 15:40:37.000000 netqasm-0.9.0/netqasm/examples/apps/bb84/alice.yaml
--rw-rw-r--   0 bart      (1000) bart      (1000)     7669 2022-02-28 14:01:35.000000 netqasm-0.9.0/netqasm/examples/apps/bb84/app_alice.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     7240 2022-02-28 14:01:35.000000 netqasm-0.9.0/netqasm/examples/apps/bb84/app_bob.py
--rw-rw-r--   0 bart      (1000) bart      (1000)       12 2022-01-17 15:40:37.000000 netqasm-0.9.0/netqasm/examples/apps/bb84/bob.yaml
--rw-rw-r--   0 bart      (1000) bart      (1000)      250 2022-01-17 15:40:37.000000 netqasm-0.9.0/netqasm/examples/apps/bb84/network.yaml
--rw-rw-r--   0 bart      (1000) bart      (1000)     4382 2022-01-17 15:40:37.000000 netqasm-0.9.0/netqasm/examples/apps/bb84/results_config.json
--rw-rw-r--   0 bart      (1000) bart      (1000)       22 2022-01-17 15:40:37.000000 netqasm-0.9.0/netqasm/examples/apps/bb84/roles.yaml
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:35.520216 netqasm-0.9.0/netqasm/examples/apps/blind_grover/
--rw-rw-r--   0 bart      (1000) bart      (1000)     3353 2021-05-19 15:28:08.000000 netqasm-0.9.0/netqasm/examples/apps/blind_grover/README.md
--rw-rw-r--   0 bart      (1000) bart      (1000)        0 2021-05-19 15:28:08.000000 netqasm-0.9.0/netqasm/examples/apps/blind_grover/__init__.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     3204 2022-01-17 15:40:12.000000 netqasm-0.9.0/netqasm/examples/apps/blind_grover/app_client.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     1824 2022-01-17 15:40:12.000000 netqasm-0.9.0/netqasm/examples/apps/blind_grover/app_server.py
--rw-rw-r--   0 bart      (1000) bart      (1000)       47 2021-05-19 15:28:08.000000 netqasm-0.9.0/netqasm/examples/apps/blind_grover/client.yaml
--rw-rw-r--   0 bart      (1000) bart      (1000)        0 2021-05-19 15:28:08.000000 netqasm-0.9.0/netqasm/examples/apps/blind_grover/server.yaml
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:35.524216 netqasm-0.9.0/netqasm/examples/apps/blind_rotation/
--rw-rw-r--   0 bart      (1000) bart      (1000)     2344 2021-05-19 15:28:08.000000 netqasm-0.9.0/netqasm/examples/apps/blind_rotation/README.md
--rw-rw-r--   0 bart      (1000) bart      (1000)        0 2021-05-19 15:28:08.000000 netqasm-0.9.0/netqasm/examples/apps/blind_rotation/__init__.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     2761 2022-01-17 15:40:12.000000 netqasm-0.9.0/netqasm/examples/apps/blind_rotation/app_client.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     1551 2022-01-17 15:40:12.000000 netqasm-0.9.0/netqasm/examples/apps/blind_rotation/app_server.py
--rw-rw-r--   0 bart      (1000) bart      (1000)       67 2021-05-19 15:28:08.000000 netqasm-0.9.0/netqasm/examples/apps/blind_rotation/client.yaml
--rw-rw-r--   0 bart      (1000) bart      (1000)       11 2021-05-19 15:28:08.000000 netqasm-0.9.0/netqasm/examples/apps/blind_rotation/server.yaml
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:35.532216 netqasm-0.9.0/netqasm/examples/apps/chsh/
--rw-rw-r--   0 bart      (1000) bart      (1000)     1168 2021-05-19 15:28:08.000000 netqasm-0.9.0/netqasm/examples/apps/chsh/README.md
--rw-rw-r--   0 bart      (1000) bart      (1000)        0 2021-05-19 15:28:08.000000 netqasm-0.9.0/netqasm/examples/apps/chsh/__init__.py
--rw-rw-r--   0 bart      (1000) bart      (1000)        4 2021-05-19 15:28:08.000000 netqasm-0.9.0/netqasm/examples/apps/chsh/alice.yaml
--rwxrwxr-x   0 bart      (1000) bart      (1000)     1163 2022-02-28 14:01:35.000000 netqasm-0.9.0/netqasm/examples/apps/chsh/app_alice.py
--rwxrwxr-x   0 bart      (1000) bart      (1000)     1565 2022-02-28 14:01:35.000000 netqasm-0.9.0/netqasm/examples/apps/chsh/app_bob.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     1040 2022-02-28 14:01:35.000000 netqasm-0.9.0/netqasm/examples/apps/chsh/app_repeater.py
--rw-rw-r--   0 bart      (1000) bart      (1000)        4 2021-05-19 15:28:08.000000 netqasm-0.9.0/netqasm/examples/apps/chsh/bob.yaml
--rw-rw-r--   0 bart      (1000) bart      (1000)      689 2021-05-19 15:28:08.000000 netqasm-0.9.0/netqasm/examples/apps/chsh/network.yaml
--rw-rw-r--   0 bart      (1000) bart      (1000)       50 2021-05-19 15:28:08.000000 netqasm-0.9.0/netqasm/examples/apps/chsh/roles.yaml
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:35.556217 netqasm-0.9.0/netqasm/examples/apps/dist_cnot/
--rw-rw-r--   0 bart      (1000) bart      (1000)      718 2021-05-19 15:28:08.000000 netqasm-0.9.0/netqasm/examples/apps/dist_cnot/README.md
--rw-rw-r--   0 bart      (1000) bart      (1000)        0 2021-05-19 15:28:08.000000 netqasm-0.9.0/netqasm/examples/apps/dist_cnot/__init__.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     1775 2022-02-28 14:01:35.000000 netqasm-0.9.0/netqasm/examples/apps/dist_cnot/app_controller.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     1868 2022-02-28 14:01:35.000000 netqasm-0.9.0/netqasm/examples/apps/dist_cnot/app_target.py
--rw-rw-r--   0 bart      (1000) bart      (1000)       21 2022-01-17 15:40:37.000000 netqasm-0.9.0/netqasm/examples/apps/dist_cnot/controller.yaml
--rw-rw-r--   0 bart      (1000) bart      (1000)       17 2022-01-17 15:38:44.000000 netqasm-0.9.0/netqasm/examples/apps/dist_cnot/target.yaml
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:35.556217 netqasm-0.9.0/netqasm/examples/apps/link_layer_ck/
--rw-rw-r--   0 bart      (1000) bart      (1000)        0 2022-01-17 15:35:34.000000 netqasm-0.9.0/netqasm/examples/apps/link_layer_ck/__init__.py
--rwxrwxr-x   0 bart      (1000) bart      (1000)      928 2022-02-28 14:01:35.000000 netqasm-0.9.0/netqasm/examples/apps/link_layer_ck/app_client.py
--rwxrwxr-x   0 bart      (1000) bart      (1000)      926 2022-02-28 14:01:35.000000 netqasm-0.9.0/netqasm/examples/apps/link_layer_ck/app_server.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:35.560217 netqasm-0.9.0/netqasm/examples/apps/link_layer_md/
--rw-rw-r--   0 bart      (1000) bart      (1000)        0 2022-01-17 15:35:34.000000 netqasm-0.9.0/netqasm/examples/apps/link_layer_md/__init__.py
--rwxrwxr-x   0 bart      (1000) bart      (1000)      720 2022-02-28 14:01:35.000000 netqasm-0.9.0/netqasm/examples/apps/link_layer_md/app_client.py
--rwxrwxr-x   0 bart      (1000) bart      (1000)      600 2022-02-28 14:01:35.000000 netqasm-0.9.0/netqasm/examples/apps/link_layer_md/app_server.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:35.564217 netqasm-0.9.0/netqasm/examples/apps/magic_square/
--rw-rw-r--   0 bart      (1000) bart      (1000)      618 2021-05-19 15:28:08.000000 netqasm-0.9.0/netqasm/examples/apps/magic_square/README.md
--rw-rw-r--   0 bart      (1000) bart      (1000)        0 2021-05-19 15:28:08.000000 netqasm-0.9.0/netqasm/examples/apps/magic_square/__init__.py
--rwxrwxr-x   0 bart      (1000) bart      (1000)     1987 2022-02-28 14:01:35.000000 netqasm-0.9.0/netqasm/examples/apps/magic_square/app_player1.py
--rwxrwxr-x   0 bart      (1000) bart      (1000)     2022 2022-02-28 14:01:35.000000 netqasm-0.9.0/netqasm/examples/apps/magic_square/app_player2.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      121 2021-05-19 15:28:08.000000 netqasm-0.9.0/netqasm/examples/apps/magic_square/player1.yaml
--rw-rw-r--   0 bart      (1000) bart      (1000)      134 2022-01-17 15:40:37.000000 netqasm-0.9.0/netqasm/examples/apps/magic_square/player2.yaml
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:35.572217 netqasm-0.9.0/netqasm/examples/apps/multiple_files/
--rw-rw-r--   0 bart      (1000) bart      (1000)        0 2021-05-19 15:28:08.000000 netqasm-0.9.0/netqasm/examples/apps/multiple_files/__init__.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      702 2022-01-17 15:40:12.000000 netqasm-0.9.0/netqasm/examples/apps/multiple_files/app_alice.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      627 2022-01-17 15:40:12.000000 netqasm-0.9.0/netqasm/examples/apps/multiple_files/app_bob.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:35.572217 netqasm-0.9.0/netqasm/examples/apps/multiple_files/shared/
--rw-rw-r--   0 bart      (1000) bart      (1000)        0 2021-05-19 15:28:08.000000 netqasm-0.9.0/netqasm/examples/apps/multiple_files/shared/__init__.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      163 2021-05-19 15:28:08.000000 netqasm-0.9.0/netqasm/examples/apps/multiple_files/shared/myfuncs.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:35.576217 netqasm-0.9.0/netqasm/examples/apps/single_node/
--rw-rw-r--   0 bart      (1000) bart      (1000)        0 2021-05-19 15:28:08.000000 netqasm-0.9.0/netqasm/examples/apps/single_node/__init__.py
--rw-rw-r--   0 bart      (1000) bart      (1000)       20 2021-05-19 15:28:08.000000 netqasm-0.9.0/netqasm/examples/apps/single_node/alice.yaml
--rwxrwxr-x   0 bart      (1000) bart      (1000)      726 2022-01-17 15:35:34.000000 netqasm-0.9.0/netqasm/examples/apps/single_node/app_alice.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:35.584217 netqasm-0.9.0/netqasm/examples/apps/teleport/
--rw-rw-r--   0 bart      (1000) bart      (1000)      423 2021-05-19 15:28:08.000000 netqasm-0.9.0/netqasm/examples/apps/teleport/README.md
--rw-rw-r--   0 bart      (1000) bart      (1000)        0 2021-05-19 15:28:08.000000 netqasm-0.9.0/netqasm/examples/apps/teleport/__init__.py
--rwxrwxr-x   0 bart      (1000) bart      (1000)     2399 2022-02-28 14:01:35.000000 netqasm-0.9.0/netqasm/examples/apps/teleport/app_receiver.py
--rwxrwxr-x   0 bart      (1000) bart      (1000)     1795 2022-02-28 14:01:35.000000 netqasm-0.9.0/netqasm/examples/apps/teleport/app_sender.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      444 2022-01-17 15:23:58.000000 netqasm-0.9.0/netqasm/examples/apps/teleport/network.yaml
--rw-rw-r--   0 bart      (1000) bart      (1000)        0 2021-05-19 15:28:08.000000 netqasm-0.9.0/netqasm/examples/apps/teleport/receiver.yaml
--rw-rw-r--   0 bart      (1000) bart      (1000)     1816 2022-01-17 15:40:37.000000 netqasm-0.9.0/netqasm/examples/apps/teleport/results_config.json
--rw-rw-r--   0 bart      (1000) bart      (1000)       37 2021-05-19 15:28:08.000000 netqasm-0.9.0/netqasm/examples/apps/teleport/roles.yaml
--rw-rw-r--   0 bart      (1000) bart      (1000)       19 2022-01-17 15:40:37.000000 netqasm-0.9.0/netqasm/examples/apps/teleport/sender.yaml
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:35.588217 netqasm-0.9.0/netqasm/examples/apps/three_nodes/
--rw-rw-r--   0 bart      (1000) bart      (1000)        0 2021-05-19 15:28:08.000000 netqasm-0.9.0/netqasm/examples/apps/three_nodes/__init__.py
--rwxrwxr-x   0 bart      (1000) bart      (1000)      964 2022-02-28 14:01:35.000000 netqasm-0.9.0/netqasm/examples/apps/three_nodes/app_alice.py
--rwxrwxr-x   0 bart      (1000) bart      (1000)      972 2022-02-28 14:01:35.000000 netqasm-0.9.0/netqasm/examples/apps/three_nodes/app_bob.py
--rwxrwxr-x   0 bart      (1000) bart      (1000)      905 2022-02-28 14:01:35.000000 netqasm-0.9.0/netqasm/examples/apps/three_nodes/app_charlie.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      797 2021-05-19 15:28:08.000000 netqasm-0.9.0/netqasm/examples/apps/three_nodes/network.yaml
--rw-rw-r--   0 bart      (1000) bart      (1000)       49 2021-05-19 15:28:08.000000 netqasm-0.9.0/netqasm/examples/apps/three_nodes/roles.yaml
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:35.588217 netqasm-0.9.0/netqasm/examples/lib/
--rw-rw-r--   0 bart      (1000) bart      (1000)        0 2021-05-19 15:28:08.000000 netqasm-0.9.0/netqasm/examples/lib/__init__.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     1548 2022-02-28 14:01:35.000000 netqasm-0.9.0/netqasm/examples/lib/bqc.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     2837 2022-01-17 15:40:12.000000 netqasm-0.9.0/netqasm/examples/run_examples.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:35.592217 netqasm-0.9.0/netqasm/examples/sdk_compilation/
--rw-rw-r--   0 bart      (1000) bart      (1000)        0 2022-01-17 15:40:12.000000 netqasm-0.9.0/netqasm/examples/sdk_compilation/__init__.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     1214 2022-01-31 10:25:20.000000 netqasm-0.9.0/netqasm/examples/sdk_compilation/example_bb84.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      711 2022-01-17 15:40:12.000000 netqasm-0.9.0/netqasm/examples/sdk_compilation/example_enumerate.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      700 2022-01-17 15:40:12.000000 netqasm-0.9.0/netqasm/examples/sdk_compilation/example_loop.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      726 2022-01-17 15:40:12.000000 netqasm-0.9.0/netqasm/examples/sdk_compilation/example_post_epr.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      667 2022-02-28 14:01:35.000000 netqasm-0.9.0/netqasm/examples/sdk_compilation/example_rsp.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      545 2022-01-17 15:40:12.000000 netqasm-0.9.0/netqasm/examples/sdk_compilation/example_simple_loop.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:35.600217 netqasm-0.9.0/netqasm/lang/
--rw-rw-r--   0 bart      (1000) bart      (1000)        0 2021-05-19 15:28:08.000000 netqasm-0.9.0/netqasm/lang/__init__.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     6804 2022-01-17 15:40:12.000000 netqasm-0.9.0/netqasm/lang/encoding.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:35.604217 netqasm-0.9.0/netqasm/lang/instr/
--rw-rw-r--   0 bart      (1000) bart      (1000)      111 2022-01-17 15:35:34.000000 netqasm-0.9.0/netqasm/lang/instr/__init__.py
--rw-rw-r--   0 bart      (1000) bart      (1000)    22917 2022-01-17 15:40:12.000000 netqasm-0.9.0/netqasm/lang/instr/base.py
--rw-rw-r--   0 bart      (1000) bart      (1000)    11443 2022-01-17 15:40:12.000000 netqasm-0.9.0/netqasm/lang/instr/core.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     3325 2022-01-17 15:40:12.000000 netqasm-0.9.0/netqasm/lang/instr/flavour.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     3007 2022-01-17 15:35:34.000000 netqasm-0.9.0/netqasm/lang/instr/nv.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     3827 2022-01-17 15:35:34.000000 netqasm-0.9.0/netqasm/lang/instr/vanilla.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     5528 2022-02-28 13:02:08.000000 netqasm-0.9.0/netqasm/lang/ir.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     3910 2022-01-17 15:35:34.000000 netqasm-0.9.0/netqasm/lang/operand.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:35.608217 netqasm-0.9.0/netqasm/lang/parsing/
--rw-rw-r--   0 bart      (1000) bart      (1000)      147 2022-01-17 15:35:34.000000 netqasm-0.9.0/netqasm/lang/parsing/__init__.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     2385 2022-01-17 15:35:34.000000 netqasm-0.9.0/netqasm/lang/parsing/binary.py
--rw-rw-r--   0 bart      (1000) bart      (1000)    19082 2022-01-24 14:24:18.000000 netqasm-0.9.0/netqasm/lang/parsing/text.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     1577 2022-01-17 15:35:34.000000 netqasm-0.9.0/netqasm/lang/subroutine.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      357 2022-01-17 15:40:37.000000 netqasm-0.9.0/netqasm/lang/symbols.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:35.612218 netqasm-0.9.0/netqasm/logging/
--rw-rw-r--   0 bart      (1000) bart      (1000)        0 2021-05-19 15:28:08.000000 netqasm-0.9.0/netqasm/logging/__init__.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     1039 2022-01-17 15:40:12.000000 netqasm-0.9.0/netqasm/logging/glob.py
--rw-rw-r--   0 bart      (1000) bart      (1000)    12547 2022-01-17 15:44:13.000000 netqasm-0.9.0/netqasm/logging/output.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     9902 2022-02-28 14:01:35.000000 netqasm-0.9.0/netqasm/qlink_compat.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:35.624218 netqasm-0.9.0/netqasm/runtime/
--rw-rw-r--   0 bart      (1000) bart      (1000)        0 2021-05-19 15:28:08.000000 netqasm-0.9.0/netqasm/runtime/__init__.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      510 2022-01-17 15:35:34.000000 netqasm-0.9.0/netqasm/runtime/app_config.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     6460 2022-01-17 15:35:34.000000 netqasm-0.9.0/netqasm/runtime/application.py
--rw-rw-r--   0 bart      (1000) bart      (1000)    12507 2022-01-17 15:40:12.000000 netqasm-0.9.0/netqasm/runtime/cli.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      491 2022-01-17 15:35:34.000000 netqasm-0.9.0/netqasm/runtime/debug.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     8925 2022-01-17 15:40:12.000000 netqasm-0.9.0/netqasm/runtime/env.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     2337 2022-01-17 15:40:12.000000 netqasm-0.9.0/netqasm/runtime/hardware.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:35.636218 netqasm-0.9.0/netqasm/runtime/interface/
--rw-rw-r--   0 bart      (1000) bart      (1000)      170 2022-01-17 15:35:34.000000 netqasm-0.9.0/netqasm/runtime/interface/__init__.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     3498 2022-01-17 15:35:34.000000 netqasm-0.9.0/netqasm/runtime/interface/config.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     4831 2022-01-17 15:44:13.000000 netqasm-0.9.0/netqasm/runtime/interface/logging.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      146 2022-01-17 15:35:34.000000 netqasm-0.9.0/netqasm/runtime/interface/results.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     2970 2022-01-17 15:35:34.000000 netqasm-0.9.0/netqasm/runtime/process_logs.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      838 2022-01-17 15:35:34.000000 netqasm-0.9.0/netqasm/runtime/runtime_mgr.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      864 2022-01-17 15:35:34.000000 netqasm-0.9.0/netqasm/runtime/settings.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:35.680218 netqasm-0.9.0/netqasm/sdk/
--rw-rw-r--   0 bart      (1000) bart      (1000)      220 2022-01-17 15:35:34.000000 netqasm-0.9.0/netqasm/sdk/__init__.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     7238 2022-02-28 14:01:35.000000 netqasm-0.9.0/netqasm/sdk/build_epr.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      552 2022-02-28 14:01:35.000000 netqasm-0.9.0/netqasm/sdk/build_nv.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     2123 2022-02-28 14:01:35.000000 netqasm-0.9.0/netqasm/sdk/build_types.py
--rw-rw-r--   0 bart      (1000) bart      (1000)    78479 2022-02-28 14:01:35.000000 netqasm-0.9.0/netqasm/sdk/builder.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:35.688218 netqasm-0.9.0/netqasm/sdk/classical_communication/
--rw-rw-r--   0 bart      (1000) bart      (1000)       82 2022-01-17 15:35:34.000000 netqasm-0.9.0/netqasm/sdk/classical_communication/__init__.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     4546 2022-02-28 13:02:08.000000 netqasm-0.9.0/netqasm/sdk/classical_communication/broadcast_channel.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      105 2022-01-17 15:23:58.000000 netqasm-0.9.0/netqasm/sdk/classical_communication/message.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     4795 2022-02-28 13:02:08.000000 netqasm-0.9.0/netqasm/sdk/classical_communication/socket.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:35.692218 netqasm-0.9.0/netqasm/sdk/classical_communication/thread_socket/
--rw-rw-r--   0 bart      (1000) bart      (1000)      393 2022-01-17 15:35:34.000000 netqasm-0.9.0/netqasm/sdk/classical_communication/thread_socket/__init__.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      385 2022-02-28 13:02:08.000000 netqasm-0.9.0/netqasm/sdk/classical_communication/thread_socket/broadcast_channel.py
--rw-rw-r--   0 bart      (1000) bart      (1000)    13555 2022-01-17 15:40:12.000000 netqasm-0.9.0/netqasm/sdk/classical_communication/thread_socket/socket.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     7670 2022-02-28 13:02:08.000000 netqasm-0.9.0/netqasm/sdk/classical_communication/thread_socket/socket_hub.py
--rw-rw-r--   0 bart      (1000) bart      (1000)    22670 2022-02-28 14:01:35.000000 netqasm-0.9.0/netqasm/sdk/compiling.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      350 2022-01-17 15:35:34.000000 netqasm-0.9.0/netqasm/sdk/config.py
--rw-rw-r--   0 bart      (1000) bart      (1000)    33248 2022-02-28 14:01:35.000000 netqasm-0.9.0/netqasm/sdk/connection.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      833 2022-02-28 14:01:35.000000 netqasm-0.9.0/netqasm/sdk/constraint.py
--rw-rw-r--   0 bart      (1000) bart      (1000)    39028 2022-02-28 14:01:35.000000 netqasm-0.9.0/netqasm/sdk/epr_socket.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     4156 2022-01-17 15:40:12.000000 netqasm-0.9.0/netqasm/sdk/external.py
--rw-rw-r--   0 bart      (1000) bart      (1000)    23172 2022-02-28 14:01:35.000000 netqasm-0.9.0/netqasm/sdk/futures.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     6328 2022-02-28 14:01:35.000000 netqasm-0.9.0/netqasm/sdk/memmgr.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     1317 2022-01-17 15:35:34.000000 netqasm-0.9.0/netqasm/sdk/network.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      803 2022-01-17 15:35:34.000000 netqasm-0.9.0/netqasm/sdk/progress_bar.py
--rw-rw-r--   0 bart      (1000) bart      (1000)    13666 2022-02-28 14:01:35.000000 netqasm-0.9.0/netqasm/sdk/qubit.py
--rw-rw-r--   0 bart      (1000) bart      (1000)    11706 2022-02-28 13:02:08.000000 netqasm-0.9.0/netqasm/sdk/shared_memory.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:35.704218 netqasm-0.9.0/netqasm/sdk/toolbox/
--rw-rw-r--   0 bart      (1000) bart      (1000)      183 2022-01-17 15:35:34.000000 netqasm-0.9.0/netqasm/sdk/toolbox/__init__.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      787 2022-01-17 15:35:34.000000 netqasm-0.9.0/netqasm/sdk/toolbox/gates.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     3433 2022-01-17 15:35:34.000000 netqasm-0.9.0/netqasm/sdk/toolbox/measurements.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     4634 2022-02-28 14:01:35.000000 netqasm-0.9.0/netqasm/sdk/toolbox/multi_node.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     1516 2022-01-17 15:40:12.000000 netqasm-0.9.0/netqasm/sdk/toolbox/sim_states.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     2026 2022-02-28 13:02:08.000000 netqasm-0.9.0/netqasm/sdk/toolbox/state_prep.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      106 2022-01-17 15:35:34.000000 netqasm-0.9.0/netqasm/typedefs.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      347 2021-05-19 15:28:08.000000 netqasm-0.9.0/netqasm/typing.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:35.712219 netqasm-0.9.0/netqasm/util/
--rw-rw-r--   0 bart      (1000) bart      (1000)        0 2021-05-19 15:28:08.000000 netqasm-0.9.0/netqasm/util/__init__.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      252 2022-01-17 15:35:34.000000 netqasm-0.9.0/netqasm/util/error.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     1922 2022-01-17 15:35:34.000000 netqasm-0.9.0/netqasm/util/log.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     3501 2022-02-28 14:01:35.000000 netqasm-0.9.0/netqasm/util/quantum_gates.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      914 2022-02-28 13:02:08.000000 netqasm-0.9.0/netqasm/util/states.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     2858 2022-01-17 15:35:34.000000 netqasm-0.9.0/netqasm/util/string.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      519 2021-05-19 15:28:08.000000 netqasm-0.9.0/netqasm/util/thread.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      445 2022-01-17 15:35:34.000000 netqasm-0.9.0/netqasm/util/yaml.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:35.492216 netqasm-0.9.0/netqasm.egg-info/
--rw-rw-r--   0 bart      (1000) bart      (1000)     5201 2022-03-03 14:44:33.000000 netqasm-0.9.0/netqasm.egg-info/PKG-INFO
--rw-rw-r--   0 bart      (1000) bart      (1000)    24275 2022-03-03 14:44:34.000000 netqasm-0.9.0/netqasm.egg-info/SOURCES.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)        1 2022-03-03 14:44:34.000000 netqasm-0.9.0/netqasm.egg-info/dependency_links.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)       52 2022-03-03 14:44:34.000000 netqasm-0.9.0/netqasm.egg-info/entry_points.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)      286 2022-03-03 14:44:34.000000 netqasm-0.9.0/netqasm.egg-info/requires.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)        8 2022-03-03 14:44:34.000000 netqasm-0.9.0/netqasm.egg-info/top_level.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)      249 2022-01-17 15:40:12.000000 netqasm-0.9.0/pyproject.toml
--rw-rw-r--   0 bart      (1000) bart      (1000)      182 2022-01-17 15:38:44.000000 netqasm-0.9.0/requirements.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)      545 2022-03-03 14:44:35.736219 netqasm-0.9.0/setup.cfg
--rw-rw-r--   0 bart      (1000) bart      (1000)      578 2022-01-17 15:40:12.000000 netqasm-0.9.0/setup.py
--rw-rw-r--   0 bart      (1000) bart      (1000)       99 2022-01-17 15:38:44.000000 netqasm-0.9.0/test_requirements.txt
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:35.716219 netqasm-0.9.0/tests/
--rw-rw-r--   0 bart      (1000) bart      (1000)    24497 2022-02-28 14:01:35.000000 netqasm-0.9.0/tests/test_builder.py
--rw-rw-r--   0 bart      (1000) bart      (1000)    11006 2022-01-17 15:38:44.000000 netqasm-0.9.0/tests/test_cli.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     8471 2022-01-17 15:40:12.000000 netqasm-0.9.0/tests/test_compiling.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     2392 2022-01-17 15:44:13.000000 netqasm-0.9.0/tests/test_encoding.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     3332 2022-01-17 15:44:13.000000 netqasm-0.9.0/tests/test_executor.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:35.716219 netqasm-0.9.0/tests/test_external/
--rw-rw-r--   0 bart      (1000) bart      (1000)     4177 2022-01-17 15:40:12.000000 netqasm-0.9.0/tests/test_external/test_examples.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:35.728219 netqasm-0.9.0/tests/test_external/test_sdk/
--rw-rw-r--   0 bart      (1000) bart      (1000)     1725 2022-01-17 15:40:12.000000 netqasm-0.9.0/tests/test_external/test_sdk/test_create_epr.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     1471 2022-01-17 15:40:12.000000 netqasm-0.9.0/tests/test_external/test_sdk/test_create_epr_m.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     1150 2022-02-28 14:01:35.000000 netqasm-0.9.0/tests/test_external/test_sdk/test_enumerate.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     1180 2022-01-17 15:40:12.000000 netqasm-0.9.0/tests/test_external/test_sdk/test_foreach.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      793 2022-01-17 15:40:12.000000 netqasm-0.9.0/tests/test_external/test_sdk/test_measure.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      858 2022-01-17 15:40:12.000000 netqasm-0.9.0/tests/test_external/test_sdk/test_measure_if_conn.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      795 2022-01-17 15:40:12.000000 netqasm-0.9.0/tests/test_external/test_sdk/test_measure_if_future.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      945 2022-02-28 14:01:35.000000 netqasm-0.9.0/tests/test_external/test_sdk/test_measure_loop.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     1132 2022-01-17 15:40:12.000000 netqasm-0.9.0/tests/test_external/test_sdk/test_measure_loop_context.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     1161 2022-02-28 14:01:35.000000 netqasm-0.9.0/tests/test_external/test_sdk/test_nested_loop.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     1180 2022-02-28 14:01:35.000000 netqasm-0.9.0/tests/test_external/test_sdk/test_new_array.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     1503 2022-02-14 15:52:46.000000 netqasm-0.9.0/tests/test_external/test_sdk/test_post_epr.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     1386 2022-01-27 15:33:30.000000 netqasm-0.9.0/tests/test_external/test_sdk/test_post_epr_context.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      907 2022-01-17 15:40:12.000000 netqasm-0.9.0/tests/test_external/test_sdk/test_rotations.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     2050 2022-01-17 15:40:12.000000 netqasm-0.9.0/tests/test_external/test_sdk/test_teleport.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     2236 2022-01-17 15:40:12.000000 netqasm-0.9.0/tests/test_external/test_sdk/test_teleport_without_corrections.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     1063 2022-01-17 15:40:12.000000 netqasm-0.9.0/tests/test_external/test_sdk/test_two_nodes.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     4031 2022-01-17 15:35:34.000000 netqasm-0.9.0/tests/test_external/test_toolbox.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:35.728219 netqasm-0.9.0/tests/test_parsing/
--rw-rw-r--   0 bart      (1000) bart      (1000)     2158 2022-01-17 15:44:13.000000 netqasm-0.9.0/tests/test_parsing/test_binary.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     8671 2022-01-17 15:44:13.000000 netqasm-0.9.0/tests/test_parsing/test_text.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-03-03 14:44:35.732219 netqasm-0.9.0/tests/test_sdk/
--rw-rw-r--   0 bart      (1000) bart      (1000)     5612 2022-01-17 15:40:12.000000 netqasm-0.9.0/tests/test_sdk/test_classical_communication.py
--rw-rw-r--   0 bart      (1000) bart      (1000)    35647 2022-02-28 14:01:35.000000 netqasm-0.9.0/tests/test_sdk/test_connection.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      998 2022-01-17 15:35:34.000000 netqasm-0.9.0/tests/test_sdk/test_future.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     1369 2022-01-17 15:35:34.000000 netqasm-0.9.0/tests/test_states_util.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     3051 2022-01-17 15:35:34.000000 netqasm-0.9.0/tests/test_string_util.py
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:27.489104 netqasm-0.9.1/
+-rw-rw-r--   0 bart      (1000) bart      (1000)      186 2022-03-25 17:15:19.000000 netqasm-0.9.1/.flake8
+-rw-rw-r--   0 bart      (1000) bart      (1000)    11644 2022-04-07 14:08:27.000000 netqasm-0.9.1/CHANGELOG.md
+-rw-rw-r--   0 bart      (1000) bart      (1000)     1063 2022-03-28 08:45:06.000000 netqasm-0.9.1/LICENSE
+-rw-rw-r--   0 bart      (1000) bart      (1000)      210 2022-03-28 08:45:06.000000 netqasm-0.9.1/MANIFEST.in
+-rw-rw-r--   0 bart      (1000) bart      (1000)     2736 2022-03-28 08:45:06.000000 netqasm-0.9.1/Makefile
+-rw-rw-r--   0 bart      (1000) bart      (1000)     5201 2022-04-07 14:53:27.489104 netqasm-0.9.1/PKG-INFO
+-rw-rw-r--   0 bart      (1000) bart      (1000)     4841 2022-04-07 14:51:03.000000 netqasm-0.9.1/README.md
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:26.801099 netqasm-0.9.1/docs/
+-rw-rw-r--   0 bart      (1000) bart      (1000)      912 2021-05-19 15:28:08.000000 netqasm-0.9.1/docs/Makefile
+-rw-rw-r--   0 bart      (1000) bart      (1000)      504 2022-03-25 17:15:19.000000 netqasm-0.9.1/docs/README.md
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:26.805099 netqasm-0.9.1/docs/api_backend/
+-rw-rw-r--   0 bart      (1000) bart      (1000)      174 2022-03-25 17:15:19.000000 netqasm-0.9.1/docs/api_backend/netqasm.backend.executor.rst
+-rw-rw-r--   0 bart      (1000) bart      (1000)      174 2022-03-25 17:15:19.000000 netqasm-0.9.1/docs/api_backend/netqasm.backend.messages.rst
+-rw-rw-r--   0 bart      (1000) bart      (1000)      188 2022-03-25 17:15:19.000000 netqasm-0.9.1/docs/api_backend/netqasm.backend.network_stack.rst
+-rw-rw-r--   0 bart      (1000) bart      (1000)      172 2022-03-25 17:15:19.000000 netqasm-0.9.1/docs/api_backend/netqasm.backend.qnodeos.rst
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:26.813099 netqasm-0.9.1/docs/api_lang/
+-rw-rw-r--   0 bart      (1000) bart      (1000)      168 2022-03-25 17:15:19.000000 netqasm-0.9.1/docs/api_lang/netqasm.lang.encoding.rst
+-rw-rw-r--   0 bart      (1000) bart      (1000)      816 2022-03-25 17:15:19.000000 netqasm-0.9.1/docs/api_lang/netqasm.lang.instr.rst
+-rw-rw-r--   0 bart      (1000) bart      (1000)      156 2022-03-25 17:15:19.000000 netqasm-0.9.1/docs/api_lang/netqasm.lang.ir.rst
+-rw-rw-r--   0 bart      (1000) bart      (1000)      166 2022-03-25 17:15:19.000000 netqasm-0.9.1/docs/api_lang/netqasm.lang.operand.rst
+-rw-rw-r--   0 bart      (1000) bart      (1000)      366 2022-03-25 17:15:19.000000 netqasm-0.9.1/docs/api_lang/netqasm.lang.parsing.rst
+-rw-rw-r--   0 bart      (1000) bart      (1000)      172 2022-03-25 17:15:19.000000 netqasm-0.9.1/docs/api_lang/netqasm.lang.subroutine.rst
+-rw-rw-r--   0 bart      (1000) bart      (1000)      166 2022-03-25 17:15:19.000000 netqasm-0.9.1/docs/api_lang/netqasm.lang.symbols.rst
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:26.813099 netqasm-0.9.1/docs/api_logging/
+-rw-rw-r--   0 bart      (1000) bart      (1000)      170 2022-03-25 17:15:19.000000 netqasm-0.9.1/docs/api_logging/netqasm.logging.glob.rst
+-rw-rw-r--   0 bart      (1000) bart      (1000)      166 2022-03-25 17:15:19.000000 netqasm-0.9.1/docs/api_logging/netqasm.logging.output.rst
+-rw-rw-r--   0 bart      (1000) bart      (1000)      176 2022-03-28 08:45:06.000000 netqasm-0.9.1/docs/api_root.rst
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:26.821100 netqasm-0.9.1/docs/api_runtime/
+-rw-rw-r--   0 bart      (1000) bart      (1000)      179 2022-03-28 08:45:06.000000 netqasm-0.9.1/docs/api_runtime/netqasm.runtime.app_config.rst
+-rw-rw-r--   0 bart      (1000) bart      (1000)      182 2022-03-28 08:45:06.000000 netqasm-0.9.1/docs/api_runtime/netqasm.runtime.application.rst
+-rw-rw-r--   0 bart      (1000) bart      (1000)      164 2022-03-25 17:15:19.000000 netqasm-0.9.1/docs/api_runtime/netqasm.runtime.cli.rst
+-rw-rw-r--   0 bart      (1000) bart      (1000)      168 2022-03-25 17:15:19.000000 netqasm-0.9.1/docs/api_runtime/netqasm.runtime.debug.rst
+-rw-rw-r--   0 bart      (1000) bart      (1000)      164 2022-03-25 17:15:19.000000 netqasm-0.9.1/docs/api_runtime/netqasm.runtime.env.rst
+-rw-rw-r--   0 bart      (1000) bart      (1000)      174 2022-03-25 17:15:19.000000 netqasm-0.9.1/docs/api_runtime/netqasm.runtime.hardware.rst
+-rw-rw-r--   0 bart      (1000) bart      (1000)      593 2022-03-28 08:45:06.000000 netqasm-0.9.1/docs/api_runtime/netqasm.runtime.interface.rst
+-rw-rw-r--   0 bart      (1000) bart      (1000)      185 2022-03-28 08:45:06.000000 netqasm-0.9.1/docs/api_runtime/netqasm.runtime.process_logs.rst
+-rw-rw-r--   0 bart      (1000) bart      (1000)      174 2022-03-25 17:15:19.000000 netqasm-0.9.1/docs/api_runtime/netqasm.runtime.settings.rst
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:26.833100 netqasm-0.9.1/docs/api_sdk/
+-rw-rw-r--   0 bart      (1000) bart      (1000)      164 2022-03-25 17:15:19.000000 netqasm-0.9.1/docs/api_sdk/netqasm.sdk.builder.rst
+-rw-rw-r--   0 bart      (1000) bart      (1000)     1493 2022-03-28 08:45:06.000000 netqasm-0.9.1/docs/api_sdk/netqasm.sdk.classical_communication.rst
+-rw-rw-r--   0 bart      (1000) bart      (1000)      168 2022-03-25 17:15:19.000000 netqasm-0.9.1/docs/api_sdk/netqasm.sdk.compiling.rst
+-rw-rw-r--   0 bart      (1000) bart      (1000)      162 2022-03-25 17:15:19.000000 netqasm-0.9.1/docs/api_sdk/netqasm.sdk.config.rst
+-rw-rw-r--   0 bart      (1000) bart      (1000)      170 2022-03-25 17:15:19.000000 netqasm-0.9.1/docs/api_sdk/netqasm.sdk.connection.rst
+-rw-rw-r--   0 bart      (1000) bart      (1000)      170 2022-03-25 17:15:19.000000 netqasm-0.9.1/docs/api_sdk/netqasm.sdk.epr_socket.rst
+-rw-rw-r--   0 bart      (1000) bart      (1000)      166 2022-03-25 17:15:19.000000 netqasm-0.9.1/docs/api_sdk/netqasm.sdk.external.rst
+-rw-rw-r--   0 bart      (1000) bart      (1000)      164 2022-03-25 17:15:19.000000 netqasm-0.9.1/docs/api_sdk/netqasm.sdk.futures.rst
+-rw-rw-r--   0 bart      (1000) bart      (1000)      164 2022-03-25 17:15:19.000000 netqasm-0.9.1/docs/api_sdk/netqasm.sdk.network.rst
+-rw-rw-r--   0 bart      (1000) bart      (1000)      174 2022-03-25 17:15:19.000000 netqasm-0.9.1/docs/api_sdk/netqasm.sdk.progress_bar.rst
+-rw-rw-r--   0 bart      (1000) bart      (1000)      160 2022-03-25 17:15:19.000000 netqasm-0.9.1/docs/api_sdk/netqasm.sdk.qubit.rst
+-rw-rw-r--   0 bart      (1000) bart      (1000)      176 2022-03-25 17:15:19.000000 netqasm-0.9.1/docs/api_sdk/netqasm.sdk.shared_memory.rst
+-rw-rw-r--   0 bart      (1000) bart      (1000)      994 2022-03-25 17:15:19.000000 netqasm-0.9.1/docs/api_sdk/netqasm.sdk.toolbox.rst
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:26.841100 netqasm-0.9.1/docs/api_util/
+-rw-rw-r--   0 bart      (1000) bart      (1000)      162 2022-03-25 17:15:19.000000 netqasm-0.9.1/docs/api_util/netqasm.util.error.rst
+-rw-rw-r--   0 bart      (1000) bart      (1000)      158 2022-03-25 17:15:19.000000 netqasm-0.9.1/docs/api_util/netqasm.util.log.rst
+-rw-rw-r--   0 bart      (1000) bart      (1000)      179 2022-03-25 17:15:19.000000 netqasm-0.9.1/docs/api_util/netqasm.util.quantum_gates.rst
+-rw-rw-r--   0 bart      (1000) bart      (1000)      164 2022-03-25 17:15:19.000000 netqasm-0.9.1/docs/api_util/netqasm.util.states.rst
+-rw-rw-r--   0 bart      (1000) bart      (1000)      164 2022-03-25 17:15:19.000000 netqasm-0.9.1/docs/api_util/netqasm.util.string.rst
+-rw-rw-r--   0 bart      (1000) bart      (1000)      164 2022-03-25 17:15:19.000000 netqasm-0.9.1/docs/api_util/netqasm.util.thread.rst
+-rw-rw-r--   0 bart      (1000) bart      (1000)      160 2022-03-25 17:15:19.000000 netqasm-0.9.1/docs/api_util/netqasm.util.yaml.rst
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:26.773099 netqasm-0.9.1/docs/build/
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:26.853100 netqasm-0.9.1/docs/build/doctrees/
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:26.857100 netqasm-0.9.1/docs/build/doctrees/api_backend/
+-rw-rw-r--   0 bart      (1000) bart      (1000)    82242 2021-11-25 15:03:24.000000 netqasm-0.9.1/docs/build/doctrees/api_backend/netqasm.backend.executor.doctree
+-rw-rw-r--   0 bart      (1000) bart      (1000)   139066 2021-11-25 15:03:25.000000 netqasm-0.9.1/docs/build/doctrees/api_backend/netqasm.backend.messages.doctree
+-rw-rw-r--   0 bart      (1000) bart      (1000)    28783 2021-11-25 15:03:25.000000 netqasm-0.9.1/docs/build/doctrees/api_backend/netqasm.backend.network_stack.doctree
+-rw-rw-r--   0 bart      (1000) bart      (1000)    33566 2021-11-25 15:03:25.000000 netqasm-0.9.1/docs/build/doctrees/api_backend/netqasm.backend.qnodeos.doctree
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:26.869100 netqasm-0.9.1/docs/build/doctrees/api_lang/
+-rw-rw-r--   0 bart      (1000) bart      (1000)   171040 2021-11-25 15:03:26.000000 netqasm-0.9.1/docs/build/doctrees/api_lang/netqasm.lang.encoding.doctree
+-rw-rw-r--   0 bart      (1000) bart      (1000)  1273221 2021-11-25 15:03:28.000000 netqasm-0.9.1/docs/build/doctrees/api_lang/netqasm.lang.instr.doctree
+-rw-rw-r--   0 bart      (1000) bart      (1000)    95126 2021-11-25 15:03:28.000000 netqasm-0.9.1/docs/build/doctrees/api_lang/netqasm.lang.ir.doctree
+-rw-rw-r--   0 bart      (1000) bart      (1000)    54066 2021-11-25 15:03:28.000000 netqasm-0.9.1/docs/build/doctrees/api_lang/netqasm.lang.operand.doctree
+-rw-rw-r--   0 bart      (1000) bart      (1000)    49063 2021-11-25 15:03:29.000000 netqasm-0.9.1/docs/build/doctrees/api_lang/netqasm.lang.parsing.doctree
+-rw-rw-r--   0 bart      (1000) bart      (1000)    16479 2021-11-25 15:03:29.000000 netqasm-0.9.1/docs/build/doctrees/api_lang/netqasm.lang.subroutine.doctree
+-rw-rw-r--   0 bart      (1000) bart      (1000)    17646 2021-11-25 15:03:29.000000 netqasm-0.9.1/docs/build/doctrees/api_lang/netqasm.lang.symbols.doctree
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:26.873100 netqasm-0.9.1/docs/build/doctrees/api_logging/
+-rw-rw-r--   0 bart      (1000) bart      (1000)    35023 2021-11-25 15:03:29.000000 netqasm-0.9.1/docs/build/doctrees/api_logging/netqasm.logging.glob.doctree
+-rw-rw-r--   0 bart      (1000) bart      (1000)    12936 2021-11-25 15:03:29.000000 netqasm-0.9.1/docs/build/doctrees/api_logging/netqasm.logging.output.doctree
+-rw-rw-r--   0 bart      (1000) bart      (1000)     2764 2021-11-25 15:03:29.000000 netqasm-0.9.1/docs/build/doctrees/api_root.doctree
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:26.881100 netqasm-0.9.1/docs/build/doctrees/api_runtime/
+-rw-rw-r--   0 bart      (1000) bart      (1000)    22045 2021-11-25 15:03:29.000000 netqasm-0.9.1/docs/build/doctrees/api_runtime/netqasm.runtime.app_config.doctree
+-rw-rw-r--   0 bart      (1000) bart      (1000)    87474 2021-11-25 15:03:29.000000 netqasm-0.9.1/docs/build/doctrees/api_runtime/netqasm.runtime.application.doctree
+-rw-rw-r--   0 bart      (1000) bart      (1000)     3904 2021-11-25 15:03:30.000000 netqasm-0.9.1/docs/build/doctrees/api_runtime/netqasm.runtime.cli.doctree
+-rw-rw-r--   0 bart      (1000) bart      (1000)     8798 2021-11-25 15:03:30.000000 netqasm-0.9.1/docs/build/doctrees/api_runtime/netqasm.runtime.debug.doctree
+-rw-rw-r--   0 bart      (1000) bart      (1000)    27798 2021-11-25 15:03:30.000000 netqasm-0.9.1/docs/build/doctrees/api_runtime/netqasm.runtime.env.doctree
+-rw-rw-r--   0 bart      (1000) bart      (1000)     9841 2021-11-25 15:03:30.000000 netqasm-0.9.1/docs/build/doctrees/api_runtime/netqasm.runtime.hardware.doctree
+-rw-rw-r--   0 bart      (1000) bart      (1000)   211388 2021-11-25 15:03:30.000000 netqasm-0.9.1/docs/build/doctrees/api_runtime/netqasm.runtime.interface.doctree
+-rw-rw-r--   0 bart      (1000) bart      (1000)     5378 2021-11-26 13:17:03.000000 netqasm-0.9.1/docs/build/doctrees/api_runtime/netqasm.runtime.process_logs.doctree
+-rw-rw-r--   0 bart      (1000) bart      (1000)    22712 2021-11-25 15:03:30.000000 netqasm-0.9.1/docs/build/doctrees/api_runtime/netqasm.runtime.settings.doctree
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:26.909100 netqasm-0.9.1/docs/build/doctrees/api_sdk/
+-rw-rw-r--   0 bart      (1000) bart      (1000)   194990 2021-11-26 13:17:04.000000 netqasm-0.9.1/docs/build/doctrees/api_sdk/netqasm.sdk.builder.doctree
+-rw-rw-r--   0 bart      (1000) bart      (1000)   224332 2021-11-25 15:03:31.000000 netqasm-0.9.1/docs/build/doctrees/api_sdk/netqasm.sdk.classical_communication.doctree
+-rw-rw-r--   0 bart      (1000) bart      (1000)    31842 2021-11-25 15:03:32.000000 netqasm-0.9.1/docs/build/doctrees/api_sdk/netqasm.sdk.compiling.doctree
+-rw-rw-r--   0 bart      (1000) bart      (1000)    26587 2021-11-25 15:03:32.000000 netqasm-0.9.1/docs/build/doctrees/api_sdk/netqasm.sdk.config.doctree
+-rw-rw-r--   0 bart      (1000) bart      (1000)   352590 2021-11-26 13:17:05.000000 netqasm-0.9.1/docs/build/doctrees/api_sdk/netqasm.sdk.connection.doctree
+-rw-rw-r--   0 bart      (1000) bart      (1000)   106762 2021-11-26 13:17:05.000000 netqasm-0.9.1/docs/build/doctrees/api_sdk/netqasm.sdk.epr_socket.doctree
+-rw-rw-r--   0 bart      (1000) bart      (1000)     5791 2021-11-26 13:17:05.000000 netqasm-0.9.1/docs/build/doctrees/api_sdk/netqasm.sdk.external.doctree
+-rw-rw-r--   0 bart      (1000) bart      (1000)   232150 2021-11-26 13:17:06.000000 netqasm-0.9.1/docs/build/doctrees/api_sdk/netqasm.sdk.futures.doctree
+-rw-rw-r--   0 bart      (1000) bart      (1000)    12254 2021-11-25 15:03:33.000000 netqasm-0.9.1/docs/build/doctrees/api_sdk/netqasm.sdk.network.doctree
+-rw-rw-r--   0 bart      (1000) bart      (1000)    10804 2021-11-25 15:03:33.000000 netqasm-0.9.1/docs/build/doctrees/api_sdk/netqasm.sdk.progress_bar.doctree
+-rw-rw-r--   0 bart      (1000) bart      (1000)   167266 2021-11-26 13:17:06.000000 netqasm-0.9.1/docs/build/doctrees/api_sdk/netqasm.sdk.qubit.doctree
+-rw-rw-r--   0 bart      (1000) bart      (1000)    64515 2021-11-25 15:03:34.000000 netqasm-0.9.1/docs/build/doctrees/api_sdk/netqasm.sdk.shared_memory.doctree
+-rw-rw-r--   0 bart      (1000) bart      (1000)    62171 2021-11-26 13:17:06.000000 netqasm-0.9.1/docs/build/doctrees/api_sdk/netqasm.sdk.toolbox.doctree
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:26.913100 netqasm-0.9.1/docs/build/doctrees/api_util/
+-rw-rw-r--   0 bart      (1000) bart      (1000)    26943 2021-11-25 15:03:34.000000 netqasm-0.9.1/docs/build/doctrees/api_util/netqasm.util.error.doctree
+-rw-rw-r--   0 bart      (1000) bart      (1000)    10895 2021-11-25 15:03:34.000000 netqasm-0.9.1/docs/build/doctrees/api_util/netqasm.util.log.doctree
+-rw-rw-r--   0 bart      (1000) bart      (1000)    10783 2021-11-25 15:03:34.000000 netqasm-0.9.1/docs/build/doctrees/api_util/netqasm.util.quantum_gates.doctree
+-rw-rw-r--   0 bart      (1000) bart      (1000)     6777 2021-11-25 15:03:34.000000 netqasm-0.9.1/docs/build/doctrees/api_util/netqasm.util.states.doctree
+-rw-rw-r--   0 bart      (1000) bart      (1000)    12193 2021-11-25 15:03:34.000000 netqasm-0.9.1/docs/build/doctrees/api_util/netqasm.util.string.doctree
+-rw-rw-r--   0 bart      (1000) bart      (1000)     4896 2021-11-25 15:03:34.000000 netqasm-0.9.1/docs/build/doctrees/api_util/netqasm.util.thread.doctree
+-rw-rw-r--   0 bart      (1000) bart      (1000)     5239 2021-11-25 15:03:34.000000 netqasm-0.9.1/docs/build/doctrees/api_util/netqasm.util.yaml.doctree
+-rw-rw-r--   0 bart      (1000) bart      (1000)   366848 2021-11-26 13:17:14.000000 netqasm-0.9.1/docs/build/doctrees/environment.pickle
+-rw-rw-r--   0 bart      (1000) bart      (1000)     3929 2021-11-26 13:17:06.000000 netqasm-0.9.1/docs/build/doctrees/index.doctree
+-rw-rw-r--   0 bart      (1000) bart      (1000)    11959 2021-11-26 13:17:06.000000 netqasm-0.9.1/docs/build/doctrees/installation.doctree
+-rw-rw-r--   0 bart      (1000) bart      (1000)     3593 2021-11-26 13:17:06.000000 netqasm-0.9.1/docs/build/doctrees/known_issues.doctree
+-rw-rw-r--   0 bart      (1000) bart      (1000)     2842 2021-11-25 15:03:34.000000 netqasm-0.9.1/docs/build/doctrees/netqasm.backend.doctree
+-rw-rw-r--   0 bart      (1000) bart      (1000)     4180 2021-11-26 13:17:14.000000 netqasm-0.9.1/docs/build/doctrees/netqasm.examples.doctree
+-rw-rw-r--   0 bart      (1000) bart      (1000)     2897 2021-11-25 15:03:34.000000 netqasm-0.9.1/docs/build/doctrees/netqasm.lang.doctree
+-rw-rw-r--   0 bart      (1000) bart      (1000)     2744 2021-11-25 15:03:34.000000 netqasm-0.9.1/docs/build/doctrees/netqasm.logging.doctree
+-rw-rw-r--   0 bart      (1000) bart      (1000)     3055 2021-11-25 15:03:34.000000 netqasm-0.9.1/docs/build/doctrees/netqasm.runtime.doctree
+-rw-rw-r--   0 bart      (1000) bart      (1000)     3122 2021-11-25 15:03:34.000000 netqasm-0.9.1/docs/build/doctrees/netqasm.sdk.doctree
+-rw-rw-r--   0 bart      (1000) bart      (1000)     2894 2021-11-25 15:03:34.000000 netqasm-0.9.1/docs/build/doctrees/netqasm.util.doctree
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:26.921100 netqasm-0.9.1/docs/build/doctrees/quickstart/
+-rw-rw-r--   0 bart      (1000) bart      (1000)    37590 2021-11-26 13:17:06.000000 netqasm-0.9.1/docs/build/doctrees/quickstart/file_structure.doctree
+-rw-rw-r--   0 bart      (1000) bart      (1000)    24910 2021-11-26 13:17:06.000000 netqasm-0.9.1/docs/build/doctrees/quickstart/first-app.doctree
+-rw-rw-r--   0 bart      (1000) bart      (1000)   503162 2021-11-26 13:17:07.000000 netqasm-0.9.1/docs/build/doctrees/quickstart/modules.doctree
+-rw-rw-r--   0 bart      (1000) bart      (1000)    71705 2021-11-26 13:17:07.000000 netqasm-0.9.1/docs/build/doctrees/quickstart/using-sdk.doctree
+-rw-rw-r--   0 bart      (1000) bart      (1000)     5490 2021-11-26 13:17:06.000000 netqasm-0.9.1/docs/build/doctrees/quickstart.doctree
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:26.937100 netqasm-0.9.1/docs/build/html/
+-rw-rw-r--   0 bart      (1000) bart      (1000)      230 2021-11-26 13:17:15.000000 netqasm-0.9.1/docs/build/html/.buildinfo
+-rw-rw-r--   0 bart      (1000) bart      (1000)        0 2021-11-26 13:17:14.000000 netqasm-0.9.1/docs/build/html/.nojekyll
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:26.949100 netqasm-0.9.1/docs/build/html/_sources/
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:26.953100 netqasm-0.9.1/docs/build/html/_sources/api_backend/
+-rw-rw-r--   0 bart      (1000) bart      (1000)      174 2021-11-09 12:09:06.000000 netqasm-0.9.1/docs/build/html/_sources/api_backend/netqasm.backend.executor.rst.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)      174 2021-11-09 12:09:06.000000 netqasm-0.9.1/docs/build/html/_sources/api_backend/netqasm.backend.messages.rst.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)      188 2021-11-09 12:09:06.000000 netqasm-0.9.1/docs/build/html/_sources/api_backend/netqasm.backend.network_stack.rst.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)      172 2021-11-09 12:09:06.000000 netqasm-0.9.1/docs/build/html/_sources/api_backend/netqasm.backend.qnodeos.rst.txt
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:26.961100 netqasm-0.9.1/docs/build/html/_sources/api_lang/
+-rw-rw-r--   0 bart      (1000) bart      (1000)      168 2021-11-09 12:09:06.000000 netqasm-0.9.1/docs/build/html/_sources/api_lang/netqasm.lang.encoding.rst.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)      816 2021-11-09 12:09:06.000000 netqasm-0.9.1/docs/build/html/_sources/api_lang/netqasm.lang.instr.rst.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)      156 2021-11-09 12:09:06.000000 netqasm-0.9.1/docs/build/html/_sources/api_lang/netqasm.lang.ir.rst.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)      166 2021-11-09 12:09:06.000000 netqasm-0.9.1/docs/build/html/_sources/api_lang/netqasm.lang.operand.rst.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)      366 2021-11-09 12:09:06.000000 netqasm-0.9.1/docs/build/html/_sources/api_lang/netqasm.lang.parsing.rst.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)      172 2021-11-09 12:09:06.000000 netqasm-0.9.1/docs/build/html/_sources/api_lang/netqasm.lang.subroutine.rst.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)      166 2021-11-09 12:09:06.000000 netqasm-0.9.1/docs/build/html/_sources/api_lang/netqasm.lang.symbols.rst.txt
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:26.961100 netqasm-0.9.1/docs/build/html/_sources/api_logging/
+-rw-rw-r--   0 bart      (1000) bart      (1000)      170 2021-11-09 12:09:06.000000 netqasm-0.9.1/docs/build/html/_sources/api_logging/netqasm.logging.glob.rst.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)      166 2021-11-09 12:09:06.000000 netqasm-0.9.1/docs/build/html/_sources/api_logging/netqasm.logging.output.rst.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)      176 2021-11-09 15:38:36.000000 netqasm-0.9.1/docs/build/html/_sources/api_root.rst.txt
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:26.981101 netqasm-0.9.1/docs/build/html/_sources/api_runtime/
+-rw-rw-r--   0 bart      (1000) bart      (1000)      179 2021-11-09 15:39:26.000000 netqasm-0.9.1/docs/build/html/_sources/api_runtime/netqasm.runtime.app_config.rst.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)      182 2021-11-09 15:39:31.000000 netqasm-0.9.1/docs/build/html/_sources/api_runtime/netqasm.runtime.application.rst.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)      164 2021-11-09 12:09:06.000000 netqasm-0.9.1/docs/build/html/_sources/api_runtime/netqasm.runtime.cli.rst.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)      168 2021-11-09 12:09:06.000000 netqasm-0.9.1/docs/build/html/_sources/api_runtime/netqasm.runtime.debug.rst.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)      164 2021-11-09 12:09:06.000000 netqasm-0.9.1/docs/build/html/_sources/api_runtime/netqasm.runtime.env.rst.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)      174 2021-11-09 12:09:06.000000 netqasm-0.9.1/docs/build/html/_sources/api_runtime/netqasm.runtime.hardware.rst.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)      593 2021-11-09 15:41:50.000000 netqasm-0.9.1/docs/build/html/_sources/api_runtime/netqasm.runtime.interface.rst.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)      185 2021-11-09 15:39:35.000000 netqasm-0.9.1/docs/build/html/_sources/api_runtime/netqasm.runtime.process_logs.rst.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)      174 2021-11-09 12:09:06.000000 netqasm-0.9.1/docs/build/html/_sources/api_runtime/netqasm.runtime.settings.rst.txt
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:27.001101 netqasm-0.9.1/docs/build/html/_sources/api_sdk/
+-rw-rw-r--   0 bart      (1000) bart      (1000)      164 2021-11-09 12:09:06.000000 netqasm-0.9.1/docs/build/html/_sources/api_sdk/netqasm.sdk.builder.rst.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)     1493 2021-11-09 15:40:16.000000 netqasm-0.9.1/docs/build/html/_sources/api_sdk/netqasm.sdk.classical_communication.rst.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)      168 2021-11-09 12:09:06.000000 netqasm-0.9.1/docs/build/html/_sources/api_sdk/netqasm.sdk.compiling.rst.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)      162 2021-11-09 12:09:06.000000 netqasm-0.9.1/docs/build/html/_sources/api_sdk/netqasm.sdk.config.rst.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)      170 2021-11-09 12:09:06.000000 netqasm-0.9.1/docs/build/html/_sources/api_sdk/netqasm.sdk.connection.rst.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)      170 2021-11-09 12:09:06.000000 netqasm-0.9.1/docs/build/html/_sources/api_sdk/netqasm.sdk.epr_socket.rst.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)      166 2021-11-09 12:09:06.000000 netqasm-0.9.1/docs/build/html/_sources/api_sdk/netqasm.sdk.external.rst.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)      164 2021-11-09 12:09:06.000000 netqasm-0.9.1/docs/build/html/_sources/api_sdk/netqasm.sdk.futures.rst.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)      164 2021-11-09 12:09:06.000000 netqasm-0.9.1/docs/build/html/_sources/api_sdk/netqasm.sdk.network.rst.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)      174 2021-11-09 12:09:06.000000 netqasm-0.9.1/docs/build/html/_sources/api_sdk/netqasm.sdk.progress_bar.rst.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)      160 2021-11-09 12:09:06.000000 netqasm-0.9.1/docs/build/html/_sources/api_sdk/netqasm.sdk.qubit.rst.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)      176 2021-11-09 12:09:06.000000 netqasm-0.9.1/docs/build/html/_sources/api_sdk/netqasm.sdk.shared_memory.rst.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)      994 2021-11-09 12:09:06.000000 netqasm-0.9.1/docs/build/html/_sources/api_sdk/netqasm.sdk.toolbox.rst.txt
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:27.013101 netqasm-0.9.1/docs/build/html/_sources/api_util/
+-rw-rw-r--   0 bart      (1000) bart      (1000)      162 2021-11-09 12:09:06.000000 netqasm-0.9.1/docs/build/html/_sources/api_util/netqasm.util.error.rst.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)      158 2021-11-09 12:09:06.000000 netqasm-0.9.1/docs/build/html/_sources/api_util/netqasm.util.log.rst.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)      179 2021-11-09 12:09:06.000000 netqasm-0.9.1/docs/build/html/_sources/api_util/netqasm.util.quantum_gates.rst.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)      164 2021-11-09 12:09:06.000000 netqasm-0.9.1/docs/build/html/_sources/api_util/netqasm.util.states.rst.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)      164 2021-11-09 12:09:06.000000 netqasm-0.9.1/docs/build/html/_sources/api_util/netqasm.util.string.rst.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)      164 2021-11-09 12:09:06.000000 netqasm-0.9.1/docs/build/html/_sources/api_util/netqasm.util.thread.rst.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)      160 2021-11-09 12:09:06.000000 netqasm-0.9.1/docs/build/html/_sources/api_util/netqasm.util.yaml.rst.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)      606 2021-11-26 13:15:04.000000 netqasm-0.9.1/docs/build/html/_sources/index.rst.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)     1591 2021-11-25 15:27:32.000000 netqasm-0.9.1/docs/build/html/_sources/installation.rst.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)      356 2021-11-26 13:16:56.000000 netqasm-0.9.1/docs/build/html/_sources/known_issues.rst.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)      249 2021-11-09 12:09:06.000000 netqasm-0.9.1/docs/build/html/_sources/netqasm.backend.rst.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)      255 2021-11-09 12:09:06.000000 netqasm-0.9.1/docs/build/html/_sources/netqasm.examples.rst.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)      310 2021-11-09 12:09:06.000000 netqasm-0.9.1/docs/build/html/_sources/netqasm.lang.rst.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)      159 2021-11-09 12:09:06.000000 netqasm-0.9.1/docs/build/html/_sources/netqasm.logging.rst.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)      442 2021-11-09 12:09:06.000000 netqasm-0.9.1/docs/build/html/_sources/netqasm.runtime.rst.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)      517 2021-11-09 12:09:06.000000 netqasm-0.9.1/docs/build/html/_sources/netqasm.sdk.rst.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)      307 2021-11-09 12:09:06.000000 netqasm-0.9.1/docs/build/html/_sources/netqasm.util.rst.txt
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:27.021101 netqasm-0.9.1/docs/build/html/_sources/quickstart/
+-rw-rw-r--   0 bart      (1000) bart      (1000)     6364 2021-11-26 13:12:18.000000 netqasm-0.9.1/docs/build/html/_sources/quickstart/file_structure.rst.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)     4854 2021-11-25 15:31:56.000000 netqasm-0.9.1/docs/build/html/_sources/quickstart/first-app.rst.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)     2996 2021-11-09 12:09:06.000000 netqasm-0.9.1/docs/build/html/_sources/quickstart/modules.rst.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)    19303 2021-11-26 13:15:49.000000 netqasm-0.9.1/docs/build/html/_sources/quickstart/using-sdk.rst.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)      677 2021-11-25 14:54:59.000000 netqasm-0.9.1/docs/build/html/_sources/quickstart.rst.txt
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:27.053101 netqasm-0.9.1/docs/build/html/_static/
+-rw-rw-r--   0 bart      (1000) bart      (1000)    13877 2021-11-26 13:17:15.000000 netqasm-0.9.1/docs/build/html/_static/basic.css
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:27.053101 netqasm-0.9.1/docs/build/html/_static/css/
+-rw-rw-r--   0 bart      (1000) bart      (1000)     3275 2021-04-07 12:13:34.000000 netqasm-0.9.1/docs/build/html/_static/css/badge_only.css
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:27.141102 netqasm-0.9.1/docs/build/html/_static/css/fonts/
+-rw-rw-r--   0 bart      (1000) bart      (1000)    87624 2021-04-07 12:13:34.000000 netqasm-0.9.1/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff
+-rw-rw-r--   0 bart      (1000) bart      (1000)    67312 2021-04-07 12:13:34.000000 netqasm-0.9.1/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-rw-r--   0 bart      (1000) bart      (1000)    86288 2021-04-07 12:13:34.000000 netqasm-0.9.1/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff
+-rw-rw-r--   0 bart      (1000) bart      (1000)    66444 2021-04-07 12:13:34.000000 netqasm-0.9.1/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-rw-r--   0 bart      (1000) bart      (1000)   165742 2021-04-07 12:13:34.000000 netqasm-0.9.1/docs/build/html/_static/css/fonts/fontawesome-webfont.eot
+-rw-rw-r--   0 bart      (1000) bart      (1000)   444379 2021-04-07 12:13:34.000000 netqasm-0.9.1/docs/build/html/_static/css/fonts/fontawesome-webfont.svg
+-rw-rw-r--   0 bart      (1000) bart      (1000)   165548 2021-04-07 12:13:34.000000 netqasm-0.9.1/docs/build/html/_static/css/fonts/fontawesome-webfont.ttf
+-rw-rw-r--   0 bart      (1000) bart      (1000)    98024 2021-04-07 12:13:34.000000 netqasm-0.9.1/docs/build/html/_static/css/fonts/fontawesome-webfont.woff
+-rw-rw-r--   0 bart      (1000) bart      (1000)    77160 2021-04-07 12:13:34.000000 netqasm-0.9.1/docs/build/html/_static/css/fonts/fontawesome-webfont.woff2
+-rw-rw-r--   0 bart      (1000) bart      (1000)   323344 2021-04-07 12:13:34.000000 netqasm-0.9.1/docs/build/html/_static/css/fonts/lato-bold-italic.woff
+-rw-rw-r--   0 bart      (1000) bart      (1000)   193308 2021-04-07 12:13:34.000000 netqasm-0.9.1/docs/build/html/_static/css/fonts/lato-bold-italic.woff2
+-rw-rw-r--   0 bart      (1000) bart      (1000)   309728 2021-04-07 12:13:34.000000 netqasm-0.9.1/docs/build/html/_static/css/fonts/lato-bold.woff
+-rw-rw-r--   0 bart      (1000) bart      (1000)   184912 2021-04-07 12:13:34.000000 netqasm-0.9.1/docs/build/html/_static/css/fonts/lato-bold.woff2
+-rw-rw-r--   0 bart      (1000) bart      (1000)   328412 2021-04-07 12:13:34.000000 netqasm-0.9.1/docs/build/html/_static/css/fonts/lato-normal-italic.woff
+-rw-rw-r--   0 bart      (1000) bart      (1000)   195704 2021-04-07 12:13:34.000000 netqasm-0.9.1/docs/build/html/_static/css/fonts/lato-normal-italic.woff2
+-rw-rw-r--   0 bart      (1000) bart      (1000)   309192 2021-04-07 12:13:34.000000 netqasm-0.9.1/docs/build/html/_static/css/fonts/lato-normal.woff
+-rw-rw-r--   0 bart      (1000) bart      (1000)   182708 2021-04-07 12:13:34.000000 netqasm-0.9.1/docs/build/html/_static/css/fonts/lato-normal.woff2
+-rw-rw-r--   0 bart      (1000) bart      (1000)   123687 2021-04-07 12:13:34.000000 netqasm-0.9.1/docs/build/html/_static/css/theme.css
+-rw-rw-r--   0 bart      (1000) bart      (1000)     9592 2021-11-09 15:36:03.000000 netqasm-0.9.1/docs/build/html/_static/doctools.js
+-rw-rw-r--   0 bart      (1000) bart      (1000)      355 2021-11-26 13:17:15.000000 netqasm-0.9.1/docs/build/html/_static/documentation_options.js
+-rw-rw-r--   0 bart      (1000) bart      (1000)      286 2021-11-09 15:36:03.000000 netqasm-0.9.1/docs/build/html/_static/file.png
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:27.181102 netqasm-0.9.1/docs/build/html/_static/fonts/
+-rw-rw-r--   0 bart      (1000) bart      (1000)   109948 2021-04-07 12:13:34.000000 netqasm-0.9.1/docs/build/html/_static/fonts/Inconsolata-Bold.ttf
+-rw-rw-r--   0 bart      (1000) bart      (1000)    96964 2021-04-07 12:13:34.000000 netqasm-0.9.1/docs/build/html/_static/fonts/Inconsolata-Regular.ttf
+-rw-rw-r--   0 bart      (1000) bart      (1000)    63184 2021-04-07 12:13:34.000000 netqasm-0.9.1/docs/build/html/_static/fonts/Inconsolata.ttf
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:27.233102 netqasm-0.9.1/docs/build/html/_static/fonts/Lato/
+-rw-rw-r--   0 bart      (1000) bart      (1000)   256056 2021-04-07 12:13:34.000000 netqasm-0.9.1/docs/build/html/_static/fonts/Lato/lato-bold.eot
+-rw-rw-r--   0 bart      (1000) bart      (1000)   600856 2021-04-07 12:13:34.000000 netqasm-0.9.1/docs/build/html/_static/fonts/Lato/lato-bold.ttf
+-rw-rw-r--   0 bart      (1000) bart      (1000)   309728 2021-04-07 12:13:34.000000 netqasm-0.9.1/docs/build/html/_static/fonts/Lato/lato-bold.woff
+-rw-rw-r--   0 bart      (1000) bart      (1000)   184912 2021-04-07 12:13:34.000000 netqasm-0.9.1/docs/build/html/_static/fonts/Lato/lato-bold.woff2
+-rw-rw-r--   0 bart      (1000) bart      (1000)   266158 2021-04-07 12:13:34.000000 netqasm-0.9.1/docs/build/html/_static/fonts/Lato/lato-bolditalic.eot
+-rw-rw-r--   0 bart      (1000) bart      (1000)   622572 2021-04-07 12:13:34.000000 netqasm-0.9.1/docs/build/html/_static/fonts/Lato/lato-bolditalic.ttf
+-rw-rw-r--   0 bart      (1000) bart      (1000)   323344 2021-04-07 12:13:34.000000 netqasm-0.9.1/docs/build/html/_static/fonts/Lato/lato-bolditalic.woff
+-rw-rw-r--   0 bart      (1000) bart      (1000)   193308 2021-04-07 12:13:34.000000 netqasm-0.9.1/docs/build/html/_static/fonts/Lato/lato-bolditalic.woff2
+-rw-rw-r--   0 bart      (1000) bart      (1000)   268604 2021-04-07 12:13:34.000000 netqasm-0.9.1/docs/build/html/_static/fonts/Lato/lato-italic.eot
+-rw-rw-r--   0 bart      (1000) bart      (1000)   639388 2021-04-07 12:13:34.000000 netqasm-0.9.1/docs/build/html/_static/fonts/Lato/lato-italic.ttf
+-rw-rw-r--   0 bart      (1000) bart      (1000)   328412 2021-04-07 12:13:34.000000 netqasm-0.9.1/docs/build/html/_static/fonts/Lato/lato-italic.woff
+-rw-rw-r--   0 bart      (1000) bart      (1000)   195704 2021-04-07 12:13:34.000000 netqasm-0.9.1/docs/build/html/_static/fonts/Lato/lato-italic.woff2
+-rw-rw-r--   0 bart      (1000) bart      (1000)   253461 2021-04-07 12:13:34.000000 netqasm-0.9.1/docs/build/html/_static/fonts/Lato/lato-regular.eot
+-rw-rw-r--   0 bart      (1000) bart      (1000)   607720 2021-04-07 12:13:34.000000 netqasm-0.9.1/docs/build/html/_static/fonts/Lato/lato-regular.ttf
+-rw-rw-r--   0 bart      (1000) bart      (1000)   309192 2021-04-07 12:13:34.000000 netqasm-0.9.1/docs/build/html/_static/fonts/Lato/lato-regular.woff
+-rw-rw-r--   0 bart      (1000) bart      (1000)   182708 2021-04-07 12:13:34.000000 netqasm-0.9.1/docs/build/html/_static/fonts/Lato/lato-regular.woff2
+-rw-rw-r--   0 bart      (1000) bart      (1000)   656544 2021-04-07 12:13:34.000000 netqasm-0.9.1/docs/build/html/_static/fonts/Lato-Bold.ttf
+-rw-rw-r--   0 bart      (1000) bart      (1000)   656568 2021-04-07 12:13:34.000000 netqasm-0.9.1/docs/build/html/_static/fonts/Lato-Regular.ttf
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:27.249102 netqasm-0.9.1/docs/build/html/_static/fonts/RobotoSlab/
+-rw-rw-r--   0 bart      (1000) bart      (1000)    79520 2021-04-07 12:13:34.000000 netqasm-0.9.1/docs/build/html/_static/fonts/RobotoSlab/roboto-slab-v7-bold.eot
+-rw-rw-r--   0 bart      (1000) bart      (1000)   170616 2021-04-07 12:13:34.000000 netqasm-0.9.1/docs/build/html/_static/fonts/RobotoSlab/roboto-slab-v7-bold.ttf
+-rw-rw-r--   0 bart      (1000) bart      (1000)    87624 2021-04-07 12:13:34.000000 netqasm-0.9.1/docs/build/html/_static/fonts/RobotoSlab/roboto-slab-v7-bold.woff
+-rw-rw-r--   0 bart      (1000) bart      (1000)    67312 2021-04-07 12:13:34.000000 netqasm-0.9.1/docs/build/html/_static/fonts/RobotoSlab/roboto-slab-v7-bold.woff2
+-rw-rw-r--   0 bart      (1000) bart      (1000)    78331 2021-04-07 12:13:34.000000 netqasm-0.9.1/docs/build/html/_static/fonts/RobotoSlab/roboto-slab-v7-regular.eot
+-rw-rw-r--   0 bart      (1000) bart      (1000)   169064 2021-04-07 12:13:34.000000 netqasm-0.9.1/docs/build/html/_static/fonts/RobotoSlab/roboto-slab-v7-regular.ttf
+-rw-rw-r--   0 bart      (1000) bart      (1000)    86288 2021-04-07 12:13:34.000000 netqasm-0.9.1/docs/build/html/_static/fonts/RobotoSlab/roboto-slab-v7-regular.woff
+-rw-rw-r--   0 bart      (1000) bart      (1000)    66444 2021-04-07 12:13:34.000000 netqasm-0.9.1/docs/build/html/_static/fonts/RobotoSlab/roboto-slab-v7-regular.woff2
+-rw-rw-r--   0 bart      (1000) bart      (1000)   170616 2021-04-07 12:13:34.000000 netqasm-0.9.1/docs/build/html/_static/fonts/RobotoSlab-Bold.ttf
+-rw-rw-r--   0 bart      (1000) bart      (1000)   169064 2021-04-07 12:13:34.000000 netqasm-0.9.1/docs/build/html/_static/fonts/RobotoSlab-Regular.ttf
+-rw-rw-r--   0 bart      (1000) bart      (1000)   165742 2021-04-07 12:13:34.000000 netqasm-0.9.1/docs/build/html/_static/fonts/fontawesome-webfont.eot
+-rw-rw-r--   0 bart      (1000) bart      (1000)   444379 2021-04-07 12:13:34.000000 netqasm-0.9.1/docs/build/html/_static/fonts/fontawesome-webfont.svg
+-rw-rw-r--   0 bart      (1000) bart      (1000)   165548 2021-04-07 12:13:34.000000 netqasm-0.9.1/docs/build/html/_static/fonts/fontawesome-webfont.ttf
+-rw-rw-r--   0 bart      (1000) bart      (1000)    98024 2021-04-07 12:13:34.000000 netqasm-0.9.1/docs/build/html/_static/fonts/fontawesome-webfont.woff
+-rw-rw-r--   0 bart      (1000) bart      (1000)    77160 2021-04-07 12:13:34.000000 netqasm-0.9.1/docs/build/html/_static/fonts/fontawesome-webfont.woff2
+-rw-rw-r--   0 bart      (1000) bart      (1000)   287630 2021-11-09 15:36:03.000000 netqasm-0.9.1/docs/build/html/_static/jquery-3.5.1.js
+-rw-rw-r--   0 bart      (1000) bart      (1000)    89476 2021-11-09 15:36:03.000000 netqasm-0.9.1/docs/build/html/_static/jquery.js
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:27.257102 netqasm-0.9.1/docs/build/html/_static/js/
+-rw-rw-r--   0 bart      (1000) bart      (1000)      934 2021-04-07 12:13:34.000000 netqasm-0.9.1/docs/build/html/_static/js/badge_only.js
+-rw-rw-r--   0 bart      (1000) bart      (1000)     4370 2021-04-07 12:13:34.000000 netqasm-0.9.1/docs/build/html/_static/js/html5shiv-printshiv.min.js
+-rw-rw-r--   0 bart      (1000) bart      (1000)     2734 2021-04-07 12:13:34.000000 netqasm-0.9.1/docs/build/html/_static/js/html5shiv.min.js
+-rw-rw-r--   0 bart      (1000) bart      (1000)    15414 2021-04-07 12:13:34.000000 netqasm-0.9.1/docs/build/html/_static/js/modernizr.min.js
+-rw-rw-r--   0 bart      (1000) bart      (1000)     4916 2021-04-07 12:13:34.000000 netqasm-0.9.1/docs/build/html/_static/js/theme.js
+-rw-rw-r--   0 bart      (1000) bart      (1000)    10854 2021-11-26 13:17:15.000000 netqasm-0.9.1/docs/build/html/_static/language_data.js
+-rw-rw-r--   0 bart      (1000) bart      (1000)       90 2021-11-09 15:36:03.000000 netqasm-0.9.1/docs/build/html/_static/minus.png
+-rw-rw-r--   0 bart      (1000) bart      (1000)       90 2021-11-09 15:36:03.000000 netqasm-0.9.1/docs/build/html/_static/plus.png
+-rw-rw-r--   0 bart      (1000) bart      (1000)     4368 2021-11-26 13:17:15.000000 netqasm-0.9.1/docs/build/html/_static/pygments.css
+-rw-rw-r--   0 bart      (1000) bart      (1000)    16582 2021-11-09 15:36:03.000000 netqasm-0.9.1/docs/build/html/_static/searchtools.js
+-rw-rw-r--   0 bart      (1000) bart      (1000)    67692 2021-11-09 15:36:03.000000 netqasm-0.9.1/docs/build/html/_static/underscore-1.12.0.js
+-rw-rw-r--   0 bart      (1000) bart      (1000)    19358 2021-11-09 15:36:03.000000 netqasm-0.9.1/docs/build/html/_static/underscore.js
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:27.261102 netqasm-0.9.1/docs/build/html/api_backend/
+-rw-rw-r--   0 bart      (1000) bart      (1000)    30383 2021-11-25 15:03:36.000000 netqasm-0.9.1/docs/build/html/api_backend/netqasm.backend.executor.html
+-rw-rw-r--   0 bart      (1000) bart      (1000)    54015 2021-11-25 15:03:36.000000 netqasm-0.9.1/docs/build/html/api_backend/netqasm.backend.messages.html
+-rw-rw-r--   0 bart      (1000) bart      (1000)    14197 2021-11-25 15:03:36.000000 netqasm-0.9.1/docs/build/html/api_backend/netqasm.backend.network_stack.html
+-rw-rw-r--   0 bart      (1000) bart      (1000)    16641 2021-11-25 15:03:36.000000 netqasm-0.9.1/docs/build/html/api_backend/netqasm.backend.qnodeos.html
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:27.277103 netqasm-0.9.1/docs/build/html/api_lang/
+-rw-rw-r--   0 bart      (1000) bart      (1000)    68663 2021-11-25 15:03:36.000000 netqasm-0.9.1/docs/build/html/api_lang/netqasm.lang.encoding.html
+-rw-rw-r--   0 bart      (1000) bart      (1000)   465784 2021-11-25 15:03:37.000000 netqasm-0.9.1/docs/build/html/api_lang/netqasm.lang.instr.html
+-rw-rw-r--   0 bart      (1000) bart      (1000)    40953 2021-11-25 15:03:37.000000 netqasm-0.9.1/docs/build/html/api_lang/netqasm.lang.ir.html
+-rw-rw-r--   0 bart      (1000) bart      (1000)    26633 2021-11-25 15:03:37.000000 netqasm-0.9.1/docs/build/html/api_lang/netqasm.lang.operand.html
+-rw-rw-r--   0 bart      (1000) bart      (1000)    25406 2021-11-25 15:03:37.000000 netqasm-0.9.1/docs/build/html/api_lang/netqasm.lang.parsing.html
+-rw-rw-r--   0 bart      (1000) bart      (1000)    12733 2021-11-25 15:03:37.000000 netqasm-0.9.1/docs/build/html/api_lang/netqasm.lang.subroutine.html
+-rw-rw-r--   0 bart      (1000) bart      (1000)    13385 2021-11-25 15:03:37.000000 netqasm-0.9.1/docs/build/html/api_lang/netqasm.lang.symbols.html
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:27.277103 netqasm-0.9.1/docs/build/html/api_logging/
+-rw-rw-r--   0 bart      (1000) bart      (1000)    19497 2021-11-25 15:03:37.000000 netqasm-0.9.1/docs/build/html/api_logging/netqasm.logging.glob.html
+-rw-rw-r--   0 bart      (1000) bart      (1000)     9623 2021-11-25 15:03:37.000000 netqasm-0.9.1/docs/build/html/api_logging/netqasm.logging.output.html
+-rw-rw-r--   0 bart      (1000) bart      (1000)    15793 2021-11-25 15:03:37.000000 netqasm-0.9.1/docs/build/html/api_root.html
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:27.285102 netqasm-0.9.1/docs/build/html/api_runtime/
+-rw-rw-r--   0 bart      (1000) bart      (1000)    13847 2021-11-25 15:03:37.000000 netqasm-0.9.1/docs/build/html/api_runtime/netqasm.runtime.app_config.html
+-rw-rw-r--   0 bart      (1000) bart      (1000)    34669 2021-11-25 15:03:37.000000 netqasm-0.9.1/docs/build/html/api_runtime/netqasm.runtime.application.html
+-rw-rw-r--   0 bart      (1000) bart      (1000)     7965 2021-11-25 15:03:37.000000 netqasm-0.9.1/docs/build/html/api_runtime/netqasm.runtime.cli.html
+-rw-rw-r--   0 bart      (1000) bart      (1000)    10206 2021-11-25 15:03:38.000000 netqasm-0.9.1/docs/build/html/api_runtime/netqasm.runtime.debug.html
+-rw-rw-r--   0 bart      (1000) bart      (1000)    16787 2021-11-25 15:03:38.000000 netqasm-0.9.1/docs/build/html/api_runtime/netqasm.runtime.env.html
+-rw-rw-r--   0 bart      (1000) bart      (1000)    10348 2021-11-25 15:03:38.000000 netqasm-0.9.1/docs/build/html/api_runtime/netqasm.runtime.hardware.html
+-rw-rw-r--   0 bart      (1000) bart      (1000)    74476 2021-11-25 15:03:38.000000 netqasm-0.9.1/docs/build/html/api_runtime/netqasm.runtime.interface.html
+-rw-rw-r--   0 bart      (1000) bart      (1000)     9048 2021-11-26 13:17:07.000000 netqasm-0.9.1/docs/build/html/api_runtime/netqasm.runtime.process_logs.html
+-rw-rw-r--   0 bart      (1000) bart      (1000)    15215 2021-11-25 15:03:38.000000 netqasm-0.9.1/docs/build/html/api_runtime/netqasm.runtime.settings.html
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:27.301102 netqasm-0.9.1/docs/build/html/api_sdk/
+-rw-rw-r--   0 bart      (1000) bart      (1000)    71598 2021-11-26 13:17:07.000000 netqasm-0.9.1/docs/build/html/api_sdk/netqasm.sdk.builder.html
+-rw-rw-r--   0 bart      (1000) bart      (1000)    78245 2021-11-25 15:03:38.000000 netqasm-0.9.1/docs/build/html/api_sdk/netqasm.sdk.classical_communication.html
+-rw-rw-r--   0 bart      (1000) bart      (1000)    21092 2021-11-25 15:03:38.000000 netqasm-0.9.1/docs/build/html/api_sdk/netqasm.sdk.compiling.html
+-rw-rw-r--   0 bart      (1000) bart      (1000)    17467 2021-11-25 15:03:38.000000 netqasm-0.9.1/docs/build/html/api_sdk/netqasm.sdk.config.html
+-rw-rw-r--   0 bart      (1000) bart      (1000)   117484 2021-11-26 13:17:08.000000 netqasm-0.9.1/docs/build/html/api_sdk/netqasm.sdk.connection.html
+-rw-rw-r--   0 bart      (1000) bart      (1000)    44288 2021-11-26 13:17:08.000000 netqasm-0.9.1/docs/build/html/api_sdk/netqasm.sdk.epr_socket.html
+-rw-rw-r--   0 bart      (1000) bart      (1000)    10889 2021-11-26 13:17:08.000000 netqasm-0.9.1/docs/build/html/api_sdk/netqasm.sdk.external.html
+-rw-rw-r--   0 bart      (1000) bart      (1000)    87852 2021-11-26 13:17:08.000000 netqasm-0.9.1/docs/build/html/api_sdk/netqasm.sdk.futures.html
+-rw-rw-r--   0 bart      (1000) bart      (1000)    12813 2021-11-25 15:03:39.000000 netqasm-0.9.1/docs/build/html/api_sdk/netqasm.sdk.network.html
+-rw-rw-r--   0 bart      (1000) bart      (1000)    12378 2021-11-25 15:03:39.000000 netqasm-0.9.1/docs/build/html/api_sdk/netqasm.sdk.progress_bar.html
+-rw-rw-r--   0 bart      (1000) bart      (1000)    60622 2021-11-26 13:17:08.000000 netqasm-0.9.1/docs/build/html/api_sdk/netqasm.sdk.qubit.html
+-rw-rw-r--   0 bart      (1000) bart      (1000)    29496 2021-11-25 15:03:39.000000 netqasm-0.9.1/docs/build/html/api_sdk/netqasm.sdk.shared_memory.html
+-rw-rw-r--   0 bart      (1000) bart      (1000)    28186 2021-11-26 13:17:08.000000 netqasm-0.9.1/docs/build/html/api_sdk/netqasm.sdk.toolbox.html
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:27.305103 netqasm-0.9.1/docs/build/html/api_util/
+-rw-rw-r--   0 bart      (1000) bart      (1000)    15286 2021-11-25 15:03:39.000000 netqasm-0.9.1/docs/build/html/api_util/netqasm.util.error.html
+-rw-rw-r--   0 bart      (1000) bart      (1000)     9833 2021-11-25 15:03:39.000000 netqasm-0.9.1/docs/build/html/api_util/netqasm.util.log.html
+-rw-rw-r--   0 bart      (1000) bart      (1000)     9918 2021-11-25 15:03:39.000000 netqasm-0.9.1/docs/build/html/api_util/netqasm.util.quantum_gates.html
+-rw-rw-r--   0 bart      (1000) bart      (1000)     7859 2021-11-25 15:03:39.000000 netqasm-0.9.1/docs/build/html/api_util/netqasm.util.states.html
+-rw-rw-r--   0 bart      (1000) bart      (1000)    10553 2021-11-25 15:03:39.000000 netqasm-0.9.1/docs/build/html/api_util/netqasm.util.string.html
+-rw-rw-r--   0 bart      (1000) bart      (1000)     7744 2021-11-25 15:03:39.000000 netqasm-0.9.1/docs/build/html/api_util/netqasm.util.thread.html
+-rw-rw-r--   0 bart      (1000) bart      (1000)     7622 2021-11-25 15:03:40.000000 netqasm-0.9.1/docs/build/html/api_util/netqasm.util.yaml.html
+-rw-rw-r--   0 bart      (1000) bart      (1000)   256777 2021-11-26 13:17:15.000000 netqasm-0.9.1/docs/build/html/genindex.html
+-rw-rw-r--   0 bart      (1000) bart      (1000)     7038 2021-11-26 13:17:15.000000 netqasm-0.9.1/docs/build/html/index.html
+-rw-rw-r--   0 bart      (1000) bart      (1000)     8450 2021-11-26 13:17:08.000000 netqasm-0.9.1/docs/build/html/installation.html
+-rw-rw-r--   0 bart      (1000) bart      (1000)     5527 2021-11-26 13:17:08.000000 netqasm-0.9.1/docs/build/html/known_issues.html
+-rw-rw-r--   0 bart      (1000) bart      (1000)     7025 2021-11-25 15:03:40.000000 netqasm-0.9.1/docs/build/html/netqasm.backend.html
+-rw-rw-r--   0 bart      (1000) bart      (1000)     4582 2021-11-26 13:17:15.000000 netqasm-0.9.1/docs/build/html/netqasm.examples.html
+-rw-rw-r--   0 bart      (1000) bart      (1000)     9942 2021-11-25 15:03:40.000000 netqasm-0.9.1/docs/build/html/netqasm.lang.html
+-rw-rw-r--   0 bart      (1000) bart      (1000)     6481 2021-11-25 15:03:40.000000 netqasm-0.9.1/docs/build/html/netqasm.logging.html
+-rw-rw-r--   0 bart      (1000) bart      (1000)     9726 2021-11-26 13:17:08.000000 netqasm-0.9.1/docs/build/html/netqasm.runtime.html
+-rw-rw-r--   0 bart      (1000) bart      (1000)    13938 2021-11-26 13:17:08.000000 netqasm-0.9.1/docs/build/html/netqasm.sdk.html
+-rw-rw-r--   0 bart      (1000) bart      (1000)     7648 2021-11-25 15:03:40.000000 netqasm-0.9.1/docs/build/html/netqasm.util.html
+-rw-rw-r--   0 bart      (1000) bart      (1000)     9657 2021-11-26 13:17:15.000000 netqasm-0.9.1/docs/build/html/objects.inv
+-rw-rw-r--   0 bart      (1000) bart      (1000)    19451 2021-11-26 13:17:15.000000 netqasm-0.9.1/docs/build/html/py-modindex.html
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:27.305103 netqasm-0.9.1/docs/build/html/quickstart/
+-rw-rw-r--   0 bart      (1000) bart      (1000)    20367 2021-11-26 13:17:09.000000 netqasm-0.9.1/docs/build/html/quickstart/file_structure.html
+-rw-rw-r--   0 bart      (1000) bart      (1000)    15255 2021-11-26 13:17:09.000000 netqasm-0.9.1/docs/build/html/quickstart/first-app.html
+-rw-rw-r--   0 bart      (1000) bart      (1000)   158293 2021-11-26 13:17:09.000000 netqasm-0.9.1/docs/build/html/quickstart/modules.html
+-rw-rw-r--   0 bart      (1000) bart      (1000)    67594 2021-11-26 13:17:09.000000 netqasm-0.9.1/docs/build/html/quickstart/using-sdk.html
+-rw-rw-r--   0 bart      (1000) bart      (1000)     9774 2021-11-26 13:17:08.000000 netqasm-0.9.1/docs/build/html/quickstart.html
+-rw-rw-r--   0 bart      (1000) bart      (1000)     4770 2021-11-26 13:17:15.000000 netqasm-0.9.1/docs/build/html/search.html
+-rw-rw-r--   0 bart      (1000) bart      (1000)    79169 2021-11-26 13:17:15.000000 netqasm-0.9.1/docs/build/html/searchindex.js
+-rw-rw-r--   0 bart      (1000) bart      (1000)     2873 2022-04-07 14:51:03.000000 netqasm-0.9.1/docs/conf.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)      606 2022-03-28 08:45:06.000000 netqasm-0.9.1/docs/index.rst
+-rw-rw-r--   0 bart      (1000) bart      (1000)     1591 2022-03-28 08:45:06.000000 netqasm-0.9.1/docs/installation.rst
+-rw-rw-r--   0 bart      (1000) bart      (1000)      356 2022-03-28 08:45:06.000000 netqasm-0.9.1/docs/known_issues.rst
+-rw-rw-r--   0 bart      (1000) bart      (1000)      760 2020-05-04 09:19:07.000000 netqasm-0.9.1/docs/make.bat
+-rw-rw-r--   0 bart      (1000) bart      (1000)      249 2022-03-25 17:15:19.000000 netqasm-0.9.1/docs/netqasm.backend.rst
+-rw-rw-r--   0 bart      (1000) bart      (1000)      255 2022-03-25 17:15:19.000000 netqasm-0.9.1/docs/netqasm.examples.rst
+-rw-rw-r--   0 bart      (1000) bart      (1000)      310 2022-03-25 17:15:19.000000 netqasm-0.9.1/docs/netqasm.lang.rst
+-rw-rw-r--   0 bart      (1000) bart      (1000)      159 2022-03-25 17:15:19.000000 netqasm-0.9.1/docs/netqasm.logging.rst
+-rw-rw-r--   0 bart      (1000) bart      (1000)      442 2022-03-25 17:15:19.000000 netqasm-0.9.1/docs/netqasm.runtime.rst
+-rw-rw-r--   0 bart      (1000) bart      (1000)      517 2022-03-25 17:15:19.000000 netqasm-0.9.1/docs/netqasm.sdk.rst
+-rw-rw-r--   0 bart      (1000) bart      (1000)      307 2022-03-25 17:15:19.000000 netqasm-0.9.1/docs/netqasm.util.rst
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:27.313103 netqasm-0.9.1/docs/quickstart/
+-rw-rw-r--   0 bart      (1000) bart      (1000)     6364 2022-03-28 08:45:06.000000 netqasm-0.9.1/docs/quickstart/file_structure.rst
+-rw-rw-r--   0 bart      (1000) bart      (1000)     4854 2022-03-28 08:45:06.000000 netqasm-0.9.1/docs/quickstart/first-app.rst
+-rw-rw-r--   0 bart      (1000) bart      (1000)     2996 2022-03-25 17:15:19.000000 netqasm-0.9.1/docs/quickstart/modules.rst
+-rw-rw-r--   0 bart      (1000) bart      (1000)    19303 2022-03-28 08:45:06.000000 netqasm-0.9.1/docs/quickstart/using-sdk.rst
+-rw-rw-r--   0 bart      (1000) bart      (1000)      677 2022-03-28 08:45:06.000000 netqasm-0.9.1/docs/quickstart.rst
+-rw-rw-r--   0 bart      (1000) bart      (1000)       92 2022-03-25 17:15:19.000000 netqasm-0.9.1/docs/requirements.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)       87 2021-05-19 15:28:08.000000 netqasm-0.9.1/mypy.ini
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:27.317103 netqasm-0.9.1/netqasm/
+-rw-rw-r--   0 bart      (1000) bart      (1000)       99 2022-04-07 14:51:03.000000 netqasm-0.9.1/netqasm/__init__.py
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:27.325103 netqasm-0.9.1/netqasm/backend/
+-rw-rw-r--   0 bart      (1000) bart      (1000)        0 2021-05-19 15:28:08.000000 netqasm-0.9.1/netqasm/backend/__init__.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)    66890 2022-04-07 14:43:59.000000 netqasm-0.9.1/netqasm/backend/executor.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     9606 2022-03-25 17:15:19.000000 netqasm-0.9.1/netqasm/backend/messages.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     1561 2022-03-25 17:15:19.000000 netqasm-0.9.1/netqasm/backend/network_stack.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     6404 2022-03-28 08:45:06.000000 netqasm-0.9.1/netqasm/backend/qnodeos.py
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:27.325103 netqasm-0.9.1/netqasm/examples/
+-rw-rw-r--   0 bart      (1000) bart      (1000)        0 2021-05-19 15:28:08.000000 netqasm-0.9.1/netqasm/examples/__init__.py
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:27.325103 netqasm-0.9.1/netqasm/examples/apps/
+-rw-rw-r--   0 bart      (1000) bart      (1000)        0 2021-05-19 15:28:08.000000 netqasm-0.9.1/netqasm/examples/apps/__init__.py
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:27.329103 netqasm-0.9.1/netqasm/examples/apps/anonymous_transmission/
+-rw-rw-r--   0 bart      (1000) bart      (1000)      508 2021-05-19 15:28:08.000000 netqasm-0.9.1/netqasm/examples/apps/anonymous_transmission/README.md
+-rw-rw-r--   0 bart      (1000) bart      (1000)        0 2021-05-19 15:28:08.000000 netqasm-0.9.1/netqasm/examples/apps/anonymous_transmission/__init__.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)       49 2021-05-19 15:28:08.000000 netqasm-0.9.1/netqasm/examples/apps/anonymous_transmission/alice.yaml
+-rw-rw-r--   0 bart      (1000) bart      (1000)      377 2022-03-25 17:15:19.000000 netqasm-0.9.1/netqasm/examples/apps/anonymous_transmission/app_alice.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)      375 2022-03-25 17:15:19.000000 netqasm-0.9.1/netqasm/examples/apps/anonymous_transmission/app_bob.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)      379 2022-03-25 17:15:19.000000 netqasm-0.9.1/netqasm/examples/apps/anonymous_transmission/app_charlie.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)      377 2022-03-25 17:15:19.000000 netqasm-0.9.1/netqasm/examples/apps/anonymous_transmission/app_david.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)        0 2021-05-19 15:28:08.000000 netqasm-0.9.1/netqasm/examples/apps/anonymous_transmission/bob.yaml
+-rw-rw-r--   0 bart      (1000) bart      (1000)        0 2021-05-19 15:28:08.000000 netqasm-0.9.1/netqasm/examples/apps/anonymous_transmission/charlie.yaml
+-rw-rw-r--   0 bart      (1000) bart      (1000)       29 2021-05-19 15:28:08.000000 netqasm-0.9.1/netqasm/examples/apps/anonymous_transmission/david.yaml
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:27.333103 netqasm-0.9.1/netqasm/examples/apps/anonymous_transmission/src/
+-rw-rw-r--   0 bart      (1000) bart      (1000)        0 2021-05-19 15:28:08.000000 netqasm-0.9.1/netqasm/examples/apps/anonymous_transmission/src/__init__.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)       44 2022-03-25 17:15:19.000000 netqasm-0.9.1/netqasm/examples/apps/anonymous_transmission/src/conf.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     1480 2022-03-28 08:45:06.000000 netqasm-0.9.1/netqasm/examples/apps/anonymous_transmission/src/protocol.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     5655 2022-03-25 17:15:19.000000 netqasm-0.9.1/netqasm/examples/apps/anonymous_transmission/src/sub_protocols.py
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:27.337103 netqasm-0.9.1/netqasm/examples/apps/bb84/
+-rw-rw-r--   0 bart      (1000) bart      (1000)      571 2022-01-17 15:40:37.000000 netqasm-0.9.1/netqasm/examples/apps/bb84/README.md
+-rw-rw-r--   0 bart      (1000) bart      (1000)        0 2022-01-17 15:40:37.000000 netqasm-0.9.1/netqasm/examples/apps/bb84/__init__.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)       12 2022-03-28 08:45:06.000000 netqasm-0.9.1/netqasm/examples/apps/bb84/alice.yaml
+-rw-rw-r--   0 bart      (1000) bart      (1000)     7669 2022-04-07 14:08:27.000000 netqasm-0.9.1/netqasm/examples/apps/bb84/app_alice.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     7240 2022-04-07 14:08:27.000000 netqasm-0.9.1/netqasm/examples/apps/bb84/app_bob.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)       12 2022-03-28 08:45:06.000000 netqasm-0.9.1/netqasm/examples/apps/bb84/bob.yaml
+-rw-rw-r--   0 bart      (1000) bart      (1000)      250 2022-03-25 16:50:13.000000 netqasm-0.9.1/netqasm/examples/apps/bb84/network.yaml
+-rw-rw-r--   0 bart      (1000) bart      (1000)     4382 2022-03-25 17:15:19.000000 netqasm-0.9.1/netqasm/examples/apps/bb84/results_config.json
+-rw-rw-r--   0 bart      (1000) bart      (1000)       22 2022-03-25 16:50:13.000000 netqasm-0.9.1/netqasm/examples/apps/bb84/roles.yaml
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:27.337103 netqasm-0.9.1/netqasm/examples/apps/blind_grover/
+-rw-rw-r--   0 bart      (1000) bart      (1000)     3353 2021-05-19 15:28:08.000000 netqasm-0.9.1/netqasm/examples/apps/blind_grover/README.md
+-rw-rw-r--   0 bart      (1000) bart      (1000)        0 2021-05-19 15:28:08.000000 netqasm-0.9.1/netqasm/examples/apps/blind_grover/__init__.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     3204 2022-03-28 08:45:06.000000 netqasm-0.9.1/netqasm/examples/apps/blind_grover/app_client.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     1824 2022-03-28 08:45:06.000000 netqasm-0.9.1/netqasm/examples/apps/blind_grover/app_server.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)       47 2021-05-19 15:28:08.000000 netqasm-0.9.1/netqasm/examples/apps/blind_grover/client.yaml
+-rw-rw-r--   0 bart      (1000) bart      (1000)        0 2021-05-19 15:28:08.000000 netqasm-0.9.1/netqasm/examples/apps/blind_grover/server.yaml
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:27.341103 netqasm-0.9.1/netqasm/examples/apps/blind_rotation/
+-rw-rw-r--   0 bart      (1000) bart      (1000)     2344 2021-05-19 15:28:08.000000 netqasm-0.9.1/netqasm/examples/apps/blind_rotation/README.md
+-rw-rw-r--   0 bart      (1000) bart      (1000)        0 2021-05-19 15:28:08.000000 netqasm-0.9.1/netqasm/examples/apps/blind_rotation/__init__.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     2761 2022-03-28 08:45:06.000000 netqasm-0.9.1/netqasm/examples/apps/blind_rotation/app_client.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     1551 2022-03-28 08:45:06.000000 netqasm-0.9.1/netqasm/examples/apps/blind_rotation/app_server.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)       67 2021-05-19 15:28:08.000000 netqasm-0.9.1/netqasm/examples/apps/blind_rotation/client.yaml
+-rw-rw-r--   0 bart      (1000) bart      (1000)       11 2021-05-19 15:28:08.000000 netqasm-0.9.1/netqasm/examples/apps/blind_rotation/server.yaml
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:27.345103 netqasm-0.9.1/netqasm/examples/apps/chsh/
+-rw-rw-r--   0 bart      (1000) bart      (1000)     1168 2021-05-19 15:28:08.000000 netqasm-0.9.1/netqasm/examples/apps/chsh/README.md
+-rw-rw-r--   0 bart      (1000) bart      (1000)        0 2021-05-19 15:28:08.000000 netqasm-0.9.1/netqasm/examples/apps/chsh/__init__.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)        4 2021-05-19 15:28:08.000000 netqasm-0.9.1/netqasm/examples/apps/chsh/alice.yaml
+-rwxrwxr-x   0 bart      (1000) bart      (1000)     1163 2022-04-07 14:08:27.000000 netqasm-0.9.1/netqasm/examples/apps/chsh/app_alice.py
+-rwxrwxr-x   0 bart      (1000) bart      (1000)     1565 2022-04-07 14:08:27.000000 netqasm-0.9.1/netqasm/examples/apps/chsh/app_bob.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     1040 2022-04-07 14:08:27.000000 netqasm-0.9.1/netqasm/examples/apps/chsh/app_repeater.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)        4 2021-05-19 15:28:08.000000 netqasm-0.9.1/netqasm/examples/apps/chsh/bob.yaml
+-rw-rw-r--   0 bart      (1000) bart      (1000)      689 2021-05-19 15:28:08.000000 netqasm-0.9.1/netqasm/examples/apps/chsh/network.yaml
+-rw-rw-r--   0 bart      (1000) bart      (1000)       50 2021-05-19 15:28:08.000000 netqasm-0.9.1/netqasm/examples/apps/chsh/roles.yaml
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:27.349103 netqasm-0.9.1/netqasm/examples/apps/dist_cnot/
+-rw-rw-r--   0 bart      (1000) bart      (1000)      718 2021-05-19 15:28:08.000000 netqasm-0.9.1/netqasm/examples/apps/dist_cnot/README.md
+-rw-rw-r--   0 bart      (1000) bart      (1000)        0 2021-05-19 15:28:08.000000 netqasm-0.9.1/netqasm/examples/apps/dist_cnot/__init__.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     1775 2022-04-07 14:08:27.000000 netqasm-0.9.1/netqasm/examples/apps/dist_cnot/app_controller.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     1868 2022-04-07 14:08:27.000000 netqasm-0.9.1/netqasm/examples/apps/dist_cnot/app_target.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)       21 2022-03-25 17:15:19.000000 netqasm-0.9.1/netqasm/examples/apps/dist_cnot/controller.yaml
+-rw-rw-r--   0 bart      (1000) bart      (1000)       17 2022-03-25 17:15:19.000000 netqasm-0.9.1/netqasm/examples/apps/dist_cnot/target.yaml
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:27.349103 netqasm-0.9.1/netqasm/examples/apps/link_layer_ck/
+-rw-rw-r--   0 bart      (1000) bart      (1000)        0 2022-03-25 17:15:19.000000 netqasm-0.9.1/netqasm/examples/apps/link_layer_ck/__init__.py
+-rwxrwxr-x   0 bart      (1000) bart      (1000)      928 2022-04-07 14:08:27.000000 netqasm-0.9.1/netqasm/examples/apps/link_layer_ck/app_client.py
+-rwxrwxr-x   0 bart      (1000) bart      (1000)      926 2022-04-07 14:08:27.000000 netqasm-0.9.1/netqasm/examples/apps/link_layer_ck/app_server.py
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:27.349103 netqasm-0.9.1/netqasm/examples/apps/link_layer_md/
+-rw-rw-r--   0 bart      (1000) bart      (1000)        0 2022-03-25 17:15:19.000000 netqasm-0.9.1/netqasm/examples/apps/link_layer_md/__init__.py
+-rwxrwxr-x   0 bart      (1000) bart      (1000)      720 2022-04-07 14:08:27.000000 netqasm-0.9.1/netqasm/examples/apps/link_layer_md/app_client.py
+-rwxrwxr-x   0 bart      (1000) bart      (1000)      600 2022-04-07 14:08:27.000000 netqasm-0.9.1/netqasm/examples/apps/link_layer_md/app_server.py
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:27.353103 netqasm-0.9.1/netqasm/examples/apps/magic_square/
+-rw-rw-r--   0 bart      (1000) bart      (1000)      618 2021-05-19 15:28:08.000000 netqasm-0.9.1/netqasm/examples/apps/magic_square/README.md
+-rw-rw-r--   0 bart      (1000) bart      (1000)        0 2021-05-19 15:28:08.000000 netqasm-0.9.1/netqasm/examples/apps/magic_square/__init__.py
+-rwxrwxr-x   0 bart      (1000) bart      (1000)     1987 2022-04-07 14:08:27.000000 netqasm-0.9.1/netqasm/examples/apps/magic_square/app_player1.py
+-rwxrwxr-x   0 bart      (1000) bart      (1000)     2022 2022-04-07 14:08:27.000000 netqasm-0.9.1/netqasm/examples/apps/magic_square/app_player2.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)      121 2021-05-19 15:28:08.000000 netqasm-0.9.1/netqasm/examples/apps/magic_square/player1.yaml
+-rw-rw-r--   0 bart      (1000) bart      (1000)      134 2022-03-25 17:15:19.000000 netqasm-0.9.1/netqasm/examples/apps/magic_square/player2.yaml
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:27.353103 netqasm-0.9.1/netqasm/examples/apps/multiple_files/
+-rw-rw-r--   0 bart      (1000) bart      (1000)        0 2021-05-19 15:28:08.000000 netqasm-0.9.1/netqasm/examples/apps/multiple_files/__init__.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)      702 2022-03-28 08:45:06.000000 netqasm-0.9.1/netqasm/examples/apps/multiple_files/app_alice.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)      627 2022-03-28 08:45:06.000000 netqasm-0.9.1/netqasm/examples/apps/multiple_files/app_bob.py
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:27.353103 netqasm-0.9.1/netqasm/examples/apps/multiple_files/shared/
+-rw-rw-r--   0 bart      (1000) bart      (1000)        0 2021-05-19 15:28:08.000000 netqasm-0.9.1/netqasm/examples/apps/multiple_files/shared/__init__.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)      163 2021-05-19 15:28:08.000000 netqasm-0.9.1/netqasm/examples/apps/multiple_files/shared/myfuncs.py
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:27.353103 netqasm-0.9.1/netqasm/examples/apps/single_node/
+-rw-rw-r--   0 bart      (1000) bart      (1000)        0 2021-05-19 15:28:08.000000 netqasm-0.9.1/netqasm/examples/apps/single_node/__init__.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)       20 2021-05-19 15:28:08.000000 netqasm-0.9.1/netqasm/examples/apps/single_node/alice.yaml
+-rwxrwxr-x   0 bart      (1000) bart      (1000)      726 2022-03-25 17:15:19.000000 netqasm-0.9.1/netqasm/examples/apps/single_node/app_alice.py
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:27.361103 netqasm-0.9.1/netqasm/examples/apps/teleport/
+-rw-rw-r--   0 bart      (1000) bart      (1000)      423 2021-05-19 15:28:08.000000 netqasm-0.9.1/netqasm/examples/apps/teleport/README.md
+-rw-rw-r--   0 bart      (1000) bart      (1000)        0 2021-05-19 15:28:08.000000 netqasm-0.9.1/netqasm/examples/apps/teleport/__init__.py
+-rwxrwxr-x   0 bart      (1000) bart      (1000)     2399 2022-04-07 14:08:27.000000 netqasm-0.9.1/netqasm/examples/apps/teleport/app_receiver.py
+-rwxrwxr-x   0 bart      (1000) bart      (1000)     1795 2022-04-07 14:08:27.000000 netqasm-0.9.1/netqasm/examples/apps/teleport/app_sender.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)      444 2022-03-17 13:37:07.000000 netqasm-0.9.1/netqasm/examples/apps/teleport/network.yaml
+-rw-rw-r--   0 bart      (1000) bart      (1000)        0 2021-05-19 15:28:08.000000 netqasm-0.9.1/netqasm/examples/apps/teleport/receiver.yaml
+-rw-rw-r--   0 bart      (1000) bart      (1000)     1816 2022-03-25 17:15:19.000000 netqasm-0.9.1/netqasm/examples/apps/teleport/results_config.json
+-rw-rw-r--   0 bart      (1000) bart      (1000)       37 2021-05-19 15:28:08.000000 netqasm-0.9.1/netqasm/examples/apps/teleport/roles.yaml
+-rw-rw-r--   0 bart      (1000) bart      (1000)       19 2022-03-25 17:15:19.000000 netqasm-0.9.1/netqasm/examples/apps/teleport/sender.yaml
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:27.361103 netqasm-0.9.1/netqasm/examples/apps/three_nodes/
+-rw-rw-r--   0 bart      (1000) bart      (1000)        0 2021-05-19 15:28:08.000000 netqasm-0.9.1/netqasm/examples/apps/three_nodes/__init__.py
+-rwxrwxr-x   0 bart      (1000) bart      (1000)      964 2022-04-07 14:08:27.000000 netqasm-0.9.1/netqasm/examples/apps/three_nodes/app_alice.py
+-rwxrwxr-x   0 bart      (1000) bart      (1000)      972 2022-04-07 14:08:27.000000 netqasm-0.9.1/netqasm/examples/apps/three_nodes/app_bob.py
+-rwxrwxr-x   0 bart      (1000) bart      (1000)      905 2022-04-07 14:08:27.000000 netqasm-0.9.1/netqasm/examples/apps/three_nodes/app_charlie.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)      797 2021-05-19 15:28:08.000000 netqasm-0.9.1/netqasm/examples/apps/three_nodes/network.yaml
+-rw-rw-r--   0 bart      (1000) bart      (1000)       49 2021-05-19 15:28:08.000000 netqasm-0.9.1/netqasm/examples/apps/three_nodes/roles.yaml
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:27.361103 netqasm-0.9.1/netqasm/examples/lib/
+-rw-rw-r--   0 bart      (1000) bart      (1000)        0 2021-05-19 15:28:08.000000 netqasm-0.9.1/netqasm/examples/lib/__init__.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     1548 2022-04-07 14:08:27.000000 netqasm-0.9.1/netqasm/examples/lib/bqc.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     2837 2022-03-28 08:45:06.000000 netqasm-0.9.1/netqasm/examples/run_examples.py
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:27.365103 netqasm-0.9.1/netqasm/examples/sdk_compilation/
+-rw-rw-r--   0 bart      (1000) bart      (1000)        0 2022-03-28 08:45:06.000000 netqasm-0.9.1/netqasm/examples/sdk_compilation/__init__.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     1214 2022-03-28 08:45:06.000000 netqasm-0.9.1/netqasm/examples/sdk_compilation/example_bb84.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)      711 2022-03-28 08:45:06.000000 netqasm-0.9.1/netqasm/examples/sdk_compilation/example_enumerate.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)      700 2022-03-28 08:45:06.000000 netqasm-0.9.1/netqasm/examples/sdk_compilation/example_loop.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)      726 2022-03-28 08:45:06.000000 netqasm-0.9.1/netqasm/examples/sdk_compilation/example_post_epr.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)      667 2022-04-07 14:08:27.000000 netqasm-0.9.1/netqasm/examples/sdk_compilation/example_rsp.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)      545 2022-03-28 08:45:06.000000 netqasm-0.9.1/netqasm/examples/sdk_compilation/example_simple_loop.py
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:27.365103 netqasm-0.9.1/netqasm/lang/
+-rw-rw-r--   0 bart      (1000) bart      (1000)        0 2021-05-19 15:28:08.000000 netqasm-0.9.1/netqasm/lang/__init__.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     6804 2022-04-07 14:43:59.000000 netqasm-0.9.1/netqasm/lang/encoding.py
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:27.369103 netqasm-0.9.1/netqasm/lang/instr/
+-rw-rw-r--   0 bart      (1000) bart      (1000)      111 2022-03-25 17:15:19.000000 netqasm-0.9.1/netqasm/lang/instr/__init__.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)    22917 2022-04-07 14:43:59.000000 netqasm-0.9.1/netqasm/lang/instr/base.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)    11443 2022-04-07 14:43:59.000000 netqasm-0.9.1/netqasm/lang/instr/core.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     3325 2022-04-07 14:43:59.000000 netqasm-0.9.1/netqasm/lang/instr/flavour.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     3007 2022-04-07 14:21:48.000000 netqasm-0.9.1/netqasm/lang/instr/nv.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     3827 2022-04-07 14:21:48.000000 netqasm-0.9.1/netqasm/lang/instr/vanilla.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     5528 2022-04-07 14:43:59.000000 netqasm-0.9.1/netqasm/lang/ir.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     3910 2022-04-07 14:43:59.000000 netqasm-0.9.1/netqasm/lang/operand.py
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:27.369103 netqasm-0.9.1/netqasm/lang/parsing/
+-rw-rw-r--   0 bart      (1000) bart      (1000)      147 2022-03-25 17:15:19.000000 netqasm-0.9.1/netqasm/lang/parsing/__init__.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     2385 2022-04-07 14:43:59.000000 netqasm-0.9.1/netqasm/lang/parsing/binary.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)    19082 2022-04-07 14:43:59.000000 netqasm-0.9.1/netqasm/lang/parsing/text.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     1577 2022-04-07 14:43:59.000000 netqasm-0.9.1/netqasm/lang/subroutine.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)      357 2022-04-07 14:43:59.000000 netqasm-0.9.1/netqasm/lang/symbols.py
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:27.369103 netqasm-0.9.1/netqasm/logging/
+-rw-rw-r--   0 bart      (1000) bart      (1000)        0 2021-05-19 15:28:08.000000 netqasm-0.9.1/netqasm/logging/__init__.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     1039 2022-03-28 08:45:06.000000 netqasm-0.9.1/netqasm/logging/glob.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)    12547 2022-04-07 14:21:48.000000 netqasm-0.9.1/netqasm/logging/output.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     9902 2022-04-07 14:08:27.000000 netqasm-0.9.1/netqasm/qlink_compat.py
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:27.373103 netqasm-0.9.1/netqasm/runtime/
+-rw-rw-r--   0 bart      (1000) bart      (1000)        0 2021-05-19 15:28:08.000000 netqasm-0.9.1/netqasm/runtime/__init__.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)      510 2022-03-25 17:15:19.000000 netqasm-0.9.1/netqasm/runtime/app_config.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     6460 2022-03-25 17:15:19.000000 netqasm-0.9.1/netqasm/runtime/application.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)    12507 2022-03-28 08:45:06.000000 netqasm-0.9.1/netqasm/runtime/cli.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)      491 2022-03-25 17:15:19.000000 netqasm-0.9.1/netqasm/runtime/debug.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     8925 2022-03-28 08:45:06.000000 netqasm-0.9.1/netqasm/runtime/env.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     2337 2022-03-28 08:45:06.000000 netqasm-0.9.1/netqasm/runtime/hardware.py
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:27.373103 netqasm-0.9.1/netqasm/runtime/interface/
+-rw-rw-r--   0 bart      (1000) bart      (1000)      170 2022-03-25 17:15:19.000000 netqasm-0.9.1/netqasm/runtime/interface/__init__.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     3498 2022-03-25 17:15:19.000000 netqasm-0.9.1/netqasm/runtime/interface/config.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     4831 2022-03-28 08:45:06.000000 netqasm-0.9.1/netqasm/runtime/interface/logging.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)      146 2022-03-25 17:15:19.000000 netqasm-0.9.1/netqasm/runtime/interface/results.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     2970 2022-03-25 17:15:19.000000 netqasm-0.9.1/netqasm/runtime/process_logs.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)      838 2022-03-25 17:15:19.000000 netqasm-0.9.1/netqasm/runtime/runtime_mgr.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)      864 2022-03-25 17:15:19.000000 netqasm-0.9.1/netqasm/runtime/settings.py
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:27.405103 netqasm-0.9.1/netqasm/sdk/
+-rw-rw-r--   0 bart      (1000) bart      (1000)      220 2022-03-25 17:15:19.000000 netqasm-0.9.1/netqasm/sdk/__init__.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     7238 2022-04-07 14:08:27.000000 netqasm-0.9.1/netqasm/sdk/build_epr.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)      552 2022-04-07 14:08:27.000000 netqasm-0.9.1/netqasm/sdk/build_nv.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     2123 2022-04-07 14:08:27.000000 netqasm-0.9.1/netqasm/sdk/build_types.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)    78479 2022-04-07 14:43:59.000000 netqasm-0.9.1/netqasm/sdk/builder.py
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:27.409103 netqasm-0.9.1/netqasm/sdk/classical_communication/
+-rw-rw-r--   0 bart      (1000) bart      (1000)       82 2022-03-25 17:15:19.000000 netqasm-0.9.1/netqasm/sdk/classical_communication/__init__.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     4546 2022-03-28 08:45:06.000000 netqasm-0.9.1/netqasm/sdk/classical_communication/broadcast_channel.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)      105 2022-01-17 15:23:58.000000 netqasm-0.9.1/netqasm/sdk/classical_communication/message.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     4795 2022-03-28 08:45:06.000000 netqasm-0.9.1/netqasm/sdk/classical_communication/socket.py
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:27.409103 netqasm-0.9.1/netqasm/sdk/classical_communication/thread_socket/
+-rw-rw-r--   0 bart      (1000) bart      (1000)      393 2022-03-25 17:15:19.000000 netqasm-0.9.1/netqasm/sdk/classical_communication/thread_socket/__init__.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)      385 2022-03-28 08:45:06.000000 netqasm-0.9.1/netqasm/sdk/classical_communication/thread_socket/broadcast_channel.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)    13555 2022-03-28 08:45:06.000000 netqasm-0.9.1/netqasm/sdk/classical_communication/thread_socket/socket.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     7670 2022-03-28 08:45:06.000000 netqasm-0.9.1/netqasm/sdk/classical_communication/thread_socket/socket_hub.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)    22670 2022-04-07 14:43:59.000000 netqasm-0.9.1/netqasm/sdk/compiling.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)      350 2022-03-25 17:15:19.000000 netqasm-0.9.1/netqasm/sdk/config.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)    33248 2022-04-07 14:43:59.000000 netqasm-0.9.1/netqasm/sdk/connection.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)      833 2022-04-07 14:08:27.000000 netqasm-0.9.1/netqasm/sdk/constraint.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)    39028 2022-04-07 14:08:27.000000 netqasm-0.9.1/netqasm/sdk/epr_socket.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     4156 2022-03-28 08:45:06.000000 netqasm-0.9.1/netqasm/sdk/external.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)    23172 2022-04-07 14:43:59.000000 netqasm-0.9.1/netqasm/sdk/futures.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     6328 2022-04-07 14:21:48.000000 netqasm-0.9.1/netqasm/sdk/memmgr.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     1317 2022-03-25 17:15:19.000000 netqasm-0.9.1/netqasm/sdk/network.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)      803 2022-03-25 17:15:19.000000 netqasm-0.9.1/netqasm/sdk/progress_bar.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)    13666 2022-04-07 14:43:59.000000 netqasm-0.9.1/netqasm/sdk/qubit.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)    11706 2022-04-07 14:21:48.000000 netqasm-0.9.1/netqasm/sdk/shared_memory.py
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:27.437103 netqasm-0.9.1/netqasm/sdk/toolbox/
+-rw-rw-r--   0 bart      (1000) bart      (1000)      183 2022-03-25 17:15:19.000000 netqasm-0.9.1/netqasm/sdk/toolbox/__init__.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)      787 2022-03-25 17:15:19.000000 netqasm-0.9.1/netqasm/sdk/toolbox/gates.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     3433 2022-03-25 17:15:19.000000 netqasm-0.9.1/netqasm/sdk/toolbox/measurements.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     4634 2022-04-07 14:08:27.000000 netqasm-0.9.1/netqasm/sdk/toolbox/multi_node.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     1516 2022-03-28 08:45:06.000000 netqasm-0.9.1/netqasm/sdk/toolbox/sim_states.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     2026 2022-04-07 14:21:48.000000 netqasm-0.9.1/netqasm/sdk/toolbox/state_prep.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)      106 2022-03-25 17:15:19.000000 netqasm-0.9.1/netqasm/typedefs.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)      347 2021-05-19 15:28:08.000000 netqasm-0.9.1/netqasm/typing.py
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:27.437103 netqasm-0.9.1/netqasm/util/
+-rw-rw-r--   0 bart      (1000) bart      (1000)        0 2021-05-19 15:28:08.000000 netqasm-0.9.1/netqasm/util/__init__.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)      252 2022-03-25 17:15:19.000000 netqasm-0.9.1/netqasm/util/error.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     1922 2022-03-25 17:15:19.000000 netqasm-0.9.1/netqasm/util/log.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     3501 2022-04-07 14:21:49.000000 netqasm-0.9.1/netqasm/util/quantum_gates.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)      914 2022-03-28 08:45:06.000000 netqasm-0.9.1/netqasm/util/states.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     2858 2022-03-25 17:15:19.000000 netqasm-0.9.1/netqasm/util/string.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)      519 2021-05-19 15:28:08.000000 netqasm-0.9.1/netqasm/util/thread.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)      445 2022-03-25 17:15:19.000000 netqasm-0.9.1/netqasm/util/yaml.py
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:27.321103 netqasm-0.9.1/netqasm.egg-info/
+-rw-rw-r--   0 bart      (1000) bart      (1000)     5201 2022-04-07 14:53:25.000000 netqasm-0.9.1/netqasm.egg-info/PKG-INFO
+-rw-rw-r--   0 bart      (1000) bart      (1000)    24275 2022-04-07 14:53:26.000000 netqasm-0.9.1/netqasm.egg-info/SOURCES.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)        1 2022-04-07 14:53:25.000000 netqasm-0.9.1/netqasm.egg-info/dependency_links.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)       52 2022-04-07 14:53:26.000000 netqasm-0.9.1/netqasm.egg-info/entry_points.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)      300 2022-04-07 14:53:26.000000 netqasm-0.9.1/netqasm.egg-info/requires.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)        8 2022-04-07 14:53:26.000000 netqasm-0.9.1/netqasm.egg-info/top_level.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)      249 2022-03-28 08:45:06.000000 netqasm-0.9.1/pyproject.toml
+-rw-rw-r--   0 bart      (1000) bart      (1000)      196 2022-04-07 14:44:30.000000 netqasm-0.9.1/requirements.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)      545 2022-04-07 14:53:27.489104 netqasm-0.9.1/setup.cfg
+-rw-rw-r--   0 bart      (1000) bart      (1000)      578 2022-03-28 08:45:06.000000 netqasm-0.9.1/setup.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)       99 2022-04-07 14:44:48.000000 netqasm-0.9.1/test_requirements.txt
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:27.445104 netqasm-0.9.1/tests/
+-rw-rw-r--   0 bart      (1000) bart      (1000)    24497 2022-04-07 14:43:59.000000 netqasm-0.9.1/tests/test_builder.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)    11006 2022-03-25 17:15:19.000000 netqasm-0.9.1/tests/test_cli.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     8471 2022-04-07 14:43:59.000000 netqasm-0.9.1/tests/test_compiling.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     2392 2022-03-28 08:45:06.000000 netqasm-0.9.1/tests/test_encoding.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     3332 2022-03-28 08:45:06.000000 netqasm-0.9.1/tests/test_executor.py
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:27.445104 netqasm-0.9.1/tests/test_external/
+-rw-rw-r--   0 bart      (1000) bart      (1000)     4177 2022-03-28 08:45:06.000000 netqasm-0.9.1/tests/test_external/test_examples.py
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:27.465104 netqasm-0.9.1/tests/test_external/test_sdk/
+-rw-rw-r--   0 bart      (1000) bart      (1000)     1725 2022-03-28 08:45:06.000000 netqasm-0.9.1/tests/test_external/test_sdk/test_create_epr.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     1471 2022-03-28 08:45:06.000000 netqasm-0.9.1/tests/test_external/test_sdk/test_create_epr_m.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     1150 2022-04-07 14:08:27.000000 netqasm-0.9.1/tests/test_external/test_sdk/test_enumerate.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     1180 2022-03-28 08:45:06.000000 netqasm-0.9.1/tests/test_external/test_sdk/test_foreach.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)      793 2022-03-28 08:45:06.000000 netqasm-0.9.1/tests/test_external/test_sdk/test_measure.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)      858 2022-03-28 08:45:06.000000 netqasm-0.9.1/tests/test_external/test_sdk/test_measure_if_conn.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)      795 2022-03-28 08:45:06.000000 netqasm-0.9.1/tests/test_external/test_sdk/test_measure_if_future.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)      945 2022-04-07 14:08:27.000000 netqasm-0.9.1/tests/test_external/test_sdk/test_measure_loop.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     1132 2022-03-28 08:45:06.000000 netqasm-0.9.1/tests/test_external/test_sdk/test_measure_loop_context.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     1161 2022-04-07 14:08:27.000000 netqasm-0.9.1/tests/test_external/test_sdk/test_nested_loop.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     1180 2022-04-07 14:08:27.000000 netqasm-0.9.1/tests/test_external/test_sdk/test_new_array.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     1503 2022-03-28 08:45:06.000000 netqasm-0.9.1/tests/test_external/test_sdk/test_post_epr.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     1386 2022-03-28 08:45:06.000000 netqasm-0.9.1/tests/test_external/test_sdk/test_post_epr_context.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)      907 2022-03-28 08:45:06.000000 netqasm-0.9.1/tests/test_external/test_sdk/test_rotations.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     2050 2022-03-28 08:45:06.000000 netqasm-0.9.1/tests/test_external/test_sdk/test_teleport.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     2236 2022-03-28 08:45:06.000000 netqasm-0.9.1/tests/test_external/test_sdk/test_teleport_without_corrections.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     1063 2022-03-28 08:45:06.000000 netqasm-0.9.1/tests/test_external/test_sdk/test_two_nodes.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     4031 2022-03-25 17:15:19.000000 netqasm-0.9.1/tests/test_external/test_toolbox.py
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:27.481104 netqasm-0.9.1/tests/test_parsing/
+-rw-rw-r--   0 bart      (1000) bart      (1000)     2158 2022-04-07 14:43:59.000000 netqasm-0.9.1/tests/test_parsing/test_binary.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     8671 2022-04-07 14:43:59.000000 netqasm-0.9.1/tests/test_parsing/test_text.py
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2022-04-07 14:53:27.489104 netqasm-0.9.1/tests/test_sdk/
+-rw-rw-r--   0 bart      (1000) bart      (1000)     5612 2022-03-28 08:45:06.000000 netqasm-0.9.1/tests/test_sdk/test_classical_communication.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)    35647 2022-04-07 14:43:59.000000 netqasm-0.9.1/tests/test_sdk/test_connection.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)      998 2022-03-25 17:15:19.000000 netqasm-0.9.1/tests/test_sdk/test_future.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     1369 2022-03-25 17:15:19.000000 netqasm-0.9.1/tests/test_states_util.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     3051 2022-03-25 17:15:19.000000 netqasm-0.9.1/tests/test_string_util.py
```

### Comparing `netqasm-0.9.0/CHANGELOG.md` & `netqasm-0.9.1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/LICENSE` & `netqasm-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/Makefile` & `netqasm-0.9.1/Makefile`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/PKG-INFO` & `netqasm-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: netqasm
-Version: 0.9.0
+Version: 0.9.1
 Summary: Tool for parsing, encoding, decoding and executing NetQASM applications
 Home-page: https://github.com/QuTech-Delft/netqasm
 Author: Axel Dahlberg, Bart van der Vecht
 Author-email: b.vandervecht@tudelft.nl
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# NetQASM (0.9.0)
+# NetQASM (0.9.1)
 [![Documentation](https://readthedocs.org/projects/netqasm/badge/?version=latest)](https://netqasm.readthedocs.io/en/latest/?badge=latest)
 
 Utilities for writing, compiling, and running quantum network applications.
 
 ## Intro
 NetQASM is an instruction set architecture that allows one to interface with quantum network controllers and run applications on a quantum network. Applications may be written directly in the NetQASM language, which resembles assembly code. However, this package also provides an SDK which allows writing application code in Python.
 For the paper introducing NetQASM, see [here](https://arxiv.org/abs/2111.09823).
```

### Comparing `netqasm-0.9.0/README.md` & `netqasm-0.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# NetQASM (0.9.0)
+# NetQASM (0.9.1)
 [![Documentation](https://readthedocs.org/projects/netqasm/badge/?version=latest)](https://netqasm.readthedocs.io/en/latest/?badge=latest)
 
 Utilities for writing, compiling, and running quantum network applications.
 
 ## Intro
 NetQASM is an instruction set architecture that allows one to interface with quantum network controllers and run applications on a quantum network. Applications may be written directly in the NetQASM language, which resembles assembly code. However, this package also provides an SDK which allows writing application code in Python.
 For the paper introducing NetQASM, see [here](https://arxiv.org/abs/2111.09823).
```

### Comparing `netqasm-0.9.0/docs/Makefile` & `netqasm-0.9.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/api_lang/netqasm.lang.instr.rst` & `netqasm-0.9.1/docs/api_lang/netqasm.lang.instr.rst`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/api_runtime/netqasm.runtime.interface.rst` & `netqasm-0.9.1/docs/api_runtime/netqasm.runtime.interface.rst`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/api_sdk/netqasm.sdk.classical_communication.rst` & `netqasm-0.9.1/docs/api_sdk/netqasm.sdk.classical_communication.rst`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/api_sdk/netqasm.sdk.toolbox.rst` & `netqasm-0.9.1/docs/api_sdk/netqasm.sdk.toolbox.rst`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/doctrees/api_backend/netqasm.backend.executor.doctree` & `netqasm-0.9.1/docs/build/doctrees/api_backend/netqasm.backend.executor.doctree`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/doctrees/api_backend/netqasm.backend.messages.doctree` & `netqasm-0.9.1/docs/build/doctrees/api_backend/netqasm.backend.messages.doctree`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/doctrees/api_backend/netqasm.backend.network_stack.doctree` & `netqasm-0.9.1/docs/build/doctrees/api_backend/netqasm.backend.network_stack.doctree`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/doctrees/api_backend/netqasm.backend.qnodeos.doctree` & `netqasm-0.9.1/docs/build/doctrees/api_backend/netqasm.backend.qnodeos.doctree`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/doctrees/api_lang/netqasm.lang.encoding.doctree` & `netqasm-0.9.1/docs/build/doctrees/api_lang/netqasm.lang.encoding.doctree`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/doctrees/api_lang/netqasm.lang.instr.doctree` & `netqasm-0.9.1/docs/build/doctrees/api_lang/netqasm.lang.instr.doctree`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/doctrees/api_lang/netqasm.lang.ir.doctree` & `netqasm-0.9.1/docs/build/doctrees/api_lang/netqasm.lang.ir.doctree`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/doctrees/api_lang/netqasm.lang.operand.doctree` & `netqasm-0.9.1/docs/build/doctrees/api_lang/netqasm.lang.operand.doctree`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/doctrees/api_lang/netqasm.lang.parsing.doctree` & `netqasm-0.9.1/docs/build/doctrees/api_lang/netqasm.lang.parsing.doctree`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/doctrees/api_lang/netqasm.lang.subroutine.doctree` & `netqasm-0.9.1/docs/build/doctrees/api_lang/netqasm.lang.subroutine.doctree`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/doctrees/api_lang/netqasm.lang.symbols.doctree` & `netqasm-0.9.1/docs/build/doctrees/api_lang/netqasm.lang.symbols.doctree`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/doctrees/api_logging/netqasm.logging.glob.doctree` & `netqasm-0.9.1/docs/build/doctrees/api_logging/netqasm.logging.glob.doctree`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/doctrees/api_logging/netqasm.logging.output.doctree` & `netqasm-0.9.1/docs/build/doctrees/api_logging/netqasm.logging.output.doctree`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/doctrees/api_root.doctree` & `netqasm-0.9.1/docs/build/doctrees/api_root.doctree`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/doctrees/api_runtime/netqasm.runtime.app_config.doctree` & `netqasm-0.9.1/docs/build/doctrees/api_runtime/netqasm.runtime.app_config.doctree`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/doctrees/api_runtime/netqasm.runtime.application.doctree` & `netqasm-0.9.1/docs/build/doctrees/api_runtime/netqasm.runtime.application.doctree`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/doctrees/api_runtime/netqasm.runtime.cli.doctree` & `netqasm-0.9.1/docs/build/doctrees/api_runtime/netqasm.runtime.cli.doctree`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/doctrees/api_runtime/netqasm.runtime.debug.doctree` & `netqasm-0.9.1/docs/build/doctrees/api_runtime/netqasm.runtime.debug.doctree`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/doctrees/api_runtime/netqasm.runtime.env.doctree` & `netqasm-0.9.1/docs/build/doctrees/api_runtime/netqasm.runtime.env.doctree`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/doctrees/api_runtime/netqasm.runtime.hardware.doctree` & `netqasm-0.9.1/docs/build/doctrees/api_runtime/netqasm.runtime.hardware.doctree`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/doctrees/api_runtime/netqasm.runtime.interface.doctree` & `netqasm-0.9.1/docs/build/doctrees/api_runtime/netqasm.runtime.interface.doctree`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/doctrees/api_runtime/netqasm.runtime.process_logs.doctree` & `netqasm-0.9.1/docs/build/doctrees/api_runtime/netqasm.runtime.process_logs.doctree`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/doctrees/api_runtime/netqasm.runtime.settings.doctree` & `netqasm-0.9.1/docs/build/doctrees/api_runtime/netqasm.runtime.settings.doctree`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/doctrees/api_sdk/netqasm.sdk.builder.doctree` & `netqasm-0.9.1/docs/build/doctrees/api_sdk/netqasm.sdk.builder.doctree`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/doctrees/api_sdk/netqasm.sdk.classical_communication.doctree` & `netqasm-0.9.1/docs/build/doctrees/api_sdk/netqasm.sdk.classical_communication.doctree`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/doctrees/api_sdk/netqasm.sdk.compiling.doctree` & `netqasm-0.9.1/docs/build/doctrees/api_sdk/netqasm.sdk.compiling.doctree`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/doctrees/api_sdk/netqasm.sdk.config.doctree` & `netqasm-0.9.1/docs/build/doctrees/api_sdk/netqasm.sdk.config.doctree`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/doctrees/api_sdk/netqasm.sdk.connection.doctree` & `netqasm-0.9.1/docs/build/doctrees/api_sdk/netqasm.sdk.connection.doctree`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/doctrees/api_sdk/netqasm.sdk.epr_socket.doctree` & `netqasm-0.9.1/docs/build/doctrees/api_sdk/netqasm.sdk.epr_socket.doctree`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/doctrees/api_sdk/netqasm.sdk.external.doctree` & `netqasm-0.9.1/docs/build/doctrees/api_sdk/netqasm.sdk.external.doctree`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/doctrees/api_sdk/netqasm.sdk.futures.doctree` & `netqasm-0.9.1/docs/build/doctrees/api_sdk/netqasm.sdk.futures.doctree`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/doctrees/api_sdk/netqasm.sdk.network.doctree` & `netqasm-0.9.1/docs/build/doctrees/api_sdk/netqasm.sdk.network.doctree`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/doctrees/api_sdk/netqasm.sdk.progress_bar.doctree` & `netqasm-0.9.1/docs/build/doctrees/api_sdk/netqasm.sdk.progress_bar.doctree`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/doctrees/api_sdk/netqasm.sdk.qubit.doctree` & `netqasm-0.9.1/docs/build/doctrees/api_sdk/netqasm.sdk.qubit.doctree`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/doctrees/api_sdk/netqasm.sdk.shared_memory.doctree` & `netqasm-0.9.1/docs/build/doctrees/api_sdk/netqasm.sdk.shared_memory.doctree`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/doctrees/api_sdk/netqasm.sdk.toolbox.doctree` & `netqasm-0.9.1/docs/build/doctrees/api_sdk/netqasm.sdk.toolbox.doctree`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/doctrees/api_util/netqasm.util.error.doctree` & `netqasm-0.9.1/docs/build/doctrees/api_util/netqasm.util.error.doctree`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/doctrees/api_util/netqasm.util.log.doctree` & `netqasm-0.9.1/docs/build/doctrees/api_util/netqasm.util.log.doctree`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/doctrees/api_util/netqasm.util.quantum_gates.doctree` & `netqasm-0.9.1/docs/build/doctrees/api_util/netqasm.util.quantum_gates.doctree`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/doctrees/api_util/netqasm.util.states.doctree` & `netqasm-0.9.1/docs/build/doctrees/api_util/netqasm.util.states.doctree`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/doctrees/api_util/netqasm.util.string.doctree` & `netqasm-0.9.1/docs/build/doctrees/api_util/netqasm.util.string.doctree`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/doctrees/api_util/netqasm.util.thread.doctree` & `netqasm-0.9.1/docs/build/doctrees/api_util/netqasm.util.thread.doctree`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/doctrees/api_util/netqasm.util.yaml.doctree` & `netqasm-0.9.1/docs/build/doctrees/api_util/netqasm.util.yaml.doctree`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/doctrees/environment.pickle` & `netqasm-0.9.1/docs/build/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/doctrees/index.doctree` & `netqasm-0.9.1/docs/build/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/doctrees/installation.doctree` & `netqasm-0.9.1/docs/build/doctrees/installation.doctree`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/doctrees/known_issues.doctree` & `netqasm-0.9.1/docs/build/doctrees/known_issues.doctree`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/doctrees/netqasm.backend.doctree` & `netqasm-0.9.1/docs/build/doctrees/netqasm.backend.doctree`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/doctrees/netqasm.examples.doctree` & `netqasm-0.9.1/docs/build/doctrees/netqasm.examples.doctree`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/doctrees/netqasm.lang.doctree` & `netqasm-0.9.1/docs/build/doctrees/netqasm.lang.doctree`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/doctrees/netqasm.logging.doctree` & `netqasm-0.9.1/docs/build/doctrees/netqasm.logging.doctree`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/doctrees/netqasm.runtime.doctree` & `netqasm-0.9.1/docs/build/doctrees/netqasm.runtime.doctree`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/doctrees/netqasm.sdk.doctree` & `netqasm-0.9.1/docs/build/doctrees/netqasm.sdk.doctree`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/doctrees/netqasm.util.doctree` & `netqasm-0.9.1/docs/build/doctrees/netqasm.util.doctree`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/doctrees/quickstart/file_structure.doctree` & `netqasm-0.9.1/docs/build/doctrees/quickstart/file_structure.doctree`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/doctrees/quickstart/first-app.doctree` & `netqasm-0.9.1/docs/build/doctrees/quickstart/first-app.doctree`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/doctrees/quickstart/modules.doctree` & `netqasm-0.9.1/docs/build/doctrees/quickstart/modules.doctree`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/doctrees/quickstart/using-sdk.doctree` & `netqasm-0.9.1/docs/build/doctrees/quickstart/using-sdk.doctree`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/doctrees/quickstart.doctree` & `netqasm-0.9.1/docs/build/doctrees/quickstart.doctree`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_sources/api_lang/netqasm.lang.instr.rst.txt` & `netqasm-0.9.1/docs/build/html/_sources/api_lang/netqasm.lang.instr.rst.txt`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_sources/api_runtime/netqasm.runtime.interface.rst.txt` & `netqasm-0.9.1/docs/build/html/_sources/api_runtime/netqasm.runtime.interface.rst.txt`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_sources/api_sdk/netqasm.sdk.classical_communication.rst.txt` & `netqasm-0.9.1/docs/build/html/_sources/api_sdk/netqasm.sdk.classical_communication.rst.txt`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_sources/api_sdk/netqasm.sdk.toolbox.rst.txt` & `netqasm-0.9.1/docs/build/html/_sources/api_sdk/netqasm.sdk.toolbox.rst.txt`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_sources/index.rst.txt` & `netqasm-0.9.1/docs/build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_sources/installation.rst.txt` & `netqasm-0.9.1/docs/build/html/_sources/installation.rst.txt`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_sources/netqasm.sdk.rst.txt` & `netqasm-0.9.1/docs/build/html/_sources/netqasm.sdk.rst.txt`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_sources/quickstart/file_structure.rst.txt` & `netqasm-0.9.1/docs/build/html/_sources/quickstart/file_structure.rst.txt`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_sources/quickstart/first-app.rst.txt` & `netqasm-0.9.1/docs/build/html/_sources/quickstart/first-app.rst.txt`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_sources/quickstart/modules.rst.txt` & `netqasm-0.9.1/docs/build/html/_sources/quickstart/modules.rst.txt`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_sources/quickstart/using-sdk.rst.txt` & `netqasm-0.9.1/docs/build/html/_sources/quickstart/using-sdk.rst.txt`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_sources/quickstart.rst.txt` & `netqasm-0.9.1/docs/build/html/_sources/quickstart.rst.txt`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_static/basic.css` & `netqasm-0.9.1/docs/build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_static/css/badge_only.css` & `netqasm-0.9.1/docs/build/html/_static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff` & `netqasm-0.9.1/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2` & `netqasm-0.9.1/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff` & `netqasm-0.9.1/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2` & `netqasm-0.9.1/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_static/css/fonts/fontawesome-webfont.eot` & `netqasm-0.9.1/docs/build/html/_static/css/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_static/css/fonts/fontawesome-webfont.svg` & `netqasm-0.9.1/docs/build/html/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_static/css/fonts/fontawesome-webfont.ttf` & `netqasm-0.9.1/docs/build/html/_static/css/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_static/css/fonts/fontawesome-webfont.woff` & `netqasm-0.9.1/docs/build/html/_static/css/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_static/css/fonts/fontawesome-webfont.woff2` & `netqasm-0.9.1/docs/build/html/_static/css/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_static/css/fonts/lato-bold-italic.woff` & `netqasm-0.9.1/docs/build/html/_static/css/fonts/lato-bold-italic.woff`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_static/css/fonts/lato-bold-italic.woff2` & `netqasm-0.9.1/docs/build/html/_static/css/fonts/lato-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_static/css/fonts/lato-bold.woff` & `netqasm-0.9.1/docs/build/html/_static/css/fonts/lato-bold.woff`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_static/css/fonts/lato-bold.woff2` & `netqasm-0.9.1/docs/build/html/_static/css/fonts/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_static/css/fonts/lato-normal-italic.woff` & `netqasm-0.9.1/docs/build/html/_static/css/fonts/lato-normal-italic.woff`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_static/css/fonts/lato-normal-italic.woff2` & `netqasm-0.9.1/docs/build/html/_static/css/fonts/lato-normal-italic.woff2`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_static/css/fonts/lato-normal.woff` & `netqasm-0.9.1/docs/build/html/_static/css/fonts/lato-normal.woff`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_static/css/fonts/lato-normal.woff2` & `netqasm-0.9.1/docs/build/html/_static/css/fonts/lato-normal.woff2`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_static/css/theme.css` & `netqasm-0.9.1/docs/build/html/_static/css/theme.css`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_static/doctools.js` & `netqasm-0.9.1/docs/build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_static/fonts/Inconsolata-Bold.ttf` & `netqasm-0.9.1/docs/build/html/_static/fonts/Inconsolata-Bold.ttf`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_static/fonts/Inconsolata-Regular.ttf` & `netqasm-0.9.1/docs/build/html/_static/fonts/Inconsolata-Regular.ttf`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_static/fonts/Inconsolata.ttf` & `netqasm-0.9.1/docs/build/html/_static/fonts/Inconsolata.ttf`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_static/fonts/Lato/lato-bold.eot` & `netqasm-0.9.1/docs/build/html/_static/fonts/Lato/lato-bold.eot`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_static/fonts/Lato/lato-bold.ttf` & `netqasm-0.9.1/docs/build/html/_static/fonts/Lato/lato-bold.ttf`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_static/fonts/Lato/lato-bold.woff` & `netqasm-0.9.1/docs/build/html/_static/fonts/Lato/lato-bold.woff`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_static/fonts/Lato/lato-bold.woff2` & `netqasm-0.9.1/docs/build/html/_static/fonts/Lato/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_static/fonts/Lato/lato-bolditalic.eot` & `netqasm-0.9.1/docs/build/html/_static/fonts/Lato/lato-bolditalic.eot`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_static/fonts/Lato/lato-bolditalic.ttf` & `netqasm-0.9.1/docs/build/html/_static/fonts/Lato/lato-bolditalic.ttf`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_static/fonts/Lato/lato-bolditalic.woff` & `netqasm-0.9.1/docs/build/html/_static/fonts/Lato/lato-bolditalic.woff`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_static/fonts/Lato/lato-bolditalic.woff2` & `netqasm-0.9.1/docs/build/html/_static/fonts/Lato/lato-bolditalic.woff2`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_static/fonts/Lato/lato-italic.eot` & `netqasm-0.9.1/docs/build/html/_static/fonts/Lato/lato-italic.eot`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_static/fonts/Lato/lato-italic.ttf` & `netqasm-0.9.1/docs/build/html/_static/fonts/Lato/lato-italic.ttf`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_static/fonts/Lato/lato-italic.woff` & `netqasm-0.9.1/docs/build/html/_static/fonts/Lato/lato-italic.woff`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_static/fonts/Lato/lato-italic.woff2` & `netqasm-0.9.1/docs/build/html/_static/fonts/Lato/lato-italic.woff2`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_static/fonts/Lato/lato-regular.eot` & `netqasm-0.9.1/docs/build/html/_static/fonts/Lato/lato-regular.eot`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_static/fonts/Lato/lato-regular.ttf` & `netqasm-0.9.1/docs/build/html/_static/fonts/Lato/lato-regular.ttf`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_static/fonts/Lato/lato-regular.woff` & `netqasm-0.9.1/docs/build/html/_static/fonts/Lato/lato-regular.woff`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_static/fonts/Lato/lato-regular.woff2` & `netqasm-0.9.1/docs/build/html/_static/fonts/Lato/lato-regular.woff2`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_static/fonts/Lato-Bold.ttf` & `netqasm-0.9.1/docs/build/html/_static/fonts/Lato-Bold.ttf`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_static/fonts/Lato-Regular.ttf` & `netqasm-0.9.1/docs/build/html/_static/fonts/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_static/fonts/RobotoSlab/roboto-slab-v7-bold.eot` & `netqasm-0.9.1/docs/build/html/_static/fonts/RobotoSlab/roboto-slab-v7-bold.eot`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_static/fonts/RobotoSlab/roboto-slab-v7-bold.ttf` & `netqasm-0.9.1/docs/build/html/_static/fonts/RobotoSlab/roboto-slab-v7-bold.ttf`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_static/fonts/RobotoSlab/roboto-slab-v7-bold.woff` & `netqasm-0.9.1/docs/build/html/_static/fonts/RobotoSlab/roboto-slab-v7-bold.woff`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_static/fonts/RobotoSlab/roboto-slab-v7-bold.woff2` & `netqasm-0.9.1/docs/build/html/_static/fonts/RobotoSlab/roboto-slab-v7-bold.woff2`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_static/fonts/RobotoSlab/roboto-slab-v7-regular.eot` & `netqasm-0.9.1/docs/build/html/_static/fonts/RobotoSlab/roboto-slab-v7-regular.eot`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_static/fonts/RobotoSlab/roboto-slab-v7-regular.ttf` & `netqasm-0.9.1/docs/build/html/_static/fonts/RobotoSlab/roboto-slab-v7-regular.ttf`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_static/fonts/RobotoSlab/roboto-slab-v7-regular.woff` & `netqasm-0.9.1/docs/build/html/_static/fonts/RobotoSlab/roboto-slab-v7-regular.woff`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_static/fonts/RobotoSlab/roboto-slab-v7-regular.woff2` & `netqasm-0.9.1/docs/build/html/_static/fonts/RobotoSlab/roboto-slab-v7-regular.woff2`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_static/fonts/RobotoSlab-Bold.ttf` & `netqasm-0.9.1/docs/build/html/_static/fonts/RobotoSlab-Bold.ttf`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_static/fonts/RobotoSlab-Regular.ttf` & `netqasm-0.9.1/docs/build/html/_static/fonts/RobotoSlab-Regular.ttf`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_static/fonts/fontawesome-webfont.eot` & `netqasm-0.9.1/docs/build/html/_static/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_static/fonts/fontawesome-webfont.svg` & `netqasm-0.9.1/docs/build/html/_static/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_static/fonts/fontawesome-webfont.ttf` & `netqasm-0.9.1/docs/build/html/_static/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_static/fonts/fontawesome-webfont.woff` & `netqasm-0.9.1/docs/build/html/_static/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_static/fonts/fontawesome-webfont.woff2` & `netqasm-0.9.1/docs/build/html/_static/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_static/jquery-3.5.1.js` & `netqasm-0.9.1/docs/build/html/_static/jquery-3.5.1.js`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_static/jquery.js` & `netqasm-0.9.1/docs/build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_static/js/badge_only.js` & `netqasm-0.9.1/docs/build/html/_static/js/badge_only.js`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_static/js/html5shiv-printshiv.min.js` & `netqasm-0.9.1/docs/build/html/_static/js/html5shiv-printshiv.min.js`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_static/js/html5shiv.min.js` & `netqasm-0.9.1/docs/build/html/_static/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_static/js/modernizr.min.js` & `netqasm-0.9.1/docs/build/html/_static/js/modernizr.min.js`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_static/js/theme.js` & `netqasm-0.9.1/docs/build/html/_static/js/theme.js`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_static/language_data.js` & `netqasm-0.9.1/docs/build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_static/pygments.css` & `netqasm-0.9.1/docs/build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_static/searchtools.js` & `netqasm-0.9.1/docs/build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_static/underscore-1.12.0.js` & `netqasm-0.9.1/docs/build/html/_static/underscore-1.12.0.js`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/_static/underscore.js` & `netqasm-0.9.1/docs/build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/api_backend/netqasm.backend.executor.html` & `netqasm-0.9.1/docs/build/html/api_backend/netqasm.backend.executor.html`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/api_backend/netqasm.backend.messages.html` & `netqasm-0.9.1/docs/build/html/api_backend/netqasm.backend.messages.html`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/api_backend/netqasm.backend.network_stack.html` & `netqasm-0.9.1/docs/build/html/api_backend/netqasm.backend.network_stack.html`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/api_backend/netqasm.backend.qnodeos.html` & `netqasm-0.9.1/docs/build/html/api_backend/netqasm.backend.qnodeos.html`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/api_lang/netqasm.lang.encoding.html` & `netqasm-0.9.1/docs/build/html/api_lang/netqasm.lang.encoding.html`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/api_lang/netqasm.lang.instr.html` & `netqasm-0.9.1/docs/build/html/api_lang/netqasm.lang.instr.html`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/api_lang/netqasm.lang.ir.html` & `netqasm-0.9.1/docs/build/html/api_lang/netqasm.lang.ir.html`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/api_lang/netqasm.lang.operand.html` & `netqasm-0.9.1/docs/build/html/api_lang/netqasm.lang.operand.html`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/api_lang/netqasm.lang.parsing.html` & `netqasm-0.9.1/docs/build/html/api_lang/netqasm.lang.parsing.html`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/api_lang/netqasm.lang.subroutine.html` & `netqasm-0.9.1/docs/build/html/api_lang/netqasm.lang.subroutine.html`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/api_lang/netqasm.lang.symbols.html` & `netqasm-0.9.1/docs/build/html/api_lang/netqasm.lang.symbols.html`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/api_logging/netqasm.logging.glob.html` & `netqasm-0.9.1/docs/build/html/api_logging/netqasm.logging.glob.html`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/api_logging/netqasm.logging.output.html` & `netqasm-0.9.1/docs/build/html/api_logging/netqasm.logging.output.html`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/api_root.html` & `netqasm-0.9.1/docs/build/html/api_root.html`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/api_runtime/netqasm.runtime.app_config.html` & `netqasm-0.9.1/docs/build/html/api_runtime/netqasm.runtime.app_config.html`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/api_runtime/netqasm.runtime.application.html` & `netqasm-0.9.1/docs/build/html/api_runtime/netqasm.runtime.application.html`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/api_runtime/netqasm.runtime.cli.html` & `netqasm-0.9.1/docs/build/html/api_runtime/netqasm.runtime.cli.html`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/api_runtime/netqasm.runtime.debug.html` & `netqasm-0.9.1/docs/build/html/api_runtime/netqasm.runtime.debug.html`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/api_runtime/netqasm.runtime.env.html` & `netqasm-0.9.1/docs/build/html/api_runtime/netqasm.runtime.env.html`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/api_runtime/netqasm.runtime.hardware.html` & `netqasm-0.9.1/docs/build/html/api_runtime/netqasm.runtime.hardware.html`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/api_runtime/netqasm.runtime.interface.html` & `netqasm-0.9.1/docs/build/html/api_runtime/netqasm.runtime.interface.html`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/api_runtime/netqasm.runtime.process_logs.html` & `netqasm-0.9.1/docs/build/html/api_runtime/netqasm.runtime.process_logs.html`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/api_runtime/netqasm.runtime.settings.html` & `netqasm-0.9.1/docs/build/html/api_runtime/netqasm.runtime.settings.html`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/api_sdk/netqasm.sdk.builder.html` & `netqasm-0.9.1/docs/build/html/api_sdk/netqasm.sdk.builder.html`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/api_sdk/netqasm.sdk.classical_communication.html` & `netqasm-0.9.1/docs/build/html/api_sdk/netqasm.sdk.classical_communication.html`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/api_sdk/netqasm.sdk.compiling.html` & `netqasm-0.9.1/docs/build/html/api_sdk/netqasm.sdk.compiling.html`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/api_sdk/netqasm.sdk.config.html` & `netqasm-0.9.1/docs/build/html/api_sdk/netqasm.sdk.config.html`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/api_sdk/netqasm.sdk.connection.html` & `netqasm-0.9.1/docs/build/html/api_sdk/netqasm.sdk.connection.html`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/api_sdk/netqasm.sdk.epr_socket.html` & `netqasm-0.9.1/docs/build/html/api_sdk/netqasm.sdk.epr_socket.html`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/api_sdk/netqasm.sdk.external.html` & `netqasm-0.9.1/docs/build/html/api_sdk/netqasm.sdk.external.html`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/api_sdk/netqasm.sdk.futures.html` & `netqasm-0.9.1/docs/build/html/api_sdk/netqasm.sdk.futures.html`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/api_sdk/netqasm.sdk.network.html` & `netqasm-0.9.1/docs/build/html/api_sdk/netqasm.sdk.network.html`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/api_sdk/netqasm.sdk.progress_bar.html` & `netqasm-0.9.1/docs/build/html/api_sdk/netqasm.sdk.progress_bar.html`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/api_sdk/netqasm.sdk.qubit.html` & `netqasm-0.9.1/docs/build/html/api_sdk/netqasm.sdk.qubit.html`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/api_sdk/netqasm.sdk.shared_memory.html` & `netqasm-0.9.1/docs/build/html/api_sdk/netqasm.sdk.shared_memory.html`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/api_sdk/netqasm.sdk.toolbox.html` & `netqasm-0.9.1/docs/build/html/api_sdk/netqasm.sdk.toolbox.html`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/api_util/netqasm.util.error.html` & `netqasm-0.9.1/docs/build/html/api_util/netqasm.util.error.html`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/api_util/netqasm.util.log.html` & `netqasm-0.9.1/docs/build/html/api_util/netqasm.util.log.html`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/api_util/netqasm.util.quantum_gates.html` & `netqasm-0.9.1/docs/build/html/api_util/netqasm.util.quantum_gates.html`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/api_util/netqasm.util.states.html` & `netqasm-0.9.1/docs/build/html/api_util/netqasm.util.states.html`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/api_util/netqasm.util.string.html` & `netqasm-0.9.1/docs/build/html/api_util/netqasm.util.string.html`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/api_util/netqasm.util.thread.html` & `netqasm-0.9.1/docs/build/html/api_util/netqasm.util.thread.html`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/api_util/netqasm.util.yaml.html` & `netqasm-0.9.1/docs/build/html/api_util/netqasm.util.yaml.html`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/genindex.html` & `netqasm-0.9.1/docs/build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/index.html` & `netqasm-0.9.1/docs/build/html/index.html`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/installation.html` & `netqasm-0.9.1/docs/build/html/installation.html`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/known_issues.html` & `netqasm-0.9.1/docs/build/html/known_issues.html`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/netqasm.backend.html` & `netqasm-0.9.1/docs/build/html/netqasm.backend.html`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/netqasm.examples.html` & `netqasm-0.9.1/docs/build/html/netqasm.examples.html`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/netqasm.lang.html` & `netqasm-0.9.1/docs/build/html/netqasm.lang.html`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/netqasm.logging.html` & `netqasm-0.9.1/docs/build/html/netqasm.logging.html`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/netqasm.runtime.html` & `netqasm-0.9.1/docs/build/html/netqasm.runtime.html`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/netqasm.sdk.html` & `netqasm-0.9.1/docs/build/html/netqasm.sdk.html`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/netqasm.util.html` & `netqasm-0.9.1/docs/build/html/netqasm.util.html`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/objects.inv` & `netqasm-0.9.1/docs/build/html/objects.inv`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/py-modindex.html` & `netqasm-0.9.1/docs/build/html/py-modindex.html`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/quickstart/file_structure.html` & `netqasm-0.9.1/docs/build/html/quickstart/file_structure.html`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/quickstart/first-app.html` & `netqasm-0.9.1/docs/build/html/quickstart/first-app.html`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/quickstart/modules.html` & `netqasm-0.9.1/docs/build/html/quickstart/modules.html`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/quickstart/using-sdk.html` & `netqasm-0.9.1/docs/build/html/quickstart/using-sdk.html`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/quickstart.html` & `netqasm-0.9.1/docs/build/html/quickstart.html`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/search.html` & `netqasm-0.9.1/docs/build/html/search.html`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/build/html/searchindex.js` & `netqasm-0.9.1/docs/build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/conf.py` & `netqasm-0.9.1/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "netqasm"
 copyright = "2021, QuTech"
 author = "QuTech"
 
 # The full version, including alpha/beta/rc tags
-release = "0.9.0"
+release = "0.9.1"
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `netqasm-0.9.0/docs/index.rst` & `netqasm-0.9.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/installation.rst` & `netqasm-0.9.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/make.bat` & `netqasm-0.9.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/netqasm.sdk.rst` & `netqasm-0.9.1/docs/netqasm.sdk.rst`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/quickstart/file_structure.rst` & `netqasm-0.9.1/docs/quickstart/file_structure.rst`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/quickstart/first-app.rst` & `netqasm-0.9.1/docs/quickstart/first-app.rst`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/quickstart/modules.rst` & `netqasm-0.9.1/docs/quickstart/modules.rst`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/quickstart/using-sdk.rst` & `netqasm-0.9.1/docs/quickstart/using-sdk.rst`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/docs/quickstart.rst` & `netqasm-0.9.1/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/backend/executor.py` & `netqasm-0.9.1/netqasm/backend/executor.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/backend/messages.py` & `netqasm-0.9.1/netqasm/backend/messages.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/backend/network_stack.py` & `netqasm-0.9.1/netqasm/backend/network_stack.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/backend/qnodeos.py` & `netqasm-0.9.1/netqasm/backend/qnodeos.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/examples/apps/anonymous_transmission/src/protocol.py` & `netqasm-0.9.1/netqasm/examples/apps/anonymous_transmission/src/protocol.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/examples/apps/anonymous_transmission/src/sub_protocols.py` & `netqasm-0.9.1/netqasm/examples/apps/anonymous_transmission/src/sub_protocols.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/examples/apps/bb84/README.md` & `netqasm-0.9.1/netqasm/examples/apps/bb84/README.md`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/examples/apps/bb84/app_alice.py` & `netqasm-0.9.1/netqasm/examples/apps/bb84/app_alice.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/examples/apps/bb84/app_bob.py` & `netqasm-0.9.1/netqasm/examples/apps/bb84/app_bob.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/examples/apps/bb84/results_config.json` & `netqasm-0.9.1/netqasm/examples/apps/bb84/results_config.json`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/examples/apps/blind_grover/README.md` & `netqasm-0.9.1/netqasm/examples/apps/blind_grover/README.md`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/examples/apps/blind_grover/app_client.py` & `netqasm-0.9.1/netqasm/examples/apps/blind_grover/app_client.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/examples/apps/blind_grover/app_server.py` & `netqasm-0.9.1/netqasm/examples/apps/blind_grover/app_server.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/examples/apps/blind_rotation/README.md` & `netqasm-0.9.1/netqasm/examples/apps/blind_rotation/README.md`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/examples/apps/blind_rotation/app_client.py` & `netqasm-0.9.1/netqasm/examples/apps/blind_rotation/app_client.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/examples/apps/blind_rotation/app_server.py` & `netqasm-0.9.1/netqasm/examples/apps/blind_rotation/app_server.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/examples/apps/chsh/README.md` & `netqasm-0.9.1/netqasm/examples/apps/chsh/README.md`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/examples/apps/chsh/app_alice.py` & `netqasm-0.9.1/netqasm/examples/apps/chsh/app_alice.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/examples/apps/chsh/app_bob.py` & `netqasm-0.9.1/netqasm/examples/apps/chsh/app_bob.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/examples/apps/chsh/app_repeater.py` & `netqasm-0.9.1/netqasm/examples/apps/chsh/app_repeater.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/examples/apps/chsh/network.yaml` & `netqasm-0.9.1/netqasm/examples/apps/chsh/network.yaml`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/examples/apps/dist_cnot/README.md` & `netqasm-0.9.1/netqasm/examples/apps/dist_cnot/README.md`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/examples/apps/dist_cnot/app_controller.py` & `netqasm-0.9.1/netqasm/examples/apps/dist_cnot/app_controller.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/examples/apps/dist_cnot/app_target.py` & `netqasm-0.9.1/netqasm/examples/apps/dist_cnot/app_target.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/examples/apps/link_layer_ck/app_client.py` & `netqasm-0.9.1/netqasm/examples/apps/link_layer_ck/app_client.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/examples/apps/link_layer_ck/app_server.py` & `netqasm-0.9.1/netqasm/examples/apps/link_layer_ck/app_server.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/examples/apps/link_layer_md/app_client.py` & `netqasm-0.9.1/netqasm/examples/apps/link_layer_md/app_client.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/examples/apps/link_layer_md/app_server.py` & `netqasm-0.9.1/netqasm/examples/apps/link_layer_md/app_server.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/examples/apps/magic_square/README.md` & `netqasm-0.9.1/netqasm/examples/apps/magic_square/README.md`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/examples/apps/magic_square/app_player1.py` & `netqasm-0.9.1/netqasm/examples/apps/magic_square/app_player1.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/examples/apps/magic_square/app_player2.py` & `netqasm-0.9.1/netqasm/examples/apps/magic_square/app_player2.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/examples/apps/multiple_files/app_alice.py` & `netqasm-0.9.1/netqasm/examples/apps/multiple_files/app_alice.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/examples/apps/multiple_files/app_bob.py` & `netqasm-0.9.1/netqasm/examples/apps/multiple_files/app_bob.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/examples/apps/single_node/app_alice.py` & `netqasm-0.9.1/netqasm/examples/apps/single_node/app_alice.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/examples/apps/teleport/app_receiver.py` & `netqasm-0.9.1/netqasm/examples/apps/teleport/app_receiver.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/examples/apps/teleport/app_sender.py` & `netqasm-0.9.1/netqasm/examples/apps/teleport/app_sender.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/examples/apps/teleport/results_config.json` & `netqasm-0.9.1/netqasm/examples/apps/teleport/results_config.json`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/examples/apps/three_nodes/app_alice.py` & `netqasm-0.9.1/netqasm/examples/apps/three_nodes/app_alice.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/examples/apps/three_nodes/app_bob.py` & `netqasm-0.9.1/netqasm/examples/apps/three_nodes/app_bob.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/examples/apps/three_nodes/app_charlie.py` & `netqasm-0.9.1/netqasm/examples/apps/three_nodes/app_charlie.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/examples/apps/three_nodes/network.yaml` & `netqasm-0.9.1/netqasm/examples/apps/three_nodes/network.yaml`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/examples/lib/bqc.py` & `netqasm-0.9.1/netqasm/examples/lib/bqc.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/examples/run_examples.py` & `netqasm-0.9.1/netqasm/examples/run_examples.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/examples/sdk_compilation/example_bb84.py` & `netqasm-0.9.1/netqasm/examples/sdk_compilation/example_bb84.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/examples/sdk_compilation/example_enumerate.py` & `netqasm-0.9.1/netqasm/examples/sdk_compilation/example_enumerate.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/examples/sdk_compilation/example_loop.py` & `netqasm-0.9.1/netqasm/examples/sdk_compilation/example_loop.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/examples/sdk_compilation/example_post_epr.py` & `netqasm-0.9.1/netqasm/examples/sdk_compilation/example_post_epr.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/examples/sdk_compilation/example_rsp.py` & `netqasm-0.9.1/netqasm/examples/sdk_compilation/example_rsp.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/examples/sdk_compilation/example_simple_loop.py` & `netqasm-0.9.1/netqasm/examples/sdk_compilation/example_simple_loop.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/lang/encoding.py` & `netqasm-0.9.1/netqasm/lang/encoding.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/lang/instr/base.py` & `netqasm-0.9.1/netqasm/lang/instr/base.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/lang/instr/core.py` & `netqasm-0.9.1/netqasm/lang/instr/core.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/lang/instr/flavour.py` & `netqasm-0.9.1/netqasm/lang/instr/flavour.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/lang/instr/nv.py` & `netqasm-0.9.1/netqasm/lang/instr/nv.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/lang/instr/vanilla.py` & `netqasm-0.9.1/netqasm/lang/instr/vanilla.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/lang/ir.py` & `netqasm-0.9.1/netqasm/lang/ir.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/lang/operand.py` & `netqasm-0.9.1/netqasm/lang/operand.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/lang/parsing/binary.py` & `netqasm-0.9.1/netqasm/lang/parsing/binary.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/lang/parsing/text.py` & `netqasm-0.9.1/netqasm/lang/parsing/text.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/lang/subroutine.py` & `netqasm-0.9.1/netqasm/lang/subroutine.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/logging/glob.py` & `netqasm-0.9.1/netqasm/logging/glob.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/logging/output.py` & `netqasm-0.9.1/netqasm/logging/output.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/qlink_compat.py` & `netqasm-0.9.1/netqasm/qlink_compat.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/runtime/application.py` & `netqasm-0.9.1/netqasm/runtime/application.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/runtime/cli.py` & `netqasm-0.9.1/netqasm/runtime/cli.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/runtime/env.py` & `netqasm-0.9.1/netqasm/runtime/env.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/runtime/hardware.py` & `netqasm-0.9.1/netqasm/runtime/hardware.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/runtime/interface/config.py` & `netqasm-0.9.1/netqasm/runtime/interface/config.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/runtime/interface/logging.py` & `netqasm-0.9.1/netqasm/runtime/interface/logging.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/runtime/process_logs.py` & `netqasm-0.9.1/netqasm/runtime/process_logs.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/runtime/runtime_mgr.py` & `netqasm-0.9.1/netqasm/runtime/runtime_mgr.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/runtime/settings.py` & `netqasm-0.9.1/netqasm/runtime/settings.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/sdk/build_epr.py` & `netqasm-0.9.1/netqasm/sdk/build_epr.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/sdk/build_nv.py` & `netqasm-0.9.1/netqasm/sdk/build_nv.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/sdk/build_types.py` & `netqasm-0.9.1/netqasm/sdk/build_types.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/sdk/builder.py` & `netqasm-0.9.1/netqasm/sdk/builder.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/sdk/classical_communication/broadcast_channel.py` & `netqasm-0.9.1/netqasm/sdk/classical_communication/broadcast_channel.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/sdk/classical_communication/socket.py` & `netqasm-0.9.1/netqasm/sdk/classical_communication/socket.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/sdk/classical_communication/thread_socket/socket.py` & `netqasm-0.9.1/netqasm/sdk/classical_communication/thread_socket/socket.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/sdk/classical_communication/thread_socket/socket_hub.py` & `netqasm-0.9.1/netqasm/sdk/classical_communication/thread_socket/socket_hub.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/sdk/compiling.py` & `netqasm-0.9.1/netqasm/sdk/compiling.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/sdk/connection.py` & `netqasm-0.9.1/netqasm/sdk/connection.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/sdk/constraint.py` & `netqasm-0.9.1/netqasm/sdk/constraint.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/sdk/epr_socket.py` & `netqasm-0.9.1/netqasm/sdk/epr_socket.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/sdk/external.py` & `netqasm-0.9.1/netqasm/sdk/external.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/sdk/futures.py` & `netqasm-0.9.1/netqasm/sdk/futures.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/sdk/memmgr.py` & `netqasm-0.9.1/netqasm/sdk/memmgr.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/sdk/network.py` & `netqasm-0.9.1/netqasm/sdk/network.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/sdk/progress_bar.py` & `netqasm-0.9.1/netqasm/sdk/progress_bar.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/sdk/qubit.py` & `netqasm-0.9.1/netqasm/sdk/qubit.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/sdk/shared_memory.py` & `netqasm-0.9.1/netqasm/sdk/shared_memory.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/sdk/toolbox/gates.py` & `netqasm-0.9.1/netqasm/sdk/toolbox/gates.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/sdk/toolbox/measurements.py` & `netqasm-0.9.1/netqasm/sdk/toolbox/measurements.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/sdk/toolbox/multi_node.py` & `netqasm-0.9.1/netqasm/sdk/toolbox/multi_node.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/sdk/toolbox/sim_states.py` & `netqasm-0.9.1/netqasm/sdk/toolbox/sim_states.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/sdk/toolbox/state_prep.py` & `netqasm-0.9.1/netqasm/sdk/toolbox/state_prep.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/util/log.py` & `netqasm-0.9.1/netqasm/util/log.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/util/quantum_gates.py` & `netqasm-0.9.1/netqasm/util/quantum_gates.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/util/states.py` & `netqasm-0.9.1/netqasm/util/states.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/util/string.py` & `netqasm-0.9.1/netqasm/util/string.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm/util/thread.py` & `netqasm-0.9.1/netqasm/util/thread.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/netqasm.egg-info/PKG-INFO` & `netqasm-0.9.1/netqasm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: netqasm
-Version: 0.9.0
+Version: 0.9.1
 Summary: Tool for parsing, encoding, decoding and executing NetQASM applications
 Home-page: https://github.com/QuTech-Delft/netqasm
 Author: Axel Dahlberg, Bart van der Vecht
 Author-email: b.vandervecht@tudelft.nl
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# NetQASM (0.9.0)
+# NetQASM (0.9.1)
 [![Documentation](https://readthedocs.org/projects/netqasm/badge/?version=latest)](https://netqasm.readthedocs.io/en/latest/?badge=latest)
 
 Utilities for writing, compiling, and running quantum network applications.
 
 ## Intro
 NetQASM is an instruction set architecture that allows one to interface with quantum network controllers and run applications on a quantum network. Applications may be written directly in the NetQASM language, which resembles assembly code. However, this package also provides an SDK which allows writing application code in Python.
 For the paper introducing NetQASM, see [here](https://arxiv.org/abs/2111.09823).
```

### Comparing `netqasm-0.9.0/netqasm.egg-info/SOURCES.txt` & `netqasm-0.9.1/netqasm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/setup.cfg` & `netqasm-0.9.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = netqasm
-version = 0.9.0
+version = 0.9.1
 author = Axel Dahlberg, Bart van der Vecht
 author-email = b.vandervecht@tudelft.nl
 description = Tool for parsing, encoding, decoding and executing NetQASM applications
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
 home-page = https://github.com/QuTech-Delft/netqasm
```

### Comparing `netqasm-0.9.0/setup.py` & `netqasm-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/tests/test_builder.py` & `netqasm-0.9.1/tests/test_builder.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/tests/test_cli.py` & `netqasm-0.9.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/tests/test_compiling.py` & `netqasm-0.9.1/tests/test_compiling.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/tests/test_encoding.py` & `netqasm-0.9.1/tests/test_encoding.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/tests/test_executor.py` & `netqasm-0.9.1/tests/test_executor.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/tests/test_external/test_examples.py` & `netqasm-0.9.1/tests/test_external/test_examples.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/tests/test_external/test_sdk/test_create_epr.py` & `netqasm-0.9.1/tests/test_external/test_sdk/test_create_epr.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/tests/test_external/test_sdk/test_create_epr_m.py` & `netqasm-0.9.1/tests/test_external/test_sdk/test_create_epr_m.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/tests/test_external/test_sdk/test_enumerate.py` & `netqasm-0.9.1/tests/test_external/test_sdk/test_enumerate.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/tests/test_external/test_sdk/test_foreach.py` & `netqasm-0.9.1/tests/test_external/test_sdk/test_foreach.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/tests/test_external/test_sdk/test_measure.py` & `netqasm-0.9.1/tests/test_external/test_sdk/test_measure.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/tests/test_external/test_sdk/test_measure_if_conn.py` & `netqasm-0.9.1/tests/test_external/test_sdk/test_measure_if_conn.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/tests/test_external/test_sdk/test_measure_if_future.py` & `netqasm-0.9.1/tests/test_external/test_sdk/test_measure_if_future.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/tests/test_external/test_sdk/test_measure_loop.py` & `netqasm-0.9.1/tests/test_external/test_sdk/test_measure_loop.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/tests/test_external/test_sdk/test_measure_loop_context.py` & `netqasm-0.9.1/tests/test_external/test_sdk/test_measure_loop_context.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/tests/test_external/test_sdk/test_nested_loop.py` & `netqasm-0.9.1/tests/test_external/test_sdk/test_nested_loop.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/tests/test_external/test_sdk/test_new_array.py` & `netqasm-0.9.1/tests/test_external/test_sdk/test_new_array.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/tests/test_external/test_sdk/test_post_epr.py` & `netqasm-0.9.1/tests/test_external/test_sdk/test_post_epr.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/tests/test_external/test_sdk/test_post_epr_context.py` & `netqasm-0.9.1/tests/test_external/test_sdk/test_post_epr_context.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/tests/test_external/test_sdk/test_rotations.py` & `netqasm-0.9.1/tests/test_external/test_sdk/test_rotations.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/tests/test_external/test_sdk/test_teleport.py` & `netqasm-0.9.1/tests/test_external/test_sdk/test_teleport.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/tests/test_external/test_sdk/test_teleport_without_corrections.py` & `netqasm-0.9.1/tests/test_external/test_sdk/test_teleport_without_corrections.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/tests/test_external/test_sdk/test_two_nodes.py` & `netqasm-0.9.1/tests/test_external/test_sdk/test_two_nodes.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/tests/test_external/test_toolbox.py` & `netqasm-0.9.1/tests/test_external/test_toolbox.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/tests/test_parsing/test_binary.py` & `netqasm-0.9.1/tests/test_parsing/test_binary.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/tests/test_parsing/test_text.py` & `netqasm-0.9.1/tests/test_parsing/test_text.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/tests/test_sdk/test_classical_communication.py` & `netqasm-0.9.1/tests/test_sdk/test_classical_communication.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/tests/test_sdk/test_connection.py` & `netqasm-0.9.1/tests/test_sdk/test_connection.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/tests/test_sdk/test_future.py` & `netqasm-0.9.1/tests/test_sdk/test_future.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/tests/test_states_util.py` & `netqasm-0.9.1/tests/test_states_util.py`

 * *Files identical despite different names*

### Comparing `netqasm-0.9.0/tests/test_string_util.py` & `netqasm-0.9.1/tests/test_string_util.py`

 * *Files identical despite different names*

