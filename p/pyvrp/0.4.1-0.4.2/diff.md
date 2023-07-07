# Comparing `tmp/pyvrp-0.4.1.tar.gz` & `tmp/pyvrp-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvrp-0.4.1.tar", max compression
+gzip compressed data, was "pyvrp-0.4.2.tar", max compression
```

## Comparing `pyvrp-0.4.1.tar` & `pyvrp-0.4.2.tar`

### file list

```diff
@@ -1,167 +1,167 @@
--rw-r--r--   0        0        0     1175 2023-07-04 09:33:31.369422 pyvrp-0.4.1/LICENSE
--rw-r--r--   0        0        0     2963 2023-07-04 09:33:31.369422 pyvrp-0.4.1/README.md
--rw-r--r--   0        0        0     3563 2023-07-04 09:33:31.369422 pyvrp-0.4.1/build_extensions.py
--rw-r--r--   0        0        0     3747 2023-07-04 09:33:31.397423 pyvrp-0.4.1/meson.build
--rw-r--r--   0        0        0      302 2023-07-04 09:33:31.397423 pyvrp-0.4.1/meson_options.txt
--rw-r--r--   0        0        0     3505 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     6822 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/GeneticAlgorithm.py
--rw-r--r--   0        0        0     8577 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/Model.py
--rw-r--r--   0        0        0     8807 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/PenaltyManager.py
--rw-r--r--   0        0        0     6608 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/Population.py
--rw-r--r--   0        0        0     2922 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/Result.py
--rw-r--r--   0        0        0     6191 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/Statistics.py
--rw-r--r--   0        0        0     1375 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/_CostEvaluator.pyi
--rw-r--r--   0        0        0      563 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/_Matrix.pyi
--rw-r--r--   0        0        0     5791 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/_ProblemData.pyi
--rw-r--r--   0        0        0     6397 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/_Solution.pyi
--rw-r--r--   0        0        0     4089 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/_SubPopulation.pyi
--rw-r--r--   0        0        0     1664 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/_TimeWindowSegment.pyi
--rw-r--r--   0        0        0      267 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/_XorShift128.pyi
--rw-r--r--   0        0        0      554 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/__init__.py
--rw-r--r--   0        0        0     8947 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cli.py
--rw-r--r--   0        0        0       45 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/constants.py
--rw-r--r--   0        0        0      854 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cpp/CostEvaluator.cpp
--rw-r--r--   0        0        0     2039 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cpp/CostEvaluator.h
--rw-r--r--   0        0        0     1354 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cpp/CostEvaluator_bindings.cpp
--rw-r--r--   0        0        0     2751 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cpp/Matrix.h
--rw-r--r--   0        0        0     1041 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cpp/Matrix_bindings.cpp
--rw-r--r--   0        0        0     5569 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cpp/Measure.h
--rw-r--r--   0        0        0     2466 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cpp/ProblemData.cpp
--rw-r--r--   0        0        0     4789 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cpp/ProblemData.h
--rw-r--r--   0        0        0     5227 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cpp/ProblemData_bindings.cpp
--rw-r--r--   0        0        0      745 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cpp/README.md
--rw-r--r--   0        0        0    11014 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cpp/Solution.cpp
--rw-r--r--   0        0        0     6952 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cpp/Solution.h
--rw-r--r--   0        0        0     5857 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cpp/Solution_bindings.cpp
--rw-r--r--   0        0        0     4670 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cpp/SubPopulation.cpp
--rw-r--r--   0        0        0     3036 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cpp/SubPopulation.h
--rw-r--r--   0        0        0     2744 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cpp/SubPopulation_bindings.cpp
--rw-r--r--   0        0        0     3725 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cpp/TimeWindowSegment.h
--rw-r--r--   0        0        0     1603 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cpp/TimeWindowSegment_bindings.cpp
--rw-r--r--   0        0        0      581 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cpp/XorShift128.cpp
--rw-r--r--   0        0        0     2109 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cpp/XorShift128.h
--rw-r--r--   0        0        0      467 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cpp/XorShift128_bindings.cpp
--rw-r--r--   0        0        0     5340 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cpp/crossover/crossover.cpp
--rw-r--r--   0        0        0     2010 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cpp/crossover/crossover.h
--rw-r--r--   0        0        0     8610 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cpp/crossover/selective_route_exchange.cpp
--rw-r--r--   0        0        0      375 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cpp/crossover/selective_route_exchange_bindings.cpp
--rw-r--r--   0        0        0     1003 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cpp/diversity/broken_pairs_distance.cpp
--rw-r--r--   0        0        0      254 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cpp/diversity/broken_pairs_distance_bindings.cpp
--rw-r--r--   0        0        0      636 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cpp/diversity/diversity.h
--rw-r--r--   0        0        0     3048 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cpp/search/CircleSector.h
--rw-r--r--   0        0        0    11425 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cpp/search/Exchange.h
--rw-r--r--   0        0        0     2173 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cpp/search/Exchange_bindings.cpp
--rw-r--r--   0        0        0    14552 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cpp/search/LocalSearch.cpp
--rw-r--r--   0        0        0     3734 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cpp/search/LocalSearch.h
--rw-r--r--   0        0        0     2647 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cpp/search/LocalSearchOperator.h
--rw-r--r--   0        0        0     1329 2023-07-04 09:33:31.397423 pyvrp-0.4.1/pyvrp/cpp/search/LocalSearch_bindings.cpp
--rw-r--r--   0        0        0     3733 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/cpp/search/MoveTwoClientsReversed.cpp
--rw-r--r--   0        0        0      504 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/cpp/search/MoveTwoClientsReversed.h
--rw-r--r--   0        0        0      482 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/cpp/search/MoveTwoClientsReversed_bindings.cpp
--rw-r--r--   0        0        0      970 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/cpp/search/Node.cpp
--rw-r--r--   0        0        0     1616 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/cpp/search/Node.h
--rw-r--r--   0        0        0     1175 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/cpp/search/RelocateStar.cpp
--rw-r--r--   0        0        0      755 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/cpp/search/RelocateStar.h
--rw-r--r--   0        0        0      436 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/cpp/search/RelocateStar_bindings.cpp
--rw-r--r--   0        0        0     3952 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/cpp/search/Route.cpp
--rw-r--r--   0        0        0     5350 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/cpp/search/Route.h
--rw-r--r--   0        0        0    10975 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/cpp/search/SwapStar.cpp
--rw-r--r--   0        0        0     3399 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/cpp/search/SwapStar.h
--rw-r--r--   0        0        0      420 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/cpp/search/SwapStar_bindings.cpp
--rw-r--r--   0        0        0     4352 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/cpp/search/TwoOpt.cpp
--rw-r--r--   0        0        0      922 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/cpp/search/TwoOpt.h
--rw-r--r--   0        0        0      409 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/cpp/search/TwoOpt_bindings.cpp
--rw-r--r--   0        0        0       63 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/crossover/__init__.py
--rw-r--r--   0        0        0      364 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/crossover/_selective_route_exchange.pyi
--rw-r--r--   0        0        0     1949 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/crossover/selective_route_exchange.py
--rw-r--r--   0        0        0    12528 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/crossover/tests/test_selective_route_exchange.py
--rw-r--r--   0        0        0       58 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/diversity/__init__.py
--rw-r--r--   0        0        0     1444 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/diversity/_broken_pairs_distance.pyi
--rw-r--r--   0        0        0     1171 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/diversity/tests/test_broken_pairs_distance.py
--rw-r--r--   0        0        0      580 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/exceptions.py
--rw-r--r--   0        0        0      436 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/plotting/__init__.py
--rw-r--r--   0        0        0     1106 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/plotting/plot_coordinates.py
--rw-r--r--   0        0        0     1358 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/plotting/plot_demands.py
--rw-r--r--   0        0        0     1199 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/plotting/plot_diversity.py
--rw-r--r--   0        0        0     1129 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/plotting/plot_instance.py
--rw-r--r--   0        0        0     2344 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/plotting/plot_objectives.py
--rw-r--r--   0        0        0     1608 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/plotting/plot_result.py
--rw-r--r--   0        0        0     4690 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/plotting/plot_route_schedule.py
--rw-r--r--   0        0        0     1136 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/plotting/plot_runtimes.py
--rw-r--r--   0        0        0     1782 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/plotting/plot_solution.py
--rw-r--r--   0        0        0     1226 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/plotting/plot_time_windows.py
--rw-r--r--   0        0        0        0 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/plotting/tests/__init__.py
--rw-r--r--   0        0        0    47981 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/plotting/tests/baseline_images/test_plotting/plot_instance.png
--rw-r--r--   0        0        0   141297 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/plotting/tests/baseline_images/test_plotting/plot_result.png
--rw-r--r--   0        0        0    35194 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/plotting/tests/baseline_images/test_plotting/plot_route_schedule.png
--rw-r--r--   0        0        0    25609 2023-07-04 09:33:31.401423 pyvrp-0.4.1/pyvrp/plotting/tests/baseline_images/test_plotting/plot_solution.png
--rw-r--r--   0        0        0    43058 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/plotting/tests/baseline_images/test_plotting/plot_solution_with_customers.png
--rw-r--r--   0        0        0     3079 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/plotting/tests/test_plotting.py
--rw-r--r--   0        0        0     6782 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/read.py
--rw-r--r--   0        0        0     6559 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/search/LocalSearch.py
--rw-r--r--   0        0        0      896 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/search/_Exchange.pyi
--rw-r--r--   0        0        0      891 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/search/_LocalSearch.pyi
--rw-r--r--   0        0        0      204 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/search/_MoveTwoClientsReversed.pyi
--rw-r--r--   0        0        0      196 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/search/_RelocateStar.pyi
--rw-r--r--   0        0        0      192 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/search/_SwapStar.pyi
--rw-r--r--   0        0        0      188 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/search/_TwoOpt.pyi
--rw-r--r--   0        0        0      708 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/search/__init__.py
--rw-r--r--   0        0        0     5149 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/search/neighbourhood.py
--rw-r--r--   0        0        0        0 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/search/tests/__init__.py
--rw-r--r--   0        0        0    10470 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/search/tests/test_Exchange.py
--rw-r--r--   0        0        0     8638 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/search/tests/test_LocalSearch.py
--rw-r--r--   0        0        0     2633 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/search/tests/test_MoveTwoClientsReversed.py
--rw-r--r--   0        0        0     3029 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/search/tests/test_RelocateStar.py
--rw-r--r--   0        0        0     2918 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/search/tests/test_SwapStar.py
--rw-r--r--   0        0        0     3970 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/search/tests/test_TwoOpt.py
--rw-r--r--   0        0        0     6091 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/search/tests/test_neighbourhood.py
--rw-r--r--   0        0        0     1048 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/show_versions.py
--rw-r--r--   0        0        0      444 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/stop/MaxIterations.py
--rw-r--r--   0        0        0      589 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/stop/MaxRuntime.py
--rw-r--r--   0        0        0      819 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/stop/NoImprovement.py
--rw-r--r--   0        0        0      573 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/stop/StoppingCriterion.py
--rw-r--r--   0        0        0      575 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/stop/TimedNoImprovement.py
--rw-r--r--   0        0        0      217 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/stop/__init__.py
--rw-r--r--   0        0        0        0 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/stop/tests/__init__.py
--rw-r--r--   0        0        0      839 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/stop/tests/test_MaxIterations.py
--rw-r--r--   0        0        0     1031 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/stop/tests/test_MaxRuntime.py
--rw-r--r--   0        0        0     1777 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/stop/tests/test_NoImprovement.py
--rw-r--r--   0        0        0     1292 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/stop/tests/test_TimedNoImprovement.py
--rw-r--r--   0        0        0        0 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/__init__.py
--rw-r--r--   0        0        0      189 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/data/DepotNotOne.txt
--rw-r--r--   0        0        0      607 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/data/E-n22-k4.txt
--rw-r--r--   0        0        0      671 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/data/EdgeWeightsNoExplicit.txt
--rw-r--r--   0        0        0      668 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/data/EdgeWeightsNotFullMatrix.txt
--rw-r--r--   0        0        0      389 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/data/FileWithUnknownSection.txt
--rw-r--r--   0        0        0      191 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/data/MoreThanOneDepot.txt
--rw-r--r--   0        0        0      371 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/data/NonZeroDepotDemand.txt
--rw-r--r--   0        0        0      371 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/data/NonZeroDepotOpenTimeWindow.txt
--rw-r--r--   0        0        0      371 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/data/NonZeroDepotReleaseTime.txt
--rw-r--r--   0        0        0      371 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/data/NonZeroDepotServiceDuration.txt
--rw-r--r--   0        0        0      675 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/data/OkSmall.txt
--rw-r--r--   0        0        0      697 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/data/OkSmallGreedyRepair.txt
--rw-r--r--   0        0        0      754 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/data/OkSmallPrizes.txt
--rw-r--r--   0        0        0      744 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/data/OkSmallReleaseTimes.txt
--rw-r--r--   0        0        0      347 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/data/RC208.sol
--rw-r--r--   0        0        0     7524 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/data/RC208.txt
--rw-r--r--   0        0        0      681 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/data/ReallyLargeDistance.txt
--rw-r--r--   0        0        0      369 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/data/TimeWindowOpenLargerThanClose.txt
--rw-r--r--   0        0        0      187 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/data/UnknownEdgeWeightFmt.txt
--rw-r--r--   0        0        0      154 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/data/UnknownEdgeWeightType.txt
--rw-r--r--   0        0        0     2005 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/data/p06-2-50.vrp
--rw-r--r--   0        0        0     1985 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/helpers.py
--rw-r--r--   0        0        0     4674 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/test_CostEvaluator.py
--rw-r--r--   0        0        0     7586 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/test_GeneticAlgorithm.py
--rw-r--r--   0        0        0     1348 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/test_Matrix.py
--rw-r--r--   0        0        0     8491 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/test_Model.py
--rw-r--r--   0        0        0     9864 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/test_PenaltyManager.py
--rw-r--r--   0        0        0    12503 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/test_Population.py
--rw-r--r--   0        0        0     3570 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/test_ProblemData.py
--rw-r--r--   0        0        0     2645 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/test_Result.py
--rw-r--r--   0        0        0    19074 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/test_Solution.py
--rw-r--r--   0        0        0     1134 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/test_Statistics.py
--rw-r--r--   0        0        0     5882 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/test_SubPopulation.py
--rw-r--r--   0        0        0     2240 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/test_TimeWindowSegment.py
--rw-r--r--   0        0        0     1101 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/test_XorShift128.py
--rw-r--r--   0        0        0     7153 2023-07-04 09:33:31.405423 pyvrp-0.4.1/pyvrp/tests/test_read.py
--rw-r--r--   0        0        0     4088 1970-01-01 00:00:00.000000 pyvrp-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1175 2023-07-07 13:06:32.814027 pyvrp-0.4.2/LICENSE
+-rw-r--r--   0        0        0     2963 2023-07-07 13:06:32.814027 pyvrp-0.4.2/README.md
+-rw-r--r--   0        0        0     3563 2023-07-07 13:06:32.814027 pyvrp-0.4.2/build_extensions.py
+-rw-r--r--   0        0        0     3747 2023-07-07 13:06:32.842027 pyvrp-0.4.2/meson.build
+-rw-r--r--   0        0        0      302 2023-07-07 13:06:32.842027 pyvrp-0.4.2/meson_options.txt
+-rw-r--r--   0        0        0     3505 2023-07-07 13:06:32.842027 pyvrp-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     6822 2023-07-07 13:06:32.842027 pyvrp-0.4.2/pyvrp/GeneticAlgorithm.py
+-rw-r--r--   0        0        0     8577 2023-07-07 13:06:32.842027 pyvrp-0.4.2/pyvrp/Model.py
+-rw-r--r--   0        0        0     8807 2023-07-07 13:06:32.842027 pyvrp-0.4.2/pyvrp/PenaltyManager.py
+-rw-r--r--   0        0        0     6608 2023-07-07 13:06:32.842027 pyvrp-0.4.2/pyvrp/Population.py
+-rw-r--r--   0        0        0     2922 2023-07-07 13:06:32.842027 pyvrp-0.4.2/pyvrp/Result.py
+-rw-r--r--   0        0        0     6191 2023-07-07 13:06:32.842027 pyvrp-0.4.2/pyvrp/Statistics.py
+-rw-r--r--   0        0        0     1375 2023-07-07 13:06:32.842027 pyvrp-0.4.2/pyvrp/_CostEvaluator.pyi
+-rw-r--r--   0        0        0      563 2023-07-07 13:06:32.842027 pyvrp-0.4.2/pyvrp/_Matrix.pyi
+-rw-r--r--   0        0        0     5791 2023-07-07 13:06:32.842027 pyvrp-0.4.2/pyvrp/_ProblemData.pyi
+-rw-r--r--   0        0        0     6397 2023-07-07 13:06:32.842027 pyvrp-0.4.2/pyvrp/_Solution.pyi
+-rw-r--r--   0        0        0     4089 2023-07-07 13:06:32.842027 pyvrp-0.4.2/pyvrp/_SubPopulation.pyi
+-rw-r--r--   0        0        0     1664 2023-07-07 13:06:32.842027 pyvrp-0.4.2/pyvrp/_TimeWindowSegment.pyi
+-rw-r--r--   0        0        0      267 2023-07-07 13:06:32.842027 pyvrp-0.4.2/pyvrp/_XorShift128.pyi
+-rw-r--r--   0        0        0      554 2023-07-07 13:06:32.842027 pyvrp-0.4.2/pyvrp/__init__.py
+-rw-r--r--   0        0        0     9091 2023-07-07 13:06:32.842027 pyvrp-0.4.2/pyvrp/cli.py
+-rw-r--r--   0        0        0       45 2023-07-07 13:06:32.842027 pyvrp-0.4.2/pyvrp/constants.py
+-rw-r--r--   0        0        0      854 2023-07-07 13:06:32.842027 pyvrp-0.4.2/pyvrp/cpp/CostEvaluator.cpp
+-rw-r--r--   0        0        0     2039 2023-07-07 13:06:32.842027 pyvrp-0.4.2/pyvrp/cpp/CostEvaluator.h
+-rw-r--r--   0        0        0     1354 2023-07-07 13:06:32.842027 pyvrp-0.4.2/pyvrp/cpp/CostEvaluator_bindings.cpp
+-rw-r--r--   0        0        0     2751 2023-07-07 13:06:32.842027 pyvrp-0.4.2/pyvrp/cpp/Matrix.h
+-rw-r--r--   0        0        0     1041 2023-07-07 13:06:32.842027 pyvrp-0.4.2/pyvrp/cpp/Matrix_bindings.cpp
+-rw-r--r--   0        0        0     5569 2023-07-07 13:06:32.842027 pyvrp-0.4.2/pyvrp/cpp/Measure.h
+-rw-r--r--   0        0        0     2698 2023-07-07 13:06:32.842027 pyvrp-0.4.2/pyvrp/cpp/ProblemData.cpp
+-rw-r--r--   0        0        0     4738 2023-07-07 13:06:32.842027 pyvrp-0.4.2/pyvrp/cpp/ProblemData.h
+-rw-r--r--   0        0        0     5227 2023-07-07 13:06:32.842027 pyvrp-0.4.2/pyvrp/cpp/ProblemData_bindings.cpp
+-rw-r--r--   0        0        0      745 2023-07-07 13:06:32.842027 pyvrp-0.4.2/pyvrp/cpp/README.md
+-rw-r--r--   0        0        0    11014 2023-07-07 13:06:32.842027 pyvrp-0.4.2/pyvrp/cpp/Solution.cpp
+-rw-r--r--   0        0        0     6876 2023-07-07 13:06:32.842027 pyvrp-0.4.2/pyvrp/cpp/Solution.h
+-rw-r--r--   0        0        0     5857 2023-07-07 13:06:32.842027 pyvrp-0.4.2/pyvrp/cpp/Solution_bindings.cpp
+-rw-r--r--   0        0        0     4670 2023-07-07 13:06:32.842027 pyvrp-0.4.2/pyvrp/cpp/SubPopulation.cpp
+-rw-r--r--   0        0        0     3036 2023-07-07 13:06:32.842027 pyvrp-0.4.2/pyvrp/cpp/SubPopulation.h
+-rw-r--r--   0        0        0     2744 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/SubPopulation_bindings.cpp
+-rw-r--r--   0        0        0     3725 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/TimeWindowSegment.h
+-rw-r--r--   0        0        0     1603 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/TimeWindowSegment_bindings.cpp
+-rw-r--r--   0        0        0      581 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/XorShift128.cpp
+-rw-r--r--   0        0        0     2109 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/XorShift128.h
+-rw-r--r--   0        0        0      467 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/XorShift128_bindings.cpp
+-rw-r--r--   0        0        0     5318 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/crossover/crossover.cpp
+-rw-r--r--   0        0        0     2010 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/crossover/crossover.h
+-rw-r--r--   0        0        0     8610 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/crossover/selective_route_exchange.cpp
+-rw-r--r--   0        0        0      375 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/crossover/selective_route_exchange_bindings.cpp
+-rw-r--r--   0        0        0     1003 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/diversity/broken_pairs_distance.cpp
+-rw-r--r--   0        0        0      254 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/diversity/broken_pairs_distance_bindings.cpp
+-rw-r--r--   0        0        0      636 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/diversity/diversity.h
+-rw-r--r--   0        0        0     3048 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/search/CircleSector.h
+-rw-r--r--   0        0        0    11425 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/search/Exchange.h
+-rw-r--r--   0        0        0     2173 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/search/Exchange_bindings.cpp
+-rw-r--r--   0        0        0    14552 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/search/LocalSearch.cpp
+-rw-r--r--   0        0        0     3734 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/search/LocalSearch.h
+-rw-r--r--   0        0        0     2647 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/search/LocalSearchOperator.h
+-rw-r--r--   0        0        0     1329 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/search/LocalSearch_bindings.cpp
+-rw-r--r--   0        0        0     3733 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/search/MoveTwoClientsReversed.cpp
+-rw-r--r--   0        0        0      504 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/search/MoveTwoClientsReversed.h
+-rw-r--r--   0        0        0      482 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/search/MoveTwoClientsReversed_bindings.cpp
+-rw-r--r--   0        0        0      970 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/search/Node.cpp
+-rw-r--r--   0        0        0     1616 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/search/Node.h
+-rw-r--r--   0        0        0     1175 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/search/RelocateStar.cpp
+-rw-r--r--   0        0        0      755 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/search/RelocateStar.h
+-rw-r--r--   0        0        0      436 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/search/RelocateStar_bindings.cpp
+-rw-r--r--   0        0        0     3952 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/search/Route.cpp
+-rw-r--r--   0        0        0     5350 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/search/Route.h
+-rw-r--r--   0        0        0    10975 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/search/SwapStar.cpp
+-rw-r--r--   0        0        0     3399 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/search/SwapStar.h
+-rw-r--r--   0        0        0      420 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/search/SwapStar_bindings.cpp
+-rw-r--r--   0        0        0     4352 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/search/TwoOpt.cpp
+-rw-r--r--   0        0        0      922 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/search/TwoOpt.h
+-rw-r--r--   0        0        0      409 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/search/TwoOpt_bindings.cpp
+-rw-r--r--   0        0        0       63 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/crossover/__init__.py
+-rw-r--r--   0        0        0      364 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/crossover/_selective_route_exchange.pyi
+-rw-r--r--   0        0        0     1949 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/crossover/selective_route_exchange.py
+-rw-r--r--   0        0        0    12528 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/crossover/tests/test_selective_route_exchange.py
+-rw-r--r--   0        0        0       58 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/diversity/__init__.py
+-rw-r--r--   0        0        0     1444 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/diversity/_broken_pairs_distance.pyi
+-rw-r--r--   0        0        0     1171 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/diversity/tests/test_broken_pairs_distance.py
+-rw-r--r--   0        0        0      580 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/exceptions.py
+-rw-r--r--   0        0        0      436 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/plotting/__init__.py
+-rw-r--r--   0        0        0     1106 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/plotting/plot_coordinates.py
+-rw-r--r--   0        0        0     1358 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/plotting/plot_demands.py
+-rw-r--r--   0        0        0     1199 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/plotting/plot_diversity.py
+-rw-r--r--   0        0        0     1129 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/plotting/plot_instance.py
+-rw-r--r--   0        0        0     2344 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/plotting/plot_objectives.py
+-rw-r--r--   0        0        0     1608 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/plotting/plot_result.py
+-rw-r--r--   0        0        0     4690 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/plotting/plot_route_schedule.py
+-rw-r--r--   0        0        0     1136 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/plotting/plot_runtimes.py
+-rw-r--r--   0        0        0     1782 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/plotting/plot_solution.py
+-rw-r--r--   0        0        0     1226 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/plotting/plot_time_windows.py
+-rw-r--r--   0        0        0        0 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/plotting/tests/__init__.py
+-rw-r--r--   0        0        0    47981 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/plotting/tests/baseline_images/test_plotting/plot_instance.png
+-rw-r--r--   0        0        0   141297 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/plotting/tests/baseline_images/test_plotting/plot_result.png
+-rw-r--r--   0        0        0    35194 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/plotting/tests/baseline_images/test_plotting/plot_route_schedule.png
+-rw-r--r--   0        0        0    25609 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/plotting/tests/baseline_images/test_plotting/plot_solution.png
+-rw-r--r--   0        0        0    43058 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/plotting/tests/baseline_images/test_plotting/plot_solution_with_customers.png
+-rw-r--r--   0        0        0     3079 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/plotting/tests/test_plotting.py
+-rw-r--r--   0        0        0     6782 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/read.py
+-rw-r--r--   0        0        0     6559 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/search/LocalSearch.py
+-rw-r--r--   0        0        0      896 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/search/_Exchange.pyi
+-rw-r--r--   0        0        0      891 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/search/_LocalSearch.pyi
+-rw-r--r--   0        0        0      204 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/search/_MoveTwoClientsReversed.pyi
+-rw-r--r--   0        0        0      196 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/search/_RelocateStar.pyi
+-rw-r--r--   0        0        0      192 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/search/_SwapStar.pyi
+-rw-r--r--   0        0        0      188 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/search/_TwoOpt.pyi
+-rw-r--r--   0        0        0      708 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/search/__init__.py
+-rw-r--r--   0        0        0     5149 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/search/neighbourhood.py
+-rw-r--r--   0        0        0        0 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/search/tests/__init__.py
+-rw-r--r--   0        0        0    10470 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/search/tests/test_Exchange.py
+-rw-r--r--   0        0        0     8638 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/search/tests/test_LocalSearch.py
+-rw-r--r--   0        0        0     2633 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/search/tests/test_MoveTwoClientsReversed.py
+-rw-r--r--   0        0        0     3029 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/search/tests/test_RelocateStar.py
+-rw-r--r--   0        0        0     2918 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/search/tests/test_SwapStar.py
+-rw-r--r--   0        0        0     3970 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/search/tests/test_TwoOpt.py
+-rw-r--r--   0        0        0     6091 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/search/tests/test_neighbourhood.py
+-rw-r--r--   0        0        0     1048 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/show_versions.py
+-rw-r--r--   0        0        0      444 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/stop/MaxIterations.py
+-rw-r--r--   0        0        0      589 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/stop/MaxRuntime.py
+-rw-r--r--   0        0        0      819 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/stop/NoImprovement.py
+-rw-r--r--   0        0        0      573 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/stop/StoppingCriterion.py
+-rw-r--r--   0        0        0      575 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/stop/TimedNoImprovement.py
+-rw-r--r--   0        0        0      217 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/stop/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/stop/tests/__init__.py
+-rw-r--r--   0        0        0      839 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/stop/tests/test_MaxIterations.py
+-rw-r--r--   0        0        0     1031 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/stop/tests/test_MaxRuntime.py
+-rw-r--r--   0        0        0     1777 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/stop/tests/test_NoImprovement.py
+-rw-r--r--   0        0        0     1292 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/stop/tests/test_TimedNoImprovement.py
+-rw-r--r--   0        0        0        0 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/__init__.py
+-rw-r--r--   0        0        0      189 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/data/DepotNotOne.txt
+-rw-r--r--   0        0        0      607 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/data/E-n22-k4.txt
+-rw-r--r--   0        0        0      671 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/data/EdgeWeightsNoExplicit.txt
+-rw-r--r--   0        0        0      668 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/data/EdgeWeightsNotFullMatrix.txt
+-rw-r--r--   0        0        0      389 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/data/FileWithUnknownSection.txt
+-rw-r--r--   0        0        0      191 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/data/MoreThanOneDepot.txt
+-rw-r--r--   0        0        0      371 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/data/NonZeroDepotDemand.txt
+-rw-r--r--   0        0        0      371 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/data/NonZeroDepotOpenTimeWindow.txt
+-rw-r--r--   0        0        0      371 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/data/NonZeroDepotReleaseTime.txt
+-rw-r--r--   0        0        0      371 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/data/NonZeroDepotServiceDuration.txt
+-rw-r--r--   0        0        0      675 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/data/OkSmall.txt
+-rw-r--r--   0        0        0      697 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/data/OkSmallGreedyRepair.txt
+-rw-r--r--   0        0        0      754 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/data/OkSmallPrizes.txt
+-rw-r--r--   0        0        0      744 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/data/OkSmallReleaseTimes.txt
+-rw-r--r--   0        0        0      347 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/data/RC208.sol
+-rw-r--r--   0        0        0     7524 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/data/RC208.txt
+-rw-r--r--   0        0        0      681 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/data/ReallyLargeDistance.txt
+-rw-r--r--   0        0        0      369 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/data/TimeWindowOpenLargerThanClose.txt
+-rw-r--r--   0        0        0      187 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/data/UnknownEdgeWeightFmt.txt
+-rw-r--r--   0        0        0      154 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/data/UnknownEdgeWeightType.txt
+-rw-r--r--   0        0        0     2005 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/data/p06-2-50.vrp
+-rw-r--r--   0        0        0     1985 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/helpers.py
+-rw-r--r--   0        0        0     4674 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/test_CostEvaluator.py
+-rw-r--r--   0        0        0     7586 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/test_GeneticAlgorithm.py
+-rw-r--r--   0        0        0     1348 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/test_Matrix.py
+-rw-r--r--   0        0        0     8491 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/test_Model.py
+-rw-r--r--   0        0        0     9864 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/test_PenaltyManager.py
+-rw-r--r--   0        0        0    12503 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/test_Population.py
+-rw-r--r--   0        0        0     3570 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/test_ProblemData.py
+-rw-r--r--   0        0        0     2645 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/test_Result.py
+-rw-r--r--   0        0        0    19074 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/test_Solution.py
+-rw-r--r--   0        0        0     1134 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/test_Statistics.py
+-rw-r--r--   0        0        0     5882 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/test_SubPopulation.py
+-rw-r--r--   0        0        0     2240 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/test_TimeWindowSegment.py
+-rw-r--r--   0        0        0     1101 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/test_XorShift128.py
+-rw-r--r--   0        0        0     7153 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/test_read.py
+-rw-r--r--   0        0        0     4088 1970-01-01 00:00:00.000000 pyvrp-0.4.2/PKG-INFO
```

### Comparing `pyvrp-0.4.1/LICENSE` & `pyvrp-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/README.md` & `pyvrp-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/build_extensions.py` & `pyvrp-0.4.2/build_extensions.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/meson.build` & `pyvrp-0.4.2/meson.build`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyproject.toml` & `pyvrp-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyvrp"
-version = "0.4.1"
+version = "0.4.2"
 description = "A state-of-the-art vehicle routing problem solver."
 authors = [
     "Niels Wouda <nielswouda@gmail.com>",
     "Leon Lan <leon.lanyidong@gmail.com>",
     "Wouter Kool <wouter.kool@ortec.com>",
 ]
 license = "MIT"
```

