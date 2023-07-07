# Comparing `tmp/SELDOMpy-0.9.6.tar.gz` & `tmp/SELDOMpy-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\SELDOMpy-0.9.6.tar", last modified: Fri Jul  7 14:20:39 2023, max compression
+gzip compressed data, was "dist\SELDOMpy-0.9.7.tar", last modified: Fri Jul  7 14:24:17 2023, max compression
```

## Comparing `SELDOMpy-0.9.6.tar` & `SELDOMpy-0.9.7.tar`

### file list

```diff
@@ -1,175 +1,135 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 14:20:39.969282 SELDOMpy-0.9.6/
--rw-rw-rw-   0        0        0    35149 2023-07-05 16:32:35.000000 SELDOMpy-0.9.6/LICENSE.txt
--rw-rw-rw-   0        0        0      596 2023-07-07 14:20:18.000000 SELDOMpy-0.9.6/MANIFEST.in
--rw-rw-rw-   0        0        0     4171 2023-07-07 14:20:39.969282 SELDOMpy-0.9.6/PKG-INFO
--rw-rw-rw-   0        0        0     3446 2023-07-06 08:12:36.000000 SELDOMpy-0.9.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-07 14:20:39.662304 SELDOMpy-0.9.6/SELDOMpy/
--rw-rw-rw-   0        0        0      490 2023-07-06 11:23:03.000000 SELDOMpy-0.9.6/SELDOMpy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-07 14:20:39.652266 SELDOMpy-0.9.6/SELDOMpy/examples/
-drwxrwxrwx   0        0        0        0 2023-07-07 14:20:39.714250 SELDOMpy-0.9.6/SELDOMpy/examples/MAPK/
--rw-rw-rw-   0        0        0    13667 2023-04-19 10:00:19.000000 SELDOMpy-0.9.6/SELDOMpy/examples/MAPK/MAPK.xlsx
--rw-rw-rw-   0        0        0     5830 2023-07-07 11:25:38.000000 SELDOMpy-0.9.6/SELDOMpy/examples/MAPK/MAPK_training_and_reduce.py
--rw-rw-rw-   0        0        0    10464 2023-07-07 13:51:52.000000 SELDOMpy-0.9.6/SELDOMpy/examples/MAPK/MAPK_training_and_reduce_pyPESTO.py
-drwxrwxrwx   0        0        0        0 2023-07-07 14:20:39.716250 SELDOMpy-0.9.6/SELDOMpy/examples/SP/
--rw-rw-rw-   0        0        0    23018 2023-06-21 18:44:38.000000 SELDOMpy-0.9.6/SELDOMpy/examples/SP/SP.xlsx
--rw-rw-rw-   0        0        0     6011 2023-07-07 11:49:56.000000 SELDOMpy-0.9.6/SELDOMpy/examples/SP/SP_training_and_reduce.py
--rw-rw-rw-   0        0        0    10661 2023-07-07 13:32:38.000000 SELDOMpy-0.9.6/SELDOMpy/examples/SP/SP_training_and_reduce_pyPESTO.py
-drwxrwxrwx   0        0        0        0 2023-07-07 14:20:39.724250 SELDOMpy-0.9.6/SELDOMpy/functions/
--rw-rw-rw-   0        0        0     1799 2023-07-06 13:38:27.000000 SELDOMpy-0.9.6/SELDOMpy/functions/buildmim.py
--rw-rw-rw-   0        0        0     1280 2023-07-07 07:34:51.000000 SELDOMpy-0.9.6/SELDOMpy/functions/extras.py
--rw-rw-rw-   0        0        0     4037 2023-07-07 11:47:15.000000 SELDOMpy-0.9.6/SELDOMpy/functions/gen_exps.py
--rw-rw-rw-   0        0        0     4860 2023-07-07 07:34:51.000000 SELDOMpy-0.9.6/SELDOMpy/functions/getLBODEmodel.py
--rw-rw-rw-   0        0        0     3156 2023-07-07 07:34:50.000000 SELDOMpy-0.9.6/SELDOMpy/functions/getRandomLBODEmodel.py
--rw-rw-rw-   0        0        0     2313 2023-07-07 11:11:37.000000 SELDOMpy-0.9.6/SELDOMpy/functions/optimization.py
--rw-rw-rw-   0        0        0     1509 2023-07-07 07:39:33.000000 SELDOMpy-0.9.6/SELDOMpy/functions/plot_results.py
--rw-rw-rw-   0        0        0     2748 2023-07-07 07:41:41.000000 SELDOMpy-0.9.6/SELDOMpy/functions/reduce_fun.py
--rw-rw-rw-   0        0        0     3802 2023-07-07 07:48:40.000000 SELDOMpy-0.9.6/SELDOMpy/functions/simulate_logic_based_ode.py
--rw-rw-rw-   0        0        0     3595 2023-07-07 07:52:38.000000 SELDOMpy-0.9.6/SELDOMpy/functions/simulate_logic_based_ode_obs.py
-drwxrwxrwx   0        0        0        0 2023-07-07 14:20:39.654297 SELDOMpy-0.9.6/SELDOMpy/include/
-drwxrwxrwx   0        0        0        0 2023-07-07 14:20:39.730250 SELDOMpy-0.9.6/SELDOMpy/include/include_amigo/
--rw-rw-rw-   0        0        0        4 2022-12-07 11:24:12.000000 SELDOMpy-0.9.6/SELDOMpy/include/include_amigo/AMIGO_hdf5.h
--rw-rw-rw-   0        0        0     3769 2022-12-07 11:24:12.000000 SELDOMpy-0.9.6/SELDOMpy/include/include_amigo/AMIGO_model.h
--rw-rw-rw-   0        0        0      442 2022-12-07 11:24:12.000000 SELDOMpy-0.9.6/SELDOMpy/include/include_amigo/AMIGO_model_stats.h
--rw-rw-rw-   0        0        0     1822 2022-12-07 11:24:12.000000 SELDOMpy-0.9.6/SELDOMpy/include/include_amigo/AMIGO_problem.h
--rw-rw-rw-   0        0        0      287 2022-12-07 11:24:12.000000 SELDOMpy-0.9.6/SELDOMpy/include/include_amigo/amigoJAC.h
--rw-rw-rw-   0        0        0       24 2022-12-07 11:24:12.000000 SELDOMpy-0.9.6/SELDOMpy/include/include_amigo/amigoRHS.h
--rw-rw-rw-   0        0        0      171 2022-12-07 11:24:12.000000 SELDOMpy-0.9.6/SELDOMpy/include/include_amigo/amigoSensRHS.h
--rw-rw-rw-   0        0        0      164 2022-12-07 11:24:12.000000 SELDOMpy-0.9.6/SELDOMpy/include/include_amigo/simulate_amigo_model.h
-drwxrwxrwx   0        0        0        0 2023-07-07 14:20:39.655282 SELDOMpy-0.9.6/SELDOMpy/include/include_cvodes/
-drwxrwxrwx   0        0        0        0 2023-07-07 14:20:39.742283 SELDOMpy-0.9.6/SELDOMpy/include/include_cvodes/cvodes/
--rw-rw-rw-   0        0        0    84971 2022-12-07 11:24:12.000000 SELDOMpy-0.9.6/SELDOMpy/include/include_cvodes/cvodes/cvodes.h
--rw-rw-rw-   0        0        0     2442 2022-12-07 11:24:12.000000 SELDOMpy-0.9.6/SELDOMpy/include/include_cvodes/cvodes/cvodes_band.h
--rw-rw-rw-   0        0        0     6547 2022-12-07 11:24:12.000000 SELDOMpy-0.9.6/SELDOMpy/include/include_cvodes/cvodes/cvodes_bandpre.h
--rw-rw-rw-   0        0        0    13259 2022-12-07 11:24:12.000000 SELDOMpy-0.9.6/SELDOMpy/include/include_cvodes/cvodes/cvodes_bbdpre.h
--rw-rw-rw-   0        0        0     2122 2022-12-07 11:24:12.000000 SELDOMpy-0.9.6/SELDOMpy/include/include_cvodes/cvodes/cvodes_dense.h
--rw-rw-rw-   0        0        0     4845 2022-12-07 11:24:12.000000 SELDOMpy-0.9.6/SELDOMpy/include/include_cvodes/cvodes/cvodes_diag.h
--rw-rw-rw-   0        0        0    14031 2022-12-07 11:24:12.000000 SELDOMpy-0.9.6/SELDOMpy/include/include_cvodes/cvodes/cvodes_direct.h
--rw-rw-rw-   0        0        0     3732 2022-12-07 11:24:12.000000 SELDOMpy-0.9.6/SELDOMpy/include/include_cvodes/cvodes/cvodes_lapack.h
--rw-rw-rw-   0        0        0     3061 2022-12-07 11:24:12.000000 SELDOMpy-0.9.6/SELDOMpy/include/include_cvodes/cvodes/cvodes_spbcgs.h
--rw-rw-rw-   0        0        0     3021 2022-12-07 11:24:12.000000 SELDOMpy-0.9.6/SELDOMpy/include/include_cvodes/cvodes/cvodes_spgmr.h
--rw-rw-rw-   0        0        0    18270 2022-12-07 11:24:13.000000 SELDOMpy-0.9.6/SELDOMpy/include/include_cvodes/cvodes/cvodes_spils.h
--rw-rw-rw-   0        0        0     3085 2022-12-07 11:24:13.000000 SELDOMpy-0.9.6/SELDOMpy/include/include_cvodes/cvodes/cvodes_sptfqmr.h
-drwxrwxrwx   0        0        0        0 2023-07-07 14:20:39.743283 SELDOMpy-0.9.6/SELDOMpy/include/include_cvodes/nvector/
--rw-rw-rw-   0        0        0    10054 2022-12-07 11:24:13.000000 SELDOMpy-0.9.6/SELDOMpy/include/include_cvodes/nvector/nvector_serial.h
-drwxrwxrwx   0        0        0        0 2023-07-07 14:20:39.754286 SELDOMpy-0.9.6/SELDOMpy/include/include_cvodes/sundials/
--rw-rw-rw-   0        0        0     6539 2022-12-07 11:24:13.000000 SELDOMpy-0.9.6/SELDOMpy/include/include_cvodes/sundials/sundials_band.h
--rw-rw-rw-   0        0        0     3157 2022-12-07 11:24:13.000000 SELDOMpy-0.9.6/SELDOMpy/include/include_cvodes/sundials/sundials_config.h
--rw-rw-rw-   0        0        0     7865 2022-12-07 11:24:13.000000 SELDOMpy-0.9.6/SELDOMpy/include/include_cvodes/sundials/sundials_dense.h
--rw-rw-rw-   0        0        0    13199 2022-12-07 11:24:13.000000 SELDOMpy-0.9.6/SELDOMpy/include/include_cvodes/sundials/sundials_direct.h
--rw-rw-rw-   0        0        0     1129 2022-12-07 11:24:13.000000 SELDOMpy-0.9.6/SELDOMpy/include/include_cvodes/sundials/sundials_fnvector.h
--rw-rw-rw-   0        0        0    13127 2022-12-07 11:24:13.000000 SELDOMpy-0.9.6/SELDOMpy/include/include_cvodes/sundials/sundials_iterative.h
--rw-rw-rw-   0        0        0     4763 2022-12-07 11:24:13.000000 SELDOMpy-0.9.6/SELDOMpy/include/include_cvodes/sundials/sundials_lapack.h
--rw-rw-rw-   0        0        0     4294 2022-12-07 11:24:13.000000 SELDOMpy-0.9.6/SELDOMpy/include/include_cvodes/sundials/sundials_math.h
--rw-rw-rw-   0        0        0    15964 2022-12-07 11:24:13.000000 SELDOMpy-0.9.6/SELDOMpy/include/include_cvodes/sundials/sundials_nvector.h
--rw-rw-rw-   0        0        0     7740 2022-12-07 11:24:13.000000 SELDOMpy-0.9.6/SELDOMpy/include/include_cvodes/sundials/sundials_spbcgs.h
--rw-rw-rw-   0        0        0    12224 2022-12-07 11:24:13.000000 SELDOMpy-0.9.6/SELDOMpy/include/include_cvodes/sundials/sundials_spgmr.h
--rw-rw-rw-   0        0        0    10246 2022-12-07 11:24:13.000000 SELDOMpy-0.9.6/SELDOMpy/include/include_cvodes/sundials/sundials_sptfqmr.h
--rw-rw-rw-   0        0        0     3726 2022-12-07 11:24:13.000000 SELDOMpy-0.9.6/SELDOMpy/include/include_cvodes/sundials/sundials_types.h
-drwxrwxrwx   0        0        0        0 2023-07-07 14:20:39.765284 SELDOMpy-0.9.6/SELDOMpy/src/
--rw-rw-rw-   0        0        0    10952 2022-12-07 11:24:11.000000 SELDOMpy-0.9.6/SELDOMpy/src/AMIGO_model.c
--rw-rw-rw-   0        0        0      240 2022-12-07 11:24:11.000000 SELDOMpy-0.9.6/SELDOMpy/src/AMIGO_model_stats.c
--rw-rw-rw-   0        0        0     8027 2022-12-07 11:24:11.000000 SELDOMpy-0.9.6/SELDOMpy/src/AMIGO_problem.c
--rw-rw-rw-   0        0        0      811 2022-12-07 11:24:11.000000 SELDOMpy-0.9.6/SELDOMpy/src/CNOStructure.h
--rw-rw-rw-   0        0        0        0 2023-07-03 16:56:56.000000 SELDOMpy-0.9.6/SELDOMpy/src/__init__.py
--rw-rw-rw-   0        0        0     3389 2023-04-10 15:09:09.000000 SELDOMpy-0.9.6/SELDOMpy/src/anODEModel.c
--rw-rw-rw-   0        0        0    74908 2022-12-07 11:24:11.000000 SELDOMpy-0.9.6/SELDOMpy/src/cvodea.c
--rw-rw-rw-   0        0        0    18585 2022-12-07 11:24:11.000000 SELDOMpy-0.9.6/SELDOMpy/src/cvodea_io.c
--rw-rw-rw-   0        0        0   245647 2022-12-07 11:24:11.000000 SELDOMpy-0.9.6/SELDOMpy/src/cvodes.c
--rw-rw-rw-   0        0        0    13293 2022-12-07 11:24:11.000000 SELDOMpy-0.9.6/SELDOMpy/src/cvodes_band.c
--rw-rw-rw-   0        0        0    16826 2022-12-07 11:24:11.000000 SELDOMpy-0.9.6/SELDOMpy/src/cvodes_bandpre.c
--rw-rw-rw-   0        0        0     2272 2022-12-07 11:24:11.000000 SELDOMpy-0.9.6/SELDOMpy/src/cvodes_bandpre_impl.h
--rw-rw-rw-   0        0        0    23592 2022-12-07 11:24:11.000000 SELDOMpy-0.9.6/SELDOMpy/src/cvodes_bbdpre.c
--rw-rw-rw-   0        0        0     2929 2022-12-07 11:24:11.000000 SELDOMpy-0.9.6/SELDOMpy/src/cvodes_bbdpre_impl.h
--rw-rw-rw-   0        0        0    12594 2022-12-07 11:24:11.000000 SELDOMpy-0.9.6/SELDOMpy/src/cvodes_dense.c
--rw-rw-rw-   0        0        0    13921 2022-12-07 11:24:11.000000 SELDOMpy-0.9.6/SELDOMpy/src/cvodes_diag.c
--rw-rw-rw-   0        0        0     2258 2022-12-07 11:24:11.000000 SELDOMpy-0.9.6/SELDOMpy/src/cvodes_diag_impl.h
--rw-rw-rw-   0        0        0    20099 2022-12-07 11:24:11.000000 SELDOMpy-0.9.6/SELDOMpy/src/cvodes_direct.c
--rw-rw-rw-   0        0        0     5473 2022-12-07 11:24:11.000000 SELDOMpy-0.9.6/SELDOMpy/src/cvodes_direct_impl.h
--rw-rw-rw-   0        0        0    47504 2022-12-07 11:24:11.000000 SELDOMpy-0.9.6/SELDOMpy/src/cvodes_impl.h
--rw-rw-rw-   0        0        0    41365 2022-12-07 11:24:11.000000 SELDOMpy-0.9.6/SELDOMpy/src/cvodes_io.c
--rw-rw-rw-   0        0        0    16912 2022-12-07 11:24:11.000000 SELDOMpy-0.9.6/SELDOMpy/src/cvodes_spbcgs.c
--rw-rw-rw-   0        0        0    17029 2022-12-07 11:24:11.000000 SELDOMpy-0.9.6/SELDOMpy/src/cvodes_spgmr.c
--rw-rw-rw-   0        0        0    32809 2022-12-07 11:24:11.000000 SELDOMpy-0.9.6/SELDOMpy/src/cvodes_spils.c
--rw-rw-rw-   0        0        0     6831 2022-12-07 11:24:11.000000 SELDOMpy-0.9.6/SELDOMpy/src/cvodes_spils_impl.h
--rw-rw-rw-   0        0        0    17108 2022-12-07 11:24:11.000000 SELDOMpy-0.9.6/SELDOMpy/src/cvodes_sptfqmr.c
--rw-rw-rw-   0        0        0      405 2022-12-07 11:24:11.000000 SELDOMpy-0.9.6/SELDOMpy/src/decimal2binary.c
--rw-rw-rw-   0        0        0     3792 2022-12-07 11:24:12.000000 SELDOMpy-0.9.6/SELDOMpy/src/dhc.c
--rw-rw-rw-   0        0        0      527 2022-12-07 11:24:12.000000 SELDOMpy-0.9.6/SELDOMpy/src/findStates.c
--rw-rw-rw-   0        0        0     3433 2022-12-07 11:24:12.000000 SELDOMpy-0.9.6/SELDOMpy/src/fnvector_serial.c
--rw-rw-rw-   0        0        0     2688 2022-12-07 11:24:12.000000 SELDOMpy-0.9.6/SELDOMpy/src/fnvector_serial.h
--rw-rw-rw-   0        0        0      693 2022-12-07 11:24:12.000000 SELDOMpy-0.9.6/SELDOMpy/src/getAdjacencyMatrix.c
--rw-rw-rw-   0        0        0      463 2022-12-07 11:24:12.000000 SELDOMpy-0.9.6/SELDOMpy/src/getNumBits.c
--rw-rw-rw-   0        0        0      475 2022-12-07 11:24:12.000000 SELDOMpy-0.9.6/SELDOMpy/src/getNumInputs.c
--rw-rw-rw-   0        0        0      695 2022-12-07 11:24:12.000000 SELDOMpy-0.9.6/SELDOMpy/src/getStateIndex.c
--rw-rw-rw-   0        0        0     3859 2022-12-07 11:24:12.000000 SELDOMpy-0.9.6/SELDOMpy/src/getTruthTables.c
--rw-rw-rw-   0        0        0      451 2022-12-07 11:24:12.000000 SELDOMpy-0.9.6/SELDOMpy/src/get_count_bits.c
--rw-rw-rw-   0        0        0      487 2022-12-07 11:24:12.000000 SELDOMpy-0.9.6/SELDOMpy/src/get_input_index.c
--rw-rw-rw-   0        0        0      594 2022-12-07 11:24:12.000000 SELDOMpy-0.9.6/SELDOMpy/src/get_support_truth_tables.c
--rw-rw-rw-   0        0        0      585 2022-12-07 11:24:12.000000 SELDOMpy-0.9.6/SELDOMpy/src/get_truth_tables_index.c
--rw-rw-rw-   0        0        0      224 2022-12-07 11:24:12.000000 SELDOMpy-0.9.6/SELDOMpy/src/hill_function.c
-drwxrwxrwx   0        0        0        0 2023-07-07 14:20:39.656283 SELDOMpy-0.9.6/SELDOMpy/src/include/
-drwxrwxrwx   0        0        0        0 2023-07-07 14:20:39.778286 SELDOMpy-0.9.6/SELDOMpy/src/include/include_amigo/
--rw-rw-rw-   0        0        0        4 2022-12-07 11:24:12.000000 SELDOMpy-0.9.6/SELDOMpy/src/include/include_amigo/AMIGO_hdf5.h
--rw-rw-rw-   0        0        0     3769 2022-12-07 11:24:12.000000 SELDOMpy-0.9.6/SELDOMpy/src/include/include_amigo/AMIGO_model.h
--rw-rw-rw-   0        0        0      442 2022-12-07 11:24:12.000000 SELDOMpy-0.9.6/SELDOMpy/src/include/include_amigo/AMIGO_model_stats.h
--rw-rw-rw-   0        0        0     1822 2022-12-07 11:24:12.000000 SELDOMpy-0.9.6/SELDOMpy/src/include/include_amigo/AMIGO_problem.h
--rw-rw-rw-   0        0        0      287 2022-12-07 11:24:12.000000 SELDOMpy-0.9.6/SELDOMpy/src/include/include_amigo/amigoJAC.h
--rw-rw-rw-   0        0        0       24 2022-12-07 11:24:12.000000 SELDOMpy-0.9.6/SELDOMpy/src/include/include_amigo/amigoRHS.h
--rw-rw-rw-   0        0        0      171 2022-12-07 11:24:12.000000 SELDOMpy-0.9.6/SELDOMpy/src/include/include_amigo/amigoSensRHS.h
--rw-rw-rw-   0        0        0      164 2022-12-07 11:24:12.000000 SELDOMpy-0.9.6/SELDOMpy/src/include/include_amigo/simulate_amigo_model.h
-drwxrwxrwx   0        0        0        0 2023-07-07 14:20:39.657295 SELDOMpy-0.9.6/SELDOMpy/src/include/include_cvodes/
-drwxrwxrwx   0        0        0        0 2023-07-07 14:20:39.896303 SELDOMpy-0.9.6/SELDOMpy/src/include/include_cvodes/cvodes/
--rw-rw-rw-   0        0        0    84971 2022-12-07 11:24:12.000000 SELDOMpy-0.9.6/SELDOMpy/src/include/include_cvodes/cvodes/cvodes.h
--rw-rw-rw-   0        0        0     2442 2022-12-07 11:24:12.000000 SELDOMpy-0.9.6/SELDOMpy/src/include/include_cvodes/cvodes/cvodes_band.h
--rw-rw-rw-   0        0        0     6547 2022-12-07 11:24:12.000000 SELDOMpy-0.9.6/SELDOMpy/src/include/include_cvodes/cvodes/cvodes_bandpre.h
--rw-rw-rw-   0        0        0    13259 2022-12-07 11:24:12.000000 SELDOMpy-0.9.6/SELDOMpy/src/include/include_cvodes/cvodes/cvodes_bbdpre.h
--rw-rw-rw-   0        0        0     2122 2022-12-07 11:24:12.000000 SELDOMpy-0.9.6/SELDOMpy/src/include/include_cvodes/cvodes/cvodes_dense.h
--rw-rw-rw-   0        0        0     4845 2022-12-07 11:24:12.000000 SELDOMpy-0.9.6/SELDOMpy/src/include/include_cvodes/cvodes/cvodes_diag.h
--rw-rw-rw-   0        0        0    14031 2022-12-07 11:24:12.000000 SELDOMpy-0.9.6/SELDOMpy/src/include/include_cvodes/cvodes/cvodes_direct.h
--rw-rw-rw-   0        0        0     3732 2022-12-07 11:24:12.000000 SELDOMpy-0.9.6/SELDOMpy/src/include/include_cvodes/cvodes/cvodes_lapack.h
--rw-rw-rw-   0        0        0     3061 2022-12-07 11:24:12.000000 SELDOMpy-0.9.6/SELDOMpy/src/include/include_cvodes/cvodes/cvodes_spbcgs.h
--rw-rw-rw-   0        0        0     3021 2022-12-07 11:24:12.000000 SELDOMpy-0.9.6/SELDOMpy/src/include/include_cvodes/cvodes/cvodes_spgmr.h
--rw-rw-rw-   0        0        0    18270 2022-12-07 11:24:13.000000 SELDOMpy-0.9.6/SELDOMpy/src/include/include_cvodes/cvodes/cvodes_spils.h
--rw-rw-rw-   0        0        0     3085 2022-12-07 11:24:13.000000 SELDOMpy-0.9.6/SELDOMpy/src/include/include_cvodes/cvodes/cvodes_sptfqmr.h
-drwxrwxrwx   0        0        0        0 2023-07-07 14:20:39.900302 SELDOMpy-0.9.6/SELDOMpy/src/include/include_cvodes/nvector/
--rw-rw-rw-   0        0        0    10054 2022-12-07 11:24:13.000000 SELDOMpy-0.9.6/SELDOMpy/src/include/include_cvodes/nvector/nvector_serial.h
-drwxrwxrwx   0        0        0        0 2023-07-07 14:20:39.968252 SELDOMpy-0.9.6/SELDOMpy/src/include/include_cvodes/sundials/
--rw-rw-rw-   0        0        0     6539 2022-12-07 11:24:13.000000 SELDOMpy-0.9.6/SELDOMpy/src/include/include_cvodes/sundials/sundials_band.h
--rw-rw-rw-   0        0        0     3157 2022-12-07 11:24:13.000000 SELDOMpy-0.9.6/SELDOMpy/src/include/include_cvodes/sundials/sundials_config.h
--rw-rw-rw-   0        0        0     7865 2022-12-07 11:24:13.000000 SELDOMpy-0.9.6/SELDOMpy/src/include/include_cvodes/sundials/sundials_dense.h
--rw-rw-rw-   0        0        0    13199 2022-12-07 11:24:13.000000 SELDOMpy-0.9.6/SELDOMpy/src/include/include_cvodes/sundials/sundials_direct.h
--rw-rw-rw-   0        0        0     1129 2022-12-07 11:24:13.000000 SELDOMpy-0.9.6/SELDOMpy/src/include/include_cvodes/sundials/sundials_fnvector.h
--rw-rw-rw-   0        0        0    13127 2022-12-07 11:24:13.000000 SELDOMpy-0.9.6/SELDOMpy/src/include/include_cvodes/sundials/sundials_iterative.h
--rw-rw-rw-   0        0        0     4763 2022-12-07 11:24:13.000000 SELDOMpy-0.9.6/SELDOMpy/src/include/include_cvodes/sundials/sundials_lapack.h
--rw-rw-rw-   0        0        0     4294 2022-12-07 11:24:13.000000 SELDOMpy-0.9.6/SELDOMpy/src/include/include_cvodes/sundials/sundials_math.h
--rw-rw-rw-   0        0        0    15964 2022-12-07 11:24:13.000000 SELDOMpy-0.9.6/SELDOMpy/src/include/include_cvodes/sundials/sundials_nvector.h
--rw-rw-rw-   0        0        0     7740 2022-12-07 11:24:13.000000 SELDOMpy-0.9.6/SELDOMpy/src/include/include_cvodes/sundials/sundials_spbcgs.h
--rw-rw-rw-   0        0        0    12224 2022-12-07 11:24:13.000000 SELDOMpy-0.9.6/SELDOMpy/src/include/include_cvodes/sundials/sundials_spgmr.h
--rw-rw-rw-   0        0        0    10246 2022-12-07 11:24:13.000000 SELDOMpy-0.9.6/SELDOMpy/src/include/include_cvodes/sundials/sundials_sptfqmr.h
--rw-rw-rw-   0        0        0     3726 2022-12-07 11:24:13.000000 SELDOMpy-0.9.6/SELDOMpy/src/include/include_cvodes/sundials/sundials_types.h
--rw-rw-rw-   0        0        0      219 2022-12-07 11:24:12.000000 SELDOMpy-0.9.6/SELDOMpy/src/linear_transfer_function.c
--rw-rw-rw-   0        0        0      227 2022-12-07 11:24:12.000000 SELDOMpy-0.9.6/SELDOMpy/src/normHill.c
--rw-rw-rw-   0        0        0    20778 2022-12-07 11:24:12.000000 SELDOMpy-0.9.6/SELDOMpy/src/nvector_serial.c
--rw-rw-rw-   0        0        0      305 2022-12-07 11:24:12.000000 SELDOMpy-0.9.6/SELDOMpy/src/printAdjMat.c
--rw-rw-rw-   0        0        0      315 2022-12-07 11:24:12.000000 SELDOMpy-0.9.6/SELDOMpy/src/printInterMat.c
--rw-rw-rw-   0        0        0      553 2022-12-07 11:24:12.000000 SELDOMpy-0.9.6/SELDOMpy/src/printNminiTerms.c
--rw-rw-rw-   0        0        0      410 2022-12-07 11:24:12.000000 SELDOMpy-0.9.6/SELDOMpy/src/printTruthTables.c
--rw-rw-rw-   0        0        0    15775 2023-04-28 16:16:22.000000 SELDOMpy-0.9.6/SELDOMpy/src/sim_logic_ode.c
--rw-rw-rw-   0        0        0     9815 2022-12-07 11:24:12.000000 SELDOMpy-0.9.6/SELDOMpy/src/simulate_amigo_model.c
--rw-rw-rw-   0        0        0     6036 2022-12-07 11:24:12.000000 SELDOMpy-0.9.6/SELDOMpy/src/sundials_band.c
--rw-rw-rw-   0        0        0     8510 2022-12-07 11:24:12.000000 SELDOMpy-0.9.6/SELDOMpy/src/sundials_dense.c
--rw-rw-rw-   0        0        0     6225 2022-12-07 11:24:12.000000 SELDOMpy-0.9.6/SELDOMpy/src/sundials_direct.c
--rw-rw-rw-   0        0        0     7662 2022-12-07 11:24:12.000000 SELDOMpy-0.9.6/SELDOMpy/src/sundials_iterative.c
--rw-rw-rw-   0        0        0     2474 2022-12-07 11:24:12.000000 SELDOMpy-0.9.6/SELDOMpy/src/sundials_math.c
--rw-rw-rw-   0        0        0     4702 2022-12-07 11:24:12.000000 SELDOMpy-0.9.6/SELDOMpy/src/sundials_nvector.c
--rw-rw-rw-   0        0        0     9663 2022-12-07 11:24:12.000000 SELDOMpy-0.9.6/SELDOMpy/src/sundials_spbcgs.c
--rw-rw-rw-   0        0        0    12650 2022-12-07 11:24:12.000000 SELDOMpy-0.9.6/SELDOMpy/src/sundials_spgmr.c
--rw-rw-rw-   0        0        0    14744 2022-12-07 11:24:12.000000 SELDOMpy-0.9.6/SELDOMpy/src/sundials_sptfqmr.c
-drwxrwxrwx   0        0        0        0 2023-07-07 14:20:39.666270 SELDOMpy-0.9.6/SELDOMpy.egg-info/
--rw-rw-rw-   0        0        0     4171 2023-07-07 14:20:39.000000 SELDOMpy-0.9.6/SELDOMpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7919 2023-07-07 14:20:39.000000 SELDOMpy-0.9.6/SELDOMpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 14:20:39.000000 SELDOMpy-0.9.6/SELDOMpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       78 2023-07-07 14:20:39.000000 SELDOMpy-0.9.6/SELDOMpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-07 14:20:39.000000 SELDOMpy-0.9.6/SELDOMpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      115 2023-07-07 14:20:39.971281 SELDOMpy-0.9.6/setup.cfg
--rw-rw-rw-   0        0        0     3500 2023-07-07 14:20:18.000000 SELDOMpy-0.9.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 14:24:17.031243 SELDOMpy-0.9.7/
+-rw-rw-rw-   0        0        0    35149 2023-07-05 16:32:35.000000 SELDOMpy-0.9.7/LICENSE.txt
+-rw-rw-rw-   0        0        0      596 2023-07-07 14:20:18.000000 SELDOMpy-0.9.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     4171 2023-07-07 14:24:17.031243 SELDOMpy-0.9.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3446 2023-07-06 08:12:36.000000 SELDOMpy-0.9.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-07 14:24:16.920275 SELDOMpy-0.9.7/SELDOMpy/
+-rw-rw-rw-   0        0        0      490 2023-07-06 11:23:03.000000 SELDOMpy-0.9.7/SELDOMpy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 14:24:16.912271 SELDOMpy-0.9.7/SELDOMpy/examples/
+drwxrwxrwx   0        0        0        0 2023-07-07 14:24:16.969249 SELDOMpy-0.9.7/SELDOMpy/examples/MAPK/
+-rw-rw-rw-   0        0        0    13667 2023-04-19 10:00:19.000000 SELDOMpy-0.9.7/SELDOMpy/examples/MAPK/MAPK.xlsx
+-rw-rw-rw-   0        0        0     5830 2023-07-07 11:25:38.000000 SELDOMpy-0.9.7/SELDOMpy/examples/MAPK/MAPK_training_and_reduce.py
+-rw-rw-rw-   0        0        0    10464 2023-07-07 13:51:52.000000 SELDOMpy-0.9.7/SELDOMpy/examples/MAPK/MAPK_training_and_reduce_pyPESTO.py
+drwxrwxrwx   0        0        0        0 2023-07-07 14:24:16.972249 SELDOMpy-0.9.7/SELDOMpy/examples/SP/
+-rw-rw-rw-   0        0        0    23018 2023-06-21 18:44:38.000000 SELDOMpy-0.9.7/SELDOMpy/examples/SP/SP.xlsx
+-rw-rw-rw-   0        0        0     6011 2023-07-07 11:49:56.000000 SELDOMpy-0.9.7/SELDOMpy/examples/SP/SP_training_and_reduce.py
+-rw-rw-rw-   0        0        0    10661 2023-07-07 13:32:38.000000 SELDOMpy-0.9.7/SELDOMpy/examples/SP/SP_training_and_reduce_pyPESTO.py
+drwxrwxrwx   0        0        0        0 2023-07-07 14:24:16.983251 SELDOMpy-0.9.7/SELDOMpy/functions/
+-rw-rw-rw-   0        0        0     1799 2023-07-06 13:38:27.000000 SELDOMpy-0.9.7/SELDOMpy/functions/buildmim.py
+-rw-rw-rw-   0        0        0     1280 2023-07-07 07:34:51.000000 SELDOMpy-0.9.7/SELDOMpy/functions/extras.py
+-rw-rw-rw-   0        0        0     4037 2023-07-07 11:47:15.000000 SELDOMpy-0.9.7/SELDOMpy/functions/gen_exps.py
+-rw-rw-rw-   0        0        0     4860 2023-07-07 07:34:51.000000 SELDOMpy-0.9.7/SELDOMpy/functions/getLBODEmodel.py
+-rw-rw-rw-   0        0        0     3156 2023-07-07 07:34:50.000000 SELDOMpy-0.9.7/SELDOMpy/functions/getRandomLBODEmodel.py
+-rw-rw-rw-   0        0        0     2313 2023-07-07 11:11:37.000000 SELDOMpy-0.9.7/SELDOMpy/functions/optimization.py
+-rw-rw-rw-   0        0        0     1509 2023-07-07 07:39:33.000000 SELDOMpy-0.9.7/SELDOMpy/functions/plot_results.py
+-rw-rw-rw-   0        0        0     2748 2023-07-07 07:41:41.000000 SELDOMpy-0.9.7/SELDOMpy/functions/reduce_fun.py
+-rw-rw-rw-   0        0        0     3802 2023-07-07 07:48:40.000000 SELDOMpy-0.9.7/SELDOMpy/functions/simulate_logic_based_ode.py
+-rw-rw-rw-   0        0        0     3595 2023-07-07 07:52:38.000000 SELDOMpy-0.9.7/SELDOMpy/functions/simulate_logic_based_ode_obs.py
+drwxrwxrwx   0        0        0        0 2023-07-07 14:24:16.995251 SELDOMpy-0.9.7/SELDOMpy/src/
+-rw-rw-rw-   0        0        0    10952 2022-12-07 11:24:11.000000 SELDOMpy-0.9.7/SELDOMpy/src/AMIGO_model.c
+-rw-rw-rw-   0        0        0      240 2022-12-07 11:24:11.000000 SELDOMpy-0.9.7/SELDOMpy/src/AMIGO_model_stats.c
+-rw-rw-rw-   0        0        0     8027 2022-12-07 11:24:11.000000 SELDOMpy-0.9.7/SELDOMpy/src/AMIGO_problem.c
+-rw-rw-rw-   0        0        0      811 2022-12-07 11:24:11.000000 SELDOMpy-0.9.7/SELDOMpy/src/CNOStructure.h
+-rw-rw-rw-   0        0        0        0 2023-07-03 16:56:56.000000 SELDOMpy-0.9.7/SELDOMpy/src/__init__.py
+-rw-rw-rw-   0        0        0     3389 2023-04-10 15:09:09.000000 SELDOMpy-0.9.7/SELDOMpy/src/anODEModel.c
+-rw-rw-rw-   0        0        0    74908 2022-12-07 11:24:11.000000 SELDOMpy-0.9.7/SELDOMpy/src/cvodea.c
+-rw-rw-rw-   0        0        0    18585 2022-12-07 11:24:11.000000 SELDOMpy-0.9.7/SELDOMpy/src/cvodea_io.c
+-rw-rw-rw-   0        0        0   245647 2022-12-07 11:24:11.000000 SELDOMpy-0.9.7/SELDOMpy/src/cvodes.c
+-rw-rw-rw-   0        0        0    13293 2022-12-07 11:24:11.000000 SELDOMpy-0.9.7/SELDOMpy/src/cvodes_band.c
+-rw-rw-rw-   0        0        0    16826 2022-12-07 11:24:11.000000 SELDOMpy-0.9.7/SELDOMpy/src/cvodes_bandpre.c
+-rw-rw-rw-   0        0        0     2272 2022-12-07 11:24:11.000000 SELDOMpy-0.9.7/SELDOMpy/src/cvodes_bandpre_impl.h
+-rw-rw-rw-   0        0        0    23592 2022-12-07 11:24:11.000000 SELDOMpy-0.9.7/SELDOMpy/src/cvodes_bbdpre.c
+-rw-rw-rw-   0        0        0     2929 2022-12-07 11:24:11.000000 SELDOMpy-0.9.7/SELDOMpy/src/cvodes_bbdpre_impl.h
+-rw-rw-rw-   0        0        0    12594 2022-12-07 11:24:11.000000 SELDOMpy-0.9.7/SELDOMpy/src/cvodes_dense.c
+-rw-rw-rw-   0        0        0    13921 2022-12-07 11:24:11.000000 SELDOMpy-0.9.7/SELDOMpy/src/cvodes_diag.c
+-rw-rw-rw-   0        0        0     2258 2022-12-07 11:24:11.000000 SELDOMpy-0.9.7/SELDOMpy/src/cvodes_diag_impl.h
+-rw-rw-rw-   0        0        0    20099 2022-12-07 11:24:11.000000 SELDOMpy-0.9.7/SELDOMpy/src/cvodes_direct.c
+-rw-rw-rw-   0        0        0     5473 2022-12-07 11:24:11.000000 SELDOMpy-0.9.7/SELDOMpy/src/cvodes_direct_impl.h
+-rw-rw-rw-   0        0        0    47504 2022-12-07 11:24:11.000000 SELDOMpy-0.9.7/SELDOMpy/src/cvodes_impl.h
+-rw-rw-rw-   0        0        0    41365 2022-12-07 11:24:11.000000 SELDOMpy-0.9.7/SELDOMpy/src/cvodes_io.c
+-rw-rw-rw-   0        0        0    16912 2022-12-07 11:24:11.000000 SELDOMpy-0.9.7/SELDOMpy/src/cvodes_spbcgs.c
+-rw-rw-rw-   0        0        0    17029 2022-12-07 11:24:11.000000 SELDOMpy-0.9.7/SELDOMpy/src/cvodes_spgmr.c
+-rw-rw-rw-   0        0        0    32809 2022-12-07 11:24:11.000000 SELDOMpy-0.9.7/SELDOMpy/src/cvodes_spils.c
+-rw-rw-rw-   0        0        0     6831 2022-12-07 11:24:11.000000 SELDOMpy-0.9.7/SELDOMpy/src/cvodes_spils_impl.h
+-rw-rw-rw-   0        0        0    17108 2022-12-07 11:24:11.000000 SELDOMpy-0.9.7/SELDOMpy/src/cvodes_sptfqmr.c
+-rw-rw-rw-   0        0        0      405 2022-12-07 11:24:11.000000 SELDOMpy-0.9.7/SELDOMpy/src/decimal2binary.c
+-rw-rw-rw-   0        0        0     3792 2022-12-07 11:24:12.000000 SELDOMpy-0.9.7/SELDOMpy/src/dhc.c
+-rw-rw-rw-   0        0        0      527 2022-12-07 11:24:12.000000 SELDOMpy-0.9.7/SELDOMpy/src/findStates.c
+-rw-rw-rw-   0        0        0     3433 2022-12-07 11:24:12.000000 SELDOMpy-0.9.7/SELDOMpy/src/fnvector_serial.c
+-rw-rw-rw-   0        0        0     2688 2022-12-07 11:24:12.000000 SELDOMpy-0.9.7/SELDOMpy/src/fnvector_serial.h
+-rw-rw-rw-   0        0        0      693 2022-12-07 11:24:12.000000 SELDOMpy-0.9.7/SELDOMpy/src/getAdjacencyMatrix.c
+-rw-rw-rw-   0        0        0      463 2022-12-07 11:24:12.000000 SELDOMpy-0.9.7/SELDOMpy/src/getNumBits.c
+-rw-rw-rw-   0        0        0      475 2022-12-07 11:24:12.000000 SELDOMpy-0.9.7/SELDOMpy/src/getNumInputs.c
+-rw-rw-rw-   0        0        0      695 2022-12-07 11:24:12.000000 SELDOMpy-0.9.7/SELDOMpy/src/getStateIndex.c
+-rw-rw-rw-   0        0        0     3859 2022-12-07 11:24:12.000000 SELDOMpy-0.9.7/SELDOMpy/src/getTruthTables.c
+-rw-rw-rw-   0        0        0      451 2022-12-07 11:24:12.000000 SELDOMpy-0.9.7/SELDOMpy/src/get_count_bits.c
+-rw-rw-rw-   0        0        0      487 2022-12-07 11:24:12.000000 SELDOMpy-0.9.7/SELDOMpy/src/get_input_index.c
+-rw-rw-rw-   0        0        0      594 2022-12-07 11:24:12.000000 SELDOMpy-0.9.7/SELDOMpy/src/get_support_truth_tables.c
+-rw-rw-rw-   0        0        0      585 2022-12-07 11:24:12.000000 SELDOMpy-0.9.7/SELDOMpy/src/get_truth_tables_index.c
+-rw-rw-rw-   0        0        0      224 2022-12-07 11:24:12.000000 SELDOMpy-0.9.7/SELDOMpy/src/hill_function.c
+drwxrwxrwx   0        0        0        0 2023-07-07 14:24:16.914272 SELDOMpy-0.9.7/SELDOMpy/src/include/
+drwxrwxrwx   0        0        0        0 2023-07-07 14:24:17.008284 SELDOMpy-0.9.7/SELDOMpy/src/include/include_amigo/
+-rw-rw-rw-   0        0        0        4 2022-12-07 11:24:12.000000 SELDOMpy-0.9.7/SELDOMpy/src/include/include_amigo/AMIGO_hdf5.h
+-rw-rw-rw-   0        0        0     3769 2022-12-07 11:24:12.000000 SELDOMpy-0.9.7/SELDOMpy/src/include/include_amigo/AMIGO_model.h
+-rw-rw-rw-   0        0        0      442 2022-12-07 11:24:12.000000 SELDOMpy-0.9.7/SELDOMpy/src/include/include_amigo/AMIGO_model_stats.h
+-rw-rw-rw-   0        0        0     1822 2022-12-07 11:24:12.000000 SELDOMpy-0.9.7/SELDOMpy/src/include/include_amigo/AMIGO_problem.h
+-rw-rw-rw-   0        0        0      287 2022-12-07 11:24:12.000000 SELDOMpy-0.9.7/SELDOMpy/src/include/include_amigo/amigoJAC.h
+-rw-rw-rw-   0        0        0       24 2022-12-07 11:24:12.000000 SELDOMpy-0.9.7/SELDOMpy/src/include/include_amigo/amigoRHS.h
+-rw-rw-rw-   0        0        0      171 2022-12-07 11:24:12.000000 SELDOMpy-0.9.7/SELDOMpy/src/include/include_amigo/amigoSensRHS.h
+-rw-rw-rw-   0        0        0      164 2022-12-07 11:24:12.000000 SELDOMpy-0.9.7/SELDOMpy/src/include/include_amigo/simulate_amigo_model.h
+drwxrwxrwx   0        0        0        0 2023-07-07 14:24:16.915244 SELDOMpy-0.9.7/SELDOMpy/src/include/include_cvodes/
+drwxrwxrwx   0        0        0        0 2023-07-07 14:24:17.018250 SELDOMpy-0.9.7/SELDOMpy/src/include/include_cvodes/cvodes/
+-rw-rw-rw-   0        0        0    84971 2022-12-07 11:24:12.000000 SELDOMpy-0.9.7/SELDOMpy/src/include/include_cvodes/cvodes/cvodes.h
+-rw-rw-rw-   0        0        0     2442 2022-12-07 11:24:12.000000 SELDOMpy-0.9.7/SELDOMpy/src/include/include_cvodes/cvodes/cvodes_band.h
+-rw-rw-rw-   0        0        0     6547 2022-12-07 11:24:12.000000 SELDOMpy-0.9.7/SELDOMpy/src/include/include_cvodes/cvodes/cvodes_bandpre.h
+-rw-rw-rw-   0        0        0    13259 2022-12-07 11:24:12.000000 SELDOMpy-0.9.7/SELDOMpy/src/include/include_cvodes/cvodes/cvodes_bbdpre.h
+-rw-rw-rw-   0        0        0     2122 2022-12-07 11:24:12.000000 SELDOMpy-0.9.7/SELDOMpy/src/include/include_cvodes/cvodes/cvodes_dense.h
+-rw-rw-rw-   0        0        0     4845 2022-12-07 11:24:12.000000 SELDOMpy-0.9.7/SELDOMpy/src/include/include_cvodes/cvodes/cvodes_diag.h
+-rw-rw-rw-   0        0        0    14031 2022-12-07 11:24:12.000000 SELDOMpy-0.9.7/SELDOMpy/src/include/include_cvodes/cvodes/cvodes_direct.h
+-rw-rw-rw-   0        0        0     3732 2022-12-07 11:24:12.000000 SELDOMpy-0.9.7/SELDOMpy/src/include/include_cvodes/cvodes/cvodes_lapack.h
+-rw-rw-rw-   0        0        0     3061 2022-12-07 11:24:12.000000 SELDOMpy-0.9.7/SELDOMpy/src/include/include_cvodes/cvodes/cvodes_spbcgs.h
+-rw-rw-rw-   0        0        0     3021 2022-12-07 11:24:12.000000 SELDOMpy-0.9.7/SELDOMpy/src/include/include_cvodes/cvodes/cvodes_spgmr.h
+-rw-rw-rw-   0        0        0    18270 2022-12-07 11:24:13.000000 SELDOMpy-0.9.7/SELDOMpy/src/include/include_cvodes/cvodes/cvodes_spils.h
+-rw-rw-rw-   0        0        0     3085 2022-12-07 11:24:13.000000 SELDOMpy-0.9.7/SELDOMpy/src/include/include_cvodes/cvodes/cvodes_sptfqmr.h
+drwxrwxrwx   0        0        0        0 2023-07-07 14:24:17.019251 SELDOMpy-0.9.7/SELDOMpy/src/include/include_cvodes/nvector/
+-rw-rw-rw-   0        0        0    10054 2022-12-07 11:24:13.000000 SELDOMpy-0.9.7/SELDOMpy/src/include/include_cvodes/nvector/nvector_serial.h
+drwxrwxrwx   0        0        0        0 2023-07-07 14:24:17.030250 SELDOMpy-0.9.7/SELDOMpy/src/include/include_cvodes/sundials/
+-rw-rw-rw-   0        0        0     6539 2022-12-07 11:24:13.000000 SELDOMpy-0.9.7/SELDOMpy/src/include/include_cvodes/sundials/sundials_band.h
+-rw-rw-rw-   0        0        0     3157 2022-12-07 11:24:13.000000 SELDOMpy-0.9.7/SELDOMpy/src/include/include_cvodes/sundials/sundials_config.h
+-rw-rw-rw-   0        0        0     7865 2022-12-07 11:24:13.000000 SELDOMpy-0.9.7/SELDOMpy/src/include/include_cvodes/sundials/sundials_dense.h
+-rw-rw-rw-   0        0        0    13199 2022-12-07 11:24:13.000000 SELDOMpy-0.9.7/SELDOMpy/src/include/include_cvodes/sundials/sundials_direct.h
+-rw-rw-rw-   0        0        0     1129 2022-12-07 11:24:13.000000 SELDOMpy-0.9.7/SELDOMpy/src/include/include_cvodes/sundials/sundials_fnvector.h
+-rw-rw-rw-   0        0        0    13127 2022-12-07 11:24:13.000000 SELDOMpy-0.9.7/SELDOMpy/src/include/include_cvodes/sundials/sundials_iterative.h
+-rw-rw-rw-   0        0        0     4763 2022-12-07 11:24:13.000000 SELDOMpy-0.9.7/SELDOMpy/src/include/include_cvodes/sundials/sundials_lapack.h
+-rw-rw-rw-   0        0        0     4294 2022-12-07 11:24:13.000000 SELDOMpy-0.9.7/SELDOMpy/src/include/include_cvodes/sundials/sundials_math.h
+-rw-rw-rw-   0        0        0    15964 2022-12-07 11:24:13.000000 SELDOMpy-0.9.7/SELDOMpy/src/include/include_cvodes/sundials/sundials_nvector.h
+-rw-rw-rw-   0        0        0     7740 2022-12-07 11:24:13.000000 SELDOMpy-0.9.7/SELDOMpy/src/include/include_cvodes/sundials/sundials_spbcgs.h
+-rw-rw-rw-   0        0        0    12224 2022-12-07 11:24:13.000000 SELDOMpy-0.9.7/SELDOMpy/src/include/include_cvodes/sundials/sundials_spgmr.h
+-rw-rw-rw-   0        0        0    10246 2022-12-07 11:24:13.000000 SELDOMpy-0.9.7/SELDOMpy/src/include/include_cvodes/sundials/sundials_sptfqmr.h
+-rw-rw-rw-   0        0        0     3726 2022-12-07 11:24:13.000000 SELDOMpy-0.9.7/SELDOMpy/src/include/include_cvodes/sundials/sundials_types.h
+-rw-rw-rw-   0        0        0      219 2022-12-07 11:24:12.000000 SELDOMpy-0.9.7/SELDOMpy/src/linear_transfer_function.c
+-rw-rw-rw-   0        0        0      227 2022-12-07 11:24:12.000000 SELDOMpy-0.9.7/SELDOMpy/src/normHill.c
+-rw-rw-rw-   0        0        0    20778 2022-12-07 11:24:12.000000 SELDOMpy-0.9.7/SELDOMpy/src/nvector_serial.c
+-rw-rw-rw-   0        0        0      305 2022-12-07 11:24:12.000000 SELDOMpy-0.9.7/SELDOMpy/src/printAdjMat.c
+-rw-rw-rw-   0        0        0      315 2022-12-07 11:24:12.000000 SELDOMpy-0.9.7/SELDOMpy/src/printInterMat.c
+-rw-rw-rw-   0        0        0      553 2022-12-07 11:24:12.000000 SELDOMpy-0.9.7/SELDOMpy/src/printNminiTerms.c
+-rw-rw-rw-   0        0        0      410 2022-12-07 11:24:12.000000 SELDOMpy-0.9.7/SELDOMpy/src/printTruthTables.c
+-rw-rw-rw-   0        0        0    15775 2023-04-28 16:16:22.000000 SELDOMpy-0.9.7/SELDOMpy/src/sim_logic_ode.c
+-rw-rw-rw-   0        0        0     9815 2022-12-07 11:24:12.000000 SELDOMpy-0.9.7/SELDOMpy/src/simulate_amigo_model.c
+-rw-rw-rw-   0        0        0     6036 2022-12-07 11:24:12.000000 SELDOMpy-0.9.7/SELDOMpy/src/sundials_band.c
+-rw-rw-rw-   0        0        0     8510 2022-12-07 11:24:12.000000 SELDOMpy-0.9.7/SELDOMpy/src/sundials_dense.c
+-rw-rw-rw-   0        0        0     6225 2022-12-07 11:24:12.000000 SELDOMpy-0.9.7/SELDOMpy/src/sundials_direct.c
+-rw-rw-rw-   0        0        0     7662 2022-12-07 11:24:12.000000 SELDOMpy-0.9.7/SELDOMpy/src/sundials_iterative.c
+-rw-rw-rw-   0        0        0     2474 2022-12-07 11:24:12.000000 SELDOMpy-0.9.7/SELDOMpy/src/sundials_math.c
+-rw-rw-rw-   0        0        0     4702 2022-12-07 11:24:12.000000 SELDOMpy-0.9.7/SELDOMpy/src/sundials_nvector.c
+-rw-rw-rw-   0        0        0     9663 2022-12-07 11:24:12.000000 SELDOMpy-0.9.7/SELDOMpy/src/sundials_spbcgs.c
+-rw-rw-rw-   0        0        0    12650 2022-12-07 11:24:12.000000 SELDOMpy-0.9.7/SELDOMpy/src/sundials_spgmr.c
+-rw-rw-rw-   0        0        0    14744 2022-12-07 11:24:12.000000 SELDOMpy-0.9.7/SELDOMpy/src/sundials_sptfqmr.c
+drwxrwxrwx   0        0        0        0 2023-07-07 14:24:16.923251 SELDOMpy-0.9.7/SELDOMpy.egg-info/
+-rw-rw-rw-   0        0        0     4171 2023-07-07 14:24:16.000000 SELDOMpy-0.9.7/SELDOMpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6076 2023-07-07 14:24:16.000000 SELDOMpy-0.9.7/SELDOMpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 14:24:16.000000 SELDOMpy-0.9.7/SELDOMpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2023-07-07 14:24:16.000000 SELDOMpy-0.9.7/SELDOMpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-07 14:24:16.000000 SELDOMpy-0.9.7/SELDOMpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      115 2023-07-07 14:24:17.032249 SELDOMpy-0.9.7/setup.cfg
+-rw-rw-rw-   0        0        0     3500 2023-07-07 14:24:07.000000 SELDOMpy-0.9.7/setup.py
```

### Comparing `SELDOMpy-0.9.6/LICENSE.txt` & `SELDOMpy-0.9.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/MANIFEST.in` & `SELDOMpy-0.9.7/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/PKG-INFO` & `SELDOMpy-0.9.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SELDOMpy
-Version: 0.9.6
+Version: 0.9.7
 Summary: Dynamic modelling of cellular signalling networks.
 Home-page: https://github.com/lupralo31/SELDOMpy
 Download-URL: https://github.com/lupralo31/SELDOMpy/archive/refs/tags/V_0.2.1.tar.gz
 Author: Luis Prado
 Author-email: pradolopezluis@gmail.com
 License: GPLv3
 Keywords: SELDOMpy,SELDOM,dynamic modelling,cellular signalling networks,biomedical engineering
