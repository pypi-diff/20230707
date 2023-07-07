# Comparing `tmp/SELDOMpy-0.8.4.9.tar.gz` & `tmp/SELDOMpy-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\SELDOMpy-0.8.4.9.tar", last modified: Thu Jul  6 11:32:36 2023, max compression
+gzip compressed data, was "dist\SELDOMpy-0.9.tar", last modified: Fri Jul  7 10:49:40 2023, max compression
```

## Comparing `SELDOMpy-0.8.4.9.tar` & `SELDOMpy-0.9.tar`

### file list

```diff
@@ -1,131 +1,135 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 11:32:36.635161 SELDOMpy-0.8.4.9/
--rw-rw-rw-   0        0        0    35149 2023-07-05 16:32:35.000000 SELDOMpy-0.8.4.9/LICENSE.txt
--rw-rw-rw-   0        0        0      368 2023-07-06 11:26:53.000000 SELDOMpy-0.8.4.9/MANIFEST.in
--rw-rw-rw-   0        0        0     4195 2023-07-06 11:32:36.635161 SELDOMpy-0.8.4.9/PKG-INFO
--rw-rw-rw-   0        0        0     3446 2023-07-06 08:12:36.000000 SELDOMpy-0.8.4.9/README.md
-drwxrwxrwx   0        0        0        0 2023-07-06 11:32:36.523187 SELDOMpy-0.8.4.9/SELDOMpy/
--rw-rw-rw-   0        0        0    35149 2023-07-05 16:32:35.000000 SELDOMpy-0.8.4.9/SELDOMpy/LICENSE.txt
--rw-rw-rw-   0        0        0     3446 2023-07-06 08:12:36.000000 SELDOMpy-0.8.4.9/SELDOMpy/README.md
--rw-rw-rw-   0        0        0      490 2023-07-06 11:23:03.000000 SELDOMpy-0.8.4.9/SELDOMpy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 11:32:36.582196 SELDOMpy-0.8.4.9/SELDOMpy/functions/
--rw-rw-rw-   0        0        0     2309 2023-06-22 08:44:09.000000 SELDOMpy-0.8.4.9/SELDOMpy/functions/buildmim.py
--rw-rw-rw-   0        0        0     1288 2023-07-04 08:20:50.000000 SELDOMpy-0.8.4.9/SELDOMpy/functions/extras.py
--rw-rw-rw-   0        0        0     4159 2023-04-19 14:22:26.000000 SELDOMpy-0.8.4.9/SELDOMpy/functions/gen_exps.py
--rw-rw-rw-   0        0        0     4848 2023-07-06 11:23:03.000000 SELDOMpy-0.8.4.9/SELDOMpy/functions/getLBODEmodel.py
--rw-rw-rw-   0        0        0     3232 2023-04-24 18:45:26.000000 SELDOMpy-0.8.4.9/SELDOMpy/functions/getRandomLBODEmodel.py
--rw-rw-rw-   0        0        0     2467 2023-07-06 11:23:03.000000 SELDOMpy-0.8.4.9/SELDOMpy/functions/optimization.py
--rw-rw-rw-   0        0        0     1446 2023-07-06 08:30:16.000000 SELDOMpy-0.8.4.9/SELDOMpy/functions/plot_results.py
--rw-rw-rw-   0        0        0     2534 2023-07-06 11:23:03.000000 SELDOMpy-0.8.4.9/SELDOMpy/functions/reduce_fun.py
--rw-rw-rw-   0        0        0     4073 2023-07-06 11:23:03.000000 SELDOMpy-0.8.4.9/SELDOMpy/functions/simulate_logic_based_ode.py
--rw-rw-rw-   0        0        0     3626 2023-07-06 11:23:03.000000 SELDOMpy-0.8.4.9/SELDOMpy/functions/simulate_logic_based_ode_obs.py
-drwxrwxrwx   0        0        0        0 2023-07-06 11:32:36.513225 SELDOMpy-0.8.4.9/SELDOMpy/include/
-drwxrwxrwx   0        0        0        0 2023-07-06 11:32:36.590166 SELDOMpy-0.8.4.9/SELDOMpy/include/include_amigo/
--rw-rw-rw-   0        0        0        4 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.9/SELDOMpy/include/include_amigo/AMIGO_hdf5.h
--rw-rw-rw-   0        0        0     3769 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.9/SELDOMpy/include/include_amigo/AMIGO_model.h
--rw-rw-rw-   0        0        0      442 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.9/SELDOMpy/include/include_amigo/AMIGO_model_stats.h
--rw-rw-rw-   0        0        0     1822 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.9/SELDOMpy/include/include_amigo/AMIGO_problem.h
--rw-rw-rw-   0        0        0      287 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.9/SELDOMpy/include/include_amigo/amigoJAC.h
--rw-rw-rw-   0        0        0       24 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.9/SELDOMpy/include/include_amigo/amigoRHS.h
--rw-rw-rw-   0        0        0      171 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.9/SELDOMpy/include/include_amigo/amigoSensRHS.h
--rw-rw-rw-   0        0        0      164 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.9/SELDOMpy/include/include_amigo/simulate_amigo_model.h
-drwxrwxrwx   0        0        0        0 2023-07-06 11:32:36.514195 SELDOMpy-0.8.4.9/SELDOMpy/include/include_cvodes/
-drwxrwxrwx   0        0        0        0 2023-07-06 11:32:36.603163 SELDOMpy-0.8.4.9/SELDOMpy/include/include_cvodes/cvodes/
--rw-rw-rw-   0        0        0    84971 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.9/SELDOMpy/include/include_cvodes/cvodes/cvodes.h
--rw-rw-rw-   0        0        0     2442 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.9/SELDOMpy/include/include_cvodes/cvodes/cvodes_band.h
--rw-rw-rw-   0        0        0     6547 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.9/SELDOMpy/include/include_cvodes/cvodes/cvodes_bandpre.h
--rw-rw-rw-   0        0        0    13259 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.9/SELDOMpy/include/include_cvodes/cvodes/cvodes_bbdpre.h
--rw-rw-rw-   0        0        0     2122 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.9/SELDOMpy/include/include_cvodes/cvodes/cvodes_dense.h
--rw-rw-rw-   0        0        0     4845 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.9/SELDOMpy/include/include_cvodes/cvodes/cvodes_diag.h
--rw-rw-rw-   0        0        0    14031 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.9/SELDOMpy/include/include_cvodes/cvodes/cvodes_direct.h
--rw-rw-rw-   0        0        0     3732 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.9/SELDOMpy/include/include_cvodes/cvodes/cvodes_lapack.h
--rw-rw-rw-   0        0        0     3061 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.9/SELDOMpy/include/include_cvodes/cvodes/cvodes_spbcgs.h
--rw-rw-rw-   0        0        0     3021 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.9/SELDOMpy/include/include_cvodes/cvodes/cvodes_spgmr.h
--rw-rw-rw-   0        0        0    18270 2022-12-07 11:24:13.000000 SELDOMpy-0.8.4.9/SELDOMpy/include/include_cvodes/cvodes/cvodes_spils.h
--rw-rw-rw-   0        0        0     3085 2022-12-07 11:24:13.000000 SELDOMpy-0.8.4.9/SELDOMpy/include/include_cvodes/cvodes/cvodes_sptfqmr.h
-drwxrwxrwx   0        0        0        0 2023-07-06 11:32:36.604162 SELDOMpy-0.8.4.9/SELDOMpy/include/include_cvodes/nvector/
--rw-rw-rw-   0        0        0    10054 2022-12-07 11:24:13.000000 SELDOMpy-0.8.4.9/SELDOMpy/include/include_cvodes/nvector/nvector_serial.h
-drwxrwxrwx   0        0        0        0 2023-07-06 11:32:36.616162 SELDOMpy-0.8.4.9/SELDOMpy/include/include_cvodes/sundials/
--rw-rw-rw-   0        0        0     6539 2022-12-07 11:24:13.000000 SELDOMpy-0.8.4.9/SELDOMpy/include/include_cvodes/sundials/sundials_band.h
--rw-rw-rw-   0        0        0     3157 2022-12-07 11:24:13.000000 SELDOMpy-0.8.4.9/SELDOMpy/include/include_cvodes/sundials/sundials_config.h
--rw-rw-rw-   0        0        0     7865 2022-12-07 11:24:13.000000 SELDOMpy-0.8.4.9/SELDOMpy/include/include_cvodes/sundials/sundials_dense.h
--rw-rw-rw-   0        0        0    13199 2022-12-07 11:24:13.000000 SELDOMpy-0.8.4.9/SELDOMpy/include/include_cvodes/sundials/sundials_direct.h
--rw-rw-rw-   0        0        0     1129 2022-12-07 11:24:13.000000 SELDOMpy-0.8.4.9/SELDOMpy/include/include_cvodes/sundials/sundials_fnvector.h
--rw-rw-rw-   0        0        0    13127 2022-12-07 11:24:13.000000 SELDOMpy-0.8.4.9/SELDOMpy/include/include_cvodes/sundials/sundials_iterative.h
--rw-rw-rw-   0        0        0     4763 2022-12-07 11:24:13.000000 SELDOMpy-0.8.4.9/SELDOMpy/include/include_cvodes/sundials/sundials_lapack.h
--rw-rw-rw-   0        0        0     4294 2022-12-07 11:24:13.000000 SELDOMpy-0.8.4.9/SELDOMpy/include/include_cvodes/sundials/sundials_math.h
--rw-rw-rw-   0        0        0    15964 2022-12-07 11:24:13.000000 SELDOMpy-0.8.4.9/SELDOMpy/include/include_cvodes/sundials/sundials_nvector.h
--rw-rw-rw-   0        0        0     7740 2022-12-07 11:24:13.000000 SELDOMpy-0.8.4.9/SELDOMpy/include/include_cvodes/sundials/sundials_spbcgs.h
--rw-rw-rw-   0        0        0    12224 2022-12-07 11:24:13.000000 SELDOMpy-0.8.4.9/SELDOMpy/include/include_cvodes/sundials/sundials_spgmr.h
--rw-rw-rw-   0        0        0    10246 2022-12-07 11:24:13.000000 SELDOMpy-0.8.4.9/SELDOMpy/include/include_cvodes/sundials/sundials_sptfqmr.h
--rw-rw-rw-   0        0        0     3726 2022-12-07 11:24:13.000000 SELDOMpy-0.8.4.9/SELDOMpy/include/include_cvodes/sundials/sundials_types.h
--rw-rw-rw-   0        0        0       90 2022-12-07 15:59:05.000000 SELDOMpy-0.8.4.9/SELDOMpy/makefile
--rw-rw-rw-   0        0        0       71 2023-07-05 16:32:11.000000 SELDOMpy-0.8.4.9/SELDOMpy/setup.cfg
--rw-rw-rw-   0        0        0     3496 2023-07-06 11:27:24.000000 SELDOMpy-0.8.4.9/SELDOMpy/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-06 11:32:36.628188 SELDOMpy-0.8.4.9/SELDOMpy/src/
--rw-rw-rw-   0        0        0    10952 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.9/SELDOMpy/src/AMIGO_model.c
--rw-rw-rw-   0        0        0      240 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.9/SELDOMpy/src/AMIGO_model_stats.c
--rw-rw-rw-   0        0        0     8027 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.9/SELDOMpy/src/AMIGO_problem.c
--rw-rw-rw-   0        0        0      811 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.9/SELDOMpy/src/CNOStructure.h
--rw-rw-rw-   0        0        0        0 2023-07-03 16:56:56.000000 SELDOMpy-0.8.4.9/SELDOMpy/src/__init__.py
--rw-rw-rw-   0        0        0     3389 2023-04-10 15:09:09.000000 SELDOMpy-0.8.4.9/SELDOMpy/src/anODEModel.c
--rw-rw-rw-   0        0        0    74908 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.9/SELDOMpy/src/cvodea.c
--rw-rw-rw-   0        0        0    18585 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.9/SELDOMpy/src/cvodea_io.c
--rw-rw-rw-   0        0        0   245647 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.9/SELDOMpy/src/cvodes.c
--rw-rw-rw-   0        0        0    13293 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.9/SELDOMpy/src/cvodes_band.c
--rw-rw-rw-   0        0        0    16826 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.9/SELDOMpy/src/cvodes_bandpre.c
--rw-rw-rw-   0        0        0     2272 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.9/SELDOMpy/src/cvodes_bandpre_impl.h
--rw-rw-rw-   0        0        0    23592 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.9/SELDOMpy/src/cvodes_bbdpre.c
--rw-rw-rw-   0        0        0     2929 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.9/SELDOMpy/src/cvodes_bbdpre_impl.h
--rw-rw-rw-   0        0        0    12594 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.9/SELDOMpy/src/cvodes_dense.c
--rw-rw-rw-   0        0        0    13921 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.9/SELDOMpy/src/cvodes_diag.c
--rw-rw-rw-   0        0        0     2258 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.9/SELDOMpy/src/cvodes_diag_impl.h
--rw-rw-rw-   0        0        0    20099 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.9/SELDOMpy/src/cvodes_direct.c
--rw-rw-rw-   0        0        0     5473 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.9/SELDOMpy/src/cvodes_direct_impl.h
--rw-rw-rw-   0        0        0    47504 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.9/SELDOMpy/src/cvodes_impl.h
--rw-rw-rw-   0        0        0    41365 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.9/SELDOMpy/src/cvodes_io.c
--rw-rw-rw-   0        0        0    16912 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.9/SELDOMpy/src/cvodes_spbcgs.c
--rw-rw-rw-   0        0        0    17029 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.9/SELDOMpy/src/cvodes_spgmr.c
--rw-rw-rw-   0        0        0    32809 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.9/SELDOMpy/src/cvodes_spils.c
--rw-rw-rw-   0        0        0     6831 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.9/SELDOMpy/src/cvodes_spils_impl.h
--rw-rw-rw-   0        0        0    17108 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.9/SELDOMpy/src/cvodes_sptfqmr.c
--rw-rw-rw-   0        0        0      405 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.9/SELDOMpy/src/decimal2binary.c
--rw-rw-rw-   0        0        0     3792 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.9/SELDOMpy/src/dhc.c
--rw-rw-rw-   0        0        0      527 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.9/SELDOMpy/src/findStates.c
--rw-rw-rw-   0        0        0     3433 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.9/SELDOMpy/src/fnvector_serial.c
--rw-rw-rw-   0        0        0     2688 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.9/SELDOMpy/src/fnvector_serial.h
--rw-rw-rw-   0        0        0      693 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.9/SELDOMpy/src/getAdjacencyMatrix.c
--rw-rw-rw-   0        0        0      463 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.9/SELDOMpy/src/getNumBits.c
--rw-rw-rw-   0        0        0      475 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.9/SELDOMpy/src/getNumInputs.c
--rw-rw-rw-   0        0        0      695 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.9/SELDOMpy/src/getStateIndex.c
--rw-rw-rw-   0        0        0     3859 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.9/SELDOMpy/src/getTruthTables.c
--rw-rw-rw-   0        0        0      451 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.9/SELDOMpy/src/get_count_bits.c
--rw-rw-rw-   0        0        0      487 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.9/SELDOMpy/src/get_input_index.c
--rw-rw-rw-   0        0        0      594 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.9/SELDOMpy/src/get_support_truth_tables.c
--rw-rw-rw-   0        0        0      585 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.9/SELDOMpy/src/get_truth_tables_index.c
--rw-rw-rw-   0        0        0      224 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.9/SELDOMpy/src/hill_function.c
--rw-rw-rw-   0        0        0      219 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.9/SELDOMpy/src/linear_transfer_function.c
--rw-rw-rw-   0        0        0      227 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.9/SELDOMpy/src/normHill.c
--rw-rw-rw-   0        0        0    20778 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.9/SELDOMpy/src/nvector_serial.c
--rw-rw-rw-   0        0        0      305 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.9/SELDOMpy/src/printAdjMat.c
--rw-rw-rw-   0        0        0      315 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.9/SELDOMpy/src/printInterMat.c
--rw-rw-rw-   0        0        0      553 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.9/SELDOMpy/src/printNminiTerms.c
--rw-rw-rw-   0        0        0      410 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.9/SELDOMpy/src/printTruthTables.c
--rw-rw-rw-   0        0        0    15775 2023-04-28 16:16:22.000000 SELDOMpy-0.8.4.9/SELDOMpy/src/sim_logic_ode.c
--rw-rw-rw-   0        0        0     9815 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.9/SELDOMpy/src/simulate_amigo_model.c
--rw-rw-rw-   0        0        0     6036 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.9/SELDOMpy/src/sundials_band.c
--rw-rw-rw-   0        0        0     8510 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.9/SELDOMpy/src/sundials_dense.c
--rw-rw-rw-   0        0        0     6225 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.9/SELDOMpy/src/sundials_direct.c
--rw-rw-rw-   0        0        0     7662 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.9/SELDOMpy/src/sundials_iterative.c
--rw-rw-rw-   0        0        0     2474 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.9/SELDOMpy/src/sundials_math.c
--rw-rw-rw-   0        0        0     4702 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.9/SELDOMpy/src/sundials_nvector.c
--rw-rw-rw-   0        0        0     9663 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.9/SELDOMpy/src/sundials_spbcgs.c
--rw-rw-rw-   0        0        0    12650 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.9/SELDOMpy/src/sundials_spgmr.c
--rw-rw-rw-   0        0        0    14744 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.9/SELDOMpy/src/sundials_sptfqmr.c
-drwxrwxrwx   0        0        0        0 2023-07-06 11:32:36.527197 SELDOMpy-0.8.4.9/SELDOMpy.egg-info/
--rw-rw-rw-   0        0        0     4195 2023-07-06 11:32:36.000000 SELDOMpy-0.8.4.9/SELDOMpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5761 2023-07-06 11:32:36.000000 SELDOMpy-0.8.4.9/SELDOMpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 11:32:36.000000 SELDOMpy-0.8.4.9/SELDOMpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-07-06 11:32:36.000000 SELDOMpy-0.8.4.9/SELDOMpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-06 11:32:36.000000 SELDOMpy-0.8.4.9/SELDOMpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      115 2023-07-06 11:32:36.636195 SELDOMpy-0.8.4.9/setup.cfg
--rw-rw-rw-   0        0        0     3496 2023-07-06 11:32:33.000000 SELDOMpy-0.8.4.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-07 10:49:40.907907 SELDOMpy-0.9/
+-rw-rw-rw-   0        0        0    35149 2023-07-05 16:32:35.000000 SELDOMpy-0.9/LICENSE.txt
+-rw-rw-rw-   0        0        0      564 2023-07-07 10:48:29.000000 SELDOMpy-0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     4191 2023-07-07 10:49:40.907907 SELDOMpy-0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3446 2023-07-06 08:12:36.000000 SELDOMpy-0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-07 10:49:40.647908 SELDOMpy-0.9/SELDOMpy/
+-rw-rw-rw-   0        0        0      490 2023-07-06 11:23:03.000000 SELDOMpy-0.9/SELDOMpy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-07 10:49:40.640907 SELDOMpy-0.9/SELDOMpy/examples/
+drwxrwxrwx   0        0        0        0 2023-07-07 10:49:40.808907 SELDOMpy-0.9/SELDOMpy/examples/MAPK/
+-rw-rw-rw-   0        0        0    13667 2023-04-19 10:00:19.000000 SELDOMpy-0.9/SELDOMpy/examples/MAPK/MAPK.xlsx
+-rw-rw-rw-   0        0        0     5832 2023-07-07 10:48:29.000000 SELDOMpy-0.9/SELDOMpy/examples/MAPK/training_and_reduce.py
+-rw-rw-rw-   0        0        0    10300 2023-07-07 10:48:29.000000 SELDOMpy-0.9/SELDOMpy/examples/MAPK/training_and_reduce_pyPESTO.py
+drwxrwxrwx   0        0        0        0 2023-07-07 10:49:40.823937 SELDOMpy-0.9/SELDOMpy/examples/SP/
+-rw-rw-rw-   0        0        0    23018 2023-06-21 18:44:38.000000 SELDOMpy-0.9/SELDOMpy/examples/SP/SP.xlsx
+-rw-rw-rw-   0        0        0     6012 2023-07-07 10:49:19.000000 SELDOMpy-0.9/SELDOMpy/examples/SP/training_and_reduce.py
+-rw-rw-rw-   0        0        0    10502 2023-07-07 10:48:29.000000 SELDOMpy-0.9/SELDOMpy/examples/SP/training_and_reduce_pyPESTO.py
+drwxrwxrwx   0        0        0        0 2023-07-07 10:49:40.841961 SELDOMpy-0.9/SELDOMpy/functions/
+-rw-rw-rw-   0        0        0     1799 2023-07-06 13:38:27.000000 SELDOMpy-0.9/SELDOMpy/functions/buildmim.py
+-rw-rw-rw-   0        0        0     1280 2023-07-07 07:34:51.000000 SELDOMpy-0.9/SELDOMpy/functions/extras.py
+-rw-rw-rw-   0        0        0     4032 2023-07-07 07:34:51.000000 SELDOMpy-0.9/SELDOMpy/functions/gen_exps.py
+-rw-rw-rw-   0        0        0     4860 2023-07-07 07:34:51.000000 SELDOMpy-0.9/SELDOMpy/functions/getLBODEmodel.py
+-rw-rw-rw-   0        0        0     3156 2023-07-07 07:34:50.000000 SELDOMpy-0.9/SELDOMpy/functions/getRandomLBODEmodel.py
+-rw-rw-rw-   0        0        0     2418 2023-07-07 07:37:07.000000 SELDOMpy-0.9/SELDOMpy/functions/optimization.py
+-rw-rw-rw-   0        0        0     1509 2023-07-07 07:39:33.000000 SELDOMpy-0.9/SELDOMpy/functions/plot_results.py
+-rw-rw-rw-   0        0        0     2748 2023-07-07 07:41:41.000000 SELDOMpy-0.9/SELDOMpy/functions/reduce_fun.py
+-rw-rw-rw-   0        0        0     3802 2023-07-07 07:48:40.000000 SELDOMpy-0.9/SELDOMpy/functions/simulate_logic_based_ode.py
+-rw-rw-rw-   0        0        0     3595 2023-07-07 07:52:38.000000 SELDOMpy-0.9/SELDOMpy/functions/simulate_logic_based_ode_obs.py
+drwxrwxrwx   0        0        0        0 2023-07-07 10:49:40.641908 SELDOMpy-0.9/SELDOMpy/include/
+drwxrwxrwx   0        0        0        0 2023-07-07 10:49:40.848950 SELDOMpy-0.9/SELDOMpy/include/include_amigo/
+-rw-rw-rw-   0        0        0        4 2022-12-07 11:24:12.000000 SELDOMpy-0.9/SELDOMpy/include/include_amigo/AMIGO_hdf5.h
+-rw-rw-rw-   0        0        0     3769 2022-12-07 11:24:12.000000 SELDOMpy-0.9/SELDOMpy/include/include_amigo/AMIGO_model.h
+-rw-rw-rw-   0        0        0      442 2022-12-07 11:24:12.000000 SELDOMpy-0.9/SELDOMpy/include/include_amigo/AMIGO_model_stats.h
+-rw-rw-rw-   0        0        0     1822 2022-12-07 11:24:12.000000 SELDOMpy-0.9/SELDOMpy/include/include_amigo/AMIGO_problem.h
+-rw-rw-rw-   0        0        0      287 2022-12-07 11:24:12.000000 SELDOMpy-0.9/SELDOMpy/include/include_amigo/amigoJAC.h
+-rw-rw-rw-   0        0        0       24 2022-12-07 11:24:12.000000 SELDOMpy-0.9/SELDOMpy/include/include_amigo/amigoRHS.h
+-rw-rw-rw-   0        0        0      171 2022-12-07 11:24:12.000000 SELDOMpy-0.9/SELDOMpy/include/include_amigo/amigoSensRHS.h
+-rw-rw-rw-   0        0        0      164 2022-12-07 11:24:12.000000 SELDOMpy-0.9/SELDOMpy/include/include_amigo/simulate_amigo_model.h
+drwxrwxrwx   0        0        0        0 2023-07-07 10:49:40.642908 SELDOMpy-0.9/SELDOMpy/include/include_cvodes/
+drwxrwxrwx   0        0        0        0 2023-07-07 10:49:40.861909 SELDOMpy-0.9/SELDOMpy/include/include_cvodes/cvodes/
+-rw-rw-rw-   0        0        0    84971 2022-12-07 11:24:12.000000 SELDOMpy-0.9/SELDOMpy/include/include_cvodes/cvodes/cvodes.h
+-rw-rw-rw-   0        0        0     2442 2022-12-07 11:24:12.000000 SELDOMpy-0.9/SELDOMpy/include/include_cvodes/cvodes/cvodes_band.h
+-rw-rw-rw-   0        0        0     6547 2022-12-07 11:24:12.000000 SELDOMpy-0.9/SELDOMpy/include/include_cvodes/cvodes/cvodes_bandpre.h
+-rw-rw-rw-   0        0        0    13259 2022-12-07 11:24:12.000000 SELDOMpy-0.9/SELDOMpy/include/include_cvodes/cvodes/cvodes_bbdpre.h
+-rw-rw-rw-   0        0        0     2122 2022-12-07 11:24:12.000000 SELDOMpy-0.9/SELDOMpy/include/include_cvodes/cvodes/cvodes_dense.h
+-rw-rw-rw-   0        0        0     4845 2022-12-07 11:24:12.000000 SELDOMpy-0.9/SELDOMpy/include/include_cvodes/cvodes/cvodes_diag.h
+-rw-rw-rw-   0        0        0    14031 2022-12-07 11:24:12.000000 SELDOMpy-0.9/SELDOMpy/include/include_cvodes/cvodes/cvodes_direct.h
+-rw-rw-rw-   0        0        0     3732 2022-12-07 11:24:12.000000 SELDOMpy-0.9/SELDOMpy/include/include_cvodes/cvodes/cvodes_lapack.h
+-rw-rw-rw-   0        0        0     3061 2022-12-07 11:24:12.000000 SELDOMpy-0.9/SELDOMpy/include/include_cvodes/cvodes/cvodes_spbcgs.h
+-rw-rw-rw-   0        0        0     3021 2022-12-07 11:24:12.000000 SELDOMpy-0.9/SELDOMpy/include/include_cvodes/cvodes/cvodes_spgmr.h
+-rw-rw-rw-   0        0        0    18270 2022-12-07 11:24:13.000000 SELDOMpy-0.9/SELDOMpy/include/include_cvodes/cvodes/cvodes_spils.h
+-rw-rw-rw-   0        0        0     3085 2022-12-07 11:24:13.000000 SELDOMpy-0.9/SELDOMpy/include/include_cvodes/cvodes/cvodes_sptfqmr.h
+drwxrwxrwx   0        0        0        0 2023-07-07 10:49:40.863908 SELDOMpy-0.9/SELDOMpy/include/include_cvodes/nvector/
+-rw-rw-rw-   0        0        0    10054 2022-12-07 11:24:13.000000 SELDOMpy-0.9/SELDOMpy/include/include_cvodes/nvector/nvector_serial.h
+drwxrwxrwx   0        0        0        0 2023-07-07 10:49:40.886942 SELDOMpy-0.9/SELDOMpy/include/include_cvodes/sundials/
+-rw-rw-rw-   0        0        0     6539 2022-12-07 11:24:13.000000 SELDOMpy-0.9/SELDOMpy/include/include_cvodes/sundials/sundials_band.h
+-rw-rw-rw-   0        0        0     3157 2022-12-07 11:24:13.000000 SELDOMpy-0.9/SELDOMpy/include/include_cvodes/sundials/sundials_config.h
+-rw-rw-rw-   0        0        0     7865 2022-12-07 11:24:13.000000 SELDOMpy-0.9/SELDOMpy/include/include_cvodes/sundials/sundials_dense.h
+-rw-rw-rw-   0        0        0    13199 2022-12-07 11:24:13.000000 SELDOMpy-0.9/SELDOMpy/include/include_cvodes/sundials/sundials_direct.h
+-rw-rw-rw-   0        0        0     1129 2022-12-07 11:24:13.000000 SELDOMpy-0.9/SELDOMpy/include/include_cvodes/sundials/sundials_fnvector.h
+-rw-rw-rw-   0        0        0    13127 2022-12-07 11:24:13.000000 SELDOMpy-0.9/SELDOMpy/include/include_cvodes/sundials/sundials_iterative.h
+-rw-rw-rw-   0        0        0     4763 2022-12-07 11:24:13.000000 SELDOMpy-0.9/SELDOMpy/include/include_cvodes/sundials/sundials_lapack.h
+-rw-rw-rw-   0        0        0     4294 2022-12-07 11:24:13.000000 SELDOMpy-0.9/SELDOMpy/include/include_cvodes/sundials/sundials_math.h
+-rw-rw-rw-   0        0        0    15964 2022-12-07 11:24:13.000000 SELDOMpy-0.9/SELDOMpy/include/include_cvodes/sundials/sundials_nvector.h
+-rw-rw-rw-   0        0        0     7740 2022-12-07 11:24:13.000000 SELDOMpy-0.9/SELDOMpy/include/include_cvodes/sundials/sundials_spbcgs.h
+-rw-rw-rw-   0        0        0    12224 2022-12-07 11:24:13.000000 SELDOMpy-0.9/SELDOMpy/include/include_cvodes/sundials/sundials_spgmr.h
+-rw-rw-rw-   0        0        0    10246 2022-12-07 11:24:13.000000 SELDOMpy-0.9/SELDOMpy/include/include_cvodes/sundials/sundials_sptfqmr.h
+-rw-rw-rw-   0        0        0     3726 2022-12-07 11:24:13.000000 SELDOMpy-0.9/SELDOMpy/include/include_cvodes/sundials/sundials_types.h
+drwxrwxrwx   0        0        0        0 2023-07-07 10:49:40.900907 SELDOMpy-0.9/SELDOMpy/src/
+-rw-rw-rw-   0        0        0    10952 2022-12-07 11:24:11.000000 SELDOMpy-0.9/SELDOMpy/src/AMIGO_model.c
+-rw-rw-rw-   0        0        0      240 2022-12-07 11:24:11.000000 SELDOMpy-0.9/SELDOMpy/src/AMIGO_model_stats.c
+-rw-rw-rw-   0        0        0     8027 2022-12-07 11:24:11.000000 SELDOMpy-0.9/SELDOMpy/src/AMIGO_problem.c
+-rw-rw-rw-   0        0        0      811 2022-12-07 11:24:11.000000 SELDOMpy-0.9/SELDOMpy/src/CNOStructure.h
+-rw-rw-rw-   0        0        0        0 2023-07-03 16:56:56.000000 SELDOMpy-0.9/SELDOMpy/src/__init__.py
+-rw-rw-rw-   0        0        0     3389 2023-04-10 15:09:09.000000 SELDOMpy-0.9/SELDOMpy/src/anODEModel.c
+-rw-rw-rw-   0        0        0    74908 2022-12-07 11:24:11.000000 SELDOMpy-0.9/SELDOMpy/src/cvodea.c
+-rw-rw-rw-   0        0        0    18585 2022-12-07 11:24:11.000000 SELDOMpy-0.9/SELDOMpy/src/cvodea_io.c
+-rw-rw-rw-   0        0        0   245647 2022-12-07 11:24:11.000000 SELDOMpy-0.9/SELDOMpy/src/cvodes.c
+-rw-rw-rw-   0        0        0    13293 2022-12-07 11:24:11.000000 SELDOMpy-0.9/SELDOMpy/src/cvodes_band.c
+-rw-rw-rw-   0        0        0    16826 2022-12-07 11:24:11.000000 SELDOMpy-0.9/SELDOMpy/src/cvodes_bandpre.c
+-rw-rw-rw-   0        0        0     2272 2022-12-07 11:24:11.000000 SELDOMpy-0.9/SELDOMpy/src/cvodes_bandpre_impl.h
+-rw-rw-rw-   0        0        0    23592 2022-12-07 11:24:11.000000 SELDOMpy-0.9/SELDOMpy/src/cvodes_bbdpre.c
+-rw-rw-rw-   0        0        0     2929 2022-12-07 11:24:11.000000 SELDOMpy-0.9/SELDOMpy/src/cvodes_bbdpre_impl.h
+-rw-rw-rw-   0        0        0    12594 2022-12-07 11:24:11.000000 SELDOMpy-0.9/SELDOMpy/src/cvodes_dense.c
+-rw-rw-rw-   0        0        0    13921 2022-12-07 11:24:11.000000 SELDOMpy-0.9/SELDOMpy/src/cvodes_diag.c
+-rw-rw-rw-   0        0        0     2258 2022-12-07 11:24:11.000000 SELDOMpy-0.9/SELDOMpy/src/cvodes_diag_impl.h
+-rw-rw-rw-   0        0        0    20099 2022-12-07 11:24:11.000000 SELDOMpy-0.9/SELDOMpy/src/cvodes_direct.c
+-rw-rw-rw-   0        0        0     5473 2022-12-07 11:24:11.000000 SELDOMpy-0.9/SELDOMpy/src/cvodes_direct_impl.h
+-rw-rw-rw-   0        0        0    47504 2022-12-07 11:24:11.000000 SELDOMpy-0.9/SELDOMpy/src/cvodes_impl.h
+-rw-rw-rw-   0        0        0    41365 2022-12-07 11:24:11.000000 SELDOMpy-0.9/SELDOMpy/src/cvodes_io.c
+-rw-rw-rw-   0        0        0    16912 2022-12-07 11:24:11.000000 SELDOMpy-0.9/SELDOMpy/src/cvodes_spbcgs.c
+-rw-rw-rw-   0        0        0    17029 2022-12-07 11:24:11.000000 SELDOMpy-0.9/SELDOMpy/src/cvodes_spgmr.c
+-rw-rw-rw-   0        0        0    32809 2022-12-07 11:24:11.000000 SELDOMpy-0.9/SELDOMpy/src/cvodes_spils.c
+-rw-rw-rw-   0        0        0     6831 2022-12-07 11:24:11.000000 SELDOMpy-0.9/SELDOMpy/src/cvodes_spils_impl.h
+-rw-rw-rw-   0        0        0    17108 2022-12-07 11:24:11.000000 SELDOMpy-0.9/SELDOMpy/src/cvodes_sptfqmr.c
+-rw-rw-rw-   0        0        0      405 2022-12-07 11:24:11.000000 SELDOMpy-0.9/SELDOMpy/src/decimal2binary.c
+-rw-rw-rw-   0        0        0     3792 2022-12-07 11:24:12.000000 SELDOMpy-0.9/SELDOMpy/src/dhc.c
+-rw-rw-rw-   0        0        0      527 2022-12-07 11:24:12.000000 SELDOMpy-0.9/SELDOMpy/src/findStates.c
+-rw-rw-rw-   0        0        0     3433 2022-12-07 11:24:12.000000 SELDOMpy-0.9/SELDOMpy/src/fnvector_serial.c
+-rw-rw-rw-   0        0        0     2688 2022-12-07 11:24:12.000000 SELDOMpy-0.9/SELDOMpy/src/fnvector_serial.h
+-rw-rw-rw-   0        0        0      693 2022-12-07 11:24:12.000000 SELDOMpy-0.9/SELDOMpy/src/getAdjacencyMatrix.c
+-rw-rw-rw-   0        0        0      463 2022-12-07 11:24:12.000000 SELDOMpy-0.9/SELDOMpy/src/getNumBits.c
+-rw-rw-rw-   0        0        0      475 2022-12-07 11:24:12.000000 SELDOMpy-0.9/SELDOMpy/src/getNumInputs.c
+-rw-rw-rw-   0        0        0      695 2022-12-07 11:24:12.000000 SELDOMpy-0.9/SELDOMpy/src/getStateIndex.c
+-rw-rw-rw-   0        0        0     3859 2022-12-07 11:24:12.000000 SELDOMpy-0.9/SELDOMpy/src/getTruthTables.c
+-rw-rw-rw-   0        0        0      451 2022-12-07 11:24:12.000000 SELDOMpy-0.9/SELDOMpy/src/get_count_bits.c
+-rw-rw-rw-   0        0        0      487 2022-12-07 11:24:12.000000 SELDOMpy-0.9/SELDOMpy/src/get_input_index.c
+-rw-rw-rw-   0        0        0      594 2022-12-07 11:24:12.000000 SELDOMpy-0.9/SELDOMpy/src/get_support_truth_tables.c
+-rw-rw-rw-   0        0        0      585 2022-12-07 11:24:12.000000 SELDOMpy-0.9/SELDOMpy/src/get_truth_tables_index.c
+-rw-rw-rw-   0        0        0      224 2022-12-07 11:24:12.000000 SELDOMpy-0.9/SELDOMpy/src/hill_function.c
+-rw-rw-rw-   0        0        0      219 2022-12-07 11:24:12.000000 SELDOMpy-0.9/SELDOMpy/src/linear_transfer_function.c
+-rw-rw-rw-   0        0        0      227 2022-12-07 11:24:12.000000 SELDOMpy-0.9/SELDOMpy/src/normHill.c
+-rw-rw-rw-   0        0        0    20778 2022-12-07 11:24:12.000000 SELDOMpy-0.9/SELDOMpy/src/nvector_serial.c
+-rw-rw-rw-   0        0        0      305 2022-12-07 11:24:12.000000 SELDOMpy-0.9/SELDOMpy/src/printAdjMat.c
+-rw-rw-rw-   0        0        0      315 2022-12-07 11:24:12.000000 SELDOMpy-0.9/SELDOMpy/src/printInterMat.c
+-rw-rw-rw-   0        0        0      553 2022-12-07 11:24:12.000000 SELDOMpy-0.9/SELDOMpy/src/printNminiTerms.c
+-rw-rw-rw-   0        0        0      410 2022-12-07 11:24:12.000000 SELDOMpy-0.9/SELDOMpy/src/printTruthTables.c
+-rw-rw-rw-   0        0        0    15775 2023-04-28 16:16:22.000000 SELDOMpy-0.9/SELDOMpy/src/sim_logic_ode.c
+-rw-rw-rw-   0        0        0     9815 2022-12-07 11:24:12.000000 SELDOMpy-0.9/SELDOMpy/src/simulate_amigo_model.c
+-rw-rw-rw-   0        0        0     6036 2022-12-07 11:24:12.000000 SELDOMpy-0.9/SELDOMpy/src/sundials_band.c
+-rw-rw-rw-   0        0        0     8510 2022-12-07 11:24:12.000000 SELDOMpy-0.9/SELDOMpy/src/sundials_dense.c
+-rw-rw-rw-   0        0        0     6225 2022-12-07 11:24:12.000000 SELDOMpy-0.9/SELDOMpy/src/sundials_direct.c
+-rw-rw-rw-   0        0        0     7662 2022-12-07 11:24:12.000000 SELDOMpy-0.9/SELDOMpy/src/sundials_iterative.c
+-rw-rw-rw-   0        0        0     2474 2022-12-07 11:24:12.000000 SELDOMpy-0.9/SELDOMpy/src/sundials_math.c
+-rw-rw-rw-   0        0        0     4702 2022-12-07 11:24:12.000000 SELDOMpy-0.9/SELDOMpy/src/sundials_nvector.c
+-rw-rw-rw-   0        0        0     9663 2022-12-07 11:24:12.000000 SELDOMpy-0.9/SELDOMpy/src/sundials_spbcgs.c
+-rw-rw-rw-   0        0        0    12650 2022-12-07 11:24:12.000000 SELDOMpy-0.9/SELDOMpy/src/sundials_spgmr.c
+-rw-rw-rw-   0        0        0    14744 2022-12-07 11:24:12.000000 SELDOMpy-0.9/SELDOMpy/src/sundials_sptfqmr.c
+drwxrwxrwx   0        0        0        0 2023-07-07 10:49:40.651908 SELDOMpy-0.9/SELDOMpy.egg-info/
+-rw-rw-rw-   0        0        0     4191 2023-07-07 10:49:40.000000 SELDOMpy-0.9/SELDOMpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5924 2023-07-07 10:49:40.000000 SELDOMpy-0.9/SELDOMpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-07 10:49:40.000000 SELDOMpy-0.9/SELDOMpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2023-07-07 10:49:40.000000 SELDOMpy-0.9/SELDOMpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-07 10:49:40.000000 SELDOMpy-0.9/SELDOMpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      115 2023-07-07 10:49:40.908907 SELDOMpy-0.9/setup.cfg
+-rw-rw-rw-   0        0        0     3503 2023-07-07 10:49:19.000000 SELDOMpy-0.9/setup.py
```

### Comparing `SELDOMpy-0.8.4.9/LICENSE.txt` & `SELDOMpy-0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/PKG-INFO` & `SELDOMpy-0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SELDOMpy
-Version: 0.8.4.9
+Version: 0.9
 Summary: This package performs dynamic modelling of cellular signalling networks.
 Home-page: https://github.com/lupralo31/SELDOMpy
 Download-URL: https://github.com/lupralo31/SELDOMpy/archive/refs/tags/V_0.2.1.tar.gz
 Author: Luis Prado
 Author-email: pradolopezluis@gmail.com
 License: GPLv3
 Keywords: SELDOMpy,SELDOM,dynamic modelling,cellular signalling networks,biomedical engineering
