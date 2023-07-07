# Comparing `tmp/f3dasm-1.1.0.tar.gz` & `tmp/f3dasm-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "f3dasm-1.1.0.tar", last modified: Thu Jun 29 14:38:01 2023, max compression
+gzip compressed data, was "f3dasm-1.2.0.tar", last modified: Fri Jul  7 13:46:35 2023, max compression
```

## Comparing `f3dasm-1.1.0.tar` & `f3dasm-1.2.0.tar`

### file list

```diff
@@ -1,124 +1,69 @@
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-29 14:38:01.818372 f3dasm-1.1.0/
--rw-rw-r--   0 martin    (1000) martin    (1000)     1531 2023-03-30 12:29:51.000000 f3dasm-1.1.0/LICENSE
--rw-rw-r--   0 martin    (1000) martin    (1000)      164 2023-03-31 07:42:30.000000 f3dasm-1.1.0/MANIFEST.in
--rw-rw-r--   0 martin    (1000) martin    (1000)     3573 2023-06-29 14:38:01.818372 f3dasm-1.1.0/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)     2193 2023-04-17 07:39:19.000000 f3dasm-1.1.0/README.md
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-29 14:38:01.802372 f3dasm-1.1.0/docs/
--rw-rw-r--   0 martin    (1000) martin    (1000)       69 2023-03-31 08:16:15.000000 f3dasm-1.1.0/docs/requirements.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)      457 2023-03-31 07:42:30.000000 f3dasm-1.1.0/pyproject.toml
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-29 14:38:01.802372 f3dasm-1.1.0/requirements/
--rw-rw-r--   0 martin    (1000) martin    (1000)       18 2023-03-31 07:42:30.000000 f3dasm-1.1.0/requirements/machinelearning.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       78 2023-03-31 11:13:42.000000 f3dasm-1.1.0/requirements/optimization.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        5 2023-03-31 07:42:30.000000 f3dasm-1.1.0/requirements/sampling.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       64 2023-03-31 13:03:34.000000 f3dasm-1.1.0/requirements.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       38 2023-06-29 14:38:01.818372 f3dasm-1.1.0/setup.cfg
--rw-rw-r--   0 martin    (1000) martin    (1000)     3053 2023-06-29 14:36:32.000000 f3dasm-1.1.0/setup.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-29 14:38:01.802372 f3dasm-1.1.0/src/
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-29 14:38:01.806372 f3dasm-1.1.0/src/f3dasm/
--rw-rw-r--   0 martin    (1000) martin    (1000)        5 2023-04-03 08:58:46.000000 f3dasm-1.1.0/src/f3dasm/VERSION
--rw-rw-r--   0 martin    (1000) martin    (1000)     1723 2023-06-29 14:36:32.000000 f3dasm-1.1.0/src/f3dasm/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     5469 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/_imports.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     4886 2023-06-29 14:36:32.000000 f3dasm-1.1.0/src/f3dasm/_logging.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     3982 2023-06-29 14:36:32.000000 f3dasm-1.1.0/src/f3dasm/_show_versions.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-29 14:38:01.806372 f3dasm-1.1.0/src/f3dasm/data/
--rw-rw-r--   0 martin    (1000) martin    (1000)      153 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/data/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2693 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/data/benchmarkfunction_data.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      923 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/data/learningdata.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1790 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/data/linearregression_data.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-29 14:38:01.806372 f3dasm-1.1.0/src/f3dasm/design/
--rw-rw-r--   0 martin    (1000) martin    (1000)      885 2023-06-29 14:36:32.000000 f3dasm-1.1.0/src/f3dasm/design/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     6902 2023-06-29 14:36:32.000000 f3dasm-1.1.0/src/f3dasm/design/_data.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     4863 2023-06-29 14:36:32.000000 f3dasm-1.1.0/src/f3dasm/design/_jobqueue.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    15181 2023-06-29 14:36:32.000000 f3dasm-1.1.0/src/f3dasm/design/design.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    17309 2023-06-29 14:36:32.000000 f3dasm-1.1.0/src/f3dasm/design/experimentdata.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     5609 2023-06-29 14:36:32.000000 f3dasm-1.1.0/src/f3dasm/design/parameter.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-29 14:38:01.806372 f3dasm-1.1.0/src/f3dasm/experiment/
--rw-rw-r--   0 martin    (1000) martin    (1000)      760 2023-06-29 14:36:32.000000 f3dasm-1.1.0/src/f3dasm/experiment/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     4244 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/experiment/filehandler.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2900 2023-06-05 12:02:43.000000 f3dasm-1.1.0/src/f3dasm/experiment/logging.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     6117 2023-06-29 14:36:32.000000 f3dasm-1.1.0/src/f3dasm/experiment/parallelization.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      730 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/experiment/quickstart.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-29 14:38:01.806372 f3dasm-1.1.0/src/f3dasm/functions/
--rw-rw-r--   0 martin    (1000) martin    (1000)     3507 2023-03-31 08:39:55.000000 f3dasm-1.1.0/src/f3dasm/functions/__init__.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-29 14:38:01.810372 f3dasm-1.1.0/src/f3dasm/functions/adapters/
--rw-rw-r--   0 martin    (1000) martin    (1000)        0 2022-11-03 14:34:52.000000 f3dasm-1.1.0/src/f3dasm/functions/adapters/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     7314 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/functions/adapters/augmentor.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     4503 2023-06-29 14:36:32.000000 f3dasm-1.1.0/src/f3dasm/functions/adapters/pybenchfunction.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    10469 2023-06-29 14:36:32.000000 f3dasm-1.1.0/src/f3dasm/functions/function.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    81430 2023-06-29 14:36:32.000000 f3dasm-1.1.0/src/f3dasm/functions/pybenchfunction.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-29 14:38:01.810372 f3dasm-1.1.0/src/f3dasm/machinelearning/
--rw-rw-r--   0 martin    (1000) martin    (1000)     1760 2023-06-29 14:36:32.000000 f3dasm-1.1.0/src/f3dasm/machinelearning/__init__.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-29 14:38:01.810372 f3dasm-1.1.0/src/f3dasm/machinelearning/adapters/
--rw-rw-r--   0 martin    (1000) martin    (1000)        0 2023-03-10 12:07:18.000000 f3dasm-1.1.0/src/f3dasm/machinelearning/adapters/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     3073 2023-06-29 14:36:32.000000 f3dasm-1.1.0/src/f3dasm/machinelearning/adapters/tensorflow_implementations.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1036 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/machinelearning/all_models.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     4946 2023-05-26 13:48:37.000000 f3dasm-1.1.0/src/f3dasm/machinelearning/evaluator.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1523 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/machinelearning/linear_regression.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1039 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/machinelearning/loss_functions.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1593 2023-06-29 14:36:32.000000 f3dasm-1.1.0/src/f3dasm/machinelearning/mnist_classifier.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1280 2023-04-12 15:38:50.000000 f3dasm-1.1.0/src/f3dasm/machinelearning/model.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2475 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/machinelearning/passthrough_model.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1924 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/machinelearning/utils.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-29 14:38:01.814372 f3dasm-1.1.0/src/f3dasm/optimization/
--rw-rw-r--   0 martin    (1000) martin    (1000)     3704 2023-04-19 11:31:27.000000 f3dasm-1.1.0/src/f3dasm/optimization/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1296 2023-04-12 07:58:51.000000 f3dasm-1.1.0/src/f3dasm/optimization/_protocol.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1756 2023-04-04 11:19:13.000000 f3dasm-1.1.0/src/f3dasm/optimization/adam.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1675 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/optimization/adamax.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-29 14:38:01.814372 f3dasm-1.1.0/src/f3dasm/optimization/adapters/
--rw-rw-r--   0 martin    (1000) martin    (1000)        0 2022-11-03 14:34:52.000000 f3dasm-1.1.0/src/f3dasm/optimization/adapters/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     4745 2023-06-29 14:36:32.000000 f3dasm-1.1.0/src/f3dasm/optimization/adapters/pygmo_implementations.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     3404 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/optimization/adapters/scipy_implementations.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     4111 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/optimization/adapters/tensorflow_implementations.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2736 2023-06-29 14:36:32.000000 f3dasm-1.1.0/src/f3dasm/optimization/all_optimizers.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     3605 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/optimization/bayesianoptimization.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1131 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/optimization/cg.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1588 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/optimization/cmaes.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1377 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/optimization/cobyla.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2219 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/optimization/differentialevolution.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2108 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/optimization/ftrl.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1204 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/optimization/lbfgsb.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1664 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/optimization/nadam.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1267 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/optimization/neldermead.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     8420 2023-06-29 14:36:32.000000 f3dasm-1.1.0/src/f3dasm/optimization/optimizer.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1679 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/optimization/pso.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1666 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/optimization/randomsearch.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1707 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/optimization/rmsprop.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1832 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/optimization/sade.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1488 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/optimization/sea.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2035 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/optimization/sga.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1570 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/optimization/sgd.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1973 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/optimization/simulatedannealing.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2170 2023-04-14 09:00:21.000000 f3dasm-1.1.0/src/f3dasm/optimization/utils.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1968 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/optimization/xnes.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     7356 2023-06-29 14:36:32.000000 f3dasm-1.1.0/src/f3dasm/run_optimization.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-29 14:38:01.814372 f3dasm-1.1.0/src/f3dasm/sampling/
--rw-rw-r--   0 martin    (1000) martin    (1000)     1685 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/sampling/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1086 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/sampling/all_samplers.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1752 2023-06-29 14:36:32.000000 f3dasm-1.1.0/src/f3dasm/sampling/latinhypercube.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1307 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/sampling/randomuniform.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     6529 2023-06-29 14:36:32.000000 f3dasm-1.1.0/src/f3dasm/sampling/sampler.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1668 2023-06-23 13:36:28.000000 f3dasm-1.1.0/src/f3dasm/sampling/sobolsequence.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1826 2023-04-14 08:29:08.000000 f3dasm-1.1.0/src/f3dasm/sampling/utils.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-29 14:38:01.814372 f3dasm-1.1.0/src/f3dasm/simulation/
--rw-rw-r--   0 martin    (1000) martin    (1000)      142 2023-06-29 14:36:32.000000 f3dasm-1.1.0/src/f3dasm/simulation/__init__.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-29 14:38:01.814372 f3dasm-1.1.0/src/f3dasm/simulation/abaqus_script/
--rw-rw-r--   0 martin    (1000) martin    (1000)       63 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/simulation/abaqus_script/__init__.py
--rwxrwxr-x   0 martin    (1000) martin    (1000)    32487 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/simulation/abaqus_script/flower_rve_script.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    11667 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/simulation/abaqus_simulator.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     4520 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/simulation/abaqus_utils.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-29 14:38:01.814372 f3dasm-1.1.0/src/f3dasm/simulation/cases/
--rw-rw-r--   0 martin    (1000) martin    (1000)       34 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/simulation/cases/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     5736 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/simulation/cases/flower_rve.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1306 2023-06-29 14:36:32.000000 f3dasm-1.1.0/src/f3dasm/simulation/simulator.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1266 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/utils.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-29 14:38:01.806372 f3dasm-1.1.0/src/f3dasm.egg-info/
--rw-rw-r--   0 martin    (1000) martin    (1000)     3573 2023-06-29 14:38:01.000000 f3dasm-1.1.0/src/f3dasm.egg-info/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)     3528 2023-06-29 14:38:01.000000 f3dasm-1.1.0/src/f3dasm.egg-info/SOURCES.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-06-29 14:38:01.000000 f3dasm-1.1.0/src/f3dasm.egg-info/dependency_links.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)      532 2023-06-29 14:38:01.000000 f3dasm-1.1.0/src/f3dasm.egg-info/requires.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        7 2023-06-29 14:38:01.000000 f3dasm-1.1.0/src/f3dasm.egg-info/top_level.txt
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-29 14:38:01.814372 f3dasm-1.1.0/tests/
--rw-rw-r--   0 martin    (1000) martin    (1000)        0 2022-08-17 09:47:40.000000 f3dasm-1.1.0/tests/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      141 2022-08-31 10:13:29.000000 f3dasm-1.1.0/tests/__init__.pyc
--rw-rw-r--   0 martin    (1000) martin    (1000)      855 2023-03-31 07:42:30.000000 f3dasm-1.1.0/tests/conftest.py
--rw-rw-r--   0 martin    (1000) martin    (1000)       29 2023-03-10 12:07:18.000000 f3dasm-1.1.0/tests/requirements.txt
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-07 13:46:35.459373 f3dasm-1.2.0/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1531 2023-03-30 12:29:51.000000 f3dasm-1.2.0/LICENSE
+-rw-rw-r--   0 martin    (1000) martin    (1000)       74 2023-07-07 13:46:05.000000 f3dasm-1.2.0/MANIFEST.in
+-rw-rw-r--   0 martin    (1000) martin    (1000)     3492 2023-07-07 13:46:35.459373 f3dasm-1.2.0/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2189 2023-07-07 13:46:05.000000 f3dasm-1.2.0/README.md
+-rw-rw-r--   0 martin    (1000) martin    (1000)        5 2023-07-07 13:46:05.000000 f3dasm-1.2.0/VERSION
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-07 13:46:35.447373 f3dasm-1.2.0/docs/
+-rw-rw-r--   0 martin    (1000) martin    (1000)       69 2023-03-31 08:16:15.000000 f3dasm-1.2.0/docs/requirements.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)      457 2023-03-31 07:42:30.000000 f3dasm-1.2.0/pyproject.toml
+-rw-rw-r--   0 martin    (1000) martin    (1000)       70 2023-07-07 13:46:05.000000 f3dasm-1.2.0/requirements.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1374 2023-07-07 13:46:35.459373 f3dasm-1.2.0/setup.cfg
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-07 13:46:35.447373 f3dasm-1.2.0/src/
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-07 13:46:35.451373 f3dasm-1.2.0/src/f3dasm/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2283 2023-07-07 13:46:05.000000 f3dasm-1.2.0/src/f3dasm/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     4261 2023-07-07 13:46:05.000000 f3dasm-1.2.0/src/f3dasm/_imports.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1239 2023-07-07 13:46:05.000000 f3dasm-1.2.0/src/f3dasm/argparser.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-07 13:46:35.451373 f3dasm-1.2.0/src/f3dasm/datageneration/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1441 2023-07-07 13:46:05.000000 f3dasm-1.2.0/src/f3dasm/datageneration/__init__.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-07 13:46:35.451373 f3dasm-1.2.0/src/f3dasm/datageneration/abaqus/
+-rw-rw-r--   0 martin    (1000) martin    (1000)        0 2023-07-07 13:46:05.000000 f3dasm-1.2.0/src/f3dasm/datageneration/abaqus/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1444 2023-07-07 13:46:05.000000 f3dasm-1.2.0/src/f3dasm/datageneration/datagenerator.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-07 13:46:35.451373 f3dasm-1.2.0/src/f3dasm/datageneration/functions/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     3545 2023-07-07 13:46:05.000000 f3dasm-1.2.0/src/f3dasm/datageneration/functions/__init__.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-07 13:46:35.451373 f3dasm-1.2.0/src/f3dasm/datageneration/functions/adapters/
+-rw-rw-r--   0 martin    (1000) martin    (1000)        0 2023-07-07 13:46:05.000000 f3dasm-1.2.0/src/f3dasm/datageneration/functions/adapters/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     7378 2023-07-07 13:46:05.000000 f3dasm-1.2.0/src/f3dasm/datageneration/functions/adapters/augmentor.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     4503 2023-07-07 13:46:05.000000 f3dasm-1.2.0/src/f3dasm/datageneration/functions/adapters/pybenchfunction.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    10643 2023-07-07 13:46:05.000000 f3dasm-1.2.0/src/f3dasm/datageneration/functions/function.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    83159 2023-07-07 13:46:05.000000 f3dasm-1.2.0/src/f3dasm/datageneration/functions/pybenchfunction.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-07 13:46:35.455373 f3dasm-1.2.0/src/f3dasm/design/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1143 2023-07-07 13:46:05.000000 f3dasm-1.2.0/src/f3dasm/design/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     4228 2023-07-07 13:46:05.000000 f3dasm-1.2.0/src/f3dasm/design/_access_file.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     7458 2023-07-07 13:46:05.000000 f3dasm-1.2.0/src/f3dasm/design/_data.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     5873 2023-07-07 13:46:05.000000 f3dasm-1.2.0/src/f3dasm/design/_jobqueue.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2526 2023-07-07 13:46:05.000000 f3dasm-1.2.0/src/f3dasm/design/design.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    25259 2023-07-07 13:46:05.000000 f3dasm-1.2.0/src/f3dasm/design/domain.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    18653 2023-07-07 13:46:05.000000 f3dasm-1.2.0/src/f3dasm/design/experimentdata.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     5609 2023-06-29 14:36:32.000000 f3dasm-1.2.0/src/f3dasm/design/parameter.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     3708 2023-07-07 13:46:05.000000 f3dasm-1.2.0/src/f3dasm/logger.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-07 13:46:35.455373 f3dasm-1.2.0/src/f3dasm/machinelearning/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      635 2023-07-07 13:46:05.000000 f3dasm-1.2.0/src/f3dasm/machinelearning/__init__.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-07 13:46:35.455373 f3dasm-1.2.0/src/f3dasm/optimization/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2143 2023-07-07 13:46:05.000000 f3dasm-1.2.0/src/f3dasm/optimization/__init__.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-07 13:46:35.455373 f3dasm-1.2.0/src/f3dasm/optimization/adapters/
+-rw-rw-r--   0 martin    (1000) martin    (1000)        0 2022-11-03 14:34:52.000000 f3dasm-1.2.0/src/f3dasm/optimization/adapters/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     4759 2023-07-07 13:46:05.000000 f3dasm-1.2.0/src/f3dasm/optimization/adapters/scipy_implementations.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1133 2023-07-07 13:46:05.000000 f3dasm-1.2.0/src/f3dasm/optimization/cg.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1206 2023-07-07 13:46:05.000000 f3dasm-1.2.0/src/f3dasm/optimization/lbfgsb.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1269 2023-07-07 13:46:05.000000 f3dasm-1.2.0/src/f3dasm/optimization/neldermead.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     8435 2023-07-07 13:46:05.000000 f3dasm-1.2.0/src/f3dasm/optimization/optimizer.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1682 2023-07-07 13:46:05.000000 f3dasm-1.2.0/src/f3dasm/optimization/randomsearch.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     6431 2023-07-07 13:46:05.000000 f3dasm-1.2.0/src/f3dasm/run_optimization.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-07 13:46:35.459373 f3dasm-1.2.0/src/f3dasm/sampling/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1497 2023-07-07 13:46:05.000000 f3dasm-1.2.0/src/f3dasm/sampling/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1497 2023-07-07 13:46:05.000000 f3dasm-1.2.0/src/f3dasm/sampling/latinhypercube.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1307 2023-03-31 07:42:30.000000 f3dasm-1.2.0/src/f3dasm/sampling/randomuniform.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     6504 2023-07-07 13:46:05.000000 f3dasm-1.2.0/src/f3dasm/sampling/sampler.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1413 2023-07-07 13:46:05.000000 f3dasm-1.2.0/src/f3dasm/sampling/sobolsequence.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-07 13:46:35.451373 f3dasm-1.2.0/src/f3dasm.egg-info/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     3492 2023-07-07 13:46:35.000000 f3dasm-1.2.0/src/f3dasm.egg-info/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1703 2023-07-07 13:46:35.000000 f3dasm-1.2.0/src/f3dasm.egg-info/SOURCES.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-07-07 13:46:35.000000 f3dasm-1.2.0/src/f3dasm.egg-info/dependency_links.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       70 2023-07-07 13:46:35.000000 f3dasm-1.2.0/src/f3dasm.egg-info/requires.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        7 2023-07-07 13:46:35.000000 f3dasm-1.2.0/src/f3dasm.egg-info/top_level.txt
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-07 13:46:35.459373 f3dasm-1.2.0/tests/
+-rw-rw-r--   0 martin    (1000) martin    (1000)        0 2022-08-17 09:47:40.000000 f3dasm-1.2.0/tests/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      141 2022-08-31 10:13:29.000000 f3dasm-1.2.0/tests/__init__.pyc
+-rw-rw-r--   0 martin    (1000) martin    (1000)      855 2023-03-31 07:42:30.000000 f3dasm-1.2.0/tests/conftest.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)       29 2023-03-10 12:07:18.000000 f3dasm-1.2.0/tests/requirements.txt
```

### Comparing `f3dasm-1.1.0/LICENSE` & `f3dasm-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `f3dasm-1.1.0/PKG-INFO` & `f3dasm-1.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: f3dasm
-Version: 1.1.0
+Version: 1.2.0
 Summary: f3dasm - Framework for Data-driven development and Analysis of Structures and Materials
 Home-page: https://github.com/bessagroup/f3dasm
 Author: Martin van der Schelling
 Author-email: M.P.vanderSchelling@tudelft.nl
 License: BSD
 Project-URL: Documentation, https://bessagroup.github.io/f3dasm/
 Project-URL: Wiki, https://github.com/bessagroup/f3dasm/wiki
@@ -12,27 +12,23 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
-Requires-Python: >=3.8, <3.11
+Requires-Python: <3.11,>=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: sampling
-Provides-Extra: machinelearning
-Provides-Extra: optimization
-Provides-Extra: all
-Provides-Extra: dev
 License-File: LICENSE
 
 f3dasm
 ------
 *Framework for data-driven design \& analysis of structures and materials*
 
 ***
@@ -41,15 +37,15 @@
 [![pypi](https://img.shields.io/pypi/v/f3dasm.svg)](https://pypi.org/project/f3dasm/)
 [![GitHub license](https://img.shields.io/badge/license-BSD-blue)](https://github.com/bessagroup/f3dasm)
 
 [**Docs**](https://bessagroup.github.io/f3dasm/)
 | [**Installation**](https://bessagroup.github.io/f3dasm/general/gettingstarted.html)
 | [**GitHub**](https://github.com/bessagroup/f3dasm)
 | [**PyPI**](https://pypi.org/project/f3dasm/)
-| [**Practical sessions**](https://github.com/mpvanderschelling/F3DASM_practical)
+| [**Practical sessions**](https://github.com/mpvanderschelling/f3dasm_teach)
 
 Welcome to `f3dasm`, a Python package for data-driven design and analysis of structures and materials.
 
 * Created by M.A. Bessa (M.A.Bessa@tudelft.nl) in September 2016
 * Current developer and maintainer: [M.P. van der Schelling](https://github.com/mpvanderschelling/) (M.P.vanderSchelling@tudelft.nl)
 
 The Bessa research group at TU Delft is small... At the moment, we have limited availability to help future users/developers adapting the code to new problems, but we will do our best to help!
```

