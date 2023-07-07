# Comparing `tmp/RIFT-0.0.15.9rc5.tar.gz` & `tmp/RIFT-0.0.15.9rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RIFT-0.0.15.9rc5.tar", last modified: Wed Jun 28 10:21:01 2023, max compression
+gzip compressed data, was "RIFT-0.0.15.9rc6.tar", last modified: Fri Jul  7 00:22:00 2023, max compression
```

## Comparing `RIFT-0.0.15.9rc5.tar` & `RIFT-0.0.15.9rc6.tar`

### file list

```diff
@@ -1,193 +1,193 @@
-drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-06-28 10:21:01.986682 RIFT-0.0.15.9rc5/
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1042 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/AUTOMATED_OR_ONLINE.md
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1755 2023-04-20 10:32:56.000000 RIFT-0.0.15.9rc5/Dockerfile
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    22146 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/GETTING_STARTED.md
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3557 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/INSTALL.md
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1364 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/INSTALL_OPTIONAL_DEPENDENCIES.md
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1118 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/LICENSE.md
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      204 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MANIFEST.in
-drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-06-28 10:21:01.493681 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/
-drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-06-28 10:21:01.499681 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/
-drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-06-28 10:21:01.541681 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      173 2023-05-24 11:46:08.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/__init__.py
-drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-06-28 10:21:01.558681 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/calmarg/
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)       22 2023-05-24 11:46:08.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/calmarg/__init__.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6265 2023-05-24 11:46:08.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/calmarg/rift_source.py
-drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-06-28 10:21:01.587681 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/integrators/
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    18724 2023-04-16 18:23:39.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/integrators/MonteCarloEnsemble.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/integrators/__init__.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2592 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/integrators/direct_quadrature.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    20255 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/integrators/gaussian_mixture_model.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    53572 2023-05-30 17:28:25.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsampler.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    28350 2023-05-24 11:46:08.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsamplerEnsemble.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    69417 2023-06-19 13:21:23.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsamplerGPU.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2901 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/integrators/multivariate_truncnorm.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7235 2022-10-24 14:00:10.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/integrators/statutils.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    33113 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/integrators/weighted_gmm.py
-drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-06-28 10:21:01.612681 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/interpolators/
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     9944 2022-10-23 22:26:00.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/interpolators/BayesianLeastSquares.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3835 2022-10-23 22:26:00.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/interpolators/ConstrainedQuadraticLikelihood.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/interpolators/__init__.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2658 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/interpolators/efficient_save_sklearn_gp.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1655 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/interpolators/gp.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2518 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/interpolators/gpytorch_wrapper.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5558 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/interpolators/internal_GP.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3488 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/interpolators/interp_gpu.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    26826 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/interpolators/senni.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)   249803 2023-06-28 10:20:41.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/lalsimutils.py
-drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-06-28 10:21:01.638681 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/likelihood/
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1643 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/likelihood/Q_inner_product.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    33438 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/likelihood/SphericalHarmonics_gpu.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/likelihood/__init__.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1525 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/likelihood/cuda_Q_inner_product.cu
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    94340 2023-06-19 13:21:23.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/likelihood/factored_likelihood.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5269 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/likelihood/optimized_gpu_tools.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1451 2023-05-30 17:28:25.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/likelihood/priors_utils.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4616 2023-06-07 15:16:25.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/likelihood/vectorized_general_tools.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4706 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/likelihood/vectorized_lal_tools.py
-drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-06-28 10:21:01.676681 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/misc/
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    70947 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/misc/ModifiedScikitFit.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)       65 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/misc/__init__.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    29427 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/misc/amrlib.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7367 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/misc/bounded_kde.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      229 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/misc/common_cl.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)   109345 2023-05-24 11:46:08.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/misc/dag_utils.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     9324 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/misc/modules.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    23083 2022-10-11 14:57:54.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/misc/our_corner.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    30542 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/misc/ourparams.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    10915 2023-03-24 18:44:03.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/misc/samples_utils.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2901 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/misc/sky_rotations.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    10623 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/misc/spokes.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6975 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/misc/tools.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2641 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/misc/weight_simulations.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     8651 2023-05-30 17:28:25.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/misc/xmlutils.py
-drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-06-28 10:21:01.703681 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/physics/
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    26126 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/physics/EOBTidalExternal.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    31276 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/physics/EOBTidalExternalC.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    63809 2023-06-19 13:21:23.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/physics/EOSManager.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4776 2023-06-19 13:21:23.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/physics/GWSignal.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2654 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/physics/MonotonicSpline.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    19507 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/physics/PrecessingFisherMatrix.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    52302 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/physics/ROMWaveformManager.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)       68 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/physics/__init__.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    23733 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/physics/effectiveFisher.py
-drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-06-28 10:21:01.554681 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT.egg-info/
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6360 2023-06-28 10:20:58.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT.egg-info/PKG-INFO
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    10749 2023-06-28 10:20:59.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT.egg-info/SOURCES.txt
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        1 2023-06-28 10:20:58.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT.egg-info/dependency_links.txt
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      142 2023-06-28 10:20:58.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT.egg-info/requires.txt
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        5 2023-06-28 10:20:58.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT.egg-info/top_level.txt
-drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-06-28 10:21:01.983682 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     8723 2022-10-11 14:57:54.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/assess_propose_CIP_convergence_sequence.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    13848 2023-05-24 11:46:08.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/calibration_reweighting.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2371 2023-04-22 14:25:02.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/combine_weights_and_rejection_sample.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2800 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/config_yank.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6140 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/convergence_test_amr.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     9039 2023-06-07 15:16:25.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/convergence_test_samples.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2239 2023-04-20 10:32:56.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/convert_ascii_framechange_xphm.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1224 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/convert_dat_to_hdf5.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1920 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/convert_output_format_allnet2xml
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      541 2023-03-24 18:44:03.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/convert_output_format_ascii2h5.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    11799 2023-03-12 13:15:08.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/convert_output_format_ile2inference
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     8166 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/convert_output_format_inference2ile
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2013 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/convert_psd_ascii2xml
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     9065 2022-10-11 14:57:54.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/create_CIP_convergence_sequence.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    33867 2023-06-28 10:20:41.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/create_eos_posterior_pipeline
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    14569 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/create_event_dag_via_grid
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    88335 2022-10-11 14:57:54.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_AlternateIteration
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)   120596 2023-06-28 10:20:41.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_BasicIteration
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    71601 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_BasicMultiApproxIteration
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2768 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/create_ile_sub_dag.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    13979 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/create_postprocessing_event_dag.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    98022 2023-06-19 13:21:23.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/helper_LDG_Events.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1886 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/helper_OnlinePSDCleanup.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    20152 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/ile_postproc_add_time
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    83560 2023-03-12 13:15:08.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)   103850 2023-06-19 13:21:23.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic_batchmode
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    18630 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic_no-op
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5408 2023-03-24 18:44:03.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/make_uni_comov_skymap.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    38440 2023-06-28 10:20:41.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/plot_posterior_corner.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3746 2023-03-24 18:44:03.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/resample_uniform_comoving.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      354 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/switcheroo
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    34265 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_AMRGrid.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3696 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_AdaptiveExponent.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    18544 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_AnalyticFisherGrid.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7348 2023-06-19 13:21:23.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_BatchConvertResampleILEOutput.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1028 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_CIPdagPostprocess.sh
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      219 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_CacheFileConvert.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1436 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_CharacterizePosterior.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3934 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_CleanILE.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      876 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_CoincIFOUtility.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    15127 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_CompareWaveformsInDetectors.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      853 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_ConsolidateDAGsUnderMaster.sh
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    10380 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_ConstructBNSMarginalEOSRank.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    33309 2023-06-28 10:20:41.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_ConstructEOSPosterior.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    55368 2022-11-28 22:41:57.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_ConstructIntrinsicPosterior_GaussianResampling.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)   164169 2023-06-28 10:20:41.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_ConstructIntrinsicPosterior_GenericCoordinates.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2314 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_CoordinateNamesAngularToCartesianSpins.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     9633 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_EOBTideWriteFrame.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      389 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_EstimateWaveformDuration.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3250 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_FetchExternalGrid.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    27796 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_FitAndEvaluate_GenericCoordinates.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      256 2022-10-11 14:57:54.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_ForOSG_MakeLocalFramesDir.sh
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1640 2023-03-12 13:15:08.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_ForOSG_MakeTruncatedLocalFramesDir.sh
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3266 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_FrameZeroNoiseSNR.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    11553 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_GenerateMaxlnLWaveform.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6162 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_GenerateMaxlnLWaveform_NRFromIndex.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2223 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_GridRecenter.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    13919 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_GridSubsetOfTemplateBank.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2778 2023-04-07 18:24:37.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_HyperCombine.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1590 2023-04-07 18:24:37.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_HyperparameterGrid.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5168 2023-06-28 10:20:41.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_HyperparameterPuffball.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      829 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_ILENextGeneration.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1018 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_ILEROMdagPostprocess.sh
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1597 2022-10-11 14:57:54.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_ILEdagPostprocess.sh
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6780 2023-03-24 18:44:03.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_InitMargTable
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4553 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_IntermediateEOSIntegralFromFit.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    40228 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_IterativeFisher.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2698 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_JoinXML.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     8109 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_LALCompareApproximantsOnSamples.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7660 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_LALWriteFrame.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    50356 2022-10-11 14:57:54.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_ManualOverlapGrid.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7195 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_MarginalizedLikelihoodEOSIntegralFromIntermediate.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1214 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_MassGrid.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2450 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_MassGridCoalesce.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     8821 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_NRBestOfIndex.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6671 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_NRDumpDetectorResponse.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    20394 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_NRExtrudeOverlapGrid.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5672 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_NRIndexedFminCutToILE.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    10752 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_NRNearestSimulationTo.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4794 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_NRRelabelILE.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     9830 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_NRWriteFrame.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3377 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_NR_GWMemory.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1490 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_NRdagPostprocess.sh
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2349 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_ParameterFilter.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    12414 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_ParameterPuffball.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3665 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_ParameterRandomize.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1087 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_PosteriorPostprocess.sh
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3302 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_PrintInjection.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5424 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_RIFT_MultiMetaPipe.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    79440 2023-06-28 10:20:41.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_RIFT_pseudo_pipe.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    35804 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_RIFT_pseudo_pipe_lowlatency.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6293 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_ROMWriteFrame.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1675 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_RandomizeOverlapOrder.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3080 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_ResampleILEOutputWithExtrinsic.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3792 2023-03-24 18:44:03.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_SimInspiralToCoinc.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7587 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_TEOBResumSWriteFrame.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4982 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_TestSpokesIO.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      814 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_TestXMLParameterStorage.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    11254 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_TidalPlotSimulationStrain.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      457 2022-10-15 00:56:03.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_TruncateMergeFrames.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3430 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_WriteFrameAndCacheFromXML.sh
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2784 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_WriteInjectionFile.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1955 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_WriteXMLWithEOS.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      276 2023-04-22 14:25:02.000000 RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_shuffle_file.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3488 2022-09-24 12:18:48.000000 RIFT-0.0.15.9rc5/PACKAGING.md
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6360 2023-06-28 10:21:01.985682 RIFT-0.0.15.9rc5/PKG-INFO
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5821 2023-04-07 18:24:37.000000 RIFT-0.0.15.9rc5/README.md
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6132 2022-09-24 12:18:48.000000 RIFT-0.0.15.9rc5/TROUBLESHOOTING.md
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6136 2022-09-24 12:18:48.000000 RIFT-0.0.15.9rc5/howto.md
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)       96 2023-04-24 19:45:36.000000 RIFT-0.0.15.9rc5/pyproject.toml
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      184 2023-03-24 18:44:03.000000 RIFT-0.0.15.9rc5/requirements.txt
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)       38 2023-06-28 10:21:01.987682 RIFT-0.0.15.9rc5/setup.cfg
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2934 2023-06-28 10:20:41.000000 RIFT-0.0.15.9rc5/setup.py
+drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-07-07 00:22:00.943000 RIFT-0.0.15.9rc6/
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1042 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/AUTOMATED_OR_ONLINE.md
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1755 2023-04-20 10:32:56.000000 RIFT-0.0.15.9rc6/Dockerfile
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    22146 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/GETTING_STARTED.md
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3557 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/INSTALL.md
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1364 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/INSTALL_OPTIONAL_DEPENDENCIES.md
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1118 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/LICENSE.md
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      204 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MANIFEST.in
+drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-07-07 00:21:59.765995 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/
+drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-07-07 00:21:59.771995 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/
+drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-07-07 00:21:59.803995 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      173 2023-05-24 11:46:08.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/__init__.py
+drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-07-07 00:21:59.815995 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/calmarg/
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)       22 2023-05-24 11:46:08.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/calmarg/__init__.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6265 2023-05-24 11:46:08.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/calmarg/rift_source.py
+drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-07-07 00:21:59.889996 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/integrators/
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    18724 2023-04-16 18:23:39.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/integrators/MonteCarloEnsemble.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/integrators/__init__.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2592 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/integrators/direct_quadrature.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    20255 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/integrators/gaussian_mixture_model.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    53572 2023-05-30 17:28:25.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsampler.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    28350 2023-05-24 11:46:08.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsamplerEnsemble.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    69417 2023-06-19 13:21:23.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsamplerGPU.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2901 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/integrators/multivariate_truncnorm.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7235 2022-10-24 14:00:10.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/integrators/statutils.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    33113 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/integrators/weighted_gmm.py
+drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-07-07 00:21:59.907996 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/interpolators/
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     9944 2022-10-23 22:26:00.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/interpolators/BayesianLeastSquares.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3835 2022-10-23 22:26:00.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/interpolators/ConstrainedQuadraticLikelihood.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/interpolators/__init__.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2658 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/interpolators/efficient_save_sklearn_gp.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1655 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/interpolators/gp.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2518 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/interpolators/gpytorch_wrapper.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5558 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/interpolators/internal_GP.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3488 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/interpolators/interp_gpu.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    26826 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/interpolators/senni.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)   249803 2023-06-28 10:20:41.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/lalsimutils.py
+drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-07-07 00:21:59.928996 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/likelihood/
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1643 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/likelihood/Q_inner_product.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    33438 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/likelihood/SphericalHarmonics_gpu.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/likelihood/__init__.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1525 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/likelihood/cuda_Q_inner_product.cu
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    94340 2023-06-19 13:21:23.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/likelihood/factored_likelihood.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5269 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/likelihood/optimized_gpu_tools.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1451 2023-05-30 17:28:25.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/likelihood/priors_utils.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4616 2023-06-07 15:16:25.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/likelihood/vectorized_general_tools.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4706 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/likelihood/vectorized_lal_tools.py
+drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-07-07 00:21:59.964996 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    70947 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/ModifiedScikitFit.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)       65 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/__init__.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    29427 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/amrlib.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7367 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/bounded_kde.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      229 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/common_cl.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)   109345 2023-05-24 11:46:08.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/dag_utils.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     9324 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/modules.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    23083 2022-10-11 14:57:54.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/our_corner.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    30542 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/ourparams.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    10915 2023-03-24 18:44:03.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/samples_utils.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2901 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/sky_rotations.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    10623 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/spokes.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6975 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/tools.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2641 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/weight_simulations.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     8651 2023-05-30 17:28:25.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/xmlutils.py
+drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-07-07 00:22:00.019996 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/physics/
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    26126 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/physics/EOBTidalExternal.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    31276 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/physics/EOBTidalExternalC.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    63915 2023-07-07 00:20:50.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/physics/EOSManager.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4776 2023-06-19 13:21:23.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/physics/GWSignal.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2654 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/physics/MonotonicSpline.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    19507 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/physics/PrecessingFisherMatrix.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    52302 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/physics/ROMWaveformManager.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)       68 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/physics/__init__.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    23733 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/physics/effectiveFisher.py
+drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-07-07 00:21:59.812996 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT.egg-info/
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6360 2023-07-07 00:21:57.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT.egg-info/PKG-INFO
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    10749 2023-07-07 00:21:57.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT.egg-info/SOURCES.txt
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        1 2023-07-07 00:21:57.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT.egg-info/dependency_links.txt
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      142 2023-07-07 00:21:57.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT.egg-info/requires.txt
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        5 2023-07-07 00:21:57.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT.egg-info/top_level.txt
+drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-07-07 00:22:00.939000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     8723 2022-10-11 14:57:54.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/assess_propose_CIP_convergence_sequence.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    13848 2023-05-24 11:46:08.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/calibration_reweighting.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2371 2023-04-22 14:25:02.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/combine_weights_and_rejection_sample.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2800 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/config_yank.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6140 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/convergence_test_amr.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     9039 2023-06-07 15:16:25.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/convergence_test_samples.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2239 2023-04-20 10:32:56.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/convert_ascii_framechange_xphm.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1224 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/convert_dat_to_hdf5.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1920 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/convert_output_format_allnet2xml
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      541 2023-03-24 18:44:03.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/convert_output_format_ascii2h5.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    11799 2023-03-12 13:15:08.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/convert_output_format_ile2inference
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     8166 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/convert_output_format_inference2ile
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2013 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/convert_psd_ascii2xml
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     9065 2022-10-11 14:57:54.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/create_CIP_convergence_sequence.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    34015 2023-07-07 00:20:50.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/create_eos_posterior_pipeline
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    14569 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/create_event_dag_via_grid
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    88335 2022-10-11 14:57:54.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_AlternateIteration
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)   120734 2023-07-07 00:20:50.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_BasicIteration
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    71601 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_BasicMultiApproxIteration
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2768 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/create_ile_sub_dag.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    13979 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/create_postprocessing_event_dag.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    98022 2023-06-19 13:21:23.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/helper_LDG_Events.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1886 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/helper_OnlinePSDCleanup.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    20152 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/ile_postproc_add_time
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    83560 2023-03-12 13:15:08.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)   103850 2023-06-19 13:21:23.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic_batchmode
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    18630 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic_no-op
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5408 2023-03-24 18:44:03.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/make_uni_comov_skymap.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    38621 2023-07-07 00:20:50.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/plot_posterior_corner.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3746 2023-03-24 18:44:03.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/resample_uniform_comoving.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      354 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/switcheroo
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    34265 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_AMRGrid.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3696 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_AdaptiveExponent.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    18544 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_AnalyticFisherGrid.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7348 2023-06-19 13:21:23.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_BatchConvertResampleILEOutput.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1028 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_CIPdagPostprocess.sh
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      219 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_CacheFileConvert.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1436 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_CharacterizePosterior.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3934 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_CleanILE.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      876 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_CoincIFOUtility.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    15127 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_CompareWaveformsInDetectors.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      853 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_ConsolidateDAGsUnderMaster.sh
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    10380 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_ConstructBNSMarginalEOSRank.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    33309 2023-06-28 10:20:41.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_ConstructEOSPosterior.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    55368 2022-11-28 22:41:57.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_ConstructIntrinsicPosterior_GaussianResampling.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)   164522 2023-07-07 00:20:50.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_ConstructIntrinsicPosterior_GenericCoordinates.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2314 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_CoordinateNamesAngularToCartesianSpins.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     9633 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_EOBTideWriteFrame.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      389 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_EstimateWaveformDuration.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3250 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_FetchExternalGrid.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    27796 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_FitAndEvaluate_GenericCoordinates.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      256 2022-10-11 14:57:54.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_ForOSG_MakeLocalFramesDir.sh
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1640 2023-03-12 13:15:08.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_ForOSG_MakeTruncatedLocalFramesDir.sh
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3266 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_FrameZeroNoiseSNR.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    11553 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_GenerateMaxlnLWaveform.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6162 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_GenerateMaxlnLWaveform_NRFromIndex.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2223 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_GridRecenter.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    13919 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_GridSubsetOfTemplateBank.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3330 2023-07-07 00:20:50.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_HyperCombine.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1590 2023-04-07 18:24:37.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_HyperparameterGrid.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5168 2023-06-28 10:20:41.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_HyperparameterPuffball.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      829 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_ILENextGeneration.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1018 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_ILEROMdagPostprocess.sh
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1597 2022-10-11 14:57:54.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_ILEdagPostprocess.sh
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6780 2023-03-24 18:44:03.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_InitMargTable
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4553 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_IntermediateEOSIntegralFromFit.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    40228 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_IterativeFisher.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2698 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_JoinXML.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     8109 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_LALCompareApproximantsOnSamples.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7660 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_LALWriteFrame.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    50356 2022-10-11 14:57:54.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_ManualOverlapGrid.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7195 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_MarginalizedLikelihoodEOSIntegralFromIntermediate.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1214 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_MassGrid.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2450 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_MassGridCoalesce.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     8821 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_NRBestOfIndex.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6671 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_NRDumpDetectorResponse.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    20394 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_NRExtrudeOverlapGrid.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5672 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_NRIndexedFminCutToILE.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    10752 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_NRNearestSimulationTo.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4794 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_NRRelabelILE.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     9830 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_NRWriteFrame.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3377 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_NR_GWMemory.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1490 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_NRdagPostprocess.sh
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2349 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_ParameterFilter.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    12414 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_ParameterPuffball.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3665 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_ParameterRandomize.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1087 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_PosteriorPostprocess.sh
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3302 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_PrintInjection.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5424 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_RIFT_MultiMetaPipe.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    79440 2023-06-28 10:20:41.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_RIFT_pseudo_pipe.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    35804 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_RIFT_pseudo_pipe_lowlatency.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6293 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_ROMWriteFrame.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1675 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_RandomizeOverlapOrder.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3080 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_ResampleILEOutputWithExtrinsic.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3792 2023-03-24 18:44:03.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_SimInspiralToCoinc.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7587 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_TEOBResumSWriteFrame.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4982 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_TestSpokesIO.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      814 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_TestXMLParameterStorage.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    11254 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_TidalPlotSimulationStrain.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      457 2022-10-15 00:56:03.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_TruncateMergeFrames.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3430 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_WriteFrameAndCacheFromXML.sh
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2784 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_WriteInjectionFile.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1955 2022-09-24 12:18:47.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_WriteXMLWithEOS.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      276 2023-04-22 14:25:02.000000 RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_shuffle_file.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3488 2022-09-24 12:18:48.000000 RIFT-0.0.15.9rc6/PACKAGING.md
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6360 2023-07-07 00:22:00.941000 RIFT-0.0.15.9rc6/PKG-INFO
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5821 2023-04-07 18:24:37.000000 RIFT-0.0.15.9rc6/README.md
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6132 2022-09-24 12:18:48.000000 RIFT-0.0.15.9rc6/TROUBLESHOOTING.md
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6136 2022-09-24 12:18:48.000000 RIFT-0.0.15.9rc6/howto.md
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)       96 2023-04-24 19:45:36.000000 RIFT-0.0.15.9rc6/pyproject.toml
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      184 2023-03-24 18:44:03.000000 RIFT-0.0.15.9rc6/requirements.txt
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)       38 2023-07-07 00:22:00.943000 RIFT-0.0.15.9rc6/setup.cfg
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2934 2023-07-07 00:20:50.000000 RIFT-0.0.15.9rc6/setup.py
```

### Comparing `RIFT-0.0.15.9rc5/AUTOMATED_OR_ONLINE.md` & `RIFT-0.0.15.9rc6/AUTOMATED_OR_ONLINE.md`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/Dockerfile` & `RIFT-0.0.15.9rc6/Dockerfile`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/GETTING_STARTED.md` & `RIFT-0.0.15.9rc6/GETTING_STARTED.md`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/INSTALL.md` & `RIFT-0.0.15.9rc6/INSTALL.md`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/INSTALL_OPTIONAL_DEPENDENCIES.md` & `RIFT-0.0.15.9rc6/INSTALL_OPTIONAL_DEPENDENCIES.md`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/LICENSE.md` & `RIFT-0.0.15.9rc6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/calmarg/rift_source.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/calmarg/rift_source.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/integrators/MonteCarloEnsemble.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/integrators/MonteCarloEnsemble.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/integrators/direct_quadrature.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/integrators/direct_quadrature.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/integrators/gaussian_mixture_model.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/integrators/gaussian_mixture_model.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsampler.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsampler.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsamplerEnsemble.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsamplerEnsemble.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsamplerGPU.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsamplerGPU.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/integrators/multivariate_truncnorm.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/integrators/multivariate_truncnorm.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/integrators/statutils.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/integrators/statutils.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/integrators/weighted_gmm.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/integrators/weighted_gmm.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/interpolators/BayesianLeastSquares.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/interpolators/BayesianLeastSquares.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/interpolators/ConstrainedQuadraticLikelihood.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/interpolators/ConstrainedQuadraticLikelihood.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/interpolators/efficient_save_sklearn_gp.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/interpolators/efficient_save_sklearn_gp.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/interpolators/gp.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/interpolators/gp.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/interpolators/gpytorch_wrapper.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/interpolators/gpytorch_wrapper.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/interpolators/internal_GP.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/interpolators/internal_GP.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/interpolators/interp_gpu.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/interpolators/interp_gpu.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/interpolators/senni.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/interpolators/senni.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/lalsimutils.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/lalsimutils.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/likelihood/Q_inner_product.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/likelihood/Q_inner_product.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/likelihood/SphericalHarmonics_gpu.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/likelihood/SphericalHarmonics_gpu.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/likelihood/cuda_Q_inner_product.cu` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/likelihood/cuda_Q_inner_product.cu`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/likelihood/factored_likelihood.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/likelihood/factored_likelihood.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/likelihood/optimized_gpu_tools.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/likelihood/optimized_gpu_tools.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/likelihood/priors_utils.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/likelihood/priors_utils.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/likelihood/vectorized_general_tools.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/likelihood/vectorized_general_tools.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/likelihood/vectorized_lal_tools.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/likelihood/vectorized_lal_tools.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/misc/ModifiedScikitFit.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/ModifiedScikitFit.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/misc/amrlib.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/amrlib.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/misc/bounded_kde.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/bounded_kde.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/misc/dag_utils.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/dag_utils.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/misc/modules.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/modules.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/misc/our_corner.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/our_corner.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/misc/ourparams.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/ourparams.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/misc/samples_utils.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/samples_utils.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/misc/sky_rotations.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/sky_rotations.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/misc/spokes.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/spokes.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/misc/tools.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/tools.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/misc/weight_simulations.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/weight_simulations.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/misc/xmlutils.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/xmlutils.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/physics/EOBTidalExternal.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/physics/EOBTidalExternal.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/physics/EOBTidalExternalC.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/physics/EOBTidalExternalC.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/physics/EOSManager.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/physics/EOSManager.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,14 +73,17 @@
         return None
 
     def lambda_from_m(self, m):
         eos_fam = self.eos_fam
         if m<10**15:
             m=m*lal.MSUN_SI
 
+        if m/lal.MSUN_SI > 0.999*self.mMaxMsun:
+            return 1e-8  # not exactly zero, but tiny
+
         k2=lalsim.SimNeutronStarLoveNumberK2(m, eos_fam)
         r=lalsim.SimNeutronStarRadius(m, eos_fam)
 
         m=m*lal.G_SI/lal.C_SI**2
         lam=2./(3*lal.G_SI)*k2*r**5
         dimensionless_lam=lal.G_SI*lam*(1/m)**5
```

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/physics/GWSignal.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/physics/GWSignal.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/physics/MonotonicSpline.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/physics/MonotonicSpline.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/physics/PrecessingFisherMatrix.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/physics/PrecessingFisherMatrix.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/physics/ROMWaveformManager.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/physics/ROMWaveformManager.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT/physics/effectiveFisher.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT/physics/effectiveFisher.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT.egg-info/PKG-INFO` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RIFT
-Version: 0.0.15.9rc5
+Version: 0.0.15.9rc6
 Summary: RIFT parameter estimation pipeline. Note branch used is temp-RIT-Tides-port_python3_restructure_package (which will become master shortly)!
 Home-page: https://git.ligo.org/rapidpe-rift/rift
 Author: Richard O'Shaughnessy
 Author-email: richard.oshaughnessy@ligo.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/RIFT.egg-info/SOURCES.txt` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/RIFT.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/assess_propose_CIP_convergence_sequence.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/assess_propose_CIP_convergence_sequence.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/calibration_reweighting.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/calibration_reweighting.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/combine_weights_and_rejection_sample.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/combine_weights_and_rejection_sample.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/config_yank.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/config_yank.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/convergence_test_amr.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/convergence_test_amr.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/convergence_test_samples.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/convergence_test_samples.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/convert_ascii_framechange_xphm.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/convert_ascii_framechange_xphm.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/convert_dat_to_hdf5.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/convert_dat_to_hdf5.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/convert_output_format_allnet2xml` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/convert_output_format_allnet2xml`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/convert_output_format_ascii2h5.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/convert_output_format_ascii2h5.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/convert_output_format_ile2inference` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/convert_output_format_ile2inference`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/convert_output_format_inference2ile` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/convert_output_format_inference2ile`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/convert_psd_ascii2xml` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/convert_psd_ascii2xml`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/create_CIP_convergence_sequence.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/create_CIP_convergence_sequence.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/create_eos_posterior_pipeline` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/create_eos_posterior_pipeline`

 * *Files 2% similar despite different names*