```

### Comparing `SELDOMpy-0.8.4.9/README.md` & `SELDOMpy-0.9/README.md`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/README.md` & `SELDOMpy-0.9/SELDOMpy.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,55 +1,71 @@
-# About SELDOMpy
-
-SELDOMpy is a Python package that generates dynamic models of cell signalling networks from experimental data. The SELDOMpy algorithm consists of the following steps:
-- **Calculation of the adjacency matrix** of the network from the mutual information between all possible pairs of nodes.
-- **Generation of an initial dynamic network model** from the adjacency matrix above.
-- **Optimisation** of the value obtained from the simulation of the model.
-- **Reduction** of the number of model arrow arcs using the Akaike criterion.
-- **Simulation and saving** of the final model and graphs obtained from its simulation. 
-
-SELDOMpy implements the algorithm from the R package [SELDOM](https://zenodo.org/record/250558).
-The purpose of SELDOMpy is to create a more accessible and user-friendly tool than SELDOM. 
-It works well with simple networks, but it is not as efficient as SELDOM in larger networks since it does not have such specific optimization tools.
-
-SELDOMpy was created by **Luis Prado López**, <pradolopezluis@gmail.com>, under the supervision of [Alejandro F. Villaverde](http://afvillaverde.webs.uvigo.gal/), <afvillaverde@uvigo.gal> and [David Saque Henriques](https://www.iim.csic.es/es/personal/david-saque), <davidh@iim.csic.es>. 
-
-## Installation and requirements
-SELDOMpy requires Python 3. 
-It also consists of .c files, so there are 2 installation possibilities:
-
-a) If you are using a **64-bit Windows with Python 3.8**: You can install SELDOMpy directly using the following command: 
-
-   `pip install SELDOMpy`
-
-b) If you are using **other Python versions and operating systems**: You need to have a C compiler installed (such as Visual Studio) and follow the commands below:
-  
-  `pip install numpy`
-  
-  `python -m pip install pip==22.0.4`
-  
-  `pip install SELDOMpy`
-  
-  Once installed you can update pip to the latest version if you wish using `python -m pip install --upgrade pip`
-
-## Getting started
-The first thing is to install the package as indicated above depending on your terminal.
-To be able to use SELDOMpy in your Python project you can import all its functions with the following command: 
-
-`from SELDOMpy import *`
-
-Once imported, you can perform the steps indicated in the first section following the PDF manual that includes the package.
- 
-## Results
-The results of the final cell signaling network model are saved in a binary file (in the path indicated by the user). These results can be imported into Python if the user wishes and thus check the values of the model.
-You can also plot the results obtained from the simulation of the final model together with the experimental measurements of the nodes to verify that the modeling was performed correctly using the _plot_results_ function. 
-
-More information about SELDOMpy can be found in the [SELDOMpy manual](SELDOMpy/doc/SELDOMpy_manual.pdf)
-
-## Disclaimer
-
-This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, version 3 of the License.
-    
-This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  
-See the GNU General Public License for more details.
- 
-You should have received a copy of the GNU General Public License along with this program. If not, see <http://www.gnu.org/licenses/>.
+Metadata-Version: 2.1
+Name: SELDOMpy
+Version: 0.9
+Summary: This package performs dynamic modelling of cellular signalling networks.
+Home-page: https://github.com/lupralo31/SELDOMpy
+Download-URL: https://github.com/lupralo31/SELDOMpy/archive/refs/tags/V_0.2.1.tar.gz
+Author: Luis Prado
+Author-email: pradolopezluis@gmail.com
+License: GPLv3
+Keywords: SELDOMpy,SELDOM,dynamic modelling,cellular signalling networks,biomedical engineering
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# About SELDOMpy
+
+SELDOMpy is a Python package that generates dynamic models of cell signalling networks from experimental data. The SELDOMpy algorithm consists of the following steps:
+- **Calculation of the adjacency matrix** of the network from the mutual information between all possible pairs of nodes.
+- **Generation of an initial dynamic network model** from the adjacency matrix above.
+- **Optimisation** of the value obtained from the simulation of the model.
+- **Reduction** of the number of model arrow arcs using the Akaike criterion.
+- **Simulation and saving** of the final model and graphs obtained from its simulation. 
+
+SELDOMpy implements the algorithm from the R package [SELDOM](https://zenodo.org/record/250558).
+The purpose of SELDOMpy is to create a more accessible and user-friendly tool than SELDOM. 
+It works well with simple networks, but it is not as efficient as SELDOM in larger networks since it does not have such specific optimization tools.
+
+SELDOMpy was created by **Luis Prado López**, <pradolopezluis@gmail.com>, under the supervision of [Alejandro F. Villaverde](http://afvillaverde.webs.uvigo.gal/), <afvillaverde@uvigo.gal> and [David Saque Henriques](https://www.iim.csic.es/es/personal/david-saque), <davidh@iim.csic.es>. 
+
+## Installation and requirements
+SELDOMpy requires Python 3. 
+It also consists of .c files, so there are 2 installation possibilities:
+
+a) If you are using a **64-bit Windows with Python 3.8**: You can install SELDOMpy directly using the following command: 
+
+   `pip install SELDOMpy`
+
+b) If you are using **other Python versions and operating systems**: You need to have a C compiler installed (such as Visual Studio) and follow the commands below:
+  
+  `pip install numpy`
+  
+  `python -m pip install pip==22.0.4`
+  
+  `pip install SELDOMpy`
+  
+  Once installed you can update pip to the latest version if you wish using `python -m pip install --upgrade pip`
+
+## Getting started
+The first thing is to install the package as indicated above depending on your terminal.
+To be able to use SELDOMpy in your Python project you can import all its functions with the following command: 
+
+`from SELDOMpy import *`
+
+Once imported, you can perform the steps indicated in the first section following the PDF manual that includes the package.
+ 
+## Results
+The results of the final cell signaling network model are saved in a binary file (in the path indicated by the user). These results can be imported into Python if the user wishes and thus check the values of the model.
+You can also plot the results obtained from the simulation of the final model together with the experimental measurements of the nodes to verify that the modeling was performed correctly using the _plot_results_ function. 
+
+More information about SELDOMpy can be found in the [SELDOMpy manual](SELDOMpy/doc/SELDOMpy_manual.pdf)
+
+## Disclaimer
+
+This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, version 3 of the License.
+    
+This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  
+See the GNU General Public License for more details.
+ 
+You should have received a copy of the GNU General Public License along with this program. If not, see <http://www.gnu.org/licenses/>.
```

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/functions/getLBODEmodel.py` & `SELDOMpy-0.9/SELDOMpy/functions/getLBODEmodel.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from SELDOMpy.functions.getRandomLBODEmodel import *
-# Importo el archivo getRandomLBODEmodel en el que se realiza la ruleta para la creación de modelos
+# I import the getRandomLBODEmodel file in which the roulette is performed for the creation of models
 
 
 class Model:
     def __init__(self, n_states, n_stimuli, x, adjMat, index_opt, LB, UB, k_pars, n_pars, w_pars,
                  tau_pars, nthreads, estimated_pars=None, active_pars=None, count_inputs=None, count_active_inputs=None,
                  namesSpecies=None):