### Comparing `pyvrp-0.4.1/pyvrp/GeneticAlgorithm.py` & `pyvrp-0.4.2/pyvrp/GeneticAlgorithm.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/Model.py` & `pyvrp-0.4.2/pyvrp/Model.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/PenaltyManager.py` & `pyvrp-0.4.2/pyvrp/PenaltyManager.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/Population.py` & `pyvrp-0.4.2/pyvrp/Population.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/Result.py` & `pyvrp-0.4.2/pyvrp/Result.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/Statistics.py` & `pyvrp-0.4.2/pyvrp/Statistics.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/_CostEvaluator.pyi` & `pyvrp-0.4.2/pyvrp/_CostEvaluator.pyi`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/_Matrix.pyi` & `pyvrp-0.4.2/pyvrp/_Matrix.pyi`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/_ProblemData.pyi` & `pyvrp-0.4.2/pyvrp/_ProblemData.pyi`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/_Solution.pyi` & `pyvrp-0.4.2/pyvrp/_Solution.pyi`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/_SubPopulation.pyi` & `pyvrp-0.4.2/pyvrp/_SubPopulation.pyi`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/_TimeWindowSegment.pyi` & `pyvrp-0.4.2/pyvrp/_TimeWindowSegment.pyi`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/__init__.py` & `pyvrp-0.4.2/pyvrp/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/cli.py` & `pyvrp-0.4.2/pyvrp/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from pathlib import Path
 from typing import List, Optional
 
 import numpy as np
 
 try:
     import tomli