```diff
@@ -168,16 +168,16 @@
 if True: # not (opts.eos_post_args is None):
     with open(opts.eos_post_args) as f:
         eos_post_args_list = f.readlines()
     eos_post_args = ' '.join( [x.replace('\\','') for x in eos_post_args_list] )
     eos_post_args = ' '.join(eos_post_args.split(' ')[1:])
     # Some argument protection for later.  Make sure spaces in place to avoid breaking compound arguments like g0:[a,b] for ranges.
     # intended to make sure any spaces in arguments like [a, b] are encoded as '[a, b]' 
-    eos_post_args = eos_post_args.replace(' [', '  \'[')
-    eos_post_args = eos_post_args.replace('] ', ']\' ')
+#    eos_post_args = eos_post_args.replace(' [', '  \'[')
+#    eos_post_args = eos_post_args.replace('] ', ']\' ')
     eos_post_args=eos_post_args.rstrip()
     eos_post_args += ' --no-plots '  
     print("EOS_POST", eos_post_args)
 
 eospost_exe = which('util_ConstructEOSPosterior.py')
 if opts.eos_post_exe:
     eospost_exe = "{}".format(opts.eos_post_exe) # force clpy, so NOT BY REFERENCE
@@ -238,17 +238,17 @@
 #   - issue is that transfer files depend on event
 #   - all output goes into the same iter*_marg directory
 #   - join script will merge all together
     cip_job, cip_job_name = dag_utils.write_CIP_sub(tag='MARG',log_dir=None,arg_str=marg_event_args,using_eos='file:'+working_dir_inside_local+"/grid-$(macroiteration).dat",using_eos_index='$(macroevent)',request_memory=opts.request_memory_marg,input_net=working_dir_inside_local+'/event-$(macroid).net',output='MARG-$(macroid)-$(macroevent)',out_dir=out_dir_inside_marg,exe=marg_exe_master,universe=local_worker_universe,no_grid=not(opts.use_osg),use_osg=opts.use_osg,use_singularity=opts.use_osg and opts.use_singularity,singularity_image=singularity_image,use_simple_osg_requirements=opts.use_osg,transfer_files=['../event-$(macroid).net'])
     # Modify: set 'initialdir'
     cip_job.add_condor_cmd("initialdir",opts.working_directory+"/iteration_$(macroiteration)_marg")
     # Modify output argument: change logs and working directory to be subdirectory for the run
-    cip_job.set_log_file(opts.working_directory+"/iteration_$(macroiteration)_marg/logs/marg-$(macroevent)-$(cluster)-$(process).log")
-    cip_job.set_stderr_file(opts.working_directory+"/iteration_$(macroiteration)_marg/logs/marg-$(macroevent)-$(cluster)-$(process).err")
-    cip_job.set_stdout_file(opts.working_directory+"/iteration_$(macroiteration)_marg/logs/marg-$(macroevent)-$(cluster)-$(process).out")
+    cip_job.set_log_file(opts.working_directory+"/iteration_$(macroiteration)_marg/logs/marg-$(macroevent)-$(macroid)-$(cluster)-$(process).log")
+    cip_job.set_stderr_file(opts.working_directory+"/iteration_$(macroiteration)_marg/logs/marg-$(macroevent)-$(macroid)-$(cluster)-$(process).err")
+    cip_job.set_stdout_file(opts.working_directory+"/iteration_$(macroiteration)_marg/logs/marg-$(macroevent)-$(macroid)-$(cluster)-$(process).out")
     cip_job.add_condor_cmd('request_disk',opts.general_request_disk)
     if opts.use_full_submit_paths:
         fname = opts.working_directory+"/"+cip_job.get_sub_file()
         cip_job.set_sub_file(fname)
     cip_job.write_sub_file()
 
     # PUFF variant
@@ -267,32 +267,32 @@
 
 else:
     for indx in np.arange(len(marg_event_args_list)):
         cip_job, cip_job_name = dag_utils.write_CIP_sub(tag='MARG_{}'.format(indx),log_dir=None,exe=marg_event_exe_list[indx],arg_str=marg_event_args_list[indx],using_eos='file:'+working_dir_inside_local+"/grid-$(macroiteration).dat",using_eos_index='$(macroevent)',request_memory=opts.request_memory_marg,input_net=working_dir_inside_local+'/event-$(macroid).net',output='MARG-$(macroid)-$(macroevent)',out_dir=out_dir_inside_marg,universe=local_worker_universe,no_grid=not(opts.use_osg),use_osg=opts.use_osg,use_singularity=opts.use_osg and opts.use_singularity,singularity_image=singularity_image,use_simple_osg_requirements=opts.use_osg,transfer_files=['../event-$(macroid).net'])
         # Modify: set 'initialdir'
         cip_job.add_condor_cmd("initialdir",opts.working_directory+"/iteration_$(macroiteration)_marg")
         # Modify output argument: change logs and working directory to be subdirectory for the run
-        cip_job.set_log_file(opts.working_directory+"/iteration_$(macroiteration)_marg/logs/marg-$(macroevent)-$(cluster)-$(process).log")
-        cip_job.set_stderr_file(opts.working_directory+"/iteration_$(macroiteration)_marg/logs/marg-$(macroevent)-$(cluster)-$(process).err")
-        cip_job.set_stdout_file(opts.working_directory+"/iteration_$(macroiteration)_marg/logs/marg-$(macroevent)-$(cluster)-$(process).out")
+        cip_job.set_log_file(opts.working_directory+"/iteration_$(macroiteration)_marg/logs/marg-$(macroevent)-$(macroid)-$(cluster)-$(process).log")
+        cip_job.set_stderr_file(opts.working_directory+"/iteration_$(macroiteration)_marg/logs/marg-$(macroevent)-$(macroid)-$(cluster)-$(process).err")
+        cip_job.set_stdout_file(opts.working_directory+"/iteration_$(macroiteration)_marg/logs/marg-$(macroevent)-$(macroid)-$(cluster)-$(process).out")
         cip_job.add_condor_cmd('request_disk',opts.general_request_disk)
         if opts.use_full_submit_paths:
             fname = opts.working_directory+"/"+cip_job.get_sub_file()
             cip_job.set_sub_file(fname)
         cip_job.write_sub_file()
         cip_job_list.append(cip_job)
 
         # PUFF variant
         cipPuff_job, cipPuff_job_name = dag_utils.write_CIP_sub(tag='MARG_PUFF_{}'.format(indx),log_dir=None,exe=marg_event_exe_list[indx],arg_str=marg_event_args_list[indx],using_eos='file:'+working_dir_inside_local+"/grid_puff-$(macroiteration).dat",using_eos_index='$(macroevent)',request_memory=opts.request_memory_marg,input_net=working_dir_inside_local+'/event-$(macroid).net',output='MARG-$(macroid)-$(macroevent)',out_dir=out_dir_inside_marg,universe=local_worker_universe,no_grid=not(opts.use_osg),use_osg=opts.use_osg,use_singularity=opts.use_osg and opts.use_singularity,singularity_image=singularity_image,use_simple_osg_requirements=opts.use_osg,transfer_files=['../event-$(macroid).net'])
     # Modify: set 'initialdir'
         cipPuff_job.add_condor_cmd("initialdir",opts.working_directory+"/iteration_$(macroiteration)_marg")
     # Modify output argument: change logs and working directory to be subdirectory for the run
-        cipPuff_job.set_log_file(opts.working_directory+"/iteration_$(macroiteration)_marg/logs/margPuff-$(cluster)-$(process).log")
-        cipPuff_job.set_stderr_file(opts.working_directory+"/iteration_$(macroiteration)_marg/logs/margPuff-$(cluster)-$(process).err")
-        cipPuff_job.set_stdout_file(opts.working_directory+"/iteration_$(macroiteration)_marg/logs/margPuff-$(cluster)-$(process).out")
+        cipPuff_job.set_log_file(opts.working_directory+"/iteration_$(macroiteration)_marg/logs/margPuff-$(macroevent)-$(macroid)-$(cluster)-$(process).log")
+        cipPuff_job.set_stderr_file(opts.working_directory+"/iteration_$(macroiteration)_marg/logs/margPuff-$(macroevent)-$(macroid)-$(cluster)-$(process).err")
+        cipPuff_job.set_stdout_file(opts.working_directory+"/iteration_$(macroiteration)_marg/logs/margPuff-$(macroevent)-$(macroid)-$(cluster)-$(process).out")
         cipPuff_job.add_condor_cmd('request_disk',opts.general_request_disk)
         if opts.use_full_submit_paths:
             fname = opts.working_directory+"/"+cipPuff_job.get_sub_file()
             cipPuff_job.set_sub_file(fname)
         cipPuff_job.write_sub_file()
         cip_puff_job_list.append(cipPuff_job)
 
@@ -327,15 +327,15 @@
 ##   CON job 2 : join multiple events together into a single overall result
 #  - joins together all data files from a single run
 #  - matches duplicates, averaging likelihoods
 #  - if multiple events present, works fine,but will AVERAGE and not ADD, so not as significant as needed. Change?
 #  - skip for now, just have one event at firsty ==>? SONOT QUTE CORRECT because likelihoods are averaged, which reduces net significance.  FIXME: two-stage process
 with open("con_prod.sh",'w') as f:
     f.write("""#! /bin/bash
-{} --combination sum {}/iteration_$1_marg/consolidated_*_*.net_marg  > {}/consolidated_$1.net_marg
+{} --combination product {}/iteration_$1_marg/consolidated_*_*.net_marg  > {}/consolidated_$1.net_marg
 """.format(dag_utils.which('util_HyperCombine.py'),opts.working_directory,opts.working_directory) )
     os.system("chmod a+x con_prod.sh")
 
 con_prod_job, con_prod_job_name = dag_utils.write_convert_sub(exe=opts.working_directory+"/con_prod.sh",tag='CON_PROD',log_dir=None,arg_str='',file_input="$(macroiteration)  ",file_output="/dev/null", out_dir=opts.working_directory,universe=local_worker_universe,no_grid=no_worker_grid)
 con_prod_job.add_condor_cmd("initialdir",opts.working_directory)
 con_prod_job.set_log_file(opts.working_directory+"/iteration_$(macroiteration)_con/logs/con-$(macroevent).log")
 con_prod_job.set_stderr_file(opts.working_directory+"/iteration_$(macroiteration)_con/logs/con-$(macroevent).err")
@@ -404,15 +404,15 @@
     join_post_job.add_condor_cmd("+DESIRED_SITES",'"nogrid"')
     join_post_job.add_condor_cmd("+flock_local",'true')
 
 
 # PUFF job
 #   ... pending
 if puff_args and puff_cadence:
-    puff_job, puff_job_name = dag_utils.write_puff_sub(tag='PUFF',log_dir=None,arg_str=puff_args,request_memory=opts.request_memory_marg,input_net=opts.working_directory+'/grid-$(macroiterationnext).dat',output=opts.working_directory+'/puffball-$(macroiterationnext).dat',out_dir=opts.working_directory,exe=opts.puff_exe,universe=local_worker_universe,no_grid=no_worker_grid)
+    puff_job, puff_job_name = dag_utils.write_puff_sub(tag='PUFF',log_dir=None,arg_str=puff_args,request_memory=opts.request_memory_marg,input_net=opts.working_directory+'/grid-$(macroiterationnext).dat',output=opts.working_directory+'/grid_puff-$(macroiterationnext).dat',out_dir=opts.working_directory,exe=opts.puff_exe,universe=local_worker_universe,no_grid=no_worker_grid)
     # Modify: set 'initialdir' to CIP WORKING DIR 
     puff_job.add_condor_cmd("initialdir",opts.working_directory+"/iteration_$(macroiteration)_post")
     # Modify output argument: change logs and working directory to be subdirectory for the run
     puff_job.set_log_file(opts.working_directory+"/iteration_$(macroiteration)_post/logs/puff-$(cluster)-$(process).log")
     puff_job.set_stderr_file(opts.working_directory+"/iteration_$(macroiteration)_post/logs/puff-$(cluster)-$(process).err")
     puff_job.set_stdout_file(opts.working_directory+"/iteration_$(macroiteration)_post/logs/puff-$(cluster)-$(process).out")
     puff_job.add_condor_cmd('request_disk',opts.general_request_disk)
```

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/create_event_dag_via_grid` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/create_event_dag_via_grid`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_AlternateIteration` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_AlternateIteration`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_BasicIteration` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_BasicIteration`

 * *Files 0% similar despite different names*