-        # Constructor de la clase Model. Se utilizará en getLBODEmodel para crear un objeto con los datos de un modelo
+        # The constructor of the "Model" class. It will be used in getLBODEmodel to create an object with the data of a model
         self.n_states = n_states
         self.n_stimuli = n_stimuli
         self.x = x
         self.adjMat = adjMat
         self.index_opt = index_opt
         self.LB = LB
         self.UB = UB
@@ -30,44 +30,44 @@
                   max_w=1, min_w=0, random=False, maxInput=6):
     if is_stimuli is None:
         is_stimuli = [0, 0, 0, 0]
 
     if maxInput > len(adjMat[0]):
         maxInput = len(adjMat[0])
 
-    x = []  # La lista tita donde voy a guardar todos los parametros
+    x = []  # The list where I will save all the parameters
     index_opt = []
     LB = []
     UB = []
     index_w = []
     index_n = []
     index_k = []
     index_tau = []
 
-    counter = 0  # Inicializacion del contador
+    counter = 0  # Counter initialization
     if random:
         adjMat = getRandomLBODEmodel(adjMat, maxInput)
-        # Calculo de la matriz de adyacencia con 1s y 0s y metodo de la ruleta
+        # Adjacency matrix calculation with 1s and 0s and roulette method
 
-    for i in range(len(adjMat[0])):  # Recorro columas de adjMat
+    for i in range(len(adjMat[0])):  # AdjMat columas are toured
         counter += 1
 