+    from tqdm import tqdm
     from tqdm.contrib.concurrent import process_map
 except ModuleNotFoundError:
     msg = "Install 'tqdm' and 'tomli' to use the command line program."
     raise ModuleNotFoundError(msg)
 
 import pyvrp.search
 from pyvrp import (
@@ -193,47 +194,48 @@
         "Y" if res.is_feasible() else "N",
         round(res.cost(), 2),
         res.num_iterations,
         round(res.runtime, 3),
     )
 
 
-def benchmark(instances: List[str], **kwargs):
+def benchmark(instances: List[str], num_procs: int = 1, **kwargs):
     """
     Solves a list of instances, and prints a table with the results. Any
     additional keyword arguments are passed to ``solve()``.
 
     Parameters
     ----------
     instances
         Paths to the VRPLIB instances to solve.
+    num_procs
+        Number of processors to use. Default 1.
+    kwargs
+        Any additional keyword arguments to pass to the solving function.
     """
     maybe_mkdir(kwargs.get("stats_dir", ""))
     maybe_mkdir(kwargs.get("sol_dir", ""))
 
-    if len(instances) == 1:
-        res = solve(instances[0], **kwargs)
-        print(res)
-        return
-
     func = partial(benchmark_solve, **kwargs)
-    func_args = sorted(instances)
+    args = sorted(instances)
 