```diff
@@ -265,14 +265,16 @@
 local_worker_universe="vanilla"
 no_worker_grid=False
 if opts.condor_local_nonworker:
     local_worker_universe="local"
 if opts.condor_nogrid_nonworker:
     no_worker_grid=True
 
+if not opts.cip_explode_jobs_last:  # set realistic default, if not specified
+    opts.cip_explode_jobs_last = opts.cip_explode_jobs
 
 working_dir_inside_local = working_dir_inside = opts.working_directory
 working_dir_inside_cip = working_dir_inside_local
 out_dir_inside_cip = working_dir_inside_local
 if opts.cip_explode_jobs:
     out_dir_inside_cip+= "/iteration_$(macroiteration)_cip/"
 os.chdir(opts.working_directory)
@@ -952,15 +954,15 @@
            if opts.cip_explode_jobs_dag:
                 n_explode=1
                 fname_out = 'overlap-grid-$(macroiterationnext)-$(cluster)'
            cip_args_extra = cip_args_extra.replace('fit-save-gp','fit-load-gp')
            cip_args_extra = cip_args_extra.replace('my_fit','my_fit.pkl')
            # if the last set of workers, we are making extrinsic samples, so change the output samples  
            if indx == len(cip_args_lines) -1 and opts.last_iteration_extrinsic: # on last iteration, doing extrinsic phase
-               n_samples_per_job = int(opts.last_iteration_extrinsic_nsamples/(1.0*opts.cip_explode_jobs))
+               n_samples_per_job = int(opts.last_iteration_extrinsic_nsamples/(1.0*opts.cip_explode_jobs_last))
                cip_args_extra +=" --n-eff {} --n-output-samples {} ".format(n_samples_per_job,n_samples_per_job)
            transfer_files_cip=['../all.net']
            if opts.use_osg_cip and 'fit-method gp' in cip_args_base:
                transfer_files_cip += ['my_fit.pkl']  # transfer current working directory fit
            cip_job_worker, cip_job_worker_name = dag_utils.write_CIP_sub(tag='CIP_worker'+str(indx),log_dir=None,arg_str=cip_args_lines[indx]+cip_args_extra,request_memory=opts.request_memory_CIP,input_net=working_dir_inside_cip+'/all.net',output=fname_out,out_dir=out_dir_inside_cip,exe=cip_exe_here,ncopies=n_explode,universe=local_worker_universe,no_grid=cip_no_grid,use_osg=opts.use_osg_cip,use_singularity=opts.use_osg_cip and opts.use_singularity,singularity_image=singularity_image,use_simple_osg_requirements=opts.use_osg_cip,transfer_files=transfer_files_cip)
            # Modify: set 'initialdir'
            cip_job_worker.add_condor_cmd("initialdir",opts.working_directory+"/iteration_$(macroiteration)_cip")
```

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_BasicMultiApproxIteration` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_BasicMultiApproxIteration`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/create_ile_sub_dag.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/create_ile_sub_dag.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/create_postprocessing_event_dag.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/create_postprocessing_event_dag.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/helper_LDG_Events.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/helper_LDG_Events.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/helper_OnlinePSDCleanup.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/helper_OnlinePSDCleanup.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/ile_postproc_add_time` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/ile_postproc_add_time`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic_batchmode` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic_batchmode`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic_no-op` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic_no-op`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/make_uni_comov_skymap.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/make_uni_comov_skymap.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/plot_posterior_corner.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/plot_posterior_corner.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 import RIFT.lalsimutils as lalsimutils
 import RIFT.misc.samples_utils as samples_utils
 from RIFT.misc.samples_utils import add_field, extract_combination_from_LI, standard_expand_samples
 import lal
 import numpy as np
 import argparse