-        inputs = []  # Lista donde guardaré los indices de las filas que valgan 1 en esa columna
-        for ii in range(len(adjMat)):  # Recorro filas de la columna de adjMat
+        inputs = []  # List where I will save the indexes of the rows that are worth 1 in that column
+        for ii in range(len(adjMat)):  # I scroll through rows of the "adjMat" column
             if adjMat[ii][i] == 1:
                 inputs.append(ii)
 
-        x.append(len(inputs))  # Pongo en primera posicion el numero de entradas de esa columna
+        x.append(len(inputs))  # I put in first position the number of entries in that column
 
-        if len(inputs) > 0:  # Si hay alguna entrada en el nodo de esa columna
+        if len(inputs) > 0:  # Whether there are any entries in the node of that column
 
-            for j in range(len(inputs)):  # Recorro las entradas de esa columna
+            for j in range(len(inputs)):  # The entries in that column are traversed
                 # inputs index
                 counter += 1
-                x.append(inputs[j])  # Pongo el indice de esa entrada en esa columna
+                x.append(inputs[j])  # You put the index of that entry in that column
 
                 # k
                 counter += 1
                 x.append(0.1)
 
                 if is_stimuli[i] == 0:
                     index_k.append(counter)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/functions/optimization.py` & `SELDOMpy-0.9/SELDOMpy/functions/optimization.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 from mealpy.evolutionary_based import DE
 from SELDOMpy.functions.simulate_logic_based_ode import *