-    tqdm_kwargs = dict(max_workers=kwargs.get("num_procs", 1), unit="instance")
-    data = process_map(func, func_args, **tqdm_kwargs)
+    if len(instances) == 1 or num_procs == 1:
+        res = [func(arg) for arg in tqdm(args, unit="instance")]
+    else:
+        res = process_map(func, args, max_workers=num_procs, unit="instance")
 
     dtypes = [
         ("inst", "U37"),
         ("ok", "U1"),
         ("obj", float),
         ("iters", int),
         ("time", float),
     ]
 
-    data = np.asarray(data, dtype=dtypes)
+    data = np.asarray(res, dtype=dtypes)
     headers = ["Instance", "OK", "Obj.", "Iters. (#)", "Time (s)"]
 
     print("\n", tabulate(headers, data), "\n", sep="")
     print(f"      Avg. objective: {data['obj'].mean():.0f}")
     print(f"     Avg. iterations: {data['iters'].mean():.0f}")
     print(f"   Avg. run-time (s): {data['time'].mean():.2f}")
     print(f"        Total not OK: {np.count_nonzero(data['ok'] == 'N')}")
```

### Comparing `pyvrp-0.4.1/pyvrp/cpp/CostEvaluator.cpp` & `pyvrp-0.4.2/pyvrp/cpp/CostEvaluator.cpp`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/cpp/CostEvaluator.h` & `pyvrp-0.4.2/pyvrp/cpp/CostEvaluator.h`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/cpp/CostEvaluator_bindings.cpp` & `pyvrp-0.4.2/pyvrp/cpp/CostEvaluator_bindings.cpp`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/cpp/Matrix.h` & `pyvrp-0.4.2/pyvrp/cpp/Matrix.h`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/cpp/Matrix_bindings.cpp` & `pyvrp-0.4.2/pyvrp/cpp/Matrix_bindings.cpp`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/cpp/Measure.h` & `pyvrp-0.4.2/pyvrp/cpp/Measure.h`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/cpp/ProblemData.cpp` & `pyvrp-0.4.2/pyvrp/cpp/ProblemData.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #include "ProblemData.h"
 
 #include <cmath>
 #include <fstream>