+import numpy.lib.recfunctions as rfn
 
 eos_param_names = ['logp1', 'gamma1','gamma2', 'gamma3', 'R1_km', 'R2_km']
 
 
 try:
     import matplotlib
     print(" Matplotlib backend ", matplotlib.get_backend())
@@ -473,14 +474,15 @@
  print(opts.composite_file)
  for fname in opts.composite_file[:1]:  # Only load the first one!
     print(" Loading ... ", fname)
     if not(opts.composite_file_has_labels):
         samples = np.loadtxt(fname,dtype=composite_dtype)  # Names are not always available
     else:
         samples = np.genfromtxt(fname,names=True)
+        samples = rfn.rename_fields(samples, {'sigmalnL': 'sigmaOverL', 'sigma_lnL': 'sigmaOverL'})   # standardize names, some drift in labels
     samples = samples[ ~np.isnan(samples["lnL"])] # remove nan likelihoods -- they can creep in with poor settings/overflows
     name_ref = samples.dtype.names[0]
     if opts.sigma_cut >0:
         npts = len(samples[name_ref])
         # strip NAN
         sigma_vals = samples["sigmaOverL"]
         good_sigma = sigma_vals < opts.sigma_cut
```

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/resample_uniform_comoving.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/resample_uniform_comoving.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_AMRGrid.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_AMRGrid.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_AdaptiveExponent.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_AdaptiveExponent.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_AnalyticFisherGrid.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_AnalyticFisherGrid.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_BatchConvertResampleILEOutput.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_BatchConvertResampleILEOutput.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_CIPdagPostprocess.sh` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_CIPdagPostprocess.sh`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_CharacterizePosterior.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_CharacterizePosterior.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_CleanILE.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_CleanILE.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_CoincIFOUtility.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_CoincIFOUtility.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_CompareWaveformsInDetectors.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_CompareWaveformsInDetectors.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_ConsolidateDAGsUnderMaster.sh` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_ConsolidateDAGsUnderMaster.sh`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_ConstructBNSMarginalEOSRank.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_ConstructBNSMarginalEOSRank.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_ConstructEOSPosterior.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_ConstructEOSPosterior.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_ConstructIntrinsicPosterior_GaussianResampling.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_ConstructIntrinsicPosterior_GaussianResampling.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_ConstructIntrinsicPosterior_GenericCoordinates.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_ConstructIntrinsicPosterior_GenericCoordinates.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,14 +220,15 @@
 parser.add_argument("--fname",help="filename of *.dat file [standard ILE output]")
 parser.add_argument("--input-tides",action='store_true',help="Use input format with tidal fields included.")
 parser.add_argument("--input-eos-index",action='store_true',help="Use input format with eos index fields included")
 parser.add_argument("--input-distance",action='store_true',help="Use input format with distance fields (but not tidal fields?) enabled.")
 parser.add_argument("--fname-lalinference",help="filename of posterior_samples.dat file [standard LI output], to overlay on corner plots")
 parser.add_argument("--fname-output-samples",default="output-ILE-samples",help="output posterior samples (default output-ILE-samples -> output-ILE)")
 parser.add_argument("--fname-output-integral",default="integral_result",help="output filename for integral result. Postfixes appended")
+parser.add_argument("--no-save-samples",action='store_true')
 parser.add_argument("--approx-output",default="SEOBNRv2", help="approximant to use when writing output XML files.")
 parser.add_argument("--amplitude-order",default=-1,type=int,help="Set ampO for grid. Used in PN")
 parser.add_argument("--phase-order",default=7,type=int,help="Set phaseO for grid. Used in PN")
 parser.add_argument("--fref",default=20,type=float, help="Reference frequency used for spins in the ILE output.  (Since I usually use SEOBNRv3, the best choice is 20Hz)")
 parser.add_argument("--fmin",type=float,default=20)
 parser.add_argument("--fname-rom-samples",default=None,help="*.rom_composite output. Treated identically to set of posterior samples produced by mcsampler after constructing fit.")
 parser.add_argument("--n-output-samples",default=3000,type=int,help="output posterior samples (default 3000)")
@@ -576,14 +577,17 @@
     dlist = []
     dlist_ranges = []
 if len(dlist) != len(dlist_ranges):
     print(" downselect parameters inconsistent", dlist, dlist_ranges)
 for indx in np.arange(len(dlist_ranges)):
     downselect_dict[dlist[indx]] = dlist_ranges[indx]
 
+# If using an EOS, reject samples that are out of range for that EOS (remember, we interpolate!)
+if my_eos:
+    print(" WARNING: output not enforcing masses consistent with EOS maximum mass! Returning nearly zero tides in this case, but will run. ")
 
 chi_max = opts.chi_max
 chi_small_max = chi_max
 if not opts.chi_small_max is None:
     chi_small_max = opts.chi_small_max
 lambda_max=opts.lambda_max
 lambda_small_max  = lambda_max
@@ -2511,14 +2515,17 @@
 #     annotation_header = "lnL sigmaL neff n_ESS "
 #     str_out =list( map(str,[np.log(res), np.sqrt(var)/res, neff, n_ESS]))
 #     file_out.write("# " + annotation_header + "\n")
 #     file_out.write(' '.join( str_out +  ["\n"]))
 #np.savetxt(opts.fname_output_integral+"+annotation.dat", np.array([[np.log(res), np.sqrt(var)/res, neff]]), header=eos_extra)
 
 
+if opts.no_save_samples:
+    sys.exit(0)
+
 if neff < len(low_level_coord_names):
     print(" PLOTS WILL FAIL ")
     print(" Not enough independent Monte Carlo points to generate useful contours")
```

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_CoordinateNamesAngularToCartesianSpins.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_CoordinateNamesAngularToCartesianSpins.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_EOBTideWriteFrame.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_EOBTideWriteFrame.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_FetchExternalGrid.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_FetchExternalGrid.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_FitAndEvaluate_GenericCoordinates.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_FitAndEvaluate_GenericCoordinates.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_ForOSG_MakeTruncatedLocalFramesDir.sh` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_ForOSG_MakeTruncatedLocalFramesDir.sh`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_FrameZeroNoiseSNR.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_FrameZeroNoiseSNR.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_GenerateMaxlnLWaveform.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_GenerateMaxlnLWaveform.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_GenerateMaxlnLWaveform_NRFromIndex.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_GenerateMaxlnLWaveform_NRFromIndex.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_GridRecenter.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_GridRecenter.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_GridSubsetOfTemplateBank.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_GridSubsetOfTemplateBank.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_HyperCombine.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_HyperCombine.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,17 +19,22 @@
 
 my_digits=7  # safety for high-SNR BNS
 
 
 import argparse
 parser = argparse.ArgumentParser(usage="util_CleanILE.py fname1.dat fname2.dat ... ")
 parser.add_argument("fname",action='append',nargs='+')