-# Se importa para hacer las simulaciones en la función objetivo tratando de minimizar el valor que obtenga aquí
+# It is imported to do the simulations in the target function trying to minimize the value you get here
 import datetime
-# Se importa para guardar la fecha en time dentro del objeto de la clase Res_opt que se devuelve
+# Imported to save the date in time within the object of the Res_opt class that is returned
 import copy
 
 
 class Res_opt:
     def __init__(self, f, time, fbest, xbest, neval, numeval):
-        # Constructor de la clase Res_opt. Se utilizará en MEIGO para devolver los valores obtenidos de la optimización
+        # Class constructor "Res_opt".
         self.f = f
         self.time = time
         self.fbest = fbest
         self.xbest = xbest
         self.neval = neval
         self.numeval = numeval
 
 
-def optimization(model, exps, ivpsol):
+def optimization(model, exps, ivpsol, epoch, pop_size, miu_f, miu_cr):
     f = []
     time = []
     numeval = 0
     neval = []
     model_op = copy.deepcopy(model)
 
     def opt_fun(X):
         nonlocal numeval
-        # Me interesa que numeval no esté definida al nivel más global del módulo para que resetee cada vez que llame
-        # a optimization
+        # It is interesting that numeval is not defined at the most global level of the module so that it
+        # resets each time it calls "optimization"
         numeval += 1
 
         for p in range(len(model_op.index_opt)):
             model_op.x[model_op.index_opt[p]-1] = X[p]
 
         sol_opt_fun = simulate_logic_based_ode(model_op, exps, ivpsol)