```

### Comparing `SELDOMpy-0.9.6/README.md` & `SELDOMpy-0.9.7/README.md`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/examples/MAPK/MAPK.xlsx` & `SELDOMpy-0.9.7/SELDOMpy/examples/MAPK/MAPK.xlsx`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/examples/MAPK/MAPK_training_and_reduce.py` & `SELDOMpy-0.9.7/SELDOMpy/examples/MAPK/MAPK_training_and_reduce.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/examples/MAPK/MAPK_training_and_reduce_pyPESTO.py` & `SELDOMpy-0.9.7/SELDOMpy/examples/MAPK/MAPK_training_and_reduce_pyPESTO.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/examples/SP/SP.xlsx` & `SELDOMpy-0.9.7/SELDOMpy/examples/SP/SP.xlsx`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/examples/SP/SP_training_and_reduce.py` & `SELDOMpy-0.9.7/SELDOMpy/examples/SP/SP_training_and_reduce.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/examples/SP/SP_training_and_reduce_pyPESTO.py` & `SELDOMpy-0.9.7/SELDOMpy/examples/SP/SP_training_and_reduce_pyPESTO.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/functions/buildmim.py` & `SELDOMpy-0.9.7/SELDOMpy/functions/buildmim.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/functions/extras.py` & `SELDOMpy-0.9.7/SELDOMpy/functions/extras.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/functions/gen_exps.py` & `SELDOMpy-0.9.7/SELDOMpy/functions/gen_exps.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/functions/getLBODEmodel.py` & `SELDOMpy-0.9.7/SELDOMpy/functions/getLBODEmodel.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/functions/getRandomLBODEmodel.py` & `SELDOMpy-0.9.7/SELDOMpy/functions/getRandomLBODEmodel.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/functions/optimization.py` & `SELDOMpy-0.9.7/SELDOMpy/functions/optimization.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/functions/plot_results.py` & `SELDOMpy-0.9.7/SELDOMpy/functions/plot_results.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/functions/reduce_fun.py` & `SELDOMpy-0.9.7/SELDOMpy/functions/reduce_fun.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/functions/simulate_logic_based_ode.py` & `SELDOMpy-0.9.7/SELDOMpy/functions/simulate_logic_based_ode.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/functions/simulate_logic_based_ode_obs.py` & `SELDOMpy-0.9.7/SELDOMpy/functions/simulate_logic_based_ode_obs.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/include/include_amigo/AMIGO_model.h` & `SELDOMpy-0.9.7/SELDOMpy/src/include/include_amigo/AMIGO_model.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/include/include_amigo/AMIGO_problem.h` & `SELDOMpy-0.9.7/SELDOMpy/src/include/include_amigo/AMIGO_problem.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/include/include_cvodes/cvodes/cvodes.h` & `SELDOMpy-0.9.7/SELDOMpy/src/include/include_cvodes/cvodes/cvodes.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/include/include_cvodes/cvodes/cvodes_band.h` & `SELDOMpy-0.9.7/SELDOMpy/src/include/include_cvodes/cvodes/cvodes_band.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/include/include_cvodes/cvodes/cvodes_bandpre.h` & `SELDOMpy-0.9.7/SELDOMpy/src/include/include_cvodes/cvodes/cvodes_bandpre.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/include/include_cvodes/cvodes/cvodes_bbdpre.h` & `SELDOMpy-0.9.7/SELDOMpy/src/include/include_cvodes/cvodes/cvodes_bbdpre.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/include/include_cvodes/cvodes/cvodes_dense.h` & `SELDOMpy-0.9.7/SELDOMpy/src/include/include_cvodes/cvodes/cvodes_dense.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/include/include_cvodes/cvodes/cvodes_diag.h` & `SELDOMpy-0.9.7/SELDOMpy/src/include/include_cvodes/cvodes/cvodes_diag.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/include/include_cvodes/cvodes/cvodes_direct.h` & `SELDOMpy-0.9.7/SELDOMpy/src/include/include_cvodes/cvodes/cvodes_direct.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/include/include_cvodes/cvodes/cvodes_lapack.h` & `SELDOMpy-0.9.7/SELDOMpy/src/include/include_cvodes/cvodes/cvodes_lapack.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/include/include_cvodes/cvodes/cvodes_spbcgs.h` & `SELDOMpy-0.9.7/SELDOMpy/src/include/include_cvodes/cvodes/cvodes_spbcgs.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/include/include_cvodes/cvodes/cvodes_spgmr.h` & `SELDOMpy-0.9.7/SELDOMpy/src/include/include_cvodes/cvodes/cvodes_spgmr.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/include/include_cvodes/cvodes/cvodes_spils.h` & `SELDOMpy-0.9.7/SELDOMpy/src/include/include_cvodes/cvodes/cvodes_spils.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/include/include_cvodes/cvodes/cvodes_sptfqmr.h` & `SELDOMpy-0.9.7/SELDOMpy/src/include/include_cvodes/cvodes/cvodes_sptfqmr.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/include/include_cvodes/nvector/nvector_serial.h` & `SELDOMpy-0.9.7/SELDOMpy/src/include/include_cvodes/nvector/nvector_serial.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/include/include_cvodes/sundials/sundials_band.h` & `SELDOMpy-0.9.7/SELDOMpy/src/include/include_cvodes/sundials/sundials_band.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/include/include_cvodes/sundials/sundials_config.h` & `SELDOMpy-0.9.7/SELDOMpy/src/include/include_cvodes/sundials/sundials_config.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/include/include_cvodes/sundials/sundials_dense.h` & `SELDOMpy-0.9.7/SELDOMpy/src/include/include_cvodes/sundials/sundials_dense.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/include/include_cvodes/sundials/sundials_direct.h` & `SELDOMpy-0.9.7/SELDOMpy/src/include/include_cvodes/sundials/sundials_direct.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/include/include_cvodes/sundials/sundials_fnvector.h` & `SELDOMpy-0.9.7/SELDOMpy/src/include/include_cvodes/sundials/sundials_fnvector.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/include/include_cvodes/sundials/sundials_iterative.h` & `SELDOMpy-0.9.7/SELDOMpy/src/include/include_cvodes/sundials/sundials_iterative.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/include/include_cvodes/sundials/sundials_lapack.h` & `SELDOMpy-0.9.7/SELDOMpy/src/include/include_cvodes/sundials/sundials_lapack.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/include/include_cvodes/sundials/sundials_math.h` & `SELDOMpy-0.9.7/SELDOMpy/src/include/include_cvodes/sundials/sundials_math.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/include/include_cvodes/sundials/sundials_nvector.h` & `SELDOMpy-0.9.7/SELDOMpy/src/include/include_cvodes/sundials/sundials_nvector.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/include/include_cvodes/sundials/sundials_spbcgs.h` & `SELDOMpy-0.9.7/SELDOMpy/src/include/include_cvodes/sundials/sundials_spbcgs.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/include/include_cvodes/sundials/sundials_spgmr.h` & `SELDOMpy-0.9.7/SELDOMpy/src/include/include_cvodes/sundials/sundials_spgmr.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/include/include_cvodes/sundials/sundials_sptfqmr.h` & `SELDOMpy-0.9.7/SELDOMpy/src/include/include_cvodes/sundials/sundials_sptfqmr.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/include/include_cvodes/sundials/sundials_types.h` & `SELDOMpy-0.9.7/SELDOMpy/src/include/include_cvodes/sundials/sundials_types.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/src/AMIGO_model.c` & `SELDOMpy-0.9.7/SELDOMpy/src/AMIGO_model.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/src/AMIGO_problem.c` & `SELDOMpy-0.9.7/SELDOMpy/src/AMIGO_problem.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/src/CNOStructure.h` & `SELDOMpy-0.9.7/SELDOMpy/src/CNOStructure.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/src/anODEModel.c` & `SELDOMpy-0.9.7/SELDOMpy/src/anODEModel.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/src/cvodea.c` & `SELDOMpy-0.9.7/SELDOMpy/src/cvodea.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/src/cvodea_io.c` & `SELDOMpy-0.9.7/SELDOMpy/src/cvodea_io.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/src/cvodes.c` & `SELDOMpy-0.9.7/SELDOMpy/src/cvodes.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/src/cvodes_band.c` & `SELDOMpy-0.9.7/SELDOMpy/src/cvodes_band.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/src/cvodes_bandpre.c` & `SELDOMpy-0.9.7/SELDOMpy/src/cvodes_bandpre.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/src/cvodes_bandpre_impl.h` & `SELDOMpy-0.9.7/SELDOMpy/src/cvodes_bandpre_impl.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/src/cvodes_bbdpre.c` & `SELDOMpy-0.9.7/SELDOMpy/src/cvodes_bbdpre.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/src/cvodes_bbdpre_impl.h` & `SELDOMpy-0.9.7/SELDOMpy/src/cvodes_bbdpre_impl.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/src/cvodes_dense.c` & `SELDOMpy-0.9.7/SELDOMpy/src/cvodes_dense.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/src/cvodes_diag.c` & `SELDOMpy-0.9.7/SELDOMpy/src/cvodes_diag.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/src/cvodes_diag_impl.h` & `SELDOMpy-0.9.7/SELDOMpy/src/cvodes_diag_impl.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/src/cvodes_direct.c` & `SELDOMpy-0.9.7/SELDOMpy/src/cvodes_direct.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/src/cvodes_direct_impl.h` & `SELDOMpy-0.9.7/SELDOMpy/src/cvodes_direct_impl.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/src/cvodes_impl.h` & `SELDOMpy-0.9.7/SELDOMpy/src/cvodes_impl.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/src/cvodes_io.c` & `SELDOMpy-0.9.7/SELDOMpy/src/cvodes_io.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/src/cvodes_spbcgs.c` & `SELDOMpy-0.9.7/SELDOMpy/src/cvodes_spbcgs.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/src/cvodes_spgmr.c` & `SELDOMpy-0.9.7/SELDOMpy/src/cvodes_spgmr.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/src/cvodes_spils.c` & `SELDOMpy-0.9.7/SELDOMpy/src/cvodes_spils.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/src/cvodes_spils_impl.h` & `SELDOMpy-0.9.7/SELDOMpy/src/cvodes_spils_impl.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/src/cvodes_sptfqmr.c` & `SELDOMpy-0.9.7/SELDOMpy/src/cvodes_sptfqmr.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/src/dhc.c` & `SELDOMpy-0.9.7/SELDOMpy/src/dhc.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/src/findStates.c` & `SELDOMpy-0.9.7/SELDOMpy/src/findStates.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/src/fnvector_serial.c` & `SELDOMpy-0.9.7/SELDOMpy/src/fnvector_serial.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/src/fnvector_serial.h` & `SELDOMpy-0.9.7/SELDOMpy/src/fnvector_serial.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/src/getAdjacencyMatrix.c` & `SELDOMpy-0.9.7/SELDOMpy/src/getAdjacencyMatrix.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/src/getStateIndex.c` & `SELDOMpy-0.9.7/SELDOMpy/src/getStateIndex.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/src/getTruthTables.c` & `SELDOMpy-0.9.7/SELDOMpy/src/getTruthTables.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/src/get_support_truth_tables.c` & `SELDOMpy-0.9.7/SELDOMpy/src/get_support_truth_tables.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/src/get_truth_tables_index.c` & `SELDOMpy-0.9.7/SELDOMpy/src/get_truth_tables_index.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/src/nvector_serial.c` & `SELDOMpy-0.9.7/SELDOMpy/src/nvector_serial.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/src/printNminiTerms.c` & `SELDOMpy-0.9.7/SELDOMpy/src/printNminiTerms.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/src/sim_logic_ode.c` & `SELDOMpy-0.9.7/SELDOMpy/src/sim_logic_ode.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/src/simulate_amigo_model.c` & `SELDOMpy-0.9.7/SELDOMpy/src/simulate_amigo_model.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/src/sundials_band.c` & `SELDOMpy-0.9.7/SELDOMpy/src/sundials_band.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/src/sundials_dense.c` & `SELDOMpy-0.9.7/SELDOMpy/src/sundials_dense.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/src/sundials_direct.c` & `SELDOMpy-0.9.7/SELDOMpy/src/sundials_direct.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/src/sundials_iterative.c` & `SELDOMpy-0.9.7/SELDOMpy/src/sundials_iterative.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/src/sundials_math.c` & `SELDOMpy-0.9.7/SELDOMpy/src/sundials_math.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/src/sundials_nvector.c` & `SELDOMpy-0.9.7/SELDOMpy/src/sundials_nvector.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/src/sundials_spbcgs.c` & `SELDOMpy-0.9.7/SELDOMpy/src/sundials_spbcgs.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/src/sundials_spgmr.c` & `SELDOMpy-0.9.7/SELDOMpy/src/sundials_spgmr.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy/src/sundials_sptfqmr.c` & `SELDOMpy-0.9.7/SELDOMpy/src/sundials_sptfqmr.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.6/SELDOMpy.egg-info/PKG-INFO` & `SELDOMpy-0.9.7/SELDOMpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SELDOMpy
-Version: 0.9.6
+Version: 0.9.7
 Summary: Dynamic modelling of cellular signalling networks.
 Home-page: https://github.com/lupralo31/SELDOMpy
 Download-URL: https://github.com/lupralo31/SELDOMpy/archive/refs/tags/V_0.2.1.tar.gz
 Author: Luis Prado
 Author-email: pradolopezluis@gmail.com
 License: GPLv3
 Keywords: SELDOMpy,SELDOM,dynamic modelling,cellular signalling networks,biomedical engineering
```