-parser.add_argument("--combination",default='average',help='average|sum, depends on if we treat them as independent trials of the same quantity or independent')
+parser.add_argument("--combination",default='average',help='average|sum|product, depends on if we treat them as independent trials of the same quantity or independent')
 opts = parser.parse_args()
 
+n_terms = 0
+enforce_length=False
+if opts.combination != 'average':
+    enforce_length=True
+
 #print opts.fname
 from pathlib import Path
 for fname in opts.fname[0]: #sys.argv[1:]:
     fname  = Path(fname).resolve()
     if not( os.path.exists(fname)):  # skip symbolic links that don't resolve : important for .composite files
         continue
     if os.stat(fname).st_size==0:  # skip files of zero length
@@ -44,32 +49,41 @@
         line = np.around(line, decimals=my_digits)
         if tuple(line[2:]) in data_at_intrinsic:
 #            print " repeated occurrence ", line[1:9]
             data_at_intrinsic[tuple(line[2:])].append(line[:2])
         else:
 #            print " new key ", line[1:9]
             data_at_intrinsic[tuple(line[2:])] = [line[:2]]
+        n_terms = np.max([n_terms, data_at_intrinsic[tuple(line[2:])] ])
       except:
           continue
 
 header_str=''
 with open(opts.fname[0][0],'r') as f:
     header_str = f.readline()
     header_str = header_str.rstrip()
 
 if header_str.startswith('#'):
     print(header_str)  # repeat the header, so we recapture al the syntax
 for key in data_at_intrinsic:
+    if enforce_length:
+        if len(data_at_intrinsic[key]) < n_terms:
+            print(" Incomplete data for {} ".format(key),file=sys.stderr)
     lnL, sigmaOverL =   np.transpose(data_at_intrinsic[key])
     lnLmax = np.max(lnL)
-    sigma = sigmaOverL*np.exp(lnL-lnLmax)  # remove overall Lmax factor, which factors out from the weights constructed from \sigma
-
-    # This is an average, treating them as independent measurements
-    wts = weight_simulations.AverageSimulationWeights(None, None,sigma)   
-    lnLmeanMinusLmax = scipy.special.logsumexp((lnL - lnLmax)*wts)
-    sigmaNetOverL = (np.sqrt(1./np.sum(1./sigma/sigma)))/np.exp(lnLmeanMinusLmax)
-
-    if opts.combination =='sum':
-        lnLmeanMinusLmax *= len(wts)   # not an average !
-        sigmaNetOverL *= np.sqrt(len(wts))
+    if opts.combination =='product':
+        lnLnet = np.sum(lnL)
+        sigma = np.sqrt(np.sum(sigmaOverL**2))
+        print(" {} {} ".format(lnLnet, sigma) + ' '.join(map(str,key)) )
+    else:
+        sigma = sigmaOverL*np.exp(lnL-lnLmax)  # remove overall Lmax factor, which factors out from the weights constructed from \sigma
+
+        # This is an average, treating them as independent measurements
+        wts = weight_simulations.AverageSimulationWeights(None, None,sigma)   
+        lnLmeanMinusLmax = scipy.special.logsumexp((lnL - lnLmax)*wts)
+        sigmaNetOverL = (np.sqrt(1./np.sum(1./sigma/sigma)))/np.exp(lnLmeanMinusLmax)
+
+        if opts.combination =='sum':
+            lnLmeanMinusLmax *= len(wts)   # not an average !
+            sigmaNetOverL *= np.sqrt(len(wts))
                               