-        if not f:  # En la primera simulación
+        if not f:  # In the first simulation
             f.append(sol_opt_fun)
             time.append(datetime.datetime.now())
             neval.append(numeval)
-        if sol_opt_fun < f[-1]:  # Si el valor simulado es menor al ultimo mejor guardado en la lista f
-            f.append(sol_opt_fun)  # Guardo este nuevo valor en la lista f
-            time.append(datetime.datetime.now())  # Guardo el momento en que se produjo en la lista time
-            neval.append(numeval)  # Guardo el nº de iteración en que se evalúo ese valor
+        if sol_opt_fun < f[-1]:  # If the simulated value is less than the last best saved in list f
+            f.append(sol_opt_fun)  # This new value is saved in list f
+            time.append(datetime.datetime.now())  # The time it occurred is saved in the "time" list
+            neval.append(numeval)  # The iteration number in which that value was evaluated is saved
 
-        print(f"Iteración número: {numeval}")
-        print(f"Valor función objetivo: {sol_opt_fun}")
+        print(f"Iteration number: {numeval}")
+        print(f"Target function value: {sol_opt_fun}")
 
         return sol_opt_fun
 
     LB = []
     UB = []
     for i in range(len(model_op.LB)):
         LB.append(model_op.LB[i])
@@ -59,15 +59,15 @@
         "lb": LB,
         "ub": UB,
         "minmax": "min",
         "log_to": None,
         "save_population": False,
     }
 
-    modelo = DE.SHADE(epoch=1, pop_size=50, miu_f=0.3, miu_cr=0.6)
+    modelo = DE.SHADE(epoch=epoch, pop_size=pop_size, miu_f=miu_f, miu_cr=miu_cr)
 
     xbest, fbest = modelo.solve(problem)
 
     xbest = xbest.tolist()
 
     return Res_opt(f, time, fbest, xbest, neval, numeval)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/functions/reduce_fun.py` & `SELDOMpy-0.9/SELDOMpy/functions/reduce_fun.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from SELDOMpy.functions.simulate_logic_based_ode import *
 from math import log
 import copy
 
 
+# Function used to obtain the resulting model by reducing an arrow arc from the network
 def get_reduced_model(model, is_stimuli=None, delete_edge=-1):
     adjMat = copy.deepcopy(model.adjMat)
     model_copy = copy.deepcopy(model)
 
     if is_stimuli is None:
         is_stimuli = []
         for iii in range(len(adjMat[0])):
@@ -75,28 +76,29 @@
     model_copy.active_pars = active_pars
     model_copy.count_inputs = count_inputs
     model_copy.count_active_inputs = count_active_inputs
 
     return model_copy
 
 
+# Function used to apply akaike criteria to check whether an axis can be removed
 def akaike(x, model, exps, ivpsol, k, n_data):
     model_copy = copy.deepcopy(model)
 
     for p in range(len(model_copy.index_opt)):
         model_copy.x[model_copy.index_opt[p] - 1] = x[p]
 
     res = simulate_logic_based_ode(model_copy, exps, ivpsol)
 
     return 2*k+n_data*log(res)
 
 
+# Function used to reduce the value of the target function
 def optim_fun(X, model, exps, ivpsol):
     model_copy = copy.deepcopy(model)
 
     for p in range(len(model_copy.index_opt)):
         model_copy.x[model_copy.index_opt[p] - 1] = X[p]
 
     res = simulate_logic_based_ode(model_copy, exps, ivpsol)