+#include <numeric>
 #include <sstream>
 #include <string>
 #include <vector>
 
 ProblemData::Client::Client(Coordinate x,
                             Coordinate y,
                             Load demand,
@@ -62,18 +63,20 @@
     : centroid_({0, 0}),
       dist_(std::move(distMat)),
       dur_(std::move(durMat)),
       clients_(clients),
       vehicleTypes_(vehicleTypes),
       numClients_(std::max<size_t>(clients.size(), 1) - 1),
       numVehicleTypes_(vehicleTypes.size()),
-      numVehicles_(0)
+      numVehicles_(std::accumulate(vehicleTypes.begin(),
+                                   vehicleTypes.end(),
+                                   0,
+                                   [](auto sum, VehicleType const &type) {
+                                       return sum + type.numAvailable;
+                                   }))
 {
-    for (auto const &vehicleType : vehicleTypes)
-        numVehicles_ += vehicleType.numAvailable;
-
     for (size_t idx = 1; idx <= numClients(); ++idx)
     {
         centroid_.first += static_cast<double>(clients[idx].x) / numClients();
         centroid_.second += static_cast<double>(clients[idx].y) / numClients();
     }
 }
```

### Comparing `pyvrp-0.4.1/pyvrp/cpp/ProblemData.h` & `pyvrp-0.4.2/pyvrp/cpp/ProblemData.h`

 * *Files 2% similar despite different names*

```diff
@@ -32,28 +32,28 @@
                Duration releaseTime = 0,
                Cost prize = 0,
                bool required = true);
     };
 
     struct VehicleType
     {
-        Load capacity;        // Capacity (max total demand) of the vehicle
-        size_t numAvailable;  // Number of available vehicles of this type
+        Load const capacity;        // This type's vehicle capacity
+        size_t const numAvailable;  // Available vehicles of this type
     };
 
 private:
-    std::pair<double, double> centroid_;     // Centroid of client locations
-    Matrix<Distance> const dist_;            // Distance matrix (+depot)
-    Matrix<Duration> const dur_;             // Duration matrix (+depot)
-    std::vector<Client> clients_;            // Client (+depot) information
-    std::vector<VehicleType> vehicleTypes_;  // Vehicle type information
+    std::pair<double, double> centroid_;           // Center of client locations
+    Matrix<Distance> const dist_;                  // Distance matrix
+    Matrix<Duration> const dur_;                   // Duration matrix
+    std::vector<Client> const clients_;            // Client/depot information
+    std::vector<VehicleType> const vehicleTypes_;  // Vehicle type information
 
     size_t const numClients_;
     size_t const numVehicleTypes_;
-    size_t numVehicles_;  // Number of vehicles - derived from vehicle types
+    size_t const numVehicles_;
 
 public:
     /**
      * @param client Client whose data to return.
      * @return A struct containing the indicated client's information.
      */
     [[nodiscard]] inline Client const &client(size_t client) const;
```

### Comparing `pyvrp-0.4.1/pyvrp/cpp/ProblemData_bindings.cpp` & `pyvrp-0.4.2/pyvrp/cpp/ProblemData_bindings.cpp`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/cpp/README.md` & `pyvrp-0.4.2/pyvrp/cpp/README.md`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/cpp/Solution.cpp` & `pyvrp-0.4.2/pyvrp/cpp/Solution.cpp`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/cpp/Solution.h` & `pyvrp-0.4.2/pyvrp/cpp/Solution.h`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 
 #include <functional>
 #include <iosfwd>
 #include <vector>
 
 class Solution
 {
-    friend struct std::hash<Solution>;  // friend struct to enable hashing
-
     using Client = int;
     using VehicleType = size_t;
 
 public:
     /**
      * A simple Route class that contains the route plan and some statistics.
      */
@@ -200,18 +198,18 @@
 namespace std
 {
 template <> struct hash<Solution>
 {
     size_t operator()(Solution const &sol) const
     {
         size_t res = 17;
-        res = res * 31 + std::hash<size_t>()(sol.routes_.size());
-        res = res * 31 + std::hash<Distance>()(sol.distance_);
-        res = res * 31 + std::hash<Load>()(sol.excessLoad_);
-        res = res * 31 + std::hash<Duration>()(sol.timeWarp_);
+        res = res * 31 + std::hash<size_t>()(sol.numRoutes());
+        res = res * 31 + std::hash<Distance>()(sol.distance());
+        res = res * 31 + std::hash<Load>()(sol.excessLoad());
+        res = res * 31 + std::hash<Duration>()(sol.timeWarp());
 
         return res;
     }
 };
 }  // namespace std
 
 #endif  // PYVRP_SOLUTION_H
```

### Comparing `pyvrp-0.4.1/pyvrp/cpp/Solution_bindings.cpp` & `pyvrp-0.4.2/pyvrp/cpp/Solution_bindings.cpp`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/cpp/SubPopulation.cpp` & `pyvrp-0.4.2/pyvrp/cpp/SubPopulation.cpp`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/cpp/SubPopulation.h` & `pyvrp-0.4.2/pyvrp/cpp/SubPopulation.h`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/cpp/SubPopulation_bindings.cpp` & `pyvrp-0.4.2/pyvrp/cpp/SubPopulation_bindings.cpp`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/cpp/TimeWindowSegment.h` & `pyvrp-0.4.2/pyvrp/cpp/TimeWindowSegment.h`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/cpp/TimeWindowSegment_bindings.cpp` & `pyvrp-0.4.2/pyvrp/cpp/TimeWindowSegment_bindings.cpp`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/cpp/XorShift128.cpp` & `pyvrp-0.4.2/pyvrp/cpp/XorShift128.cpp`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/cpp/XorShift128.h` & `pyvrp-0.4.2/pyvrp/cpp/XorShift128.h`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/cpp/crossover/crossover.cpp` & `pyvrp-0.4.2/pyvrp/cpp/crossover/crossover.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -98,46 +98,46 @@
             {
                 bestRouteIdx = rIdx;
                 bestDistance = distance;
             }
         }
 
         // Find best insertion point in selected route.