-    print(" {} {} ".format(lnLmeanMinusLmax+lnLmax, sigmaNetOverL) + ' '.join(map(str,key)) )
+        print(" {} {} ".format(lnLmeanMinusLmax+lnLmax, sigmaNetOverL) + ' '.join(map(str,key)) )
```

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_HyperparameterGrid.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_HyperparameterGrid.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_HyperparameterPuffball.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_HyperparameterPuffball.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_ILENextGeneration.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_ILENextGeneration.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_ILEROMdagPostprocess.sh` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_ILEROMdagPostprocess.sh`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_ILEdagPostprocess.sh` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_ILEdagPostprocess.sh`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_InitMargTable` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_InitMargTable`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_IntermediateEOSIntegralFromFit.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_IntermediateEOSIntegralFromFit.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_IterativeFisher.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_IterativeFisher.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_JoinXML.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_JoinXML.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_LALCompareApproximantsOnSamples.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_LALCompareApproximantsOnSamples.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_LALWriteFrame.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_LALWriteFrame.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_ManualOverlapGrid.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_ManualOverlapGrid.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_MarginalizedLikelihoodEOSIntegralFromIntermediate.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_MarginalizedLikelihoodEOSIntegralFromIntermediate.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_MassGrid.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_MassGrid.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_MassGridCoalesce.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_MassGridCoalesce.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_NRBestOfIndex.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_NRBestOfIndex.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_NRDumpDetectorResponse.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_NRDumpDetectorResponse.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_NRExtrudeOverlapGrid.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_NRExtrudeOverlapGrid.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_NRIndexedFminCutToILE.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_NRIndexedFminCutToILE.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_NRNearestSimulationTo.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_NRNearestSimulationTo.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_NRRelabelILE.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_NRRelabelILE.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_NRWriteFrame.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_NRWriteFrame.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_NR_GWMemory.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_NR_GWMemory.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_NRdagPostprocess.sh` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_NRdagPostprocess.sh`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_ParameterFilter.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_ParameterFilter.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_ParameterPuffball.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_ParameterPuffball.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_ParameterRandomize.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_ParameterRandomize.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_PosteriorPostprocess.sh` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_PosteriorPostprocess.sh`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_PrintInjection.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_PrintInjection.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_RIFT_MultiMetaPipe.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_RIFT_MultiMetaPipe.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_RIFT_pseudo_pipe.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_RIFT_pseudo_pipe.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_RIFT_pseudo_pipe_lowlatency.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_RIFT_pseudo_pipe_lowlatency.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_ROMWriteFrame.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_ROMWriteFrame.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_RandomizeOverlapOrder.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_RandomizeOverlapOrder.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_ResampleILEOutputWithExtrinsic.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_ResampleILEOutputWithExtrinsic.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_SimInspiralToCoinc.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_SimInspiralToCoinc.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_TEOBResumSWriteFrame.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_TEOBResumSWriteFrame.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_TestSpokesIO.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_TestSpokesIO.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_TestXMLParameterStorage.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_TestXMLParameterStorage.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_TidalPlotSimulationStrain.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_TidalPlotSimulationStrain.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_WriteFrameAndCacheFromXML.sh` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_WriteFrameAndCacheFromXML.sh`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_WriteInjectionFile.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_WriteInjectionFile.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/MonteCarloMarginalizeCode/Code/bin/util_WriteXMLWithEOS.py` & `RIFT-0.0.15.9rc6/MonteCarloMarginalizeCode/Code/bin/util_WriteXMLWithEOS.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/PACKAGING.md` & `RIFT-0.0.15.9rc6/PACKAGING.md`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/PKG-INFO` & `RIFT-0.0.15.9rc6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RIFT
-Version: 0.0.15.9rc5
+Version: 0.0.15.9rc6
 Summary: RIFT parameter estimation pipeline. Note branch used is temp-RIT-Tides-port_python3_restructure_package (which will become master shortly)!
 Home-page: https://git.ligo.org/rapidpe-rift/rift
 Author: Richard O'Shaughnessy
 Author-email: richard.oshaughnessy@ligo.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `RIFT-0.0.15.9rc5/README.md` & `RIFT-0.0.15.9rc6/README.md`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/TROUBLESHOOTING.md` & `RIFT-0.0.15.9rc6/TROUBLESHOOTING.md`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/howto.md` & `RIFT-0.0.15.9rc6/howto.md`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.9rc5/setup.py` & `RIFT-0.0.15.9rc6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 #  - ourio.py, ourparams.py
 #  - anything with 'test'
 #print " Identified scripts ", my_scripts\
 #print setuptools.find_packages('MonteCarloMarginalizeCode/Code')
 
 setuptools.setup(
     name="RIFT",
-    version="0.0.15.9rc5", # do not build on OSX machine, side effects
+    version="0.0.15.9rc6", # do not build on OSX machine, side effects
     author="Richard O'Shaughnessy",
     author_email="richard.oshaughnessy@ligo.org",
     description="RIFT parameter estimation pipeline. Note branch used is temp-RIT-Tides-port_python3_restructure_package (which will become master shortly)!",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://git.ligo.org/rapidpe-rift/rift",
     package_dir = {'':'MonteCarloMarginalizeCode/Code'},
```