-    #print(res)
 
     return res
```

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/functions/simulate_logic_based_ode_obs.py` & `SELDOMpy-0.9/SELDOMpy/functions/simulate_logic_based_ode.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 import hello
-# Así importo la librería hello con el archivo sim_logic_ode.c y los includes compilados para poder ejecutarse
+# This is how the "hello" library is imported with the sim_logic_ode.c file and the compiled includes to be able to run
 from SELDOMpy.functions.extras import *
-# Necesario para usar la función fill_array
+# Required to use the "fill_array" function
+import decimal
 
 
-def simulate_logic_based_ode_obs(model, exps, ivpsol):
+# To avoid "overflow" problems when obtaining simulation results
 
+
+def simulate_logic_based_ode(model, exps, ivpsol):
     task = "OBS_CVODES_ODE"
 
-    # Ahora se convierten las variables a enviar al formato adecuado empezando por las del modelo "model"
+    # Now the variables to be sent are converted to the appropriate format starting with those of the "model" model
     nthreads = np.array(model.nthreads, dtype=np.int32)
     n_states = np.array(model.n_states, dtype=np.int32)
     x = np.array(model.x, dtype=np.double)
     n_stimuli = np.array(model.n_stimuli, dtype=np.int32)
 
-    # Las variables que vienen de experimentos estarán repetidas tantas veces como experimentos haya, por lo que se unen
-    # las del mismo tipo de todos los experimentos en una misma lista que luego se recorrerá en sim_logic_ode.c
+    # The variables that come from experiments will be repeated as many times as there are experiments,
+    # so those of the same type of all experiments are joined in the same list that will then be covered in sim_logic_ode.c
     n_observables = []
     t_s = []
     t_con = []
     index_observables = []
     t_0 = []
     t_f = []
     y0 = []
@@ -34,51 +37,54 @@
         t_0.append(exps[i].t_0)
         t_f.append(exps[i].t_f)
         y0.append(exps[i].y0)
         u.append(exps[i].u)
         exp_data.append(exps[i].exp_data)
 
     n_observables = np.array(n_observables, dtype=np.int32)
-    # Esto por ejemplo es una lista en formato np.array con los n_observables de todos los experimentos en orden
-    # Así para todos los demás. En las que vayan a ser listas de listas hay que ejecutarles la funcion "fill_array"
-    # ya que np.array da error si todas las listas internas no son del mismo tamaño
+    # This for example is a list in np.array format with the "n_observables" of all experiments in order
+    # So for everyone else. In those that are going to be lists of lists you have to execute the function
+    # "fill_array" since np.array gives error if all the internal lists are not of the same size
     t_s = fill_array(t_s)
     t_s = np.array(t_s, dtype=np.double)
     t_con = fill_array(t_con)
     t_con = np.array(t_con, dtype=np.double)
     index_observables = fill_array(index_observables)
     index_observables = np.array(index_observables, dtype=np.int32)
     t_0 = np.array(t_0, dtype=np.double)
     t_f = np.array(t_f, dtype=np.double)
     y0 = fill_array(y0)
     y0 = np.array(y0, dtype=np.double)
     u = fill_array(u)
     u = np.array(u, dtype=np.double)
     exp_data = fill_array(exp_data)
-    # Hago la traspuesta para ponerla tal y como lo quiere el archivo sim_logic_ode.c
+    # The transpose is done to put it as the file sim_logic_ode.c wants.
     for j in range(len(exp_data)):
         exp_data[j] = [[row[i] for row in exp_data[j]] for i in range(len(exp_data[j][0]))]
     exp_data = np.array(exp_data, dtype=np.double)
 
-    # Se convierten las variables de ipvsol
+    # "ipvsol" variables are converted
     rtol = np.array(ivpsol.rtol, dtype=np.double)
     atol = np.array(ivpsol.atol, dtype=np.double)
     max_step_size = np.array(ivpsol.max_step_size, dtype=np.double)
     max_num_steps = np.array(ivpsol.max_num_steps, dtype=np.int32)
     max_error_test_fails = np.array(ivpsol.max_error_test_fails, dtype=np.int32)
 
-    # Por último se convierte la cadena de caracteres task
+    # Finally, the "task" string is converted
     task_c = np.array(task, dtype='object')
 
-    # Se envían las variables al archivo sim_logic_ode.c
+    # Variables are sent to the sim_logic_ode.c file
     res = hello.hello_numpy(nthreads, n_states, x, n_stimuli, n_observables, t_s, t_con, index_observables, t_0, t_f,
                             y0, u, exp_data, rtol, atol, max_step_size, max_num_steps, max_error_test_fails,
                             task_c.item())
 
-    # Se redondea la solución a 8 decimales
+    solution = decimal.Decimal(0)
+
     for i in range(len(res)):
         for j in range(len(res[i])):
             for k in range(len(res[i][j])):
-                res[i][j][k] = round(res[i][j][k], 8)
+                solution += (decimal.Decimal(res[i][j][k]) - decimal.Decimal(exps[i].exp_data[j][k])) ** 2
 
-    return res
+    # The solution is rounded to 8 decimal places
+    solution = float(solution)
 
+    return solution
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/include/include_amigo/AMIGO_model.h` & `SELDOMpy-0.9/SELDOMpy/include/include_amigo/AMIGO_model.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/include/include_amigo/AMIGO_problem.h` & `SELDOMpy-0.9/SELDOMpy/include/include_amigo/AMIGO_problem.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/include/include_cvodes/cvodes/cvodes.h` & `SELDOMpy-0.9/SELDOMpy/include/include_cvodes/cvodes/cvodes.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/include/include_cvodes/cvodes/cvodes_band.h` & `SELDOMpy-0.9/SELDOMpy/include/include_cvodes/cvodes/cvodes_band.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/include/include_cvodes/cvodes/cvodes_bandpre.h` & `SELDOMpy-0.9/SELDOMpy/include/include_cvodes/cvodes/cvodes_bandpre.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/include/include_cvodes/cvodes/cvodes_bbdpre.h` & `SELDOMpy-0.9/SELDOMpy/include/include_cvodes/cvodes/cvodes_bbdpre.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/include/include_cvodes/cvodes/cvodes_dense.h` & `SELDOMpy-0.9/SELDOMpy/include/include_cvodes/cvodes/cvodes_dense.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/include/include_cvodes/cvodes/cvodes_diag.h` & `SELDOMpy-0.9/SELDOMpy/include/include_cvodes/cvodes/cvodes_diag.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/include/include_cvodes/cvodes/cvodes_direct.h` & `SELDOMpy-0.9/SELDOMpy/include/include_cvodes/cvodes/cvodes_direct.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/include/include_cvodes/cvodes/cvodes_lapack.h` & `SELDOMpy-0.9/SELDOMpy/include/include_cvodes/cvodes/cvodes_lapack.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/include/include_cvodes/cvodes/cvodes_spbcgs.h` & `SELDOMpy-0.9/SELDOMpy/include/include_cvodes/cvodes/cvodes_spbcgs.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/include/include_cvodes/cvodes/cvodes_spgmr.h` & `SELDOMpy-0.9/SELDOMpy/include/include_cvodes/cvodes/cvodes_spgmr.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/include/include_cvodes/cvodes/cvodes_spils.h` & `SELDOMpy-0.9/SELDOMpy/include/include_cvodes/cvodes/cvodes_spils.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/include/include_cvodes/cvodes/cvodes_sptfqmr.h` & `SELDOMpy-0.9/SELDOMpy/include/include_cvodes/cvodes/cvodes_sptfqmr.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/include/include_cvodes/nvector/nvector_serial.h` & `SELDOMpy-0.9/SELDOMpy/include/include_cvodes/nvector/nvector_serial.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/include/include_cvodes/sundials/sundials_band.h` & `SELDOMpy-0.9/SELDOMpy/include/include_cvodes/sundials/sundials_band.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/include/include_cvodes/sundials/sundials_config.h` & `SELDOMpy-0.9/SELDOMpy/include/include_cvodes/sundials/sundials_config.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/include/include_cvodes/sundials/sundials_dense.h` & `SELDOMpy-0.9/SELDOMpy/include/include_cvodes/sundials/sundials_dense.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/include/include_cvodes/sundials/sundials_direct.h` & `SELDOMpy-0.9/SELDOMpy/include/include_cvodes/sundials/sundials_direct.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/include/include_cvodes/sundials/sundials_fnvector.h` & `SELDOMpy-0.9/SELDOMpy/include/include_cvodes/sundials/sundials_fnvector.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/include/include_cvodes/sundials/sundials_iterative.h` & `SELDOMpy-0.9/SELDOMpy/include/include_cvodes/sundials/sundials_iterative.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/include/include_cvodes/sundials/sundials_lapack.h` & `SELDOMpy-0.9/SELDOMpy/include/include_cvodes/sundials/sundials_lapack.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/include/include_cvodes/sundials/sundials_math.h` & `SELDOMpy-0.9/SELDOMpy/include/include_cvodes/sundials/sundials_math.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/include/include_cvodes/sundials/sundials_nvector.h` & `SELDOMpy-0.9/SELDOMpy/include/include_cvodes/sundials/sundials_nvector.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/include/include_cvodes/sundials/sundials_spbcgs.h` & `SELDOMpy-0.9/SELDOMpy/include/include_cvodes/sundials/sundials_spbcgs.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/include/include_cvodes/sundials/sundials_spgmr.h` & `SELDOMpy-0.9/SELDOMpy/include/include_cvodes/sundials/sundials_spgmr.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/include/include_cvodes/sundials/sundials_sptfqmr.h` & `SELDOMpy-0.9/SELDOMpy/include/include_cvodes/sundials/sundials_sptfqmr.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/include/include_cvodes/sundials/sundials_types.h` & `SELDOMpy-0.9/SELDOMpy/include/include_cvodes/sundials/sundials_types.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/setup.py` & `SELDOMpy-0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 numpy_include = np.get_include()
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='SELDOMpy',
-    version='0.8.4.8',
+    version='0.9',
     description='This package performs dynamic modelling of cellular signalling networks.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Luis Prado',
     author_email='pradolopezluis@gmail.com',
     url='https://github.com/lupralo31/SELDOMpy',
     download_url='https://github.com/lupralo31/SELDOMpy/archive/refs/tags/V_0.2.1.tar.gz',
@@ -41,15 +41,15 @@
                  "SELDOMpy/src/simulate_amigo_model.c",
                  "SELDOMpy/src/sundials_band.c",
                  "SELDOMpy/src/sundials_dense.c", "SELDOMpy/src/sundials_direct.c", "SELDOMpy/src/sundials_iterative.c",
                  "SELDOMpy/src/sundials_math.c", "SELDOMpy/src/sundials_nvector.c", "SELDOMpy/src/sundials_spbcgs.c",
                  "SELDOMpy/src/sundials_spgmr.c", "SELDOMpy/src/sundials_sptfqmr.c"],
         include_dirs=['SELDOMpy/include/include_amigo', 'SELDOMpy/include/include_cvodes', "SELDOMpy/src", numpy_include],
     )],
-    install_requires=["numpy", "scikit-learn", "pandas", "mealpy", "matplotlib", "setuptools", "openpyxl"],
+    install_requires=["numpy", "scikit-learn", "pandas", "mealpy", "matplotlib", "setuptools", "openpyxl", "pypesto"],
     include_package_data=True,
     license='GPLv3',
     classifiers=[
         # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Operating System :: OS Independent',
```

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/src/AMIGO_model.c` & `SELDOMpy-0.9/SELDOMpy/src/AMIGO_model.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/src/AMIGO_problem.c` & `SELDOMpy-0.9/SELDOMpy/src/AMIGO_problem.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/src/CNOStructure.h` & `SELDOMpy-0.9/SELDOMpy/src/CNOStructure.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/src/anODEModel.c` & `SELDOMpy-0.9/SELDOMpy/src/anODEModel.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/src/cvodea.c` & `SELDOMpy-0.9/SELDOMpy/src/cvodea.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/src/cvodea_io.c` & `SELDOMpy-0.9/SELDOMpy/src/cvodea_io.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/src/cvodes.c` & `SELDOMpy-0.9/SELDOMpy/src/cvodes.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/src/cvodes_band.c` & `SELDOMpy-0.9/SELDOMpy/src/cvodes_band.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/src/cvodes_bandpre.c` & `SELDOMpy-0.9/SELDOMpy/src/cvodes_bandpre.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/src/cvodes_bandpre_impl.h` & `SELDOMpy-0.9/SELDOMpy/src/cvodes_bandpre_impl.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/src/cvodes_bbdpre.c` & `SELDOMpy-0.9/SELDOMpy/src/cvodes_bbdpre.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/src/cvodes_bbdpre_impl.h` & `SELDOMpy-0.9/SELDOMpy/src/cvodes_bbdpre_impl.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/src/cvodes_dense.c` & `SELDOMpy-0.9/SELDOMpy/src/cvodes_dense.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/src/cvodes_diag.c` & `SELDOMpy-0.9/SELDOMpy/src/cvodes_diag.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/src/cvodes_diag_impl.h` & `SELDOMpy-0.9/SELDOMpy/src/cvodes_diag_impl.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/src/cvodes_direct.c` & `SELDOMpy-0.9/SELDOMpy/src/cvodes_direct.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/src/cvodes_direct_impl.h` & `SELDOMpy-0.9/SELDOMpy/src/cvodes_direct_impl.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/src/cvodes_impl.h` & `SELDOMpy-0.9/SELDOMpy/src/cvodes_impl.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/src/cvodes_io.c` & `SELDOMpy-0.9/SELDOMpy/src/cvodes_io.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/src/cvodes_spbcgs.c` & `SELDOMpy-0.9/SELDOMpy/src/cvodes_spbcgs.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/src/cvodes_spgmr.c` & `SELDOMpy-0.9/SELDOMpy/src/cvodes_spgmr.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/src/cvodes_spils.c` & `SELDOMpy-0.9/SELDOMpy/src/cvodes_spils.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/src/cvodes_spils_impl.h` & `SELDOMpy-0.9/SELDOMpy/src/cvodes_spils_impl.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/src/cvodes_sptfqmr.c` & `SELDOMpy-0.9/SELDOMpy/src/cvodes_sptfqmr.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/src/dhc.c` & `SELDOMpy-0.9/SELDOMpy/src/dhc.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/src/findStates.c` & `SELDOMpy-0.9/SELDOMpy/src/findStates.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/src/fnvector_serial.c` & `SELDOMpy-0.9/SELDOMpy/src/fnvector_serial.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/src/fnvector_serial.h` & `SELDOMpy-0.9/SELDOMpy/src/fnvector_serial.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/src/getAdjacencyMatrix.c` & `SELDOMpy-0.9/SELDOMpy/src/getAdjacencyMatrix.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/src/getStateIndex.c` & `SELDOMpy-0.9/SELDOMpy/src/getStateIndex.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/src/getTruthTables.c` & `SELDOMpy-0.9/SELDOMpy/src/getTruthTables.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/src/get_support_truth_tables.c` & `SELDOMpy-0.9/SELDOMpy/src/get_support_truth_tables.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/src/get_truth_tables_index.c` & `SELDOMpy-0.9/SELDOMpy/src/get_truth_tables_index.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/src/nvector_serial.c` & `SELDOMpy-0.9/SELDOMpy/src/nvector_serial.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/src/printNminiTerms.c` & `SELDOMpy-0.9/SELDOMpy/src/printNminiTerms.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/src/sim_logic_ode.c` & `SELDOMpy-0.9/SELDOMpy/src/sim_logic_ode.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/src/simulate_amigo_model.c` & `SELDOMpy-0.9/SELDOMpy/src/simulate_amigo_model.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/src/sundials_band.c` & `SELDOMpy-0.9/SELDOMpy/src/sundials_band.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/src/sundials_dense.c` & `SELDOMpy-0.9/SELDOMpy/src/sundials_dense.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/src/sundials_direct.c` & `SELDOMpy-0.9/SELDOMpy/src/sundials_direct.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/src/sundials_iterative.c` & `SELDOMpy-0.9/SELDOMpy/src/sundials_iterative.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/src/sundials_math.c` & `SELDOMpy-0.9/SELDOMpy/src/sundials_math.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/src/sundials_nvector.c` & `SELDOMpy-0.9/SELDOMpy/src/sundials_nvector.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/src/sundials_spbcgs.c` & `SELDOMpy-0.9/SELDOMpy/src/sundials_spbcgs.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/src/sundials_spgmr.c` & `SELDOMpy-0.9/SELDOMpy/src/sundials_spgmr.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy/src/sundials_sptfqmr.c` & `SELDOMpy-0.9/SELDOMpy/src/sundials_sptfqmr.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.9/SELDOMpy.egg-info/SOURCES.txt` & `SELDOMpy-0.9/SELDOMpy.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,13 @@
 LICENSE.txt
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
-SELDOMpy/LICENSE.txt
-SELDOMpy/README.md
 SELDOMpy/__init__.py