### Comparing `f3dasm-1.1.0/README.md` & `f3dasm-1.2.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 [![pypi](https://img.shields.io/pypi/v/f3dasm.svg)](https://pypi.org/project/f3dasm/)
 [![GitHub license](https://img.shields.io/badge/license-BSD-blue)](https://github.com/bessagroup/f3dasm)
 
 [**Docs**](https://bessagroup.github.io/f3dasm/)
 | [**Installation**](https://bessagroup.github.io/f3dasm/general/gettingstarted.html)
 | [**GitHub**](https://github.com/bessagroup/f3dasm)
 | [**PyPI**](https://pypi.org/project/f3dasm/)
-| [**Practical sessions**](https://github.com/mpvanderschelling/F3DASM_practical)
+| [**Practical sessions**](https://github.com/mpvanderschelling/f3dasm_teach)
 
 Welcome to `f3dasm`, a Python package for data-driven design and analysis of structures and materials.
 
 * Created by M.A. Bessa (M.A.Bessa@tudelft.nl) in September 2016
 * Current developer and maintainer: [M.P. van der Schelling](https://github.com/mpvanderschelling/) (M.P.vanderSchelling@tudelft.nl)
 
 The Bessa research group at TU Delft is small... At the moment, we have limited availability to help future users/developers adapting the code to new problems, but we will do our best to help!
```

### Comparing `f3dasm-1.1.0/src/f3dasm/_imports.py` & `f3dasm-1.2.0/src/f3dasm/_imports.py`

 * *Files 14% similar despite different names*

```diff
@@ -112,37 +112,7 @@
         Extension name for this particular context manager
 
     Returns:
         Deferred import context manager.
 
     """
     return _DeferredImportExceptionContextManager(extension_name=extension_name)
-
-
-class _IntegrationModule(ModuleType):
-    """Module class that implements `optuna.integration` package.
-
-    This class applies lazy import under `optuna.integration`, where submodules are imported
-    when they are actually accessed. Otherwise, `import optuna` becomes much slower because it
-    imports all submodules and their dependencies (e.g., chainer, keras, lightgbm) all at once.
-    """
-
-    def __getattr__(self, name: str) -> Any:
-        self._modules = set(self._import_structure.keys())
-        self._class_to_module = {}
-        for key, values in self._import_structure.items():
-            for value in values:
-                self._class_to_module[value] = key
-
-        if name in self._modules:
-            value = self._get_module(name)
-        elif name in self._class_to_module.keys():
-            module = self._get_module(self._class_to_module[name])
-            value = getattr(module, name)
-        else:
-            raise AttributeError(f"module {self.__name__} has no attribute {name}")
-
-        setattr(self, name, value)
-        return value
-
-    def _get_module(self, module_name: str) -> ModuleType:
-        return importlib.import_module("." + module_name, self.__name__)
```

### Comparing `f3dasm-1.1.0/src/f3dasm/_logging.py` & `f3dasm-1.2.0/src/f3dasm/logger.py`

 * *Files 22% similar despite different names*

```diff
@@ -17,17 +17,14 @@
 else:
     import fcntl
 
 from functools import partial, wraps
 from time import perf_counter
 from typing import Any, Callable
 
-# Local
-from ._show_versions import __version__
-
 #                                                          Authorship & Credits
 # =============================================================================
 __author__ = 'Martin van der Schelling (M.P.vanderSchelling@tudelft.nl)'
 __credits__ = ['Martin van der Schelling']
 __status__ = 'Stable'
 # =============================================================================
 #
@@ -107,58 +104,14 @@
     """
     if os.name == 'nt':  # for Windows
         msvcrt.locking(file.fileno(), msvcrt.LK_UNLCK, 1)
     else:  # for Unix
         fcntl.flock(file, fcntl.LOCK_UN)
 
 
-def create_logger(name: str, level: int = logging.INFO, filename: str = None) -> logging.Logger:
-    """Create a logger
-
-    Parameters
-    ----------
-    name : str
-        Name of the logger
-    level : int, optional
-        Logging level, by default logging.INFO
-    filename : str, optional
-        Filename of the log file, by default None
-
-    Returns
-    -------
-    logging.Logger
-        The created logger
-    """
-
-    # Create a logger
-    logger = logging.getLogger(name)
-
-    # Set the logging level
-    logger.setLevel(level)
-
-    # Create a file handler
-    if filename is None:
-        filename = f"{name}.log"
-
-    # Check if file ends with .log
-    if not filename.endswith(".log"):
-        filename += ".log"
-
-    handler = DistributedFileHandler(filename)
-
-    # Create a logging format
-    formatter = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
-    handler.setFormatter(formatter)
-
-    # Add the handlers to the logger
-    logger.addHandler(handler)
-
-    return logger
-
-
 def _time_and_log(
     func: Callable, logger=logging.Logger
 ) -> Callable:
     @wraps(func)
     def wrapper(*args: Any, **kwargs: Any) -> Any:
         start_time = perf_counter()
         value = func(*args, **kwargs)
@@ -167,10 +120,7 @@
 
     return wrapper
 
 
 # Create a logger
 logger = logging.getLogger("f3dasm")
 time_and_log = partial(_time_and_log, logger=logger)
-
-# Log welcome message and the version of f3dasm
-logger.info(f"Imported f3dasm (version: {__version__})")
```

### Comparing `f3dasm-1.1.0/src/f3dasm/design/_data.py` & `f3dasm-1.2.0/src/f3dasm/design/_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,32 @@
+#                                                                       Modules
+# =============================================================================
 
+# Standard
 import os
 from io import TextIOWrapper
-from typing import Any, Dict, Iterator, List, Tuple
+from typing import Any, Dict, Iterator, List, Tuple, Union
 
+# Third-party
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 
-from .design import DesignSpace
+# Local
+from .domain import Domain
+from .design import Design
+
+#                                                          Authorship & Credits
+# =============================================================================
+__author__ = 'Martin van der Schelling (M.P.vanderSchelling@tudelft.nl)'
+__credits__ = ['Martin van der Schelling']
+__status__ = 'Stable'
+# =============================================================================
+#
+# =============================================================================
 
 
 class _Data:
     def __init__(self, data: pd.DataFrame):
         self.data: pd.DataFrame = data
 
     def __len__(self):
@@ -32,15 +47,15 @@
             self.current_index += 1
             return current_value
 
     def _repr_html_(self) -> str:
         return self.data._repr_html_()
 
     @classmethod
-    def from_design(cls, design: DesignSpace) -> '_Data':
+    def from_design(cls, design: Domain) -> '_Data':
         # input columns
         input_columns = [("input", name) for name, parameter in design.input_space.items()]
 
         df_input = pd.DataFrame(columns=input_columns).astype(
             design._cast_types_dataframe(design.input_space, label="input")
         )
 
@@ -82,15 +97,15 @@
                 filename = filename + '.csv'
             file = filename
         else:
             file = text_io
 
         return cls(pd.read_csv(file, header=[0, 1], index_col=0))
 
-    def reset(self, design: DesignSpace):
+    def reset(self, design: Domain):
         """Resets the data to the initial state.
 
         Parameters
         ----------
         design : DesignSpace
             The design space of the experiment.
         """
@@ -111,28 +126,14 @@
 
         if not filename.endswith('.csv'):
             filename = filename + '.csv'
         # Store the data
 
         self.data.to_csv(filename)
 
-        # if os.name == 'nt':  # Windows
-        #     # Open the data.csv file with a lock
-        #     with open(filename, 'w') as f:
-        #         msvcrt.locking(f.fileno(), msvcrt.LK_LOCK, 1)
-        #         self.data.to_csv(filename)
-        #         msvcrt.locking(f.fileno(), msvcrt.LK_UNLCK, 1)
-
-        # else:  # Unix
-        #     # Open the data.csv file with a lock
-        #     with open(filename, 'w') as f:
-        #         fcntl.flock(f, fcntl.LOCK_EX)
-        #         self.data.to_csv(filename)
-        #         fcntl.flock(f, fcntl.LOCK_UN)
-
     def select(self, indices: List[int]):
         self.data = self.data.loc[indices]
 
     def remove(self, indices: List[int]):
         self.data = self.data.drop(indices)
 
     def add(self, data: pd.DataFrame):
@@ -148,15 +149,19 @@
         data.index = new_indices
 
         self.data = pd.concat([self.data, data], ignore_index=False)
 
     def add_output(self, output: np.ndarray, label: str = "y"):
         self.data[("output", label)] = output
 
-    def add_numpy_arrays(self, input: np.ndarray, output: np.ndarray):
+    def add_numpy_arrays(self, input: np.ndarray, output: Union[np.ndarray, None]):
+
+        if output is None:
+            output = np.nan * np.ones((input.shape[0], len(self.data['output'].columns)))
+
         df = pd.DataFrame(np.hstack((input, output)),
                           columns=self.data.columns)
         self.add(df)
 
     def get_inputdata(self) -> pd.DataFrame:
         return self.data['input']
 
@@ -165,14 +170,21 @@
 
     def get_inputdata_dict(self, index: int) -> Dict[str, Any]:
         return self.data['input'].loc[index].to_dict()
 
     def get_outputdata_dict(self, index: int) -> Dict[str, Any]:
         return self.data['output'].loc[index].to_dict()
 
+    def get_design(self, index: int) -> Design:
+        return Design(self.get_inputdata_dict(index), self.get_outputdata_dict(index), index)
+
+    def set_design(self, design: Design) -> None:
+        for column, value in design._dict_output.items():
+            self.data.loc[design._jobnumber, ('output', column)] = value
+
     def set_inputdata(self, index: int, value: Any, column: str = 'input'):
         # check if the index exists
         if index not in self.data.index:
             raise IndexError(f"Index {index} does not exist in the data.")
 
         self.data.at[index, column] = value
```

### Comparing `f3dasm-1.1.0/src/f3dasm/design/_jobqueue.py` & `f3dasm-1.2.0/src/f3dasm/design/_jobqueue.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,28 @@
+#                                                                       Modules
+# =============================================================================
 
+# Standard
 from typing import List, Union
 
+# Third-party
 import pandas as pd
 
+# Local
 from ._data import _Data
 
+#                                                          Authorship & Credits
+# =============================================================================
+__author__ = 'Martin van der Schelling (M.P.vanderSchelling@tudelft.nl)'
+__credits__ = ['Martin van der Schelling']
+__status__ = 'Stable'
+# =============================================================================
+#
+# =============================================================================
+
 
 class NoOpenJobsError(Exception):
     """
     Exception raised when there are no open jobs.
 
     Attributes:
         message (str): The error message.
@@ -25,14 +39,17 @@
         'finished', or 'error'.
 
         Parameters
         ----------
         filename : str
             The name of the file that the jobs will be saved in.
         """
+        if jobs is None:
+            jobs = pd.Series(dtype='string')
+
         self.jobs: pd.Series = jobs
 
     def _repr_html_(self) -> str:
         return self.jobs.__repr__()
 
     @classmethod
     def from_data(cls, data: _Data):
@@ -102,46 +119,48 @@
         Parameters
         ----------
         indices : List[int]
             List of indices to remove.
         """
         self.jobs = self.jobs.drop(indices)
 
-    def add(self, number_of_jobs: int):
+    def add(self, number_of_jobs: int, status: str = 'open'):
         """Adds a number of jobs to the job queue.
 
         Parameters
         ----------
         number_of_jobs : int
             Number of jobs to add.
+        status : str, optional
+            Status of the jobs, by default 'open'.
         """
         try:
             last_index = self.jobs.index[-1]
         except IndexError:  # Empty Series
-            self.jobs = pd.Series(['open'] * number_of_jobs, dtype='string')
+            self.jobs = pd.Series([status] * number_of_jobs, dtype='string')
             return
 
         new_indices = pd.RangeIndex(start=last_index + 1, stop=last_index + number_of_jobs + 1, step=1)
-        jobs_to_add = pd.Series('open', index=new_indices, dtype='string')
+        jobs_to_add = pd.Series(status, index=new_indices, dtype='string')
         self.jobs = pd.concat([self.jobs, jobs_to_add], ignore_index=False)
 
     def reset(self) -> None:
         """Resets the job queue."""
-        self.jobs = pd.Series()
+        self.jobs = pd.Series(dtype='string')
 
     def get_open_job(self) -> Union[int, None]:
         """Returns the index of an open job.
 
         Returns
         -------
         int
             Index of an open job.
         """
         try:  # try to find an open job
-            return self.jobs[self.jobs == 'open'].index[0]
+            return int(self.jobs[self.jobs == 'open'].index[0])
         except IndexError:
             raise NoOpenJobsError("No open jobs found.")
 
     def mark_as_in_progress(self, index: int) -> None:
         """Marks a job as in progress.
 
         Parameters
@@ -171,14 +190,18 @@
         """
         self.jobs.loc[index] = 'error'
 
     def mark_all_in_progress_open(self) -> None:
         """Marks all jobs as 'open'."""
         self.jobs = self.jobs.replace('in progress', 'open')
 
+    def mark_all_open(self) -> None:
+        """Marks all jobs as 'open'."""
+        self.jobs = self.jobs.replace(['in progress', 'finished', 'error'], 'open')
+
     def is_all_finished(self) -> bool:
         """Checks if all jobs are finished.
 
         Returns
         -------
         bool
             True if all jobs are finished, False otherwise.
```

### Comparing `f3dasm-1.1.0/src/f3dasm/design/experimentdata.py` & `f3dasm-1.2.0/src/f3dasm/design/experimentdata.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,41 +2,49 @@
 # =============================================================================
 
 # Standard
 import errno
 import functools
 import json
 import os
+import sys
+import traceback
 from copy import deepcopy
 from io import TextIOWrapper
 from pathlib import Path
 from time import sleep
-from typing import (Any, Callable, Dict, Iterator, List, Protocol, Tuple, Type,
-                    Union)
 
-from hydra.utils import get_original_cwd
-from omegaconf import DictConfig
+if sys.version_info < (3, 8):
+    from typing_extensions import Protocol
+else:
+    from typing import Protocol
 
-from .._logging import logger
+from typing import Any, Callable, Dict, Iterator, List, Tuple, Type, Union
 
 # import msvcrt if windows, otherwise (Unix system) import fcntl
 if os.name == 'nt':
     import msvcrt
 else:
     import fcntl
 
-# Third-party core
+# Third-party
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
+from hydra.utils import get_original_cwd
+from omegaconf import DictConfig
+from pathos.helpers import mp
 
 # Local
+from ..logger import logger
+from ._access_file import access_file
 from ._data import _Data
-from ._jobqueue import _JobQueue
-from .design import DesignSpace
+from ._jobqueue import NoOpenJobsError, _JobQueue
+from .design import Design
+from .domain import Domain
 
 #                                                          Authorship & Credits
 # =============================================================================
 __author__ = 'Martin van der Schelling (M.P.vanderSchelling@tudelft.nl)'
 __credits__ = ['Martin van der Schelling']
 __status__ = 'Stable'
 # =============================================================================
@@ -45,104 +53,20 @@
 
 
 class Sampler(Protocol):
     def get_samples(numsamples: int) -> 'ExperimentData':
         ...
 
 
-def access_file(sleeptime_sec: int = 1) -> Callable:
-    """Wrapper for accessing a single resource with a file lock
-
-    Parameters
-    ----------
-    sleeptime_sec, optional
-        number of seconds to wait before trying to access resource again, by default 1
-
-    Returns
-    -------
-    decorator
-    """
-    def decorator_func(operation: Callable) -> Callable:
-        @functools.wraps(operation)
-        def wrapper_func(self, *args, **kwargs) -> None:
-            while True:
-                try:
-                    # Try to open the experimentdata file
-                    logger.debug(f"Trying to open the data file: {self.filename}_data.csv")
-                    with open(f"{self.filename}_data.csv", 'rb+') as file:
-                        logger.debug("Opened file successfully")
-                        if os.name == 'nt':
-                            msvcrt.locking(file.fileno(), msvcrt.LK_LOCK, 1)
-                        else:
-                            fcntl.flock(file, fcntl.LOCK_EX | fcntl.LOCK_NB)
-                            logger.debug("Locked file successfully")
-
-                        # Load the experimentdata from the object
-                        self.data = _Data.from_file(filename=self.filename, text_io=file)
-                        logger.debug("Loaded data successfully")
-
-                        # Load the jobs from disk
-                        self.jobs = _JobQueue.from_file(filename=f"{self.filename}_jobs")
-                        logger.debug("Loaded jobs successfully")
-
-                        # Do the operation
-                        value = operation(self, *args, **kwargs)
-
-                        # Delete existing contents of file
-                        file.seek(0, 0)
-                        file.truncate()
-
-                        # Write the data to disk
-                        self.data.store(filename=f"{self.filename}_data", text_io=file)
-                        self.jobs.store(filename=f"{self.filename}_jobs")
-
-                    break
-                except IOError as e:
-                    # the file is locked by another process
-                    if os.name == 'nt':
-                        if e.errno == 13:
-                            logger.info("The data file is currently locked by another process. "
-                                        "Retrying in 1 second...")
-                            sleep(sleeptime_sec)
-                        elif e.errno == 2:  # File not found error
-                            logger.info("The data file does not exist. Retrying in 1 second...")
-                            sleep(sleeptime_sec)
-                        else:
-                            logger.info(f"An unexpected IOError occurred: {e}")
-                            break
-                    else:
-                        if e.errno == errno.EAGAIN:
-                            logger.info("The data file is currently locked by another process. "
-                                        "Retrying in 1 second...")
-                            sleep(sleeptime_sec)
-                        elif e.errno == 2:  # File not found error
-                            logger.info("The data file does not exist. Retrying in 1 second...")
-                            sleep(sleeptime_sec)
-                        else:
-                            logger.info(f"An unexpected IOError occurred: {e}")
-                            break
-                except Exception as e:
-                    # handle any other exceptions
-                    logger.info(f"An unexpected error occurred: {e}")
-                    raise e
-                    return
-
-            return value
-
-        return wrapper_func
-
-    return decorator_func
-
-
 class ExperimentData:
     """
     A class that contains data for experiments.
     """
 
-    def __init__(self, design: DesignSpace):
+    def __init__(self, design: Domain):
         """
         Initializes an instance of ExperimentData.
 
         Parameters
         ----------
         design : DesignSpace
             A DesignSpace object defining the input and output spaces of the experiment.
@@ -166,47 +90,56 @@
 
     def __next__(self):
         self.data.__next__()
 
     def _repr_html_(self) -> str:
         return self.data._repr_html_()
 
+    #                                                      Alternative Constructors
+    # =============================================================================
+
     @classmethod
     def from_file(cls: Type['ExperimentData'], filename: str = 'doe',
                   text_io: Union[TextIOWrapper, None] = None) -> 'ExperimentData':
         """Create an ExperimentData object from .csv and .json files.
 
         Parameters
         ----------
         filename : str
             Name of the file, excluding suffix.
+        text_io : TextIOWrapper or None, optional
+            Text I/O wrapper object for reading the file, by default None.
 
         Returns
         -------
         ExperimentData
             ExperimentData object containing the loaded data.
         """
         try:
-            # Create the experimentdata object
-            design = DesignSpace.from_file(f"{filename}_design")
+            return cls._from_file_attempt(filename, text_io)
+        except FileNotFoundError:
+            try:
+                filename_with_path = Path(get_original_cwd()) / filename
+            except ValueError:  # get_original_cwd() hydra initialization error
+                raise FileNotFoundError(f"Cannot find the file {filename}_data.csv.")
+
+            return cls._from_file_attempt(filename_with_path, text_io)
+
+    @classmethod
+    def _from_file_attempt(cls: Type['ExperimentData'], filename: str,
+                           text_io: Union[TextIOWrapper, None]) -> 'ExperimentData':
+        try:
+            design = Domain.from_file(f"{filename}_design")
             experimentdata = cls(design=design)
             experimentdata.data = _Data.from_file(f"{filename}_data", text_io)
             experimentdata.jobs = _JobQueue.from_file(f"{filename}_jobs")
             experimentdata.filename = filename
             return experimentdata
-
-        # Cannot find the file, this could be due to hydra changing directories!
         except FileNotFoundError:
-            try:
-                return cls.from_file(filename=Path(get_original_cwd()) / filename)
-            except ValueError:  # get_original_cwd() hydra initialization error
-                raise FileNotFoundError(f"Cannot find the file {filename}_data.csv.")
-
-    # create an alias of from_csv
-    from_csv = from_file
+            raise FileNotFoundError(f"Cannot find the file {filename}_data.csv.")
 
     @classmethod
     def from_sampling(cls, sampler: Sampler) -> 'ExperimentData':
         """Create an ExperimentData object from a sampler.
 
         Parameters
         ----------
@@ -238,23 +171,16 @@
     def select(self, indices: List[int]) -> 'ExperimentData':
         new_experimentdata = deepcopy(self)
         new_experimentdata.data.select(indices)
         new_experimentdata.jobs.select(indices)
 
         return new_experimentdata
 
-    def reset_data(self):
-        """Reset the dataframe to an empty dataframe with the appropriate input and output columns"""
-        self.data.reset(self.design)
-        self.jobs.reset()
-
-    def show(self):
-        """Print the data to the console"""
-        print(self.data.data)
-        return
+    #                                                               Storage Methods
+    # =============================================================================
 
     def store(self, filename: str = None, text_io: Union[TextIOWrapper, None] = None):
         """Store the ExperimentData to disk, with checking for a lock
 
         Parameters
         ----------
         filename
@@ -263,14 +189,48 @@
         if filename is None:
             filename = self.filename
 
         self.data.store(f"{filename}_data")
         self.jobs.store(f"{filename}_jobs")
         self.design.store(f"{filename}_design")
 
+    def to_numpy(self) -> Tuple[np.ndarray, np.ndarray]:
+        """
+        Convert the ExperimentData object to a tuple of numpy arrays.
+
+        Returns
+        -------
+        tuple
+            A tuple containing two numpy arrays, the first one for input columns, and the second for output columns.
+        """
+        return self.data.to_numpy()
+
+    def run(self, operation: Callable, mode: str = 'sequential', kwargs: dict = None):
+
+        if kwargs is None:
+            kwargs = {}
+
+        # Check if operation is a function
+        if not callable(operation):
+            raise TypeError("operation must be a function.")
+
+        if mode.lower() == "sequential":
+            return self._run_sequential(operation, kwargs)
+        elif mode.lower() == "parallel":
+            return self._run_multiprocessing(operation, kwargs)
+        elif mode.lower() == "cluster":
+            return self._run_cluster(operation, kwargs)
+        else:
+            raise ValueError("Invalid parallelization mode specified.")
+
+    def reset_data(self):
+        """Reset the dataframe to an empty dataframe with the appropriate input and output columns"""
+        self.data.reset(self.design)
+        self.jobs.reset()
+
     def get_inputdata_by_index(self, index: int) -> dict:
         """
         Gets the input data at the given index.
 
         Parameters
         ----------
         index : int
@@ -301,14 +261,54 @@
             A dictionary containing the output data at the given index.
         """
         try:
             return self.data.get_outputdata_dict(index)
         except KeyError:
             raise KeyError('Index does not exist in dataframe!')
 
+    def get_design(self, index: int) -> Design:
+        """
+        Gets the design at the given index.
+
+        Parameters
+        ----------
+        index : int
+            The index of the design to retrieve.
+
+        Returns
+        -------
+        Design
+            The design at the given index.
+        """
+        return self.data.get_design(index)
+
+    def set_design(self, design: Design) -> None:
+        """
+        Sets the design at the given index.
+
+        Parameters
+        ----------
+        design : Design
+            The design to set.
+        """
+        self.data.set_design(design)
+        self.jobs.mark_as_finished(design._jobnumber)
+
+    @access_file()
+    def write_design(self, design: Design) -> None:
+        """
+        Sets the design at the given index.
+
+        Parameters
+        ----------
+        design : Design
+            The design to set.
+        """
+        self.set_design(design)
+
     def set_outputdata_by_index(self, index: int, value: Any):
         """
         Sets the output data at the given index to the given value.
 
         Parameters
         ----------
         index : int
@@ -336,45 +336,35 @@
         """
         self.data.set_inputdata(index, value, column)
 
     @access_file()
     def write_inputdata_by_index(self, index: int, value: Any, column: str = 'input'):
         self.set_inputdata_by_index(index=index, value=value, column=column)
 
-    def access_open_job_data(self) -> Tuple[int, Dict[str, Any], Dict[str, Any]]:
+    def access_open_job_data(self) -> Design:
         job_index = self.jobs.get_open_job()
         self.jobs.mark_as_in_progress(job_index)
-
-        input_data = self.get_inputdata_by_index(job_index)
-        output_data = self.get_outputdata_by_index(job_index)
-
-        return job_index, input_data, output_data
+        design = self.get_design(job_index)
+        return design
 
     @access_file()
-    def get_open_job_data(self) -> Tuple[int, Dict[str, Any], Dict[str, Any]]:
+    def get_open_job_data(self) -> Design:
         return self.access_open_job_data()
 
     def set_error(self, index: int):
         self.jobs.mark_as_error(index)
         self.set_outputdata_by_index(index, value='ERROR')
 
     @access_file()
     def write_error(self, index: int):
         self.set_error(index)
 
-    def to_numpy(self) -> Tuple[np.ndarray, np.ndarray]:
-        """
-        Convert the ExperimentData object to a tuple of numpy arrays.
-
-        Returns
-        -------
-        tuple
-            A tuple containing two numpy arrays, the first one for input columns, and the second for output columns.
-        """
-        return self.data.to_numpy()
+    @access_file()
+    def is_all_finished(self) -> bool:
+        return self.jobs.is_all_finished()
 
     def add(self, data: pd.DataFrame, ignore_index: bool = False):
         """
         Append data to the ExperimentData object.
 
         Parameters
         ----------
@@ -403,27 +393,32 @@
         output : np.ndarray
             Output data to append.
         label : str, optional
             Label of the output column to add to.
         """
         self.data.add_output(output, label)
 
-    def add_numpy_arrays(self, input: np.ndarray, output: np.ndarray):
+    def add_numpy_arrays(self, input: np.ndarray, output: Union[np.ndarray, None] = None):
         """
         Append a numpy array to the ExperimentData object.
 
         Parameters
         ----------
         input : np.ndarray
             2D numpy array to add to the input data.
         output : np.ndarray
             2D numpy array to add to the output data.
         """
+        if output is not None:
+            status = 'finished'
+        else:
+            status = 'open'
+
         self.data.add_numpy_arrays(input, output)
-        self.jobs.add(number_of_jobs=len(input))
+        self.jobs.add(number_of_jobs=len(input), status=status)
 
     def remove_rows_bottom(self, number_of_rows: int):
         """
         Remove a number of rows from the end of the ExperimentData object.
 
         Parameters
         ----------
@@ -519,7 +514,75 @@
         -------
         tuple
             A tuple containing the matplotlib figure and axes
         """
         fig, ax = self.data.plot()
 
         return fig, ax
+
+    #                                                               Private methods
+    # =============================================================================
+
+    def _run_sequential(self, operation: Callable, kwargs: dict):
+        while True:
+            try:
+                design = self.access_open_job_data()
+                logger.debug(f"Accessed design {design._jobnumber}")
+            except NoOpenJobsError:
+                logger.debug("No Open Jobs left")
+                break
+
+            try:
+                logger.info(
+                    f"Running design {design._jobnumber} with kwargs {kwargs}")
+                _design = operation(design, **kwargs)  # no *args!
+                self.set_design(_design)
+            except Exception as e:
+                error_msg = f"Error in design {design._jobnumber}: {e}"
+                error_traceback = traceback.format_exc()
+                logger.error(f"{error_msg}\n{error_traceback}")
+                self.set_error(design._jobnumber)
+
+    def _run_multiprocessing(self, operation: Callable, kwargs: dict):
+        # Get all the jobs
+        options = []
+        while True:
+            try:
+                design = self.access_open_job_data()
+                options.append(
+                    ({'design': design, **kwargs},))
+            except NoOpenJobsError:
+                break
+
+            def f(options: Dict[str, Any]) -> Any:
+                return operation(**options)
+
+            with mp.Pool() as pool:
+                # maybe implement pool.starmap_async ?
+                _designs: List[Design] = pool.starmap(f, options)
+
+            for _design in _designs:
+                self.set_design(_design)
+
+    def _run_cluster(self, operation: Callable, kwargs: dict):
+        # Retrieve the updated experimentdata object from disc
+        try:
+            self = self.from_file(self.filename)
+        except FileNotFoundError:  # If not found, store current
+            self.store()
+            # _data = self.from_file(self.filename)
+
+        while True:
+            try:
+                design = self.get_open_job_data()
+            except NoOpenJobsError:
+                break
+
+            try:
+                _design = operation(design, **kwargs)
+                self.write_design(_design)
+            except Exception as e:
+                error_msg = f"Error in design {design._jobnumber}: {e}"
+                error_traceback = traceback.format_exc()
+                logger.error(f"{error_msg}\n{error_traceback}")
+                self.write_error(design._jobnumber)
+                continue
```

### Comparing `f3dasm-1.1.0/src/f3dasm/design/parameter.py` & `f3dasm-1.2.0/src/f3dasm/design/parameter.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.1.0/src/f3dasm/functions/__init__.py` & `f3dasm-1.2.0/src/f3dasm/datageneration/functions/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import json
 from typing import List
 
 # Third-party
 import numpy as np
 
 from . import pybenchfunction
-from .adapters.augmentor import *
+from .adapters.augmentor import FunctionAugmentor, Noise, Offset, Scale
 from .function import Function
 from .pybenchfunction import *
 
 #                                                          Authorship & Credits
 # =============================================================================
 __author__ = 'Martin van der Schelling (M.P.vanderSchelling@tudelft.nl)'
 __credits__ = ['Martin van der Schelling']
```

### Comparing `f3dasm-1.1.0/src/f3dasm/functions/adapters/augmentor.py` & `f3dasm-1.2.0/src/f3dasm/datageneration/functions/adapters/augmentor.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #                                                                       Modules
 # =============================================================================
 
 # Standard
-from abc import ABC
+from abc import ABC, abstractmethod
 from copy import copy
 from typing import List
 
 # Third-party
 import autograd.numpy as np
 
 #                                                          Authorship & Credits
@@ -15,33 +15,34 @@
 __credits__ = ['Martin van der Schelling']
 __status__ = 'Alpha'
 # =============================================================================
 #
 # =============================================================================
 
 
-class Augmentor(ABC):
+class _Augmentor(ABC):
     """
     Base class for operations that augment an loss-funciton
     """
-
+    @abstractmethod
     def augment(self, input: np.ndarray) -> np.ndarray:
         """Stub function to augment the input of a function
 
         Parameters
         ----------
         input
             vector that needs to be augmented
 
         Returns
         -------
             augmented vector
         """
         ...
 
+    @abstractmethod
     def reverse_augment(self, output: np.ndarray) -> np.ndarray:
         """Stub function to reverse the augmented input
 
         Parameters
         ----------
         output
             augmented vector that needs to be undone
@@ -49,15 +50,15 @@
         Returns
         -------
             original vector
         """
         ...
 
 
-class Noise(Augmentor):
+class Noise(_Augmentor):
     def __init__(self, noise: float):
         """Augmentor class to add noise to a function output
 
         Parameters
         ----------
         noise
             standard deviation of Gaussian noise (mean is zero)
@@ -79,15 +80,15 @@
         y_noise = input + float(noise)
         return y_noise
 
     def reverse_augment(self, output: np.ndarray) -> np.ndarray:
         return self.augment
 
 
-class Offset(Augmentor):
+class Offset(_Augmentor):
     def __init__(self, offset: np.ndarray):
         """Augmentor class to offset the input vector of a function
 
         Parameters
         ----------
         offset
             constant vector that offsets the function input
@@ -97,15 +98,15 @@
     def augment(self, input: np.ndarray) -> np.ndarray:
         return input - self.offset
 
     def reverse_augment(self, output: np.ndarray) -> np.ndarray:
         return output + self.offset
 
 
-class Scale(Augmentor):
+class Scale(_Augmentor):
     def __init__(self, scale_bounds: np.ndarray, input_domain: np.ndarray):
         """Augmentor class to scale the input vector of a function to some bounds
 
         Parameters
         ----------
         scale_bounds
             continuous bounds (lower and upper for every dimension) to be scaled towards
@@ -126,50 +127,50 @@
     """Combination of Augmentors that can change the input and output of an objective function
 
     Args:
         input_augmentors (List[Augmentor]): list of input augmentors
         output_augmentors (List[Augmentor]): list of output augmentors
     """
 
-    def __init__(self, input_augmentors: List[Augmentor] = None, output_augmentors: List[Augmentor] = None):
+    def __init__(self, input_augmentors: List[_Augmentor] = None, output_augmentors: List[_Augmentor] = None):
         """Combination of augmentors that can change the input and output of an objective function
 
         Parameters
         ----------
         input_augmentors, optional
             list of input augmentors, by default None
         output_augmentors, optional
             list of output augmentors, by default None
         """
         self.input_augmentors = [] if input_augmentors is None else input_augmentors
         self.output_augmentors = [] if output_augmentors is None else output_augmentors
 
-    def add_input_augmentor(self, augmentor: Augmentor) -> None:
+    def add_input_augmentor(self, augmentor: _Augmentor) -> None:
         """Add an input augmentor
 
         Parameters
         ----------
         augmentor
             augmentor to be added
         """
         self.input_augmentors.append(augmentor)
 
-    def insert_input_augmentor(self, augmentor: Augmentor, position: int) -> None:
+    def insert_input_augmentor(self, augmentor: _Augmentor, position: int) -> None:
         """Insert an input augmentor at any place in the input_augmentors list
 
         Parameters
         ----------
         augmentor
             augmentor
         position
             position to put this augmentor in the input_augmentors list
         """
         self.input_augmentors.insert(position, augmentor)
 
-    def add_output_augmentor(self, augmentor: Augmentor) -> None:
+    def add_output_augmentor(self, augmentor: _Augmentor) -> None:
         """Add an output augmentor
 
         Parameters
         ----------
         augmentor
             augmentor to be added
         """
```

### Comparing `f3dasm-1.1.0/src/f3dasm/functions/adapters/pybenchfunction.py` & `f3dasm-1.2.0/src/f3dasm/datageneration/functions/adapters/pybenchfunction.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.1.0/src/f3dasm/functions/function.py` & `f3dasm-1.2.0/src/f3dasm/datageneration/functions/function.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,28 +12,29 @@
 
 # Third-party core
 import autograd.numpy as np
 import matplotlib.colors as mcol
 import matplotlib.pyplot as plt
 
 # Locals
-from ..design.experimentdata import ExperimentData
+from ...design.experimentdata import ExperimentData
+from ..datagenerator import DataGenerator
 from ..functions.adapters.augmentor import FunctionAugmentor
 
 #                                                          Authorship & Credits
 # =============================================================================
 __author__ = 'Martin van der Schelling (M.P.vanderSchelling@tudelft.nl)'
 __credits__ = ['Martin van der Schelling']
 __status__ = 'Stable'
 # =============================================================================
 #
 # =============================================================================
 
 
-class Function:
+class Function(DataGenerator):
     def __init__(self, seed=None):
         """Class for an analytical function
 
         Parameters
         ----------
         seed, optional
             seed for the random number generator, by default None
@@ -75,14 +76,17 @@
 
         # If the input is a Data object
         if isinstance(input_x, ExperimentData):
             input_x.add_output(np.array(y).reshape(-1, 1))
 
         return np.array(y).reshape(-1, 1)
 
+    def run(self, input_x: Union[np.ndarray, ExperimentData]) -> np.ndarray:
+        return self.__call__(input_x)
+
     def _retrieve_original_input(self, x: np.ndarray):
         """Retrieve the original input vector if the input is augmented
 
         Parameters
         ----------
         x
             augmented input vector
```

### Comparing `f3dasm-1.1.0/src/f3dasm/functions/pybenchfunction.py` & `f3dasm-1.2.0/src/f3dasm/datageneration/functions/pybenchfunction.py`

 * *Files 1% similar despite different names*

```diff
@@ -2931,7 +2931,82 @@
 
     def evaluate(self, X):
         d = X.shape[0]
         i = np.arange(1, d + 1)
         res = np.sum(X**2) + np.sum(0.5 * i * X) ** 2 + \
             np.sum(0.5 * i * X) ** 4
         return res
+
+
+__all__ = ['Ackley',
+           'AckleyN2',
+           'AckleyN3',
+           'AckleyN4',
+           'Adjiman',
+           'Bartels',
+           'Beale',
+           'Bird',
+           'BohachevskyN1',
+           'BohachevskyN2',
+           'BohachevskyN3',
+           'Booth',
+           'Branin',
+           'Brent',
+           'Brown',
+           'BukinN6',
+           'Colville',
+           'CrossInTray',
+           'DeJongN5',
+           'DeckkersAarts',
+           'DixonPrice',
+           'DropWave',
+           'Easom',
+           'EggCrate',
+           'EggHolder',
+           'Exponential',
+           'GoldsteinPrice',
+           'Griewank',
+           'HappyCat',
+           'Himmelblau',
+           'HolderTable',
+           'Keane',
+           'Langermann',
+           'Leon',
+           'Levy',
+           'LevyN13',
+           'Matyas',
+           'McCormick',
+           'Michalewicz',
+           'Periodic',
+           'Powell',
+           'Qing',
+           'Quartic',
+           'Rastrigin',
+           'Ridge',
+           'Rosenbrock',
+           'RotatedHyperEllipsoid',
+           'Salomon',
+           'SchaffelN1',
+           'SchaffelN2',
+           'SchaffelN3',
+           'SchaffelN4',
+           'Schwefel',
+           'Schwefel2_20',
+           'Schwefel2_21',
+           'Schwefel2_22',
+           'Schwefel2_23',
+           'Shekel',
+           'Shubert',
+           'ShubertN3',
+           'ShubertN4',
+           'Sphere',
+           'StyblinskiTang',
+           'SumSquares',
+           'Thevenot',
+           'ThreeHump',
+           'Trid',
+           'Wolfe',
+           'XinSheYang',
+           'XinSheYangN2',
+           'XinSheYangN3',
+           'XinSheYangN4',
+           'Zakharov']
```

### Comparing `f3dasm-1.1.0/src/f3dasm/optimization/adamax.py` & `f3dasm-1.2.0/src/f3dasm/optimization/lbfgsb.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,55 +1,37 @@
-"""
-Information on the Adamax optimizer
-"""
 #                                                                       Modules
 # =============================================================================
 
 # Standard
 from dataclasses import dataclass
 from typing import List
 
+from .adapters.scipy_implementations import _SciPyMinimizeOptimizer
 # Locals
-from .._imports import try_import
-from .adapters.tensorflow_implementations import TensorflowOptimizer
 from .optimizer import OptimizerParameters
 
-# Third-party extension
-with try_import('optimization') as _imports:
-    import tensorflow as tf
-
-
 #                                                          Authorship & Credits
 # =============================================================================
 __author__ = 'Martin van der Schelling (M.P.vanderSchelling@tudelft.nl)'
 __credits__ = ['Martin van der Schelling']
 __status__ = 'Stable'
 # =============================================================================
 #
 # =============================================================================
 
 
 @dataclass
-class Adamax_Parameters(OptimizerParameters):
-    """Hyperparameters for Adamax optimizer"""
+class LBFGSB_Parameters(OptimizerParameters):
+    """Hyperparameters for LBFGSB optimizer"""
+
+    ftol: float = 0.0
+    gtol: float = 0.0
+
+
+class LBFGSB(_SciPyMinimizeOptimizer):
+    """L-BFGS-B"""
 
-    learning_rate: float = 0.001
-    beta_1: float = 0.9
-    beta_2: float = 0.999
-    epsilon: float = 1e-07
-
-
-class Adamax(TensorflowOptimizer):
-    """Adamax"""
-
-    parameter: Adamax_Parameters = Adamax_Parameters()
-
-    def set_algorithm(self):
-        self.algorithm = tf.keras.optimizers.Adamax(
-            learning_rate=self.parameter.learning_rate,
-            beta_1=self.parameter.beta_1,
-            beta_2=self.parameter.beta_2,
-            epsilon=self.parameter.epsilon,
-        )
+    method: str = "L-BFGS-B"
+    parameter: LBFGSB_Parameters = LBFGSB_Parameters()
 
     def get_info(self) -> List[str]:
-        return ['Fast', 'Single-Solution']
+        return ['Stable', 'First-Order', 'Single-Solution']
```

### Comparing `f3dasm-1.1.0/src/f3dasm/optimization/adapters/scipy_implementations.py` & `f3dasm-1.2.0/src/f3dasm/optimization/adapters/scipy_implementations.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 # =============================================================================
 
 # Third-party core
 import autograd.numpy as np
 from scipy.optimize import minimize
 
 # Locals
-from .._protocol import Function
+from ...datageneration.functions import Function
 from ..optimizer import Optimizer
 
 #                                                          Authorship & Credits
 # =============================================================================
 __author__ = 'Martin van der Schelling (M.P.vanderSchelling@tudelft.nl)'
 __credits__ = ['Martin van der Schelling']
 __status__ = 'Stable'
 # =============================================================================
 #
 # =============================================================================
 
 
-class SciPyOptimizer(Optimizer):
+class _SciPyOptimizer(Optimizer):
     def _callback(self, xk: np.ndarray, *args, **kwargs) -> None:
         self.x_new.append(xk.tolist())
 
     def update_step(self):
         """Update step function"""
         raise ValueError(
             'Scipy optimizers don\'t have an update steps. Multiple iterations \
@@ -70,30 +70,63 @@
 
         # Repeat last iteration to fill up total iteration
         if len(self.x_new) < iterations:
             repeated_last_element = np.tile(
                 self.x_new[-1], (iterations - len(self.x_new), 1))
             self.x_new = np.r_[self.x_new, repeated_last_element]
 
-        self.add_iteration_to_data(x=self.x_new, y=function(self.x_new))
+        # check if fun has the original_function attribute
+        if hasattr(function, 'original_function'):
+            # Convert the input of the original function to an ndarray using a lambda function
+            def fun(x):
+                # convert the np.ndarray input to a dict with key x0, x1, x2, etc.
+                input_names = self.data.design.get_continuous_input_names()
+                x = {input_names[i]: x_i for i, x_i in enumerate(x)}
+                return function.original_function(x)
+
+        else:
+            def fun(x):
+                return function(x).item()
+
+        _y = []
+        for _x in self.x_new:
+            _y.append(fun(_x))
 
+        _y = np.array(_y).reshape(-1, 1)
 
-class SciPyMinimizeOptimizer(SciPyOptimizer):
+        # self.add_iteration_to_data(x=self.x_new, y=function(self.x_new))
+        self.add_iteration_to_data(x=self.x_new, y=_y)
+
+
+class _SciPyMinimizeOptimizer(_SciPyOptimizer):
     def run_algorithm(self, iterations: int, function: Function):
         """Run the algorithm for a number of iterations
 
         Parameters
         ----------
         iterations
             number of iterations
         function
             function to be evaluated
         """
+
+        # check if fun has the original_function attribute
+        if hasattr(function, 'original_function'):
+            # Convert the input of the original function to an ndarray using a lambda function
+            def fun(x):
+                # convert the np.ndarray input to a dict with key x0, x1, x2, etc.
+                input_names = self.data.design.get_continuous_input_names()
+                x = {input_names[i]: x_i for i, x_i in enumerate(x)}
+                return function.original_function(x)
+
+        else:
+            def fun(x):
+                return function(x).item()
         minimize(
-            fun=lambda x: function(x).item(),
+            fun=fun,
             method=self.method,
             # TODO: #89 Fix this with the newest gradient method!
             jac=lambda x: np.float64(function.dfdx_legacy(x).ravel()),
             x0=self.data.get_n_best_input_parameters_numpy(
                 nosamples=1).ravel(),
             callback=self._callback,
             options=self.parameter.__dict__,
```

### Comparing `f3dasm-1.1.0/src/f3dasm/optimization/cg.py` & `f3dasm-1.2.0/src/f3dasm/optimization/neldermead.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,35 +2,37 @@
 # =============================================================================
 
 # Standard
 from dataclasses import dataclass
 from typing import List
 
 # Locals
+from .adapters.scipy_implementations import _SciPyMinimizeOptimizer
 from .optimizer import OptimizerParameters
-from .adapters.scipy_implementations import SciPyMinimizeOptimizer
 
 #                                                          Authorship & Credits
 # =============================================================================
 __author__ = 'Martin van der Schelling (M.P.vanderSchelling@tudelft.nl)'
 __credits__ = ['Martin van der Schelling']
 __status__ = 'Stable'
 # =============================================================================
 #
 # =============================================================================
 
 
 @dataclass
-class CG_Parameters(OptimizerParameters):
-    """CG Parameters"""
+class NelderMead_Parameters(OptimizerParameters):
+    """Hyperparameters for NelderMead optimizer"""
 
-    gtol: float = 0.0
+    xatol: float = 0.0
+    fatol: float = 0.0
+    adaptive: bool = False
 
 
-class CG(SciPyMinimizeOptimizer):
-    """CG"""
+class NelderMead(_SciPyMinimizeOptimizer):
+    """Nelder-Mead"""
 
-    method: str = "CG"
-    parameter: CG_Parameters = CG_Parameters()
+    method: str = "Nelder-Mead"
+    parameter: NelderMead_Parameters = NelderMead_Parameters()
 
     def get_info(self) -> List[str]:
-        return ['Stable', 'First-Order', 'Single-Solution']
+        return ['Fast', 'Global', 'First-Order', 'Single-Solution']
```

### Comparing `f3dasm-1.1.0/src/f3dasm/optimization/cmaes.py` & `f3dasm-1.2.0/src/f3dasm/optimization/cg.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,51 +1,36 @@
 #                                                                       Modules
 # =============================================================================
 
 # Standard
 from dataclasses import dataclass
 from typing import List
 
+from .adapters.scipy_implementations import _SciPyMinimizeOptimizer
 # Locals
-from .._imports import try_import
-from .adapters.pygmo_implementations import PygmoAlgorithm
 from .optimizer import OptimizerParameters
 
-# Third-party extension
-with try_import('optimization') as _imports:
-    import pygmo as pg
-
-
 #                                                          Authorship & Credits
 # =============================================================================
 __author__ = 'Martin van der Schelling (M.P.vanderSchelling@tudelft.nl)'
 __credits__ = ['Martin van der Schelling']
 __status__ = 'Stable'
 # =============================================================================
 #
 # =============================================================================
 
 
 @dataclass
-class CMAES_Parameters(OptimizerParameters):
-    """Hyperparameters for CMAES optimizer"""
+class CG_Parameters(OptimizerParameters):
+    """CG Parameters"""
 
-    population: int = 30
+    gtol: float = 0.0
 
 
-class CMAES(PygmoAlgorithm):
-    """Covariance Matrix Adaptation Evolution Strategy optimizer implemented from pygmo"""
+class CG(_SciPyMinimizeOptimizer):
+    """CG"""
 
-    parameter: CMAES_Parameters = CMAES_Parameters()
-
-    def set_algorithm(self):
-        self.algorithm = pg.algorithm(
-            pg.cmaes(
-                gen=1,
-                memory=True,
-                seed=self.seed,
-                force_bounds=self.parameter.force_bounds,
-            )
-        )
+    method: str = "CG"
+    parameter: CG_Parameters = CG_Parameters()
 
     def get_info(self) -> List[str]:
-        return ['Stable', 'Global', 'Population-Based']
+        return ['Stable', 'First-Order', 'Single-Solution']
```

### Comparing `f3dasm-1.1.0/src/f3dasm/optimization/optimizer.py` & `f3dasm-1.2.0/src/f3dasm/optimization/optimizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 from copy import deepcopy
 from dataclasses import dataclass, field
 from typing import Any, List, Mapping, Optional, Tuple
 
 # Third-party core
 import numpy as np
 
+from ..datageneration.functions.function import Function
 # Locals
 from ..design.experimentdata import ExperimentData
-from ..functions.function import Function
 
 #                                                          Authorship & Credits
 # =============================================================================
 __author__ = 'Martin van der Schelling (M.P.vanderSchelling@tudelft.nl)'
 __credits__ = ['Martin van der Schelling']
 __status__ = 'Stable'
 # =============================================================================
```

### Comparing `f3dasm-1.1.0/src/f3dasm/optimization/randomsearch.py` & `f3dasm-1.2.0/src/f3dasm/optimization/randomsearch.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from dataclasses import dataclass
 from typing import List, Tuple
 
 # Third-party core
 import autograd.numpy as np
 
 # Locals
-from ._protocol import Function
+from ..datageneration.functions import Function
 from .optimizer import Optimizer, OptimizerParameters
 
 #                                                          Authorship & Credits
 # =============================================================================
 __author__ = 'Martin van der Schelling (M.P.vanderSchelling@tudelft.nl)'
 __credits__ = ['Martin van der Schelling']
 __status__ = 'Stable'
```

### Comparing `f3dasm-1.1.0/src/f3dasm/run_optimization.py` & `f3dasm-1.2.0/src/f3dasm/run_optimization.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,22 +10,22 @@
 from typing import Any, List, Type
 
 # Third-party
 import numpy as np
 import pandas as pd
 from pathos.helpers import mp
 
-from f3dasm.optimization import Optimizer, find_optimizer
-from f3dasm.sampling import Sampler, create_sampler_from_json
+from f3dasm.optimization import Optimizer
+from f3dasm.sampling import Sampler
 
-from ._logging import logger, time_and_log
 # Locals
 from .design import ExperimentData
-from .functions import create_function_from_json
-from .functions.function import Function
+from .datageneration.functions import create_function_from_json
+from .datageneration.functions.function import Function
+from .logger import logger, time_and_log
 
 #                                                          Authorship & Credits
 # =============================================================================
 __author__ = 'Martin van der Schelling (M.P.vanderSchelling@tudelft.nl)'
 __credits__ = ['Martin van der Schelling']
 __status__ = 'Stable'
 # =============================================================================
@@ -57,31 +57,14 @@
         self.optimizer = optimizer
         self.function = function
         self.sampler = sampler
         self.number_of_samples = number_of_samples
         self.seeds = seeds
         self._log()
 
-    @classmethod
-    def from_json(cls: Type['OptimizationResult'], json_string: str) -> 'OptimizationResult':
-        optimizationresult_dict = json.loads(json_string)
-        return cls.from_dict(optimizationresult_dict)
-
-    @classmethod
-    def from_dict(cls: Type['OptimizationResult'], optimizationresult_dict: dict) -> 'OptimizationResult':
-        args = {
-            'data': [ExperimentData.from_json(json_data) for json_data in optimizationresult_dict['data']],
-            # 'optimizer': create_optimizer_from_json(optimizationresult_dict['optimizer']),
-            'function': create_function_from_json(optimizationresult_dict['function']),
-            'sampler': create_sampler_from_json(optimizationresult_dict['sampler']),
-            'number_of_samples': optimizationresult_dict['number_of_samples'],
-            'seeds': optimizationresult_dict['seeds'],
-        }
-        return cls(**args)
-
     def to_json(self):
         args = {'data': [d.to_json() for d in self.data],
                 'optimizer': self.optimizer.to_json(),
                 'function': self.function.to_json(),
                 'sampler': self.sampler.to_json(),
                 'number_of_samples': self.number_of_samples,
                 'seeds': self.seeds
```

### Comparing `f3dasm-1.1.0/src/f3dasm/sampling/latinhypercube.py` & `f3dasm-1.2.0/src/f3dasm/sampling/latinhypercube.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,43 +1,34 @@
 #                                                                       Modules
 # =============================================================================
 
 # Standard
 from typing import Any, Union
 
-# Third-party core
+# Third-party
 import numpy as np
+from SALib.sample import latin
 
 # Locals
-from .._imports import try_import
-from ..design import DesignSpace
+from ..design import Domain
 from .sampler import Sampler
 
-# Third-party extension
-with try_import('sampling') as _imports:
-    from SALib.sample import latin
-
-
 #                                                          Authorship & Credits
 # =============================================================================
 __author__ = 'Martin van der Schelling (M.P.vanderSchelling@tudelft.nl)'
 __credits__ = ['Martin van der Schelling']
 __status__ = 'Stable'
 # =============================================================================
 #
 # =============================================================================
 
 
 class LatinHypercube(Sampler):
     """Sampling via Latin Hypercube Sampling"""
 
-    def __init__(self, design: DesignSpace, seed: Union[Any, int] = None):
-        _imports.check()
-        super().__init__(design, seed)
-
     def sample_continuous(self, numsamples: int) -> np.ndarray:
         """Sample from continuous space
 
         Parameters
         ----------
         numsamples
             number of samples
```

### Comparing `f3dasm-1.1.0/src/f3dasm/sampling/randomuniform.py` & `f3dasm-1.2.0/src/f3dasm/sampling/randomuniform.py`

 * *Files identical despite different names*

### Comparing `f3dasm-1.1.0/src/f3dasm/sampling/sampler.py` & `f3dasm-1.2.0/src/f3dasm/sampling/sampler.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 import json
 from typing import Any, List, Union
 
 # Third-party core
 import numpy as np
 import pandas as pd
 from hydra.utils import instantiate
-from omegaconf import DictConfig, OmegaConf
+from omegaconf import DictConfig
 
 # Locals
-from ..design.design import DesignSpace
+from ..design.domain import Domain
 from ..design.experimentdata import ExperimentData
 
 #                                                          Authorship & Credits
 # =============================================================================
 __author__ = 'Martin van der Schelling (M.P.vanderSchelling@tudelft.nl)'
 __credits__ = ['Martin van der Schelling']
 __status__ = 'Stable'
@@ -32,15 +32,15 @@
     ----------
     design
         design of experiments object
     seed
         seed for sampling
     """
 
-    def __init__(self, design: DesignSpace, seed: Union[Any, int] = None, number_of_samples: int = None):
+    def __init__(self, design: Domain, seed: Union[Any, int] = None, number_of_samples: int = None):
         self.design = design
         self.seed = seed
         self.number_of_samples = number_of_samples
         self.__post_init__()
 
     def __post_init__(self):
         if self.seed:
@@ -51,15 +51,15 @@
 
     @classmethod
     def from_yaml(cls, config: DictConfig) -> 'Sampler':
         """Create a sampler from a yaml configuration"""
 
         args = {**config.sampler, 'design': None}
         sampler: Sampler = instantiate(args)
-        sampler.design = DesignSpace.from_yaml(config.design)
+        sampler.design = Domain.from_yaml(config.design)
         return sampler
 
     def to_json(self):
         args = {'design': self.design.to_json(),
                 'seed': self.seed}
         name = self.__class__.__name__
         return json.dumps((args, name))
@@ -136,15 +136,15 @@
         return data
 
     def _cast_to_data_object(self, samples: np.ndarray, columnnames: List[str]) -> ExperimentData:
         """Cast the samples to a Data object"""
         data = ExperimentData(design=self.design)
 
         # First get an empty reference frame from the DoE
-        empty_frame = self.design.create_empty_dataframe()
+        empty_frame = self.design._create_empty_dataframe()
 
         # Then, create a new frame from the samples and columnnames
         samples_frame = pd.DataFrame(data=samples, columns=columnnames)
         df = pd.concat([empty_frame, samples_frame], sort=True)
 
         # Add the samples to the Data object
         data.add(data=df)
```

### Comparing `f3dasm-1.1.0/src/f3dasm/sampling/utils.py` & `f3dasm-1.2.0/src/f3dasm/sampling/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 #                                                                       Modules
 # =============================================================================
 
 # Standard
-import json
 from typing import List
 
 # Locals
-from ..design import DesignSpace
-from .all_samplers import SAMPLERS
+from .latinhypercube import LatinHypercube
+from .randomuniform import RandomUniform
 from .sampler import Sampler
+from .sobolsequence import SobolSequence
 
 #                                                          Authorship & Credits
 # =============================================================================
 __author__ = 'Martin van der Schelling (M.P.vanderSchelling@tudelft.nl)'
 __credits__ = ['Martin van der Schelling']
 __status__ = 'Stable'
 # =============================================================================
 #
 # =============================================================================
 
+# List of available samplers
+SAMPLERS: List[Sampler] = [RandomUniform, LatinHypercube, SobolSequence]
+
 
 def find_sampler(query: str) -> Sampler:
     """Find a Sampler from the f3dasm.design submodule
 
     Parameters
     ----------
     query
@@ -34,26 +37,15 @@
     """
     try:
         return list(filter(lambda parameter: parameter.__name__ == query, SAMPLERS))[0]
     except IndexError:
         return ValueError(f'Sampler {query} not found!')
 
 
-def create_sampler_from_json(json_string: str) -> Sampler:
-    """Create a Sampler object from a json string
-
-    Parameters
-    ----------
-    json_string
-        json string representation of the information to construct the Parameter
-
-    Returns
-    -------
-        Requested Sampler object
-    """
-    sampler_dict, name = json.loads(json_string)
-    return _create_sampler_from_dict(sampler_dict, name)
-
-
-def _create_sampler_from_dict(sampler_dict: dict, name: str) -> Sampler:
-    sampler_dict['design'] = DesignSpace.from_json(sampler_dict['design'])
-    return find_sampler(name)(**sampler_dict)
+__all__ = [
+    'LatinHypercube',
+    'RandomUniform',
+    'Sampler',
+    'SobolSequence',
+    'SAMPLERS',
+    'find_sampler'
+]
```

### Comparing `f3dasm-1.1.0/src/f3dasm/simulation/simulator.py` & `f3dasm-1.2.0/src/f3dasm/datageneration/datagenerator.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 #                                                                       Modules
 # =============================================================================
 
-from .._logging import logger, time_and_log
+from ..design._data import Design
+from ..logger import time_and_log
 
 #                                                          Authorship & Credits
 # =============================================================================
 __author__ = "Martin van der Schelling (M.P.vanderSchelling@tudelft.nl)"
 __credits__ = ["Martin van der Schelling"]
 __status__ = "Alpha"
 # =============================================================================
 #
 # =============================================================================
 
 
-class Simulator:
-    """Base class for a FEM simulator"""
+class DataGenerator:
+    """Base class for a data generator"""
+
+    def __init__(self, design: Design, **kwargs):
+        self.design = design
+        self.kwargs = kwargs
 
     def pre_process(self) -> None:
         """Function that handles the pre-processing"""
         ...
         # raise NotImplementedError("No pre-process function implemented!")
 
     def execute(self) -> None:
```

### Comparing `f3dasm-1.1.0/src/f3dasm.egg-info/PKG-INFO` & `f3dasm-1.2.0/src/f3dasm.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: f3dasm
-Version: 1.1.0
+Version: 1.2.0
 Summary: f3dasm - Framework for Data-driven development and Analysis of Structures and Materials
 Home-page: https://github.com/bessagroup/f3dasm
 Author: Martin van der Schelling
 Author-email: M.P.vanderSchelling@tudelft.nl
 License: BSD
 Project-URL: Documentation, https://bessagroup.github.io/f3dasm/
 Project-URL: Wiki, https://github.com/bessagroup/f3dasm/wiki
@@ -12,27 +12,23 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
-Requires-Python: >=3.8, <3.11
+Requires-Python: <3.11,>=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: sampling
-Provides-Extra: machinelearning
-Provides-Extra: optimization
-Provides-Extra: all
-Provides-Extra: dev
 License-File: LICENSE
 
 f3dasm
 ------
 *Framework for data-driven design \& analysis of structures and materials*
 
 ***
@@ -41,15 +37,15 @@
 [![pypi](https://img.shields.io/pypi/v/f3dasm.svg)](https://pypi.org/project/f3dasm/)
 [![GitHub license](https://img.shields.io/badge/license-BSD-blue)](https://github.com/bessagroup/f3dasm)
 
 [**Docs**](https://bessagroup.github.io/f3dasm/)
 | [**Installation**](https://bessagroup.github.io/f3dasm/general/gettingstarted.html)
 | [**GitHub**](https://github.com/bessagroup/f3dasm)
 | [**PyPI**](https://pypi.org/project/f3dasm/)
-| [**Practical sessions**](https://github.com/mpvanderschelling/F3DASM_practical)
+| [**Practical sessions**](https://github.com/mpvanderschelling/f3dasm_teach)
 
 Welcome to `f3dasm`, a Python package for data-driven design and analysis of structures and materials.
 
 * Created by M.A. Bessa (M.A.Bessa@tudelft.nl) in September 2016
 * Current developer and maintainer: [M.P. van der Schelling](https://github.com/mpvanderschelling/) (M.P.vanderSchelling@tudelft.nl)
 
 The Bessa research group at TU Delft is small... At the moment, we have limited availability to help future users/developers adapting the code to new problems, but we will do our best to help!
```

### Comparing `f3dasm-1.1.0/tests/conftest.py` & `f3dasm-1.2.0/tests/conftest.py`

 * *Files identical despite different names*

