# Comparing `tmp/SELDOMpy-0.9.2.tar.gz` & `tmp/SELDOMpy-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\SELDOMpy-0.9.2.tar", last modified: Fri Jul  7 11:39:08 2023, max compression
+gzip compressed data, was "dist\SELDOMpy-0.9.3.tar", last modified: Fri Jul  7 13:35:23 2023, max compression
```

## Comparing `SELDOMpy-0.9.2.tar` & `SELDOMpy-0.9.3.tar`

### file list

```diff
@@ -1,135 +1,135 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 11:39:08.339897 SELDOMpy-0.9.2/
--rw-rw-rw-   0        0        0    35149 2023-07-05 16:32:35.000000 SELDOMpy-0.9.2/LICENSE.txt
--rw-rw-rw-   0        0        0      564 2023-07-07 10:48:29.000000 SELDOMpy-0.9.2/MANIFEST.in
--rw-rw-rw-   0        0        0     4193 2023-07-07 11:39:08.340865 SELDOMpy-0.9.2/PKG-INFO
--rw-rw-rw-   0        0        0     3446 2023-07-06 08:12:36.000000 SELDOMpy-0.9.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-07 11:39:08.218907 SELDOMpy-0.9.2/SELDOMpy/
--rw-rw-rw-   0        0        0      490 2023-07-06 11:23:03.000000 SELDOMpy-0.9.2/SELDOMpy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-07 11:39:08.210908 SELDOMpy-0.9.2/SELDOMpy/examples/
-drwxrwxrwx   0        0        0        0 2023-07-07 11:39:08.270864 SELDOMpy-0.9.2/SELDOMpy/examples/MAPK/
--rw-rw-rw-   0        0        0    13667 2023-04-19 10:00:19.000000 SELDOMpy-0.9.2/SELDOMpy/examples/MAPK/MAPK.xlsx
--rw-rw-rw-   0        0        0     5830 2023-07-07 11:25:38.000000 SELDOMpy-0.9.2/SELDOMpy/examples/MAPK/training_and_reduce.py
--rw-rw-rw-   0        0        0    10300 2023-07-07 11:25:38.000000 SELDOMpy-0.9.2/SELDOMpy/examples/MAPK/training_and_reduce_pyPESTO.py
-drwxrwxrwx   0        0        0        0 2023-07-07 11:39:08.273863 SELDOMpy-0.9.2/SELDOMpy/examples/SP/
--rw-rw-rw-   0        0        0    23018 2023-06-21 18:44:38.000000 SELDOMpy-0.9.2/SELDOMpy/examples/SP/SP.xlsx
--rw-rw-rw-   0        0        0     6012 2023-07-07 11:25:38.000000 SELDOMpy-0.9.2/SELDOMpy/examples/SP/training_and_reduce.py
--rw-rw-rw-   0        0        0    10502 2023-07-07 11:25:38.000000 SELDOMpy-0.9.2/SELDOMpy/examples/SP/training_and_reduce_pyPESTO.py
-drwxrwxrwx   0        0        0        0 2023-07-07 11:39:08.283896 SELDOMpy-0.9.2/SELDOMpy/functions/
--rw-rw-rw-   0        0        0     1799 2023-07-06 13:38:27.000000 SELDOMpy-0.9.2/SELDOMpy/functions/buildmim.py
--rw-rw-rw-   0        0        0     1280 2023-07-07 07:34:51.000000 SELDOMpy-0.9.2/SELDOMpy/functions/extras.py
--rw-rw-rw-   0        0        0     4032 2023-07-07 07:34:51.000000 SELDOMpy-0.9.2/SELDOMpy/functions/gen_exps.py
--rw-rw-rw-   0        0        0     4860 2023-07-07 07:34:51.000000 SELDOMpy-0.9.2/SELDOMpy/functions/getLBODEmodel.py
--rw-rw-rw-   0        0        0     3156 2023-07-07 07:34:50.000000 SELDOMpy-0.9.2/SELDOMpy/functions/getRandomLBODEmodel.py
--rw-rw-rw-   0        0        0     2313 2023-07-07 11:11:37.000000 SELDOMpy-0.9.2/SELDOMpy/functions/optimization.py
--rw-rw-rw-   0        0        0     1509 2023-07-07 07:39:33.000000 SELDOMpy-0.9.2/SELDOMpy/functions/plot_results.py
--rw-rw-rw-   0        0        0     2748 2023-07-07 07:41:41.000000 SELDOMpy-0.9.2/SELDOMpy/functions/reduce_fun.py
--rw-rw-rw-   0        0        0     3802 2023-07-07 07:48:40.000000 SELDOMpy-0.9.2/SELDOMpy/functions/simulate_logic_based_ode.py
--rw-rw-rw-   0        0        0     3595 2023-07-07 07:52:38.000000 SELDOMpy-0.9.2/SELDOMpy/functions/simulate_logic_based_ode_obs.py
-drwxrwxrwx   0        0        0        0 2023-07-07 11:39:08.212891 SELDOMpy-0.9.2/SELDOMpy/include/
-drwxrwxrwx   0        0        0        0 2023-07-07 11:39:08.290893 SELDOMpy-0.9.2/SELDOMpy/include/include_amigo/
--rw-rw-rw-   0        0        0        4 2022-12-07 11:24:12.000000 SELDOMpy-0.9.2/SELDOMpy/include/include_amigo/AMIGO_hdf5.h
--rw-rw-rw-   0        0        0     3769 2022-12-07 11:24:12.000000 SELDOMpy-0.9.2/SELDOMpy/include/include_amigo/AMIGO_model.h
--rw-rw-rw-   0        0        0      442 2022-12-07 11:24:12.000000 SELDOMpy-0.9.2/SELDOMpy/include/include_amigo/AMIGO_model_stats.h
--rw-rw-rw-   0        0        0     1822 2022-12-07 11:24:12.000000 SELDOMpy-0.9.2/SELDOMpy/include/include_amigo/AMIGO_problem.h
--rw-rw-rw-   0        0        0      287 2022-12-07 11:24:12.000000 SELDOMpy-0.9.2/SELDOMpy/include/include_amigo/amigoJAC.h
--rw-rw-rw-   0        0        0       24 2022-12-07 11:24:12.000000 SELDOMpy-0.9.2/SELDOMpy/include/include_amigo/amigoRHS.h
--rw-rw-rw-   0        0        0      171 2022-12-07 11:24:12.000000 SELDOMpy-0.9.2/SELDOMpy/include/include_amigo/amigoSensRHS.h
--rw-rw-rw-   0        0        0      164 2022-12-07 11:24:12.000000 SELDOMpy-0.9.2/SELDOMpy/include/include_amigo/simulate_amigo_model.h
-drwxrwxrwx   0        0        0        0 2023-07-07 11:39:08.213888 SELDOMpy-0.9.2/SELDOMpy/include/include_cvodes/
-drwxrwxrwx   0        0        0        0 2023-07-07 11:39:08.304898 SELDOMpy-0.9.2/SELDOMpy/include/include_cvodes/cvodes/
--rw-rw-rw-   0        0        0    84971 2022-12-07 11:24:12.000000 SELDOMpy-0.9.2/SELDOMpy/include/include_cvodes/cvodes/cvodes.h
--rw-rw-rw-   0        0        0     2442 2022-12-07 11:24:12.000000 SELDOMpy-0.9.2/SELDOMpy/include/include_cvodes/cvodes/cvodes_band.h
--rw-rw-rw-   0        0        0     6547 2022-12-07 11:24:12.000000 SELDOMpy-0.9.2/SELDOMpy/include/include_cvodes/cvodes/cvodes_bandpre.h
--rw-rw-rw-   0        0        0    13259 2022-12-07 11:24:12.000000 SELDOMpy-0.9.2/SELDOMpy/include/include_cvodes/cvodes/cvodes_bbdpre.h
--rw-rw-rw-   0        0        0     2122 2022-12-07 11:24:12.000000 SELDOMpy-0.9.2/SELDOMpy/include/include_cvodes/cvodes/cvodes_dense.h
--rw-rw-rw-   0        0        0     4845 2022-12-07 11:24:12.000000 SELDOMpy-0.9.2/SELDOMpy/include/include_cvodes/cvodes/cvodes_diag.h
--rw-rw-rw-   0        0        0    14031 2022-12-07 11:24:12.000000 SELDOMpy-0.9.2/SELDOMpy/include/include_cvodes/cvodes/cvodes_direct.h
--rw-rw-rw-   0        0        0     3732 2022-12-07 11:24:12.000000 SELDOMpy-0.9.2/SELDOMpy/include/include_cvodes/cvodes/cvodes_lapack.h
--rw-rw-rw-   0        0        0     3061 2022-12-07 11:24:12.000000 SELDOMpy-0.9.2/SELDOMpy/include/include_cvodes/cvodes/cvodes_spbcgs.h
--rw-rw-rw-   0        0        0     3021 2022-12-07 11:24:12.000000 SELDOMpy-0.9.2/SELDOMpy/include/include_cvodes/cvodes/cvodes_spgmr.h
--rw-rw-rw-   0        0        0    18270 2022-12-07 11:24:13.000000 SELDOMpy-0.9.2/SELDOMpy/include/include_cvodes/cvodes/cvodes_spils.h
--rw-rw-rw-   0        0        0     3085 2022-12-07 11:24:13.000000 SELDOMpy-0.9.2/SELDOMpy/include/include_cvodes/cvodes/cvodes_sptfqmr.h
-drwxrwxrwx   0        0        0        0 2023-07-07 11:39:08.305899 SELDOMpy-0.9.2/SELDOMpy/include/include_cvodes/nvector/
--rw-rw-rw-   0        0        0    10054 2022-12-07 11:24:13.000000 SELDOMpy-0.9.2/SELDOMpy/include/include_cvodes/nvector/nvector_serial.h
-drwxrwxrwx   0        0        0        0 2023-07-07 11:39:08.317864 SELDOMpy-0.9.2/SELDOMpy/include/include_cvodes/sundials/
--rw-rw-rw-   0        0        0     6539 2022-12-07 11:24:13.000000 SELDOMpy-0.9.2/SELDOMpy/include/include_cvodes/sundials/sundials_band.h
--rw-rw-rw-   0        0        0     3157 2022-12-07 11:24:13.000000 SELDOMpy-0.9.2/SELDOMpy/include/include_cvodes/sundials/sundials_config.h
--rw-rw-rw-   0        0        0     7865 2022-12-07 11:24:13.000000 SELDOMpy-0.9.2/SELDOMpy/include/include_cvodes/sundials/sundials_dense.h
--rw-rw-rw-   0        0        0    13199 2022-12-07 11:24:13.000000 SELDOMpy-0.9.2/SELDOMpy/include/include_cvodes/sundials/sundials_direct.h
--rw-rw-rw-   0        0        0     1129 2022-12-07 11:24:13.000000 SELDOMpy-0.9.2/SELDOMpy/include/include_cvodes/sundials/sundials_fnvector.h
--rw-rw-rw-   0        0        0    13127 2022-12-07 11:24:13.000000 SELDOMpy-0.9.2/SELDOMpy/include/include_cvodes/sundials/sundials_iterative.h
--rw-rw-rw-   0        0        0     4763 2022-12-07 11:24:13.000000 SELDOMpy-0.9.2/SELDOMpy/include/include_cvodes/sundials/sundials_lapack.h
--rw-rw-rw-   0        0        0     4294 2022-12-07 11:24:13.000000 SELDOMpy-0.9.2/SELDOMpy/include/include_cvodes/sundials/sundials_math.h
--rw-rw-rw-   0        0        0    15964 2022-12-07 11:24:13.000000 SELDOMpy-0.9.2/SELDOMpy/include/include_cvodes/sundials/sundials_nvector.h
--rw-rw-rw-   0        0        0     7740 2022-12-07 11:24:13.000000 SELDOMpy-0.9.2/SELDOMpy/include/include_cvodes/sundials/sundials_spbcgs.h
--rw-rw-rw-   0        0        0    12224 2022-12-07 11:24:13.000000 SELDOMpy-0.9.2/SELDOMpy/include/include_cvodes/sundials/sundials_spgmr.h
--rw-rw-rw-   0        0        0    10246 2022-12-07 11:24:13.000000 SELDOMpy-0.9.2/SELDOMpy/include/include_cvodes/sundials/sundials_sptfqmr.h
--rw-rw-rw-   0        0        0     3726 2022-12-07 11:24:13.000000 SELDOMpy-0.9.2/SELDOMpy/include/include_cvodes/sundials/sundials_types.h
-drwxrwxrwx   0        0        0        0 2023-07-07 11:39:08.332861 SELDOMpy-0.9.2/SELDOMpy/src/
--rw-rw-rw-   0        0        0    10952 2022-12-07 11:24:11.000000 SELDOMpy-0.9.2/SELDOMpy/src/AMIGO_model.c
--rw-rw-rw-   0        0        0      240 2022-12-07 11:24:11.000000 SELDOMpy-0.9.2/SELDOMpy/src/AMIGO_model_stats.c
--rw-rw-rw-   0        0        0     8027 2022-12-07 11:24:11.000000 SELDOMpy-0.9.2/SELDOMpy/src/AMIGO_problem.c
--rw-rw-rw-   0        0        0      811 2022-12-07 11:24:11.000000 SELDOMpy-0.9.2/SELDOMpy/src/CNOStructure.h
--rw-rw-rw-   0        0        0        0 2023-07-03 16:56:56.000000 SELDOMpy-0.9.2/SELDOMpy/src/__init__.py
--rw-rw-rw-   0        0        0     3389 2023-04-10 15:09:09.000000 SELDOMpy-0.9.2/SELDOMpy/src/anODEModel.c
--rw-rw-rw-   0        0        0    74908 2022-12-07 11:24:11.000000 SELDOMpy-0.9.2/SELDOMpy/src/cvodea.c
--rw-rw-rw-   0        0        0    18585 2022-12-07 11:24:11.000000 SELDOMpy-0.9.2/SELDOMpy/src/cvodea_io.c
--rw-rw-rw-   0        0        0   245647 2022-12-07 11:24:11.000000 SELDOMpy-0.9.2/SELDOMpy/src/cvodes.c
--rw-rw-rw-   0        0        0    13293 2022-12-07 11:24:11.000000 SELDOMpy-0.9.2/SELDOMpy/src/cvodes_band.c
--rw-rw-rw-   0        0        0    16826 2022-12-07 11:24:11.000000 SELDOMpy-0.9.2/SELDOMpy/src/cvodes_bandpre.c
--rw-rw-rw-   0        0        0     2272 2022-12-07 11:24:11.000000 SELDOMpy-0.9.2/SELDOMpy/src/cvodes_bandpre_impl.h
--rw-rw-rw-   0        0        0    23592 2022-12-07 11:24:11.000000 SELDOMpy-0.9.2/SELDOMpy/src/cvodes_bbdpre.c
--rw-rw-rw-   0        0        0     2929 2022-12-07 11:24:11.000000 SELDOMpy-0.9.2/SELDOMpy/src/cvodes_bbdpre_impl.h
--rw-rw-rw-   0        0        0    12594 2022-12-07 11:24:11.000000 SELDOMpy-0.9.2/SELDOMpy/src/cvodes_dense.c
--rw-rw-rw-   0        0        0    13921 2022-12-07 11:24:11.000000 SELDOMpy-0.9.2/SELDOMpy/src/cvodes_diag.c
--rw-rw-rw-   0        0        0     2258 2022-12-07 11:24:11.000000 SELDOMpy-0.9.2/SELDOMpy/src/cvodes_diag_impl.h
--rw-rw-rw-   0        0        0    20099 2022-12-07 11:24:11.000000 SELDOMpy-0.9.2/SELDOMpy/src/cvodes_direct.c
--rw-rw-rw-   0        0        0     5473 2022-12-07 11:24:11.000000 SELDOMpy-0.9.2/SELDOMpy/src/cvodes_direct_impl.h
--rw-rw-rw-   0        0        0    47504 2022-12-07 11:24:11.000000 SELDOMpy-0.9.2/SELDOMpy/src/cvodes_impl.h
--rw-rw-rw-   0        0        0    41365 2022-12-07 11:24:11.000000 SELDOMpy-0.9.2/SELDOMpy/src/cvodes_io.c
--rw-rw-rw-   0        0        0    16912 2022-12-07 11:24:11.000000 SELDOMpy-0.9.2/SELDOMpy/src/cvodes_spbcgs.c
--rw-rw-rw-   0        0        0    17029 2022-12-07 11:24:11.000000 SELDOMpy-0.9.2/SELDOMpy/src/cvodes_spgmr.c
--rw-rw-rw-   0        0        0    32809 2022-12-07 11:24:11.000000 SELDOMpy-0.9.2/SELDOMpy/src/cvodes_spils.c
--rw-rw-rw-   0        0        0     6831 2022-12-07 11:24:11.000000 SELDOMpy-0.9.2/SELDOMpy/src/cvodes_spils_impl.h
--rw-rw-rw-   0        0        0    17108 2022-12-07 11:24:11.000000 SELDOMpy-0.9.2/SELDOMpy/src/cvodes_sptfqmr.c
--rw-rw-rw-   0        0        0      405 2022-12-07 11:24:11.000000 SELDOMpy-0.9.2/SELDOMpy/src/decimal2binary.c
--rw-rw-rw-   0        0        0     3792 2022-12-07 11:24:12.000000 SELDOMpy-0.9.2/SELDOMpy/src/dhc.c
--rw-rw-rw-   0        0        0      527 2022-12-07 11:24:12.000000 SELDOMpy-0.9.2/SELDOMpy/src/findStates.c
--rw-rw-rw-   0        0        0     3433 2022-12-07 11:24:12.000000 SELDOMpy-0.9.2/SELDOMpy/src/fnvector_serial.c
--rw-rw-rw-   0        0        0     2688 2022-12-07 11:24:12.000000 SELDOMpy-0.9.2/SELDOMpy/src/fnvector_serial.h
--rw-rw-rw-   0        0        0      693 2022-12-07 11:24:12.000000 SELDOMpy-0.9.2/SELDOMpy/src/getAdjacencyMatrix.c
--rw-rw-rw-   0        0        0      463 2022-12-07 11:24:12.000000 SELDOMpy-0.9.2/SELDOMpy/src/getNumBits.c
--rw-rw-rw-   0        0        0      475 2022-12-07 11:24:12.000000 SELDOMpy-0.9.2/SELDOMpy/src/getNumInputs.c
--rw-rw-rw-   0        0        0      695 2022-12-07 11:24:12.000000 SELDOMpy-0.9.2/SELDOMpy/src/getStateIndex.c
--rw-rw-rw-   0        0        0     3859 2022-12-07 11:24:12.000000 SELDOMpy-0.9.2/SELDOMpy/src/getTruthTables.c
--rw-rw-rw-   0        0        0      451 2022-12-07 11:24:12.000000 SELDOMpy-0.9.2/SELDOMpy/src/get_count_bits.c
--rw-rw-rw-   0        0        0      487 2022-12-07 11:24:12.000000 SELDOMpy-0.9.2/SELDOMpy/src/get_input_index.c
--rw-rw-rw-   0        0        0      594 2022-12-07 11:24:12.000000 SELDOMpy-0.9.2/SELDOMpy/src/get_support_truth_tables.c
--rw-rw-rw-   0        0        0      585 2022-12-07 11:24:12.000000 SELDOMpy-0.9.2/SELDOMpy/src/get_truth_tables_index.c
--rw-rw-rw-   0        0        0      224 2022-12-07 11:24:12.000000 SELDOMpy-0.9.2/SELDOMpy/src/hill_function.c
--rw-rw-rw-   0        0        0      219 2022-12-07 11:24:12.000000 SELDOMpy-0.9.2/SELDOMpy/src/linear_transfer_function.c
--rw-rw-rw-   0        0        0      227 2022-12-07 11:24:12.000000 SELDOMpy-0.9.2/SELDOMpy/src/normHill.c
--rw-rw-rw-   0        0        0    20778 2022-12-07 11:24:12.000000 SELDOMpy-0.9.2/SELDOMpy/src/nvector_serial.c
--rw-rw-rw-   0        0        0      305 2022-12-07 11:24:12.000000 SELDOMpy-0.9.2/SELDOMpy/src/printAdjMat.c
--rw-rw-rw-   0        0        0      315 2022-12-07 11:24:12.000000 SELDOMpy-0.9.2/SELDOMpy/src/printInterMat.c
--rw-rw-rw-   0        0        0      553 2022-12-07 11:24:12.000000 SELDOMpy-0.9.2/SELDOMpy/src/printNminiTerms.c
--rw-rw-rw-   0        0        0      410 2022-12-07 11:24:12.000000 SELDOMpy-0.9.2/SELDOMpy/src/printTruthTables.c
--rw-rw-rw-   0        0        0    15775 2023-04-28 16:16:22.000000 SELDOMpy-0.9.2/SELDOMpy/src/sim_logic_ode.c
--rw-rw-rw-   0        0        0     9815 2022-12-07 11:24:12.000000 SELDOMpy-0.9.2/SELDOMpy/src/simulate_amigo_model.c
--rw-rw-rw-   0        0        0     6036 2022-12-07 11:24:12.000000 SELDOMpy-0.9.2/SELDOMpy/src/sundials_band.c
--rw-rw-rw-   0        0        0     8510 2022-12-07 11:24:12.000000 SELDOMpy-0.9.2/SELDOMpy/src/sundials_dense.c
--rw-rw-rw-   0        0        0     6225 2022-12-07 11:24:12.000000 SELDOMpy-0.9.2/SELDOMpy/src/sundials_direct.c
--rw-rw-rw-   0        0        0     7662 2022-12-07 11:24:12.000000 SELDOMpy-0.9.2/SELDOMpy/src/sundials_iterative.c
--rw-rw-rw-   0        0        0     2474 2022-12-07 11:24:12.000000 SELDOMpy-0.9.2/SELDOMpy/src/sundials_math.c
--rw-rw-rw-   0        0        0     4702 2022-12-07 11:24:12.000000 SELDOMpy-0.9.2/SELDOMpy/src/sundials_nvector.c
--rw-rw-rw-   0        0        0     9663 2022-12-07 11:24:12.000000 SELDOMpy-0.9.2/SELDOMpy/src/sundials_spbcgs.c
--rw-rw-rw-   0        0        0    12650 2022-12-07 11:24:12.000000 SELDOMpy-0.9.2/SELDOMpy/src/sundials_spgmr.c
--rw-rw-rw-   0        0        0    14744 2022-12-07 11:24:12.000000 SELDOMpy-0.9.2/SELDOMpy/src/sundials_sptfqmr.c
-drwxrwxrwx   0        0        0        0 2023-07-07 11:39:08.223887 SELDOMpy-0.9.2/SELDOMpy.egg-info/
--rw-rw-rw-   0        0        0     4193 2023-07-07 11:39:07.000000 SELDOMpy-0.9.2/SELDOMpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5924 2023-07-07 11:39:08.000000 SELDOMpy-0.9.2/SELDOMpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 11:39:07.000000 SELDOMpy-0.9.2/SELDOMpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2023-07-07 11:39:07.000000 SELDOMpy-0.9.2/SELDOMpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-07 11:39:07.000000 SELDOMpy-0.9.2/SELDOMpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      115 2023-07-07 11:39:08.340865 SELDOMpy-0.9.2/setup.cfg
--rw-rw-rw-   0        0        0     3505 2023-07-07 11:39:00.000000 SELDOMpy-0.9.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 13:35:23.976190 SELDOMpy-0.9.3/
+-rw-rw-rw-   0        0        0    35149 2023-07-05 16:32:35.000000 SELDOMpy-0.9.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      580 2023-07-07 11:47:15.000000 SELDOMpy-0.9.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     4171 2023-07-07 13:35:23.976190 SELDOMpy-0.9.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3446 2023-07-06 08:12:36.000000 SELDOMpy-0.9.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-07 13:35:23.843189 SELDOMpy-0.9.3/SELDOMpy/
+-rw-rw-rw-   0        0        0      490 2023-07-06 11:23:03.000000 SELDOMpy-0.9.3/SELDOMpy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 13:35:23.833189 SELDOMpy-0.9.3/SELDOMpy/examples/
+drwxrwxrwx   0        0        0        0 2023-07-07 13:35:23.908180 SELDOMpy-0.9.3/SELDOMpy/examples/MAPK/
+-rw-rw-rw-   0        0        0    13667 2023-04-19 10:00:19.000000 SELDOMpy-0.9.3/SELDOMpy/examples/MAPK/MAPK.xlsx
+-rw-rw-rw-   0        0        0     5830 2023-07-07 11:25:38.000000 SELDOMpy-0.9.3/SELDOMpy/examples/MAPK/MAPK_training_and_reduce.py
+-rw-rw-rw-   0        0        0    10464 2023-07-07 13:32:37.000000 SELDOMpy-0.9.3/SELDOMpy/examples/MAPK/MAPK_training_and_reduce_pyPESTO.py
+drwxrwxrwx   0        0        0        0 2023-07-07 13:35:23.911204 SELDOMpy-0.9.3/SELDOMpy/examples/SP/
+-rw-rw-rw-   0        0        0    23018 2023-06-21 18:44:38.000000 SELDOMpy-0.9.3/SELDOMpy/examples/SP/SP.xlsx
+-rw-rw-rw-   0        0        0     6011 2023-07-07 11:49:56.000000 SELDOMpy-0.9.3/SELDOMpy/examples/SP/SP_training_and_reduce.py
+-rw-rw-rw-   0        0        0    10661 2023-07-07 13:32:38.000000 SELDOMpy-0.9.3/SELDOMpy/examples/SP/SP_training_and_reduce_pyPESTO.py
+drwxrwxrwx   0        0        0        0 2023-07-07 13:35:23.923188 SELDOMpy-0.9.3/SELDOMpy/functions/
+-rw-rw-rw-   0        0        0     1799 2023-07-06 13:38:27.000000 SELDOMpy-0.9.3/SELDOMpy/functions/buildmim.py
+-rw-rw-rw-   0        0        0     1280 2023-07-07 07:34:51.000000 SELDOMpy-0.9.3/SELDOMpy/functions/extras.py
+-rw-rw-rw-   0        0        0     4037 2023-07-07 11:47:15.000000 SELDOMpy-0.9.3/SELDOMpy/functions/gen_exps.py
+-rw-rw-rw-   0        0        0     4860 2023-07-07 07:34:51.000000 SELDOMpy-0.9.3/SELDOMpy/functions/getLBODEmodel.py
+-rw-rw-rw-   0        0        0     3156 2023-07-07 07:34:50.000000 SELDOMpy-0.9.3/SELDOMpy/functions/getRandomLBODEmodel.py
+-rw-rw-rw-   0        0        0     2313 2023-07-07 11:11:37.000000 SELDOMpy-0.9.3/SELDOMpy/functions/optimization.py
+-rw-rw-rw-   0        0        0     1509 2023-07-07 07:39:33.000000 SELDOMpy-0.9.3/SELDOMpy/functions/plot_results.py
+-rw-rw-rw-   0        0        0     2748 2023-07-07 07:41:41.000000 SELDOMpy-0.9.3/SELDOMpy/functions/reduce_fun.py
+-rw-rw-rw-   0        0        0     3802 2023-07-07 07:48:40.000000 SELDOMpy-0.9.3/SELDOMpy/functions/simulate_logic_based_ode.py
+-rw-rw-rw-   0        0        0     3595 2023-07-07 07:52:38.000000 SELDOMpy-0.9.3/SELDOMpy/functions/simulate_logic_based_ode_obs.py
+drwxrwxrwx   0        0        0        0 2023-07-07 13:35:23.836190 SELDOMpy-0.9.3/SELDOMpy/include/
+drwxrwxrwx   0        0        0        0 2023-07-07 13:35:23.932246 SELDOMpy-0.9.3/SELDOMpy/include/include_amigo/
+-rw-rw-rw-   0        0        0        4 2022-12-07 11:24:12.000000 SELDOMpy-0.9.3/SELDOMpy/include/include_amigo/AMIGO_hdf5.h
+-rw-rw-rw-   0        0        0     3769 2022-12-07 11:24:12.000000 SELDOMpy-0.9.3/SELDOMpy/include/include_amigo/AMIGO_model.h
+-rw-rw-rw-   0        0        0      442 2022-12-07 11:24:12.000000 SELDOMpy-0.9.3/SELDOMpy/include/include_amigo/AMIGO_model_stats.h
+-rw-rw-rw-   0        0        0     1822 2022-12-07 11:24:12.000000 SELDOMpy-0.9.3/SELDOMpy/include/include_amigo/AMIGO_problem.h
+-rw-rw-rw-   0        0        0      287 2022-12-07 11:24:12.000000 SELDOMpy-0.9.3/SELDOMpy/include/include_amigo/amigoJAC.h
+-rw-rw-rw-   0        0        0       24 2022-12-07 11:24:12.000000 SELDOMpy-0.9.3/SELDOMpy/include/include_amigo/amigoRHS.h
+-rw-rw-rw-   0        0        0      171 2022-12-07 11:24:12.000000 SELDOMpy-0.9.3/SELDOMpy/include/include_amigo/amigoSensRHS.h
+-rw-rw-rw-   0        0        0      164 2022-12-07 11:24:12.000000 SELDOMpy-0.9.3/SELDOMpy/include/include_amigo/simulate_amigo_model.h
+drwxrwxrwx   0        0        0        0 2023-07-07 13:35:23.837190 SELDOMpy-0.9.3/SELDOMpy/include/include_cvodes/
+drwxrwxrwx   0        0        0        0 2023-07-07 13:35:23.944208 SELDOMpy-0.9.3/SELDOMpy/include/include_cvodes/cvodes/
+-rw-rw-rw-   0        0        0    84971 2022-12-07 11:24:12.000000 SELDOMpy-0.9.3/SELDOMpy/include/include_cvodes/cvodes/cvodes.h
+-rw-rw-rw-   0        0        0     2442 2022-12-07 11:24:12.000000 SELDOMpy-0.9.3/SELDOMpy/include/include_cvodes/cvodes/cvodes_band.h
+-rw-rw-rw-   0        0        0     6547 2022-12-07 11:24:12.000000 SELDOMpy-0.9.3/SELDOMpy/include/include_cvodes/cvodes/cvodes_bandpre.h
+-rw-rw-rw-   0        0        0    13259 2022-12-07 11:24:12.000000 SELDOMpy-0.9.3/SELDOMpy/include/include_cvodes/cvodes/cvodes_bbdpre.h
+-rw-rw-rw-   0        0        0     2122 2022-12-07 11:24:12.000000 SELDOMpy-0.9.3/SELDOMpy/include/include_cvodes/cvodes/cvodes_dense.h
+-rw-rw-rw-   0        0        0     4845 2022-12-07 11:24:12.000000 SELDOMpy-0.9.3/SELDOMpy/include/include_cvodes/cvodes/cvodes_diag.h
+-rw-rw-rw-   0        0        0    14031 2022-12-07 11:24:12.000000 SELDOMpy-0.9.3/SELDOMpy/include/include_cvodes/cvodes/cvodes_direct.h
+-rw-rw-rw-   0        0        0     3732 2022-12-07 11:24:12.000000 SELDOMpy-0.9.3/SELDOMpy/include/include_cvodes/cvodes/cvodes_lapack.h
+-rw-rw-rw-   0        0        0     3061 2022-12-07 11:24:12.000000 SELDOMpy-0.9.3/SELDOMpy/include/include_cvodes/cvodes/cvodes_spbcgs.h
+-rw-rw-rw-   0        0        0     3021 2022-12-07 11:24:12.000000 SELDOMpy-0.9.3/SELDOMpy/include/include_cvodes/cvodes/cvodes_spgmr.h
+-rw-rw-rw-   0        0        0    18270 2022-12-07 11:24:13.000000 SELDOMpy-0.9.3/SELDOMpy/include/include_cvodes/cvodes/cvodes_spils.h
+-rw-rw-rw-   0        0        0     3085 2022-12-07 11:24:13.000000 SELDOMpy-0.9.3/SELDOMpy/include/include_cvodes/cvodes/cvodes_sptfqmr.h
+drwxrwxrwx   0        0        0        0 2023-07-07 13:35:23.945208 SELDOMpy-0.9.3/SELDOMpy/include/include_cvodes/nvector/
+-rw-rw-rw-   0        0        0    10054 2022-12-07 11:24:13.000000 SELDOMpy-0.9.3/SELDOMpy/include/include_cvodes/nvector/nvector_serial.h
+drwxrwxrwx   0        0        0        0 2023-07-07 13:35:23.957189 SELDOMpy-0.9.3/SELDOMpy/include/include_cvodes/sundials/
+-rw-rw-rw-   0        0        0     6539 2022-12-07 11:24:13.000000 SELDOMpy-0.9.3/SELDOMpy/include/include_cvodes/sundials/sundials_band.h
+-rw-rw-rw-   0        0        0     3157 2022-12-07 11:24:13.000000 SELDOMpy-0.9.3/SELDOMpy/include/include_cvodes/sundials/sundials_config.h
+-rw-rw-rw-   0        0        0     7865 2022-12-07 11:24:13.000000 SELDOMpy-0.9.3/SELDOMpy/include/include_cvodes/sundials/sundials_dense.h
+-rw-rw-rw-   0        0        0    13199 2022-12-07 11:24:13.000000 SELDOMpy-0.9.3/SELDOMpy/include/include_cvodes/sundials/sundials_direct.h
+-rw-rw-rw-   0        0        0     1129 2022-12-07 11:24:13.000000 SELDOMpy-0.9.3/SELDOMpy/include/include_cvodes/sundials/sundials_fnvector.h
+-rw-rw-rw-   0        0        0    13127 2022-12-07 11:24:13.000000 SELDOMpy-0.9.3/SELDOMpy/include/include_cvodes/sundials/sundials_iterative.h
+-rw-rw-rw-   0        0        0     4763 2022-12-07 11:24:13.000000 SELDOMpy-0.9.3/SELDOMpy/include/include_cvodes/sundials/sundials_lapack.h
+-rw-rw-rw-   0        0        0     4294 2022-12-07 11:24:13.000000 SELDOMpy-0.9.3/SELDOMpy/include/include_cvodes/sundials/sundials_math.h
+-rw-rw-rw-   0        0        0    15964 2022-12-07 11:24:13.000000 SELDOMpy-0.9.3/SELDOMpy/include/include_cvodes/sundials/sundials_nvector.h
+-rw-rw-rw-   0        0        0     7740 2022-12-07 11:24:13.000000 SELDOMpy-0.9.3/SELDOMpy/include/include_cvodes/sundials/sundials_spbcgs.h
+-rw-rw-rw-   0        0        0    12224 2022-12-07 11:24:13.000000 SELDOMpy-0.9.3/SELDOMpy/include/include_cvodes/sundials/sundials_spgmr.h
+-rw-rw-rw-   0        0        0    10246 2022-12-07 11:24:13.000000 SELDOMpy-0.9.3/SELDOMpy/include/include_cvodes/sundials/sundials_sptfqmr.h
+-rw-rw-rw-   0        0        0     3726 2022-12-07 11:24:13.000000 SELDOMpy-0.9.3/SELDOMpy/include/include_cvodes/sundials/sundials_types.h
+drwxrwxrwx   0        0        0        0 2023-07-07 13:35:23.970189 SELDOMpy-0.9.3/SELDOMpy/src/
+-rw-rw-rw-   0        0        0    10952 2022-12-07 11:24:11.000000 SELDOMpy-0.9.3/SELDOMpy/src/AMIGO_model.c
+-rw-rw-rw-   0        0        0      240 2022-12-07 11:24:11.000000 SELDOMpy-0.9.3/SELDOMpy/src/AMIGO_model_stats.c
+-rw-rw-rw-   0        0        0     8027 2022-12-07 11:24:11.000000 SELDOMpy-0.9.3/SELDOMpy/src/AMIGO_problem.c
+-rw-rw-rw-   0        0        0      811 2022-12-07 11:24:11.000000 SELDOMpy-0.9.3/SELDOMpy/src/CNOStructure.h
+-rw-rw-rw-   0        0        0        0 2023-07-03 16:56:56.000000 SELDOMpy-0.9.3/SELDOMpy/src/__init__.py
+-rw-rw-rw-   0        0        0     3389 2023-04-10 15:09:09.000000 SELDOMpy-0.9.3/SELDOMpy/src/anODEModel.c
+-rw-rw-rw-   0        0        0    74908 2022-12-07 11:24:11.000000 SELDOMpy-0.9.3/SELDOMpy/src/cvodea.c
+-rw-rw-rw-   0        0        0    18585 2022-12-07 11:24:11.000000 SELDOMpy-0.9.3/SELDOMpy/src/cvodea_io.c
+-rw-rw-rw-   0        0        0   245647 2022-12-07 11:24:11.000000 SELDOMpy-0.9.3/SELDOMpy/src/cvodes.c
+-rw-rw-rw-   0        0        0    13293 2022-12-07 11:24:11.000000 SELDOMpy-0.9.3/SELDOMpy/src/cvodes_band.c
+-rw-rw-rw-   0        0        0    16826 2022-12-07 11:24:11.000000 SELDOMpy-0.9.3/SELDOMpy/src/cvodes_bandpre.c
+-rw-rw-rw-   0        0        0     2272 2022-12-07 11:24:11.000000 SELDOMpy-0.9.3/SELDOMpy/src/cvodes_bandpre_impl.h
+-rw-rw-rw-   0        0        0    23592 2022-12-07 11:24:11.000000 SELDOMpy-0.9.3/SELDOMpy/src/cvodes_bbdpre.c
+-rw-rw-rw-   0        0        0     2929 2022-12-07 11:24:11.000000 SELDOMpy-0.9.3/SELDOMpy/src/cvodes_bbdpre_impl.h
+-rw-rw-rw-   0        0        0    12594 2022-12-07 11:24:11.000000 SELDOMpy-0.9.3/SELDOMpy/src/cvodes_dense.c
+-rw-rw-rw-   0        0        0    13921 2022-12-07 11:24:11.000000 SELDOMpy-0.9.3/SELDOMpy/src/cvodes_diag.c
+-rw-rw-rw-   0        0        0     2258 2022-12-07 11:24:11.000000 SELDOMpy-0.9.3/SELDOMpy/src/cvodes_diag_impl.h
+-rw-rw-rw-   0        0        0    20099 2022-12-07 11:24:11.000000 SELDOMpy-0.9.3/SELDOMpy/src/cvodes_direct.c
+-rw-rw-rw-   0        0        0     5473 2022-12-07 11:24:11.000000 SELDOMpy-0.9.3/SELDOMpy/src/cvodes_direct_impl.h
+-rw-rw-rw-   0        0        0    47504 2022-12-07 11:24:11.000000 SELDOMpy-0.9.3/SELDOMpy/src/cvodes_impl.h
+-rw-rw-rw-   0        0        0    41365 2022-12-07 11:24:11.000000 SELDOMpy-0.9.3/SELDOMpy/src/cvodes_io.c
+-rw-rw-rw-   0        0        0    16912 2022-12-07 11:24:11.000000 SELDOMpy-0.9.3/SELDOMpy/src/cvodes_spbcgs.c
+-rw-rw-rw-   0        0        0    17029 2022-12-07 11:24:11.000000 SELDOMpy-0.9.3/SELDOMpy/src/cvodes_spgmr.c
+-rw-rw-rw-   0        0        0    32809 2022-12-07 11:24:11.000000 SELDOMpy-0.9.3/SELDOMpy/src/cvodes_spils.c
+-rw-rw-rw-   0        0        0     6831 2022-12-07 11:24:11.000000 SELDOMpy-0.9.3/SELDOMpy/src/cvodes_spils_impl.h
+-rw-rw-rw-   0        0        0    17108 2022-12-07 11:24:11.000000 SELDOMpy-0.9.3/SELDOMpy/src/cvodes_sptfqmr.c
+-rw-rw-rw-   0        0        0      405 2022-12-07 11:24:11.000000 SELDOMpy-0.9.3/SELDOMpy/src/decimal2binary.c
+-rw-rw-rw-   0        0        0     3792 2022-12-07 11:24:12.000000 SELDOMpy-0.9.3/SELDOMpy/src/dhc.c
+-rw-rw-rw-   0        0        0      527 2022-12-07 11:24:12.000000 SELDOMpy-0.9.3/SELDOMpy/src/findStates.c
+-rw-rw-rw-   0        0        0     3433 2022-12-07 11:24:12.000000 SELDOMpy-0.9.3/SELDOMpy/src/fnvector_serial.c
+-rw-rw-rw-   0        0        0     2688 2022-12-07 11:24:12.000000 SELDOMpy-0.9.3/SELDOMpy/src/fnvector_serial.h
+-rw-rw-rw-   0        0        0      693 2022-12-07 11:24:12.000000 SELDOMpy-0.9.3/SELDOMpy/src/getAdjacencyMatrix.c
+-rw-rw-rw-   0        0        0      463 2022-12-07 11:24:12.000000 SELDOMpy-0.9.3/SELDOMpy/src/getNumBits.c
+-rw-rw-rw-   0        0        0      475 2022-12-07 11:24:12.000000 SELDOMpy-0.9.3/SELDOMpy/src/getNumInputs.c
+-rw-rw-rw-   0        0        0      695 2022-12-07 11:24:12.000000 SELDOMpy-0.9.3/SELDOMpy/src/getStateIndex.c
+-rw-rw-rw-   0        0        0     3859 2022-12-07 11:24:12.000000 SELDOMpy-0.9.3/SELDOMpy/src/getTruthTables.c
+-rw-rw-rw-   0        0        0      451 2022-12-07 11:24:12.000000 SELDOMpy-0.9.3/SELDOMpy/src/get_count_bits.c
+-rw-rw-rw-   0        0        0      487 2022-12-07 11:24:12.000000 SELDOMpy-0.9.3/SELDOMpy/src/get_input_index.c
+-rw-rw-rw-   0        0        0      594 2022-12-07 11:24:12.000000 SELDOMpy-0.9.3/SELDOMpy/src/get_support_truth_tables.c
+-rw-rw-rw-   0        0        0      585 2022-12-07 11:24:12.000000 SELDOMpy-0.9.3/SELDOMpy/src/get_truth_tables_index.c
+-rw-rw-rw-   0        0        0      224 2022-12-07 11:24:12.000000 SELDOMpy-0.9.3/SELDOMpy/src/hill_function.c
+-rw-rw-rw-   0        0        0      219 2022-12-07 11:24:12.000000 SELDOMpy-0.9.3/SELDOMpy/src/linear_transfer_function.c
+-rw-rw-rw-   0        0        0      227 2022-12-07 11:24:12.000000 SELDOMpy-0.9.3/SELDOMpy/src/normHill.c
+-rw-rw-rw-   0        0        0    20778 2022-12-07 11:24:12.000000 SELDOMpy-0.9.3/SELDOMpy/src/nvector_serial.c
+-rw-rw-rw-   0        0        0      305 2022-12-07 11:24:12.000000 SELDOMpy-0.9.3/SELDOMpy/src/printAdjMat.c
+-rw-rw-rw-   0        0        0      315 2022-12-07 11:24:12.000000 SELDOMpy-0.9.3/SELDOMpy/src/printInterMat.c
+-rw-rw-rw-   0        0        0      553 2022-12-07 11:24:12.000000 SELDOMpy-0.9.3/SELDOMpy/src/printNminiTerms.c
+-rw-rw-rw-   0        0        0      410 2022-12-07 11:24:12.000000 SELDOMpy-0.9.3/SELDOMpy/src/printTruthTables.c
+-rw-rw-rw-   0        0        0    15775 2023-04-28 16:16:22.000000 SELDOMpy-0.9.3/SELDOMpy/src/sim_logic_ode.c
+-rw-rw-rw-   0        0        0     9815 2022-12-07 11:24:12.000000 SELDOMpy-0.9.3/SELDOMpy/src/simulate_amigo_model.c
+-rw-rw-rw-   0        0        0     6036 2022-12-07 11:24:12.000000 SELDOMpy-0.9.3/SELDOMpy/src/sundials_band.c
+-rw-rw-rw-   0        0        0     8510 2022-12-07 11:24:12.000000 SELDOMpy-0.9.3/SELDOMpy/src/sundials_dense.c
+-rw-rw-rw-   0        0        0     6225 2022-12-07 11:24:12.000000 SELDOMpy-0.9.3/SELDOMpy/src/sundials_direct.c
+-rw-rw-rw-   0        0        0     7662 2022-12-07 11:24:12.000000 SELDOMpy-0.9.3/SELDOMpy/src/sundials_iterative.c
+-rw-rw-rw-   0        0        0     2474 2022-12-07 11:24:12.000000 SELDOMpy-0.9.3/SELDOMpy/src/sundials_math.c
+-rw-rw-rw-   0        0        0     4702 2022-12-07 11:24:12.000000 SELDOMpy-0.9.3/SELDOMpy/src/sundials_nvector.c
+-rw-rw-rw-   0        0        0     9663 2022-12-07 11:24:12.000000 SELDOMpy-0.9.3/SELDOMpy/src/sundials_spbcgs.c
+-rw-rw-rw-   0        0        0    12650 2022-12-07 11:24:12.000000 SELDOMpy-0.9.3/SELDOMpy/src/sundials_spgmr.c
+-rw-rw-rw-   0        0        0    14744 2022-12-07 11:24:12.000000 SELDOMpy-0.9.3/SELDOMpy/src/sundials_sptfqmr.c
+drwxrwxrwx   0        0        0        0 2023-07-07 13:35:23.848225 SELDOMpy-0.9.3/SELDOMpy.egg-info/
+-rw-rw-rw-   0        0        0     4171 2023-07-07 13:35:23.000000 SELDOMpy-0.9.3/SELDOMpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5940 2023-07-07 13:35:23.000000 SELDOMpy-0.9.3/SELDOMpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 13:35:23.000000 SELDOMpy-0.9.3/SELDOMpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2023-07-07 13:35:23.000000 SELDOMpy-0.9.3/SELDOMpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-07 13:35:23.000000 SELDOMpy-0.9.3/SELDOMpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      115 2023-07-07 13:35:23.977190 SELDOMpy-0.9.3/setup.cfg
+-rw-rw-rw-   0        0        0     3492 2023-07-07 13:32:38.000000 SELDOMpy-0.9.3/setup.py
```

### Comparing `SELDOMpy-0.9.2/LICENSE.txt` & `SELDOMpy-0.9.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/MANIFEST.in` & `SELDOMpy-0.9.3/MANIFEST.in`

 * *Files 19% similar despite different names*

```diff
@@ -3,12 +3,12 @@
 include SELDOMpy/include/include_amigo/*.h
 include SELDOMpy/include/include_cvodes/cvodes/*.h
 include SELDOMpy/include/include_cvodes/nvector/*.h
 include SELDOMpy/include/include_cvodes/sundials/*.h
 include SELDOMpy/src/*.h
 include SELDOMpy/functions/*.py
 include SELDOMpy/examples/MAPK/MAPK.xlsx
-include SELDOMpy/examples/MAPK/training_and_reduce.py
-include SELDOMpy/examples/SP/training_and_reduce.py
+include SELDOMpy/examples/MAPK/MAPK_training_and_reduce.py
+include SELDOMpy/examples/SP/SP_training_and_reduce.py
 include SELDOMpy/examples/SP/SP.xlsx
-include SELDOMpy/examples/MAPK/training_and_reduce_pyPESTO.py
-include SELDOMpy/examples/SP/training_and_reduce_pyPESTO.py
+include SELDOMpy/examples/MAPK/MAPK_training_and_reduce_pyPESTO.py
+include SELDOMpy/examples/SP/SP_training_and_reduce_pyPESTO.py
```

### Comparing `SELDOMpy-0.9.2/PKG-INFO` & `SELDOMpy-0.9.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: SELDOMpy
-Version: 0.9.2
-Summary: This package performs dynamic modelling of cellular signalling networks.
+Version: 0.9.3
+Summary: Dynamic modelling of cellular signalling networks.
 Home-page: https://github.com/lupralo31/SELDOMpy
 Download-URL: https://github.com/lupralo31/SELDOMpy/archive/refs/tags/V_0.2.1.tar.gz
 Author: Luis Prado
 Author-email: pradolopezluis@gmail.com
 License: GPLv3
 Keywords: SELDOMpy,SELDOM,dynamic modelling,cellular signalling networks,biomedical engineering
 Classifier: Programming Language :: Python :: 3
```

### Comparing `SELDOMpy-0.9.2/README.md` & `SELDOMpy-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/examples/MAPK/MAPK.xlsx` & `SELDOMpy-0.9.3/SELDOMpy/examples/MAPK/MAPK.xlsx`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/examples/MAPK/training_and_reduce.py` & `SELDOMpy-0.9.3/SELDOMpy/examples/MAPK/MAPK_training_and_reduce.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/examples/MAPK/training_and_reduce_pyPESTO.py` & `SELDOMpy-0.9.3/SELDOMpy/examples/MAPK/MAPK_training_and_reduce_pyPESTO.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 from SELDOMpy import *
 import os
 import pypesto
 import pypesto.optimize as optimize
 import threading
+import warnings
+from scipy.optimize import OptimizeWarning
 
+# Optimization warnings are filtered
+warnings.filterwarnings("ignore", category=OptimizeWarning)
 
 # This file is generic. In this case it is being used for the MAPK network, but it is recommended to modify the name
 # data of the Excel file, and parameters of simulations and optimization instead of creating another new file since
 # the structure of the algorithm is always the same.
 
 # In this case it is used as optimizer "pyPESTO", which gives the user the possibility to work with multiple optimizers.
 # This time the Scatter Search method is being used
@@ -202,15 +206,15 @@
         problem = pypesto.Problem(objective=objective, lb=LB, ub=UB)
 
         # The local optimizer is defined
         optimizer = optimize.ScipyOptimizer(method="Powell")
 
         # The global optimizer is defined
         optimizer_ESS = pypesto.optimize.CESSOptimizer([{"dim_refset": 20, "local_n1": 3, "local_n2": 3,
-                                                         "n_diverse": 50, "max_eval": 1, "n_procs": 8,
+                                                         "n_diverse": 50, "max_eval": 20000, "n_procs": 8,
                                                          "local_optimizer": optimizer}], max_iter=1)
 
         # The starting points of the variables to be optimized are calculated
         start = pypesto.startpoint.to_startpoint_method(pypesto.startpoint.uniform)
 
         # Optimization results are obtained
         result = optimizer_ESS.minimize(problem, start)
```

### Comparing `SELDOMpy-0.9.2/SELDOMpy/examples/SP/SP.xlsx` & `SELDOMpy-0.9.3/SELDOMpy/examples/SP/SP.xlsx`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/examples/SP/training_and_reduce.py` & `SELDOMpy-0.9.3/SELDOMpy/examples/SP/SP_training_and_reduce.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 # The adjacency matrix is calculated from "conc_data". You can also specify the number of bins
 # to be performed for the discretization of the measures in the calculation of mutual information
 adjMat = buildmim(conc_data, NBINS)
 
 
 # Generation of model parameters for subsequent simulation
-model = getLBODEmodel(adjMat, random=False, is_stimuli=exps[0].is_stimuli, maxInput=REALK, min_tau=0.1, max_tau=12,
+model = getLBODEmodel(adjMat, random=True, is_stimuli=exps[0].is_stimuli, maxInput=REALK, min_tau=0.1, max_tau=12,
                       max_n=5, min_n=1, min_k=0.1, max_k=1)
 
 
 # The "ivpsol" object is created for simulations
 ivpsol = Ivpsol(atol=1e-5, rtol=1e-5, max_step_size=0.1, max_num_steps=int(5000), max_error_test_fails=int(50))
 
 model.nthreads = int(8)
```

### Comparing `SELDOMpy-0.9.2/SELDOMpy/examples/SP/training_and_reduce_pyPESTO.py` & `SELDOMpy-0.9.3/SELDOMpy/examples/SP/SP_training_and_reduce_pyPESTO.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 from SELDOMpy import *
 import os
 import pypesto
 import pypesto.optimize as optimize
 import threading
+from scipy.optimize import OptimizeWarning
+import warnings
+
+# Optimization warnings are filtered
+warnings.filterwarnings("ignore", category=OptimizeWarning)
 
 
 # This file is generic. In this case it is being used for the MAPK network, but it is recommended to modify the name
 # data of the Excel file, and parameters of simulations and optimization instead of creating another new file since
 # the structure of the algorithm is always the same.
 
 # In this case it is used as optimizer "pyPESTO", which gives the user the possibility to work with multiple optimizers.
@@ -16,30 +21,30 @@
 
 # The initial seed that you want to use for the generation of random numbers is established
 initial_seed = 6
 rdm.seed(initial_seed)
 
 
 NBINS = 10  # Number of bins for discretization of measured values for calculation of mutual information
-REALK = 4  # Maximum number of entries (max number of 1s in each column of adjMat)
+REALK = 3  # Maximum number of entries (max number of 1s in each column of adjMat)
 
 # The object "exps" is generated with data from the experiments and the matrix "conc_data" with the measurements of the nodes
 exps, conc_data = gen_exps("SP.xlsx")
 
 for iexp in range(len(exps)):
     exps[iexp].y0 = exps[iexp].exp_data[0]
 
 
 # The adjacency matrix is calculated from "conc_data". You can also specify the number of bins
 # to be performed for the discretization of the measures in the calculation of mutual information
 adjMat = buildmim(conc_data, NBINS)
 
 
 # Generation of model parameters for subsequent simulation
-model = getLBODEmodel(adjMat, random=False, is_stimuli=exps[0].is_stimuli, maxInput=REALK, min_tau=0.1, max_tau=12,
+model = getLBODEmodel(adjMat, random=True, is_stimuli=exps[0].is_stimuli, maxInput=REALK, min_tau=0.1, max_tau=12,
                       max_n=5, min_n=1, min_k=0.1, max_k=1)
 
 
 # The "ivpsol" object is created for simulations
 ivpsol = Ivpsol(atol=1e-5, rtol=1e-5, max_step_size=0.1, max_num_steps=int(5000), max_error_test_fails=int(50))
 
 model.nthreads = int(8)
@@ -92,15 +97,15 @@
     problem = pypesto.Problem(objective=objective, lb=LB, ub=UB)
 
     # The local optimizer is defined
     optimizer = optimize.ScipyOptimizer(method="Powell")
 
     # The global optimizer is defined
     optimizer_ESS = pypesto.optimize.CESSOptimizer([{"dim_refset": 20, "local_n1": 3, "local_n2": 3,
-                                                     "n_diverse": 50, "max_eval": 200000, "n_procs": 8,
+                                                     "n_diverse": 50, "max_eval": 20000, "n_procs": 8,
                                                      "local_optimizer": optimizer}], max_iter=2)
 
     # The starting points of the variables to be optimized are calculated
     start = pypesto.startpoint.to_startpoint_method(pypesto.startpoint.uniform)
 
     # Optimization results are obtained
     result = optimizer_ESS.minimize(problem, start)
@@ -204,15 +209,15 @@
         problem = pypesto.Problem(objective=objective, lb=LB, ub=UB)
 
         # The local optimizer is defined
         optimizer = optimize.ScipyOptimizer(method="Powell")
 
         # The global optimizer is defined
         optimizer_ESS = pypesto.optimize.CESSOptimizer([{"dim_refset": 20, "local_n1": 3, "local_n2": 3,
-                                                         "n_diverse": 50, "max_eval": 200000, "n_procs": 8,
+                                                         "n_diverse": 50, "max_eval": 20000, "n_procs": 8,
                                                          "local_optimizer": optimizer}], max_iter=2)
 
         # The starting points of the variables to be optimized are calculated
         start = pypesto.startpoint.to_startpoint_method(pypesto.startpoint.uniform)
 
         # Optimization results are obtained
         result = optimizer_ESS.minimize(problem, start)
```

### Comparing `SELDOMpy-0.9.2/SELDOMpy/functions/buildmim.py` & `SELDOMpy-0.9.3/SELDOMpy/functions/buildmim.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/functions/extras.py` & `SELDOMpy-0.9.3/SELDOMpy/functions/extras.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/functions/gen_exps.py` & `SELDOMpy-0.9.3/SELDOMpy/functions/gen_exps.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,14 +85,14 @@
 
         namesSpecies = (list(experiment.index)[10]).split(',')
         for r in range(len(namesSpecies)):
             namesSpecies[r] = str(namesSpecies[r])
         # The value of "namesSpecies" is saved in a list of strings
 
         y0 = []
-        # "y0" is valued at training_and_reduce.py
+        # "y0" is valued at MAPK_training_and_reduce.py
 
         exps.append(Experiment(t_s, t_0, t_f, n_controls_t, index_observables, u, exp_data,
                                is_stimuli, y0, t_con, n_observables, namesSpecies))
         # An object of type "Experiment" is created with the calculated data and this object is added to the "exps" list
 
     return exps, conc_data
```

### Comparing `SELDOMpy-0.9.2/SELDOMpy/functions/getLBODEmodel.py` & `SELDOMpy-0.9.3/SELDOMpy/functions/getLBODEmodel.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/functions/getRandomLBODEmodel.py` & `SELDOMpy-0.9.3/SELDOMpy/functions/getRandomLBODEmodel.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/functions/optimization.py` & `SELDOMpy-0.9.3/SELDOMpy/functions/optimization.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/functions/plot_results.py` & `SELDOMpy-0.9.3/SELDOMpy/functions/plot_results.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/functions/reduce_fun.py` & `SELDOMpy-0.9.3/SELDOMpy/functions/reduce_fun.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/functions/simulate_logic_based_ode.py` & `SELDOMpy-0.9.3/SELDOMpy/functions/simulate_logic_based_ode.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/functions/simulate_logic_based_ode_obs.py` & `SELDOMpy-0.9.3/SELDOMpy/functions/simulate_logic_based_ode_obs.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/include/include_amigo/AMIGO_model.h` & `SELDOMpy-0.9.3/SELDOMpy/include/include_amigo/AMIGO_model.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/include/include_amigo/AMIGO_problem.h` & `SELDOMpy-0.9.3/SELDOMpy/include/include_amigo/AMIGO_problem.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/include/include_cvodes/cvodes/cvodes.h` & `SELDOMpy-0.9.3/SELDOMpy/include/include_cvodes/cvodes/cvodes.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/include/include_cvodes/cvodes/cvodes_band.h` & `SELDOMpy-0.9.3/SELDOMpy/include/include_cvodes/cvodes/cvodes_band.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/include/include_cvodes/cvodes/cvodes_bandpre.h` & `SELDOMpy-0.9.3/SELDOMpy/include/include_cvodes/cvodes/cvodes_bandpre.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/include/include_cvodes/cvodes/cvodes_bbdpre.h` & `SELDOMpy-0.9.3/SELDOMpy/include/include_cvodes/cvodes/cvodes_bbdpre.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/include/include_cvodes/cvodes/cvodes_dense.h` & `SELDOMpy-0.9.3/SELDOMpy/include/include_cvodes/cvodes/cvodes_dense.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/include/include_cvodes/cvodes/cvodes_diag.h` & `SELDOMpy-0.9.3/SELDOMpy/include/include_cvodes/cvodes/cvodes_diag.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/include/include_cvodes/cvodes/cvodes_direct.h` & `SELDOMpy-0.9.3/SELDOMpy/include/include_cvodes/cvodes/cvodes_direct.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/include/include_cvodes/cvodes/cvodes_lapack.h` & `SELDOMpy-0.9.3/SELDOMpy/include/include_cvodes/cvodes/cvodes_lapack.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/include/include_cvodes/cvodes/cvodes_spbcgs.h` & `SELDOMpy-0.9.3/SELDOMpy/include/include_cvodes/cvodes/cvodes_spbcgs.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/include/include_cvodes/cvodes/cvodes_spgmr.h` & `SELDOMpy-0.9.3/SELDOMpy/include/include_cvodes/cvodes/cvodes_spgmr.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/include/include_cvodes/cvodes/cvodes_spils.h` & `SELDOMpy-0.9.3/SELDOMpy/include/include_cvodes/cvodes/cvodes_spils.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/include/include_cvodes/cvodes/cvodes_sptfqmr.h` & `SELDOMpy-0.9.3/SELDOMpy/include/include_cvodes/cvodes/cvodes_sptfqmr.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/include/include_cvodes/nvector/nvector_serial.h` & `SELDOMpy-0.9.3/SELDOMpy/include/include_cvodes/nvector/nvector_serial.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/include/include_cvodes/sundials/sundials_band.h` & `SELDOMpy-0.9.3/SELDOMpy/include/include_cvodes/sundials/sundials_band.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/include/include_cvodes/sundials/sundials_config.h` & `SELDOMpy-0.9.3/SELDOMpy/include/include_cvodes/sundials/sundials_config.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/include/include_cvodes/sundials/sundials_dense.h` & `SELDOMpy-0.9.3/SELDOMpy/include/include_cvodes/sundials/sundials_dense.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/include/include_cvodes/sundials/sundials_direct.h` & `SELDOMpy-0.9.3/SELDOMpy/include/include_cvodes/sundials/sundials_direct.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/include/include_cvodes/sundials/sundials_fnvector.h` & `SELDOMpy-0.9.3/SELDOMpy/include/include_cvodes/sundials/sundials_fnvector.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/include/include_cvodes/sundials/sundials_iterative.h` & `SELDOMpy-0.9.3/SELDOMpy/include/include_cvodes/sundials/sundials_iterative.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/include/include_cvodes/sundials/sundials_lapack.h` & `SELDOMpy-0.9.3/SELDOMpy/include/include_cvodes/sundials/sundials_lapack.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/include/include_cvodes/sundials/sundials_math.h` & `SELDOMpy-0.9.3/SELDOMpy/include/include_cvodes/sundials/sundials_math.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/include/include_cvodes/sundials/sundials_nvector.h` & `SELDOMpy-0.9.3/SELDOMpy/include/include_cvodes/sundials/sundials_nvector.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/include/include_cvodes/sundials/sundials_spbcgs.h` & `SELDOMpy-0.9.3/SELDOMpy/include/include_cvodes/sundials/sundials_spbcgs.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/include/include_cvodes/sundials/sundials_spgmr.h` & `SELDOMpy-0.9.3/SELDOMpy/include/include_cvodes/sundials/sundials_spgmr.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/include/include_cvodes/sundials/sundials_sptfqmr.h` & `SELDOMpy-0.9.3/SELDOMpy/include/include_cvodes/sundials/sundials_sptfqmr.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/include/include_cvodes/sundials/sundials_types.h` & `SELDOMpy-0.9.3/SELDOMpy/include/include_cvodes/sundials/sundials_types.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/src/AMIGO_model.c` & `SELDOMpy-0.9.3/SELDOMpy/src/AMIGO_model.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/src/AMIGO_problem.c` & `SELDOMpy-0.9.3/SELDOMpy/src/AMIGO_problem.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/src/CNOStructure.h` & `SELDOMpy-0.9.3/SELDOMpy/src/CNOStructure.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/src/anODEModel.c` & `SELDOMpy-0.9.3/SELDOMpy/src/anODEModel.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/src/cvodea.c` & `SELDOMpy-0.9.3/SELDOMpy/src/cvodea.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/src/cvodea_io.c` & `SELDOMpy-0.9.3/SELDOMpy/src/cvodea_io.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/src/cvodes.c` & `SELDOMpy-0.9.3/SELDOMpy/src/cvodes.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/src/cvodes_band.c` & `SELDOMpy-0.9.3/SELDOMpy/src/cvodes_band.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/src/cvodes_bandpre.c` & `SELDOMpy-0.9.3/SELDOMpy/src/cvodes_bandpre.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/src/cvodes_bandpre_impl.h` & `SELDOMpy-0.9.3/SELDOMpy/src/cvodes_bandpre_impl.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/src/cvodes_bbdpre.c` & `SELDOMpy-0.9.3/SELDOMpy/src/cvodes_bbdpre.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/src/cvodes_bbdpre_impl.h` & `SELDOMpy-0.9.3/SELDOMpy/src/cvodes_bbdpre_impl.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/src/cvodes_dense.c` & `SELDOMpy-0.9.3/SELDOMpy/src/cvodes_dense.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/src/cvodes_diag.c` & `SELDOMpy-0.9.3/SELDOMpy/src/cvodes_diag.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/src/cvodes_diag_impl.h` & `SELDOMpy-0.9.3/SELDOMpy/src/cvodes_diag_impl.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/src/cvodes_direct.c` & `SELDOMpy-0.9.3/SELDOMpy/src/cvodes_direct.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/src/cvodes_direct_impl.h` & `SELDOMpy-0.9.3/SELDOMpy/src/cvodes_direct_impl.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/src/cvodes_impl.h` & `SELDOMpy-0.9.3/SELDOMpy/src/cvodes_impl.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/src/cvodes_io.c` & `SELDOMpy-0.9.3/SELDOMpy/src/cvodes_io.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/src/cvodes_spbcgs.c` & `SELDOMpy-0.9.3/SELDOMpy/src/cvodes_spbcgs.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/src/cvodes_spgmr.c` & `SELDOMpy-0.9.3/SELDOMpy/src/cvodes_spgmr.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/src/cvodes_spils.c` & `SELDOMpy-0.9.3/SELDOMpy/src/cvodes_spils.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/src/cvodes_spils_impl.h` & `SELDOMpy-0.9.3/SELDOMpy/src/cvodes_spils_impl.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/src/cvodes_sptfqmr.c` & `SELDOMpy-0.9.3/SELDOMpy/src/cvodes_sptfqmr.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/src/dhc.c` & `SELDOMpy-0.9.3/SELDOMpy/src/dhc.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/src/findStates.c` & `SELDOMpy-0.9.3/SELDOMpy/src/findStates.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/src/fnvector_serial.c` & `SELDOMpy-0.9.3/SELDOMpy/src/fnvector_serial.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/src/fnvector_serial.h` & `SELDOMpy-0.9.3/SELDOMpy/src/fnvector_serial.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/src/getAdjacencyMatrix.c` & `SELDOMpy-0.9.3/SELDOMpy/src/getAdjacencyMatrix.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/src/getStateIndex.c` & `SELDOMpy-0.9.3/SELDOMpy/src/getStateIndex.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/src/getTruthTables.c` & `SELDOMpy-0.9.3/SELDOMpy/src/getTruthTables.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/src/get_support_truth_tables.c` & `SELDOMpy-0.9.3/SELDOMpy/src/get_support_truth_tables.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/src/get_truth_tables_index.c` & `SELDOMpy-0.9.3/SELDOMpy/src/get_truth_tables_index.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/src/nvector_serial.c` & `SELDOMpy-0.9.3/SELDOMpy/src/nvector_serial.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/src/printNminiTerms.c` & `SELDOMpy-0.9.3/SELDOMpy/src/printNminiTerms.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/src/sim_logic_ode.c` & `SELDOMpy-0.9.3/SELDOMpy/src/sim_logic_ode.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/src/simulate_amigo_model.c` & `SELDOMpy-0.9.3/SELDOMpy/src/simulate_amigo_model.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/src/sundials_band.c` & `SELDOMpy-0.9.3/SELDOMpy/src/sundials_band.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/src/sundials_dense.c` & `SELDOMpy-0.9.3/SELDOMpy/src/sundials_dense.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/src/sundials_direct.c` & `SELDOMpy-0.9.3/SELDOMpy/src/sundials_direct.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/src/sundials_iterative.c` & `SELDOMpy-0.9.3/SELDOMpy/src/sundials_iterative.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/src/sundials_math.c` & `SELDOMpy-0.9.3/SELDOMpy/src/sundials_math.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/src/sundials_nvector.c` & `SELDOMpy-0.9.3/SELDOMpy/src/sundials_nvector.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/src/sundials_spbcgs.c` & `SELDOMpy-0.9.3/SELDOMpy/src/sundials_spbcgs.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/src/sundials_spgmr.c` & `SELDOMpy-0.9.3/SELDOMpy/src/sundials_spgmr.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy/src/sundials_sptfqmr.c` & `SELDOMpy-0.9.3/SELDOMpy/src/sundials_sptfqmr.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.9.2/SELDOMpy.egg-info/PKG-INFO` & `SELDOMpy-0.9.3/SELDOMpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: SELDOMpy
-Version: 0.9.2
-Summary: This package performs dynamic modelling of cellular signalling networks.
+Version: 0.9.3
+Summary: Dynamic modelling of cellular signalling networks.
 Home-page: https://github.com/lupralo31/SELDOMpy
 Download-URL: https://github.com/lupralo31/SELDOMpy/archive/refs/tags/V_0.2.1.tar.gz
 Author: Luis Prado
 Author-email: pradolopezluis@gmail.com
 License: GPLv3
 Keywords: SELDOMpy,SELDOM,dynamic modelling,cellular signalling networks,biomedical engineering
 Classifier: Programming Language :: Python :: 3
```

### Comparing `SELDOMpy-0.9.2/SELDOMpy.egg-info/SOURCES.txt` & `SELDOMpy-0.9.3/SELDOMpy.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -56,19 +56,19 @@
 SELDOMpy/src/sundials_iterative.c
 SELDOMpy/src/sundials_math.c
 SELDOMpy/src/sundials_nvector.c
 SELDOMpy/src/sundials_spbcgs.c
 SELDOMpy/src/sundials_spgmr.c
 SELDOMpy/src/sundials_sptfqmr.c
 SELDOMpy/examples/MAPK/MAPK.xlsx
-SELDOMpy/examples/MAPK/training_and_reduce.py
-SELDOMpy/examples/MAPK/training_and_reduce_pyPESTO.py
+SELDOMpy/examples/MAPK/MAPK_training_and_reduce.py
+SELDOMpy/examples/MAPK/MAPK_training_and_reduce_pyPESTO.py
 SELDOMpy/examples/SP/SP.xlsx
-SELDOMpy/examples/SP/training_and_reduce.py
-SELDOMpy/examples/SP/training_and_reduce_pyPESTO.py
+SELDOMpy/examples/SP/SP_training_and_reduce.py
+SELDOMpy/examples/SP/SP_training_and_reduce_pyPESTO.py
 SELDOMpy/functions/buildmim.py
 SELDOMpy/functions/extras.py
 SELDOMpy/functions/gen_exps.py
 SELDOMpy/functions/getLBODEmodel.py
 SELDOMpy/functions/getRandomLBODEmodel.py
 SELDOMpy/functions/optimization.py
 SELDOMpy/functions/plot_results.py
```

### Comparing `SELDOMpy-0.9.2/setup.py` & `SELDOMpy-0.9.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 numpy_include = np.get_include()
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='SELDOMpy',
-    version='0.9.2',
-    description='This package performs dynamic modelling of cellular signalling networks.',
+    version='0.9.3',
+    description='Dynamic modelling of cellular signalling networks.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Luis Prado',
     author_email='pradolopezluis@gmail.com',
     url='https://github.com/lupralo31/SELDOMpy',
     download_url='https://github.com/lupralo31/SELDOMpy/archive/refs/tags/V_0.2.1.tar.gz',
     packages=find_packages(exclude=('tests',)),
@@ -41,15 +41,15 @@
                  "SELDOMpy/src/simulate_amigo_model.c",
                  "SELDOMpy/src/sundials_band.c",
                  "SELDOMpy/src/sundials_dense.c", "SELDOMpy/src/sundials_direct.c", "SELDOMpy/src/sundials_iterative.c",
                  "SELDOMpy/src/sundials_math.c", "SELDOMpy/src/sundials_nvector.c", "SELDOMpy/src/sundials_spbcgs.c",
                  "SELDOMpy/src/sundials_spgmr.c", "SELDOMpy/src/sundials_sptfqmr.c"],
         include_dirs=['SELDOMpy/include/include_amigo', 'SELDOMpy/include/include_cvodes', "SELDOMpy/src", numpy_include],
     )],
-    install_requires=["numpy", "scikit-learn", "pandas", "mealpy", "matplotlib", "setuptools", "openpyxl", "pypesto"],
+    install_requires=["numpy", "scikit-learn", "pandas", "mealpy", "matplotlib", "setuptools", "openpyxl", "pypesto", "scipy"],
     include_package_data=True,
     license='GPLv3',
     classifiers=[
         # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Operating System :: OS Independent',
```