### Comparing `SELDOMpy-0.9.6/SELDOMpy.egg-info/SOURCES.txt` & `SELDOMpy-0.9.7/SELDOMpy.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -71,48 +71,14 @@
 SELDOMpy/functions/getLBODEmodel.py
 SELDOMpy/functions/getRandomLBODEmodel.py
 SELDOMpy/functions/optimization.py
 SELDOMpy/functions/plot_results.py
 SELDOMpy/functions/reduce_fun.py
 SELDOMpy/functions/simulate_logic_based_ode.py
 SELDOMpy/functions/simulate_logic_based_ode_obs.py
-SELDOMpy/include/include_amigo/AMIGO_hdf5.h
-SELDOMpy/include/include_amigo/AMIGO_model.h
-SELDOMpy/include/include_amigo/AMIGO_model_stats.h
-SELDOMpy/include/include_amigo/AMIGO_problem.h
-SELDOMpy/include/include_amigo/amigoJAC.h
-SELDOMpy/include/include_amigo/amigoRHS.h
-SELDOMpy/include/include_amigo/amigoSensRHS.h
-SELDOMpy/include/include_amigo/simulate_amigo_model.h
-SELDOMpy/include/include_cvodes/cvodes/cvodes.h
-SELDOMpy/include/include_cvodes/cvodes/cvodes_band.h
-SELDOMpy/include/include_cvodes/cvodes/cvodes_bandpre.h
-SELDOMpy/include/include_cvodes/cvodes/cvodes_bbdpre.h
-SELDOMpy/include/include_cvodes/cvodes/cvodes_dense.h
-SELDOMpy/include/include_cvodes/cvodes/cvodes_diag.h
-SELDOMpy/include/include_cvodes/cvodes/cvodes_direct.h
-SELDOMpy/include/include_cvodes/cvodes/cvodes_lapack.h
-SELDOMpy/include/include_cvodes/cvodes/cvodes_spbcgs.h
-SELDOMpy/include/include_cvodes/cvodes/cvodes_spgmr.h
-SELDOMpy/include/include_cvodes/cvodes/cvodes_spils.h
-SELDOMpy/include/include_cvodes/cvodes/cvodes_sptfqmr.h
-SELDOMpy/include/include_cvodes/nvector/nvector_serial.h
-SELDOMpy/include/include_cvodes/sundials/sundials_band.h
-SELDOMpy/include/include_cvodes/sundials/sundials_config.h
-SELDOMpy/include/include_cvodes/sundials/sundials_dense.h
-SELDOMpy/include/include_cvodes/sundials/sundials_direct.h
-SELDOMpy/include/include_cvodes/sundials/sundials_fnvector.h
-SELDOMpy/include/include_cvodes/sundials/sundials_iterative.h
-SELDOMpy/include/include_cvodes/sundials/sundials_lapack.h
-SELDOMpy/include/include_cvodes/sundials/sundials_math.h
-SELDOMpy/include/include_cvodes/sundials/sundials_nvector.h
-SELDOMpy/include/include_cvodes/sundials/sundials_spbcgs.h
-SELDOMpy/include/include_cvodes/sundials/sundials_spgmr.h
-SELDOMpy/include/include_cvodes/sundials/sundials_sptfqmr.h
-SELDOMpy/include/include_cvodes/sundials/sundials_types.h
 SELDOMpy/src/AMIGO_model.c
 SELDOMpy/src/AMIGO_model_stats.c
 SELDOMpy/src/AMIGO_problem.c
 SELDOMpy/src/CNOStructure.h
 SELDOMpy/src/__init__.py
 SELDOMpy/src/anODEModel.c
 SELDOMpy/src/cvodea.c
```

### Comparing `SELDOMpy-0.9.6/setup.py` & `SELDOMpy-0.9.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 numpy_include = np.get_include()
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='SELDOMpy',
-    version='0.9.6',
+    version='0.9.7',
     description='Dynamic modelling of cellular signalling networks.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Luis Prado',
     author_email='pradolopezluis@gmail.com',
     url='https://github.com/lupralo31/SELDOMpy',
     download_url='https://github.com/lupralo31/SELDOMpy/archive/refs/tags/V_0.2.1.tar.gz',
```