-        auto &bestRoute = routes[bestRouteIdx];
         Cost bestCost = std::numeric_limits<Cost>::max();
+        auto &route = routes[bestRouteIdx];
         auto offset = 0;
-        for (size_t idx = 0; idx <= bestRoute.size(); ++idx)
+        for (size_t idx = 0; idx <= route.size() && !route.empty(); ++idx)
         {
             Client prev, next;
 
             if (idx == 0)  // try after depot
             {
                 prev = 0;
-                next = bestRoute[0];
+                next = route[0];
             }
-            else if (idx == bestRoute.size())  // try before depot
+            else if (idx == route.size())  // try before depot
             {
-                prev = bestRoute.back();
+                prev = route.back();
                 next = 0;
             }
             else  // try between [idx - 1] and [idx]
             {
-                prev = bestRoute[idx - 1];
-                next = bestRoute[idx];
+                prev = route[idx - 1];
+                next = route[idx];
             }
 
             auto cost = deltaCost(client, prev, next, data, costEvaluator);
             if (cost < bestCost)
             {
                 bestCost = cost;
                 offset = idx;
             }
         }
 
         // Update route centroid and insert client into route.
-        auto const size = static_cast<double>(bestRoute.size());
+        auto const size = static_cast<double>(route.size());
         auto const [routeX, routeY] = centroids[bestRouteIdx];
         centroids[bestRouteIdx].first = (routeX * size + x) / (size + 1);
         centroids[bestRouteIdx].second = (routeY * size + y) / (size + 1);
-        bestRoute.insert(bestRoute.begin() + offset, client);
+        route.insert(route.begin() + offset, client);
     }
 }