-SELDOMpy/makefile
-SELDOMpy/setup.cfg
-SELDOMpy/setup.py
 SELDOMpy.egg-info/PKG-INFO
 SELDOMpy.egg-info/SOURCES.txt
 SELDOMpy.egg-info/dependency_links.txt
 SELDOMpy.egg-info/requires.txt
 SELDOMpy.egg-info/top_level.txt
 SELDOMpy/src/AMIGO_model.c
 SELDOMpy/src/AMIGO_model_stats.c
@@ -60,14 +55,20 @@
 SELDOMpy/src/sundials_direct.c
 SELDOMpy/src/sundials_iterative.c
 SELDOMpy/src/sundials_math.c
 SELDOMpy/src/sundials_nvector.c
 SELDOMpy/src/sundials_spbcgs.c
 SELDOMpy/src/sundials_spgmr.c
 SELDOMpy/src/sundials_sptfqmr.c
+SELDOMpy/examples/MAPK/MAPK.xlsx
+SELDOMpy/examples/MAPK/training_and_reduce.py
+SELDOMpy/examples/MAPK/training_and_reduce_pyPESTO.py
+SELDOMpy/examples/SP/SP.xlsx
+SELDOMpy/examples/SP/training_and_reduce.py
+SELDOMpy/examples/SP/training_and_reduce_pyPESTO.py
 SELDOMpy/functions/buildmim.py
 SELDOMpy/functions/extras.py
 SELDOMpy/functions/gen_exps.py
 SELDOMpy/functions/getLBODEmodel.py
 SELDOMpy/functions/getRandomLBODEmodel.py
 SELDOMpy/functions/optimization.py
 SELDOMpy/functions/plot_results.py
```