```

### Comparing `pyvrp-0.4.1/pyvrp/cpp/crossover/crossover.h` & `pyvrp-0.4.2/pyvrp/cpp/crossover/crossover.h`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/cpp/crossover/selective_route_exchange.cpp` & `pyvrp-0.4.2/pyvrp/cpp/crossover/selective_route_exchange.cpp`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/cpp/diversity/broken_pairs_distance.cpp` & `pyvrp-0.4.2/pyvrp/cpp/diversity/broken_pairs_distance.cpp`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/cpp/diversity/diversity.h` & `pyvrp-0.4.2/pyvrp/cpp/diversity/diversity.h`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/cpp/search/CircleSector.h` & `pyvrp-0.4.2/pyvrp/cpp/search/CircleSector.h`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/cpp/search/Exchange.h` & `pyvrp-0.4.2/pyvrp/cpp/search/Exchange.h`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/cpp/search/Exchange_bindings.cpp` & `pyvrp-0.4.2/pyvrp/cpp/search/Exchange_bindings.cpp`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/cpp/search/LocalSearch.cpp` & `pyvrp-0.4.2/pyvrp/cpp/search/LocalSearch.cpp`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/cpp/search/LocalSearch.h` & `pyvrp-0.4.2/pyvrp/cpp/search/LocalSearch.h`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/cpp/search/LocalSearchOperator.h` & `pyvrp-0.4.2/pyvrp/cpp/search/LocalSearchOperator.h`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/cpp/search/LocalSearch_bindings.cpp` & `pyvrp-0.4.2/pyvrp/cpp/search/LocalSearch_bindings.cpp`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/cpp/search/MoveTwoClientsReversed.cpp` & `pyvrp-0.4.2/pyvrp/cpp/search/MoveTwoClientsReversed.cpp`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/cpp/search/Node.cpp` & `pyvrp-0.4.2/pyvrp/cpp/search/Node.cpp`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/cpp/search/Node.h` & `pyvrp-0.4.2/pyvrp/cpp/search/Node.h`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/cpp/search/RelocateStar.cpp` & `pyvrp-0.4.2/pyvrp/cpp/search/RelocateStar.cpp`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/cpp/search/RelocateStar.h` & `pyvrp-0.4.2/pyvrp/cpp/search/RelocateStar.h`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/cpp/search/Route.cpp` & `pyvrp-0.4.2/pyvrp/cpp/search/Route.cpp`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/cpp/search/Route.h` & `pyvrp-0.4.2/pyvrp/cpp/search/Route.h`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/cpp/search/SwapStar.cpp` & `pyvrp-0.4.2/pyvrp/cpp/search/SwapStar.cpp`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/cpp/search/SwapStar.h` & `pyvrp-0.4.2/pyvrp/cpp/search/SwapStar.h`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/cpp/search/TwoOpt.cpp` & `pyvrp-0.4.2/pyvrp/cpp/search/TwoOpt.cpp`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/cpp/search/TwoOpt.h` & `pyvrp-0.4.2/pyvrp/cpp/search/TwoOpt.h`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/crossover/selective_route_exchange.py` & `pyvrp-0.4.2/pyvrp/crossover/selective_route_exchange.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/crossover/tests/test_selective_route_exchange.py` & `pyvrp-0.4.2/pyvrp/crossover/tests/test_selective_route_exchange.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/diversity/_broken_pairs_distance.pyi` & `pyvrp-0.4.2/pyvrp/diversity/_broken_pairs_distance.pyi`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/diversity/tests/test_broken_pairs_distance.py` & `pyvrp-0.4.2/pyvrp/diversity/tests/test_broken_pairs_distance.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/exceptions.py` & `pyvrp-0.4.2/pyvrp/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/plotting/plot_coordinates.py` & `pyvrp-0.4.2/pyvrp/plotting/plot_coordinates.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/plotting/plot_demands.py` & `pyvrp-0.4.2/pyvrp/plotting/plot_demands.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/plotting/plot_diversity.py` & `pyvrp-0.4.2/pyvrp/plotting/plot_diversity.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/plotting/plot_instance.py` & `pyvrp-0.4.2/pyvrp/plotting/plot_instance.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/plotting/plot_objectives.py` & `pyvrp-0.4.2/pyvrp/plotting/plot_objectives.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/plotting/plot_result.py` & `pyvrp-0.4.2/pyvrp/plotting/plot_result.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/plotting/plot_route_schedule.py` & `pyvrp-0.4.2/pyvrp/plotting/plot_route_schedule.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/plotting/plot_runtimes.py` & `pyvrp-0.4.2/pyvrp/plotting/plot_runtimes.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/plotting/plot_solution.py` & `pyvrp-0.4.2/pyvrp/plotting/plot_solution.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/plotting/plot_time_windows.py` & `pyvrp-0.4.2/pyvrp/plotting/plot_time_windows.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/plotting/tests/baseline_images/test_plotting/plot_instance.png` & `pyvrp-0.4.2/pyvrp/plotting/tests/baseline_images/test_plotting/plot_instance.png`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/plotting/tests/baseline_images/test_plotting/plot_result.png` & `pyvrp-0.4.2/pyvrp/plotting/tests/baseline_images/test_plotting/plot_result.png`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/plotting/tests/baseline_images/test_plotting/plot_route_schedule.png` & `pyvrp-0.4.2/pyvrp/plotting/tests/baseline_images/test_plotting/plot_route_schedule.png`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/plotting/tests/baseline_images/test_plotting/plot_solution.png` & `pyvrp-0.4.2/pyvrp/plotting/tests/baseline_images/test_plotting/plot_solution.png`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/plotting/tests/baseline_images/test_plotting/plot_solution_with_customers.png` & `pyvrp-0.4.2/pyvrp/plotting/tests/baseline_images/test_plotting/plot_solution_with_customers.png`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/plotting/tests/test_plotting.py` & `pyvrp-0.4.2/pyvrp/plotting/tests/test_plotting.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/read.py` & `pyvrp-0.4.2/pyvrp/read.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/search/LocalSearch.py` & `pyvrp-0.4.2/pyvrp/search/LocalSearch.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/search/_Exchange.pyi` & `pyvrp-0.4.2/pyvrp/search/_Exchange.pyi`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/search/_LocalSearch.pyi` & `pyvrp-0.4.2/pyvrp/search/_LocalSearch.pyi`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/search/__init__.py` & `pyvrp-0.4.2/pyvrp/search/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/search/neighbourhood.py` & `pyvrp-0.4.2/pyvrp/search/neighbourhood.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/search/tests/test_Exchange.py` & `pyvrp-0.4.2/pyvrp/search/tests/test_Exchange.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/search/tests/test_LocalSearch.py` & `pyvrp-0.4.2/pyvrp/search/tests/test_LocalSearch.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/search/tests/test_MoveTwoClientsReversed.py` & `pyvrp-0.4.2/pyvrp/search/tests/test_MoveTwoClientsReversed.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/search/tests/test_RelocateStar.py` & `pyvrp-0.4.2/pyvrp/search/tests/test_RelocateStar.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/search/tests/test_SwapStar.py` & `pyvrp-0.4.2/pyvrp/search/tests/test_SwapStar.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/search/tests/test_TwoOpt.py` & `pyvrp-0.4.2/pyvrp/search/tests/test_TwoOpt.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/search/tests/test_neighbourhood.py` & `pyvrp-0.4.2/pyvrp/search/tests/test_neighbourhood.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/show_versions.py` & `pyvrp-0.4.2/pyvrp/show_versions.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/stop/MaxRuntime.py` & `pyvrp-0.4.2/pyvrp/stop/MaxRuntime.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/stop/NoImprovement.py` & `pyvrp-0.4.2/pyvrp/stop/NoImprovement.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/stop/StoppingCriterion.py` & `pyvrp-0.4.2/pyvrp/stop/StoppingCriterion.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/stop/TimedNoImprovement.py` & `pyvrp-0.4.2/pyvrp/stop/TimedNoImprovement.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/stop/tests/test_MaxIterations.py` & `pyvrp-0.4.2/pyvrp/stop/tests/test_MaxIterations.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/stop/tests/test_MaxRuntime.py` & `pyvrp-0.4.2/pyvrp/stop/tests/test_MaxRuntime.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/stop/tests/test_NoImprovement.py` & `pyvrp-0.4.2/pyvrp/stop/tests/test_NoImprovement.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/stop/tests/test_TimedNoImprovement.py` & `pyvrp-0.4.2/pyvrp/stop/tests/test_TimedNoImprovement.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/tests/data/E-n22-k4.txt` & `pyvrp-0.4.2/pyvrp/tests/data/E-n22-k4.txt`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/tests/data/EdgeWeightsNoExplicit.txt` & `pyvrp-0.4.2/pyvrp/tests/data/EdgeWeightsNoExplicit.txt`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/tests/data/EdgeWeightsNotFullMatrix.txt` & `pyvrp-0.4.2/pyvrp/tests/data/EdgeWeightsNotFullMatrix.txt`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/tests/data/OkSmall.txt` & `pyvrp-0.4.2/pyvrp/tests/data/OkSmall.txt`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/tests/data/OkSmallGreedyRepair.txt` & `pyvrp-0.4.2/pyvrp/tests/data/OkSmallGreedyRepair.txt`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/tests/data/OkSmallPrizes.txt` & `pyvrp-0.4.2/pyvrp/tests/data/OkSmallPrizes.txt`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/tests/data/OkSmallReleaseTimes.txt` & `pyvrp-0.4.2/pyvrp/tests/data/OkSmallReleaseTimes.txt`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/tests/data/RC208.txt` & `pyvrp-0.4.2/pyvrp/tests/data/RC208.txt`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/tests/data/ReallyLargeDistance.txt` & `pyvrp-0.4.2/pyvrp/tests/data/ReallyLargeDistance.txt`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/tests/data/p06-2-50.vrp` & `pyvrp-0.4.2/pyvrp/tests/data/p06-2-50.vrp`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/tests/helpers.py` & `pyvrp-0.4.2/pyvrp/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/tests/test_CostEvaluator.py` & `pyvrp-0.4.2/pyvrp/tests/test_CostEvaluator.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/tests/test_GeneticAlgorithm.py` & `pyvrp-0.4.2/pyvrp/tests/test_GeneticAlgorithm.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/tests/test_Matrix.py` & `pyvrp-0.4.2/pyvrp/tests/test_Matrix.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/tests/test_Model.py` & `pyvrp-0.4.2/pyvrp/tests/test_Model.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/tests/test_PenaltyManager.py` & `pyvrp-0.4.2/pyvrp/tests/test_PenaltyManager.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/tests/test_Population.py` & `pyvrp-0.4.2/pyvrp/tests/test_Population.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/tests/test_ProblemData.py` & `pyvrp-0.4.2/pyvrp/tests/test_ProblemData.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/tests/test_Result.py` & `pyvrp-0.4.2/pyvrp/tests/test_Result.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/tests/test_Solution.py` & `pyvrp-0.4.2/pyvrp/tests/test_Solution.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/tests/test_Statistics.py` & `pyvrp-0.4.2/pyvrp/tests/test_Statistics.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/tests/test_SubPopulation.py` & `pyvrp-0.4.2/pyvrp/tests/test_SubPopulation.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/tests/test_TimeWindowSegment.py` & `pyvrp-0.4.2/pyvrp/tests/test_TimeWindowSegment.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/tests/test_XorShift128.py` & `pyvrp-0.4.2/pyvrp/tests/test_XorShift128.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/pyvrp/tests/test_read.py` & `pyvrp-0.4.2/pyvrp/tests/test_read.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.1/PKG-INFO` & `pyvrp-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvrp
-Version: 0.4.1
+Version: 0.4.2
 Summary: A state-of-the-art vehicle routing problem solver.
 Home-page: https://github.com/PyVRP/PyVRP
 License: MIT
 Author: Niels Wouda
 Author-email: nielswouda@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

