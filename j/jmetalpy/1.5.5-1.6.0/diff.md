# Comparing `tmp/jmetalpy-1.5.5.tar.gz` & `tmp/jmetalpy-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jmetalpy-1.5.5.tar", last modified: Thu Apr  9 12:56:49 2020, max compression
+gzip compressed data, was "jmetalpy-1.6.0.tar", last modified: Wed Apr 19 14:32:18 2023, max compression
```

## Comparing `jmetalpy-1.5.5.tar` & `jmetalpy-1.6.0.tar`

### file list

```diff
@@ -1,238 +1,251 @@
-drwxr-xr-x   0 benhid     (501) staff       (20)        0 2020-04-09 12:56:49.000000 jmetalpy-1.5.5/
--rw-r--r--   0 benhid     (501) staff       (20)     7097 2020-04-09 12:56:49.000000 jmetalpy-1.5.5/PKG-INFO
--rw-r--r--   0 benhid     (501) staff       (20)     5328 2020-04-09 12:56:45.000000 jmetalpy-1.5.5/README.md
-drwxr-xr-x   0 benhid     (501) staff       (20)        0 2020-04-09 12:56:49.000000 jmetalpy-1.5.5/examples/
--rw-r--r--   0 benhid     (501) staff       (20)        0 2019-10-13 12:34:24.000000 jmetalpy-1.5.5/examples/__init__.py
-drwxr-xr-x   0 benhid     (501) staff       (20)        0 2020-04-09 12:56:49.000000 jmetalpy-1.5.5/examples/experiment/
--rw-r--r--   0 benhid     (501) staff       (20)        0 2019-10-13 12:34:24.000000 jmetalpy-1.5.5/examples/experiment/__init__.py
--rw-r--r--   0 benhid     (501) staff       (20)     3226 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/examples/experiment/comparison.py
--rw-r--r--   0 benhid     (501) staff       (20)     2817 2019-10-13 12:34:24.000000 jmetalpy-1.5.5/examples/experiment/statistical_analysis.py
-drwxr-xr-x   0 benhid     (501) staff       (20)        0 2020-04-09 12:56:49.000000 jmetalpy-1.5.5/examples/multiobjective/
--rw-r--r--   0 benhid     (501) staff       (20)        0 2019-10-13 12:34:24.000000 jmetalpy-1.5.5/examples/multiobjective/__init__.py
-drwxr-xr-x   0 benhid     (501) staff       (20)        0 2020-04-09 12:56:49.000000 jmetalpy-1.5.5/examples/multiobjective/gde3/
--rw-r--r--   0 benhid     (501) staff       (20)        0 2020-01-08 13:20:59.000000 jmetalpy-1.5.5/examples/multiobjective/gde3/__init__.py
--rw-r--r--   0 benhid     (501) staff       (20)      862 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/examples/multiobjective/gde3/dynamic_gde3.py
--rw-r--r--   0 benhid     (501) staff       (20)     1066 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/examples/multiobjective/gde3/gde3_spark_evaluator.py
--rw-r--r--   0 benhid     (501) staff       (20)      930 2020-01-08 13:20:59.000000 jmetalpy-1.5.5/examples/multiobjective/gde3/gde3_zdt1.py
--rw-r--r--   0 benhid     (501) staff       (20)     1153 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/examples/multiobjective/gde3/ggde3_zdt2.py
-drwxr-xr-x   0 benhid     (501) staff       (20)        0 2020-04-09 12:56:49.000000 jmetalpy-1.5.5/examples/multiobjective/hype/
--rw-r--r--   0 benhid     (501) staff       (20)        0 2020-01-08 13:20:59.000000 jmetalpy-1.5.5/examples/multiobjective/hype/__init__.py
--rw-r--r--   0 benhid     (501) staff       (20)     1420 2020-01-08 13:20:59.000000 jmetalpy-1.5.5/examples/multiobjective/hype/hype_zdt1.py
-drwxr-xr-x   0 benhid     (501) staff       (20)        0 2020-04-09 12:56:49.000000 jmetalpy-1.5.5/examples/multiobjective/ibea/
--rw-r--r--   0 benhid     (501) staff       (20)        0 2020-01-08 13:20:59.000000 jmetalpy-1.5.5/examples/multiobjective/ibea/__init__.py
--rw-r--r--   0 benhid     (501) staff       (20)     1223 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/examples/multiobjective/ibea/ibea_zdt1.py
-drwxr-xr-x   0 benhid     (501) staff       (20)        0 2020-04-09 12:56:49.000000 jmetalpy-1.5.5/examples/multiobjective/mocell/
--rw-r--r--   0 benhid     (501) staff       (20)        0 2020-01-08 13:20:59.000000 jmetalpy-1.5.5/examples/multiobjective/mocell/__init__.py
--rw-r--r--   0 benhid     (501) staff       (20)     1423 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/examples/multiobjective/mocell/mocell_zdt1.py
-drwxr-xr-x   0 benhid     (501) staff       (20)        0 2020-04-09 12:56:49.000000 jmetalpy-1.5.5/examples/multiobjective/moead/
--rw-r--r--   0 benhid     (501) staff       (20)        0 2020-01-08 13:20:59.000000 jmetalpy-1.5.5/examples/multiobjective/moead/__init__.py
--rw-r--r--   0 benhid     (501) staff       (20)     1774 2020-04-09 12:56:45.000000 jmetalpy-1.5.5/examples/multiobjective/moead/moead_dtlz2.py
--rw-r--r--   0 benhid     (501) staff       (20)     1585 2020-04-09 12:56:45.000000 jmetalpy-1.5.5/examples/multiobjective/moead/moead_iepsilon_lircmop1.py
--rw-r--r--   0 benhid     (501) staff       (20)     1543 2020-04-09 12:56:45.000000 jmetalpy-1.5.5/examples/multiobjective/moead/moead_lz09.py
--rw-r--r--   0 benhid     (501) staff       (20)     1824 2020-04-09 12:56:45.000000 jmetalpy-1.5.5/examples/multiobjective/moead/moeaddra_lz09.py
-drwxr-xr-x   0 benhid     (501) staff       (20)        0 2020-04-09 12:56:49.000000 jmetalpy-1.5.5/examples/multiobjective/nsgaii/
--rw-r--r--   0 benhid     (501) staff       (20)        0 2020-01-08 13:20:59.000000 jmetalpy-1.5.5/examples/multiobjective/nsgaii/__init__.py
--rw-r--r--   0 benhid     (501) staff       (20)     1302 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/examples/multiobjective/nsgaii/distributed_nsgaii_with_dask.py
--rw-r--r--   0 benhid     (501) staff       (20)     1335 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/examples/multiobjective/nsgaii/distributed_nsgaii_with_dask_evaluator.py
--rw-r--r--   0 benhid     (501) staff       (20)     1345 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/examples/multiobjective/nsgaii/distributed_nsgaii_with_spark_evaluator.py
--rw-r--r--   0 benhid     (501) staff       (20)     1156 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/examples/multiobjective/nsgaii/dynamic_nsgaii_solving_fda2.py
--rw-r--r--   0 benhid     (501) staff       (20)     2532 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/examples/multiobjective/nsgaii/gnsgaii_solving_zdt2_with_reference_point.py
--rw-r--r--   0 benhid     (501) staff       (20)     1775 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/examples/multiobjective/nsgaii/nsgaii_defining_schaffer_problem_on_the_fly.py
--rw-r--r--   0 benhid     (501) staff       (20)     2086 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/examples/multiobjective/nsgaii/nsgaii_defining_srinivas_problem_on_the_fly.py
--rw-r--r--   0 benhid     (501) staff       (20)     1362 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/examples/multiobjective/nsgaii/nsgaii_solving_3D_problem.py
--rw-r--r--   0 benhid     (501) staff       (20)     1414 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/examples/multiobjective/nsgaii/nsgaii_solving_binary_problem.py
--rw-r--r--   0 benhid     (501) staff       (20)     1361 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/examples/multiobjective/nsgaii/nsgaii_solving_constrained_srinivas_problem.py
--rw-r--r--   0 benhid     (501) staff       (20)     1610 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/examples/multiobjective/nsgaii/nsgaii_solving_mixed_encoding_problem.py
--rw-r--r--   0 benhid     (501) staff       (20)     1972 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/examples/multiobjective/nsgaii/nsgaii_ssp.py
--rw-r--r--   0 benhid     (501) staff       (20)     1436 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/examples/multiobjective/nsgaii/nsgaii_standard_settings.py
--rw-r--r--   0 benhid     (501) staff       (20)     2244 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/examples/multiobjective/nsgaii/nsgaii_standard_settings_with_real_time_plotting.py
--rw-r--r--   0 benhid     (501) staff       (20)     1460 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/examples/multiobjective/nsgaii/nsgaii_steady_state.py
--rw-r--r--   0 benhid     (501) staff       (20)     2454 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/examples/multiobjective/nsgaii/nsgaii_steady_state_with_real_time_plotting.py
--rw-r--r--   0 benhid     (501) staff       (20)     1286 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/examples/multiobjective/nsgaii/parallel_nsgaii_with_multiprocess_evaluator.py
-drwxr-xr-x   0 benhid     (501) staff       (20)        0 2020-04-09 12:56:49.000000 jmetalpy-1.5.5/examples/multiobjective/nsgaiii/
--rw-r--r--   0 benhid     (501) staff       (20)        0 2020-01-08 13:20:59.000000 jmetalpy-1.5.5/examples/multiobjective/nsgaiii/__init__.py
--rw-r--r--   0 benhid     (501) staff       (20)     1332 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/examples/multiobjective/nsgaiii/nsgaiii_dtlz2.py
-drwxr-xr-x   0 benhid     (501) staff       (20)        0 2020-04-09 12:56:49.000000 jmetalpy-1.5.5/examples/multiobjective/omopso/
--rw-r--r--   0 benhid     (501) staff       (20)        0 2020-01-08 13:20:59.000000 jmetalpy-1.5.5/examples/multiobjective/omopso/__init__.py
--rw-r--r--   0 benhid     (501) staff       (20)     1767 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/examples/multiobjective/omopso/omopso_spark_evaluator.py
--rw-r--r--   0 benhid     (501) staff       (20)     1594 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/examples/multiobjective/omopso/omopso_zdt1.py
-drwxr-xr-x   0 benhid     (501) staff       (20)        0 2020-04-09 12:56:49.000000 jmetalpy-1.5.5/examples/multiobjective/random_search/
--rw-r--r--   0 benhid     (501) staff       (20)        0 2020-01-08 13:20:59.000000 jmetalpy-1.5.5/examples/multiobjective/random_search/__init__.py
--rw-r--r--   0 benhid     (501) staff       (20)      959 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/examples/multiobjective/random_search/random_search_zdt1.py
-drwxr-xr-x   0 benhid     (501) staff       (20)        0 2020-04-09 12:56:49.000000 jmetalpy-1.5.5/examples/multiobjective/smpso/
--rw-r--r--   0 benhid     (501) staff       (20)        0 2020-01-08 13:20:59.000000 jmetalpy-1.5.5/examples/multiobjective/smpso/__init__.py
--rw-r--r--   0 benhid     (501) staff       (20)     1163 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/examples/multiobjective/smpso/dynamic_smpso.py
--rw-r--r--   0 benhid     (501) staff       (20)     1452 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/examples/multiobjective/smpso/smpso_schaffer_on_the_fly.py
--rw-r--r--   0 benhid     (501) staff       (20)     1465 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/examples/multiobjective/smpso/smpso_spark_evaluator.py
--rw-r--r--   0 benhid     (501) staff       (20)     1262 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/examples/multiobjective/smpso/smpso_srinivas.py
--rw-r--r--   0 benhid     (501) staff       (20)     1757 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/examples/multiobjective/smpso/smpso_srinivas_on_the_fly.py
--rw-r--r--   0 benhid     (501) staff       (20)     1250 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/examples/multiobjective/smpso/smpso_zdt4.py
--rw-r--r--   0 benhid     (501) staff       (20)     2507 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/examples/multiobjective/smpso/smpsorp_zdt4.py
-drwxr-xr-x   0 benhid     (501) staff       (20)        0 2020-04-09 12:56:49.000000 jmetalpy-1.5.5/examples/multiobjective/spea2/
--rw-r--r--   0 benhid     (501) staff       (20)        0 2020-01-08 13:20:59.000000 jmetalpy-1.5.5/examples/multiobjective/spea2/__init__.py
--rw-r--r--   0 benhid     (501) staff       (20)     1402 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/examples/multiobjective/spea2/gspea2_zdt1.py
--rw-r--r--   0 benhid     (501) staff       (20)     1250 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/examples/multiobjective/spea2/spea2_dtlz1.py
--rw-r--r--   0 benhid     (501) staff       (20)     1245 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/examples/multiobjective/spea2/spea2_zdt1.py
-drwxr-xr-x   0 benhid     (501) staff       (20)        0 2020-04-09 12:56:49.000000 jmetalpy-1.5.5/examples/singleobjective/
--rw-r--r--   0 benhid     (501) staff       (20)        0 2019-10-13 12:34:24.000000 jmetalpy-1.5.5/examples/singleobjective/__init__.py
-drwxr-xr-x   0 benhid     (501) staff       (20)        0 2020-04-09 12:56:49.000000 jmetalpy-1.5.5/examples/singleobjective/evolution_strategy/
--rw-r--r--   0 benhid     (501) staff       (20)        0 2020-01-08 13:20:59.000000 jmetalpy-1.5.5/examples/singleobjective/evolution_strategy/__init__.py
--rw-r--r--   0 benhid     (501) staff       (20)      892 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/examples/singleobjective/evolution_strategy/evolution_strategy_binary.py
--rw-r--r--   0 benhid     (501) staff       (20)      908 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/examples/singleobjective/evolution_strategy/evolution_strategy_float.py
-drwxr-xr-x   0 benhid     (501) staff       (20)        0 2020-04-09 12:56:49.000000 jmetalpy-1.5.5/examples/singleobjective/gde3/
--rw-r--r--   0 benhid     (501) staff       (20)        0 2020-01-08 13:20:59.000000 jmetalpy-1.5.5/examples/singleobjective/gde3/__init__.py
--rw-r--r--   0 benhid     (501) staff       (20)      964 2020-01-08 13:20:59.000000 jmetalpy-1.5.5/examples/singleobjective/gde3/gde3_single_objective.py
-drwxr-xr-x   0 benhid     (501) staff       (20)        0 2020-04-09 12:56:49.000000 jmetalpy-1.5.5/examples/singleobjective/genetic_algorithm/
--rw-r--r--   0 benhid     (501) staff       (20)        0 2020-01-08 13:20:59.000000 jmetalpy-1.5.5/examples/singleobjective/genetic_algorithm/__init__.py
--rw-r--r--   0 benhid     (501) staff       (20)     1036 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/examples/singleobjective/genetic_algorithm/generational_genetic_algorithm_binary.py
--rw-r--r--   0 benhid     (501) staff       (20)     1079 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/examples/singleobjective/genetic_algorithm/generational_genetic_algorithm_float.py
--rw-r--r--   0 benhid     (501) staff       (20)     1527 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/examples/singleobjective/genetic_algorithm/generational_genetic_algorithm_tsp.py
--rw-r--r--   0 benhid     (501) staff       (20)     1961 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/examples/singleobjective/genetic_algorithm/steady_state_genetic_algorithm.py
--rw-r--r--   0 benhid     (501) staff       (20)     1185 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/examples/singleobjective/genetic_algorithm/steady_state_genetic_algorithm_with_knapsack_problem.py
-drwxr-xr-x   0 benhid     (501) staff       (20)        0 2020-04-09 12:56:49.000000 jmetalpy-1.5.5/examples/singleobjective/local_search/
--rw-r--r--   0 benhid     (501) staff       (20)        0 2020-01-08 13:20:59.000000 jmetalpy-1.5.5/examples/singleobjective/local_search/__init__.py
--rw-r--r--   0 benhid     (501) staff       (20)     1168 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/examples/singleobjective/local_search/local_search_binary.py
--rw-r--r--   0 benhid     (501) staff       (20)     1184 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/examples/singleobjective/local_search/local_search_float.py
-drwxr-xr-x   0 benhid     (501) staff       (20)        0 2020-04-09 12:56:49.000000 jmetalpy-1.5.5/examples/singleobjective/nsgaii/
--rw-r--r--   0 benhid     (501) staff       (20)        0 2020-01-08 13:20:59.000000 jmetalpy-1.5.5/examples/singleobjective/nsgaii/__init__.py
--rw-r--r--   0 benhid     (501) staff       (20)     1323 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/examples/singleobjective/nsgaii/nsgaii_single_objective_binary.py
--rw-r--r--   0 benhid     (501) staff       (20)     1374 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/examples/singleobjective/nsgaii/nsgaii_single_objective_float.py
-drwxr-xr-x   0 benhid     (501) staff       (20)        0 2020-04-09 12:56:49.000000 jmetalpy-1.5.5/examples/singleobjective/simulated_annealing/
--rw-r--r--   0 benhid     (501) staff       (20)        0 2020-01-08 13:20:59.000000 jmetalpy-1.5.5/examples/singleobjective/simulated_annealing/__init__.py
--rw-r--r--   0 benhid     (501) staff       (20)     1190 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/examples/singleobjective/simulated_annealing/simulated_annealing_binary.py
--rw-r--r--   0 benhid     (501) staff       (20)     1244 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/examples/singleobjective/simulated_annealing/simulated_annealing_float.py
-drwxr-xr-x   0 benhid     (501) staff       (20)        0 2020-04-09 12:56:49.000000 jmetalpy-1.5.5/jmetal/
--rw-r--r--   0 benhid     (501) staff       (20)      717 2020-01-08 13:20:59.000000 jmetalpy-1.5.5/jmetal/__init__.py
-drwxr-xr-x   0 benhid     (501) staff       (20)        0 2020-04-09 12:56:49.000000 jmetalpy-1.5.5/jmetal/algorithm/
--rw-r--r--   0 benhid     (501) staff       (20)        0 2019-10-13 12:34:24.000000 jmetalpy-1.5.5/jmetal/algorithm/__init__.py
-drwxr-xr-x   0 benhid     (501) staff       (20)        0 2020-04-09 12:56:49.000000 jmetalpy-1.5.5/jmetal/algorithm/multiobjective/
--rw-r--r--   0 benhid     (501) staff       (20)      361 2020-01-08 16:29:44.000000 jmetalpy-1.5.5/jmetal/algorithm/multiobjective/__init__.py
--rw-r--r--   0 benhid     (501) staff       (20)     5458 2020-01-08 16:34:01.000000 jmetalpy-1.5.5/jmetal/algorithm/multiobjective/gde3.py
--rw-r--r--   0 benhid     (501) staff       (20)     3920 2020-01-08 16:34:15.000000 jmetalpy-1.5.5/jmetal/algorithm/multiobjective/hype.py
--rw-r--r--   0 benhid     (501) staff       (20)     4647 2020-04-09 12:56:45.000000 jmetalpy-1.5.5/jmetal/algorithm/multiobjective/ibea.py
--rw-r--r--   0 benhid     (501) staff       (20)     5910 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/jmetal/algorithm/multiobjective/mocell.py
--rw-r--r--   0 benhid     (501) staff       (20)    16837 2020-01-08 13:20:59.000000 jmetalpy-1.5.5/jmetal/algorithm/multiobjective/moead.py
--rw-r--r--   0 benhid     (501) staff       (20)    12463 2020-01-08 16:30:20.000000 jmetalpy-1.5.5/jmetal/algorithm/multiobjective/nsgaii.py
--rw-r--r--   0 benhid     (501) staff       (20)    14760 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/jmetal/algorithm/multiobjective/nsgaiii.py
--rw-r--r--   0 benhid     (501) staff       (20)     8378 2020-01-08 16:30:20.000000 jmetalpy-1.5.5/jmetal/algorithm/multiobjective/omopso.py
--rw-r--r--   0 benhid     (501) staff       (20)     2256 2020-01-08 13:20:59.000000 jmetalpy-1.5.5/jmetal/algorithm/multiobjective/random_search.py
--rw-r--r--   0 benhid     (501) staff       (20)    14987 2020-01-08 13:20:59.000000 jmetalpy-1.5.5/jmetal/algorithm/multiobjective/smpso.py
--rw-r--r--   0 benhid     (501) staff       (20)     4266 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/jmetal/algorithm/multiobjective/spea2.py
-drwxr-xr-x   0 benhid     (501) staff       (20)        0 2020-04-09 12:56:49.000000 jmetalpy-1.5.5/jmetal/algorithm/singleobjective/
--rw-r--r--   0 benhid     (501) staff       (20)      188 2020-01-08 16:29:44.000000 jmetalpy-1.5.5/jmetal/algorithm/singleobjective/__init__.py
--rw-r--r--   0 benhid     (501) staff       (20)     3239 2020-04-09 12:56:45.000000 jmetalpy-1.5.5/jmetal/algorithm/singleobjective/evolution_strategy.py
--rw-r--r--   0 benhid     (501) staff       (20)     4062 2020-01-08 13:20:59.000000 jmetalpy-1.5.5/jmetal/algorithm/singleobjective/genetic_algorithm.py
--rw-r--r--   0 benhid     (501) staff       (20)     2722 2020-01-08 13:20:59.000000 jmetalpy-1.5.5/jmetal/algorithm/singleobjective/local_search.py
--rw-r--r--   0 benhid     (501) staff       (20)     3239 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/jmetal/algorithm/singleobjective/simulated_annealing.py
-drwxr-xr-x   0 benhid     (501) staff       (20)        0 2020-04-09 12:56:49.000000 jmetalpy-1.5.5/jmetal/algorithm/test/
--rw-r--r--   0 benhid     (501) staff       (20)        0 2019-10-13 12:34:24.000000 jmetalpy-1.5.5/jmetal/algorithm/test/__init__.py
--rw-r--r--   0 benhid     (501) staff       (20)     3077 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/jmetal/algorithm/test/ittest_algorithm.py
--rw-r--r--   0 benhid     (501) staff       (20)     1033 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/jmetal/config.py
-drwxr-xr-x   0 benhid     (501) staff       (20)        0 2020-04-09 12:56:49.000000 jmetalpy-1.5.5/jmetal/core/
--rw-r--r--   0 benhid     (501) staff       (20)        0 2019-10-13 12:34:24.000000 jmetalpy-1.5.5/jmetal/core/__init__.py
--rw-r--r--   0 benhid     (501) staff       (20)     6995 2019-11-05 12:03:17.000000 jmetalpy-1.5.5/jmetal/core/algorithm.py
--rw-r--r--   0 benhid     (501) staff       (20)      659 2019-10-13 12:34:24.000000 jmetalpy-1.5.5/jmetal/core/observer.py
--rw-r--r--   0 benhid     (501) staff       (20)     1660 2019-10-13 12:34:24.000000 jmetalpy-1.5.5/jmetal/core/operator.py
--rw-r--r--   0 benhid     (501) staff       (20)     5165 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/jmetal/core/problem.py
--rw-r--r--   0 benhid     (501) staff       (20)    12951 2020-04-09 12:56:45.000000 jmetalpy-1.5.5/jmetal/core/quality_indicator.py
--rw-r--r--   0 benhid     (501) staff       (20)     6288 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/jmetal/core/solution.py
-drwxr-xr-x   0 benhid     (501) staff       (20)        0 2020-04-09 12:56:49.000000 jmetalpy-1.5.5/jmetal/core/test/
--rw-r--r--   0 benhid     (501) staff       (20)        0 2019-10-13 12:34:24.000000 jmetalpy-1.5.5/jmetal/core/test/__init__.py
--rw-r--r--   0 benhid     (501) staff       (20)     1956 2019-10-13 12:34:24.000000 jmetalpy-1.5.5/jmetal/core/test/test_observable.py
--rw-r--r--   0 benhid     (501) staff       (20)     1570 2019-10-13 12:34:24.000000 jmetalpy-1.5.5/jmetal/core/test/test_operator.py
--rw-r--r--   0 benhid     (501) staff       (20)     3211 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/jmetal/core/test/test_problem.py
--rw-r--r--   0 benhid     (501) staff       (20)    10411 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/jmetal/core/test/test_quality_indicator.py
--rw-r--r--   0 benhid     (501) staff       (20)     9004 2020-04-09 12:56:45.000000 jmetalpy-1.5.5/jmetal/core/test/test_solution.py
-drwxr-xr-x   0 benhid     (501) staff       (20)        0 2020-04-09 12:56:49.000000 jmetalpy-1.5.5/jmetal/lab/
--rw-r--r--   0 benhid     (501) staff       (20)        0 2019-10-13 12:34:24.000000 jmetalpy-1.5.5/jmetal/lab/__init__.py
--rw-r--r--   0 benhid     (501) staff       (20)    21593 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/jmetal/lab/experiment.py
-drwxr-xr-x   0 benhid     (501) staff       (20)        0 2020-04-09 12:56:49.000000 jmetalpy-1.5.5/jmetal/lab/statistical_test/
--rw-r--r--   0 benhid     (501) staff       (20)        0 2019-10-13 12:34:24.000000 jmetalpy-1.5.5/jmetal/lab/statistical_test/__init__.py
--rw-r--r--   0 benhid     (501) staff       (20)    13390 2019-10-13 12:34:24.000000 jmetalpy-1.5.5/jmetal/lab/statistical_test/apv_procedures.py
--rw-r--r--   0 benhid     (501) staff       (20)     5914 2020-01-08 13:20:59.000000 jmetalpy-1.5.5/jmetal/lab/statistical_test/bayesian.py
--rw-r--r--   0 benhid     (501) staff       (20)     8819 2019-10-13 12:34:24.000000 jmetalpy-1.5.5/jmetal/lab/statistical_test/critical_distance.py
--rw-r--r--   0 benhid     (501) staff       (20)    20186 2019-10-13 12:34:24.000000 jmetalpy-1.5.5/jmetal/lab/statistical_test/functions.py
-drwxr-xr-x   0 benhid     (501) staff       (20)        0 2020-04-09 12:56:49.000000 jmetalpy-1.5.5/jmetal/lab/visualization/
--rw-r--r--   0 benhid     (501) staff       (20)      298 2020-01-08 17:05:39.000000 jmetalpy-1.5.5/jmetal/lab/visualization/__init__.py
--rw-r--r--   0 benhid     (501) staff       (20)    12391 2019-11-05 12:03:17.000000 jmetalpy-1.5.5/jmetal/lab/visualization/chord_plot.py
--rw-r--r--   0 benhid     (501) staff       (20)     7358 2020-01-08 16:29:44.000000 jmetalpy-1.5.5/jmetal/lab/visualization/interactive.py
--rw-r--r--   0 benhid     (501) staff       (20)     6807 2020-01-08 16:29:44.000000 jmetalpy-1.5.5/jmetal/lab/visualization/plotting.py
--rw-r--r--   0 benhid     (501) staff       (20)     4386 2019-10-13 12:34:24.000000 jmetalpy-1.5.5/jmetal/lab/visualization/posterior.py
--rw-r--r--   0 benhid     (501) staff       (20)     4419 2019-11-05 12:03:17.000000 jmetalpy-1.5.5/jmetal/lab/visualization/streaming.py
-drwxr-xr-x   0 benhid     (501) staff       (20)        0 2020-04-09 12:56:49.000000 jmetalpy-1.5.5/jmetal/operator/
--rw-r--r--   0 benhid     (501) staff       (20)      865 2019-10-13 12:34:24.000000 jmetalpy-1.5.5/jmetal/operator/__init__.py
--rw-r--r--   0 benhid     (501) staff       (20)    18055 2020-04-09 12:56:45.000000 jmetalpy-1.5.5/jmetal/operator/crossover.py
--rw-r--r--   0 benhid     (501) staff       (20)    10807 2020-04-09 12:56:45.000000 jmetalpy-1.5.5/jmetal/operator/mutation.py
--rw-r--r--   0 benhid     (501) staff       (20)    11901 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/jmetal/operator/selection.py
-drwxr-xr-x   0 benhid     (501) staff       (20)        0 2020-04-09 12:56:49.000000 jmetalpy-1.5.5/jmetal/operator/test/
--rw-r--r--   0 benhid     (501) staff       (20)        0 2019-10-13 12:34:24.000000 jmetalpy-1.5.5/jmetal/operator/test/__init__.py
--rw-r--r--   0 benhid     (501) staff       (20)    18773 2020-04-09 12:56:45.000000 jmetalpy-1.5.5/jmetal/operator/test/test_crossover.py
--rw-r--r--   0 benhid     (501) staff       (20)    13913 2020-04-09 12:56:45.000000 jmetalpy-1.5.5/jmetal/operator/test/test_mutation.py
--rw-r--r--   0 benhid     (501) staff       (20)    15539 2020-01-08 13:20:59.000000 jmetalpy-1.5.5/jmetal/operator/test/test_selection.py
-drwxr-xr-x   0 benhid     (501) staff       (20)        0 2020-04-09 12:56:49.000000 jmetalpy-1.5.5/jmetal/problem/
--rw-r--r--   0 benhid     (501) staff       (20)      537 2019-10-13 12:34:24.000000 jmetalpy-1.5.5/jmetal/problem/__init__.py
-drwxr-xr-x   0 benhid     (501) staff       (20)        0 2020-04-09 12:56:49.000000 jmetalpy-1.5.5/jmetal/problem/multiobjective/
--rw-r--r--   0 benhid     (501) staff       (20)        0 2019-10-13 12:34:24.000000 jmetalpy-1.5.5/jmetal/problem/multiobjective/__init__.py
--rw-r--r--   0 benhid     (501) staff       (20)     5868 2019-10-13 12:34:24.000000 jmetalpy-1.5.5/jmetal/problem/multiobjective/constrained.py
--rw-r--r--   0 benhid     (501) staff       (20)     9692 2019-10-13 12:34:24.000000 jmetalpy-1.5.5/jmetal/problem/multiobjective/dtlz.py
--rw-r--r--   0 benhid     (501) staff       (20)     9798 2019-10-18 06:43:55.000000 jmetalpy-1.5.5/jmetal/problem/multiobjective/fda.py
--rw-r--r--   0 benhid     (501) staff       (20)    19607 2020-01-08 16:29:44.000000 jmetalpy-1.5.5/jmetal/problem/multiobjective/lircmop.py
--rw-r--r--   0 benhid     (501) staff       (20)    12123 2019-10-18 06:43:55.000000 jmetalpy-1.5.5/jmetal/problem/multiobjective/lz09.py
-drwxr-xr-x   0 benhid     (501) staff       (20)        0 2020-04-09 12:56:49.000000 jmetalpy-1.5.5/jmetal/problem/multiobjective/test/
--rw-r--r--   0 benhid     (501) staff       (20)        0 2019-10-13 12:34:24.000000 jmetalpy-1.5.5/jmetal/problem/multiobjective/test/__init__.py
--rw-r--r--   0 benhid     (501) staff       (20)     2845 2019-10-18 06:43:55.000000 jmetalpy-1.5.5/jmetal/problem/multiobjective/test/test_constrained.py
--rw-r--r--   0 benhid     (501) staff       (20)     7721 2019-10-13 12:34:24.000000 jmetalpy-1.5.5/jmetal/problem/multiobjective/test/test_unconstrained.py
--rw-r--r--   0 benhid     (501) staff       (20)     9754 2019-10-13 12:34:24.000000 jmetalpy-1.5.5/jmetal/problem/multiobjective/test/test_zdt.py
--rw-r--r--   0 benhid     (501) staff       (20)     1811 2020-04-09 12:56:45.000000 jmetalpy-1.5.5/jmetal/problem/multiobjective/uf.py
--rw-r--r--   0 benhid     (501) staff       (20)     9810 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/jmetal/problem/multiobjective/unconstrained.py
--rw-r--r--   0 benhid     (501) staff       (20)     4777 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/jmetal/problem/multiobjective/zdt.py
-drwxr-xr-x   0 benhid     (501) staff       (20)        0 2020-04-09 12:56:49.000000 jmetalpy-1.5.5/jmetal/problem/singleobjective/
--rw-r--r--   0 benhid     (501) staff       (20)        0 2019-10-13 12:34:24.000000 jmetalpy-1.5.5/jmetal/problem/singleobjective/__init__.py
--rw-r--r--   0 benhid     (501) staff       (20)     2846 2019-10-13 12:34:24.000000 jmetalpy-1.5.5/jmetal/problem/singleobjective/knapsack.py
-drwxr-xr-x   0 benhid     (501) staff       (20)        0 2020-04-09 12:56:49.000000 jmetalpy-1.5.5/jmetal/problem/singleobjective/test/
--rw-r--r--   0 benhid     (501) staff       (20)        0 2019-10-13 12:34:24.000000 jmetalpy-1.5.5/jmetal/problem/singleobjective/test/__init__.py
--rw-r--r--   0 benhid     (501) staff       (20)     2726 2019-10-13 12:34:24.000000 jmetalpy-1.5.5/jmetal/problem/singleobjective/test/test_knapsack.py
--rw-r--r--   0 benhid     (501) staff       (20)     4263 2019-10-13 12:34:24.000000 jmetalpy-1.5.5/jmetal/problem/singleobjective/test/test_unconstrained.py
--rw-r--r--   0 benhid     (501) staff       (20)     3196 2019-10-13 12:34:24.000000 jmetalpy-1.5.5/jmetal/problem/singleobjective/tsp.py
--rw-r--r--   0 benhid     (501) staff       (20)     4720 2019-11-05 12:03:17.000000 jmetalpy-1.5.5/jmetal/problem/singleobjective/unconstrained.py
-drwxr-xr-x   0 benhid     (501) staff       (20)        0 2020-04-09 12:56:49.000000 jmetalpy-1.5.5/jmetal/util/
--rw-r--r--   0 benhid     (501) staff       (20)        0 2019-10-13 12:34:24.000000 jmetalpy-1.5.5/jmetal/util/__init__.py
--rw-r--r--   0 benhid     (501) staff       (20)     1394 2020-01-15 09:03:20.000000 jmetalpy-1.5.5/jmetal/util/aggregative_function.py
--rw-r--r--   0 benhid     (501) staff       (20)     7644 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/jmetal/util/archive.py
--rw-r--r--   0 benhid     (501) staff       (20)     2237 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/jmetal/util/ckecking.py
--rw-r--r--   0 benhid     (501) staff       (20)     9238 2020-01-08 16:29:44.000000 jmetalpy-1.5.5/jmetal/util/comparator.py
--rw-r--r--   0 benhid     (501) staff       (20)     1220 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/jmetal/util/constraint_handling.py
--rw-r--r--   0 benhid     (501) staff       (20)     5687 2020-01-08 13:20:59.000000 jmetalpy-1.5.5/jmetal/util/density_estimator.py
--rw-r--r--   0 benhid     (501) staff       (20)     1339 2019-10-13 12:34:24.000000 jmetalpy-1.5.5/jmetal/util/distance.py
--rw-r--r--   0 benhid     (501) staff       (20)     2702 2020-01-08 13:20:59.000000 jmetalpy-1.5.5/jmetal/util/evaluator.py
--rw-r--r--   0 benhid     (501) staff       (20)     1185 2020-01-08 13:20:59.000000 jmetalpy-1.5.5/jmetal/util/generator.py
--rw-r--r--   0 benhid     (501) staff       (20)     7693 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/jmetal/util/neighborhood.py
--rw-r--r--   0 benhid     (501) staff       (20)     1387 2019-10-13 12:34:24.000000 jmetalpy-1.5.5/jmetal/util/observable.py
--rw-r--r--   0 benhid     (501) staff       (20)     7924 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/jmetal/util/observer.py
--rw-r--r--   0 benhid     (501) staff       (20)      573 2020-01-08 13:20:59.000000 jmetalpy-1.5.5/jmetal/util/point.py
--rw-r--r--   0 benhid     (501) staff       (20)     5870 2020-01-08 13:20:59.000000 jmetalpy-1.5.5/jmetal/util/ranking.py
--rw-r--r--   0 benhid     (501) staff       (20)     2807 2019-10-13 12:34:24.000000 jmetalpy-1.5.5/jmetal/util/replacement.py
--rw-r--r--   0 benhid     (501) staff       (20)     2777 2020-01-08 16:29:44.000000 jmetalpy-1.5.5/jmetal/util/solution.py
--rw-r--r--   0 benhid     (501) staff       (20)     2618 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/jmetal/util/termination_criterion.py
-drwxr-xr-x   0 benhid     (501) staff       (20)        0 2020-04-09 12:56:49.000000 jmetalpy-1.5.5/jmetal/util/test/
--rw-r--r--   0 benhid     (501) staff       (20)        0 2019-10-13 12:34:24.000000 jmetalpy-1.5.5/jmetal/util/test/__init__.py
--rw-r--r--   0 benhid     (501) staff       (20)      570 2019-10-13 12:34:24.000000 jmetalpy-1.5.5/jmetal/util/test/test_aggregativefunction.py
--rw-r--r--   0 benhid     (501) staff       (20)    12226 2020-01-08 13:20:59.000000 jmetalpy-1.5.5/jmetal/util/test/test_archive.py
--rw-r--r--   0 benhid     (501) staff       (20)     1499 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/jmetal/util/test/test_checking.py
--rw-r--r--   0 benhid     (501) staff       (20)    14883 2020-01-08 13:20:59.000000 jmetalpy-1.5.5/jmetal/util/test/test_comparator.py
--rw-r--r--   0 benhid     (501) staff       (20)     4439 2019-10-13 12:34:24.000000 jmetalpy-1.5.5/jmetal/util/test/test_constraint_handling.py
--rw-r--r--   0 benhid     (501) staff       (20)     7638 2019-10-13 12:34:24.000000 jmetalpy-1.5.5/jmetal/util/test/test_density_estimator.py
--rw-r--r--   0 benhid     (501) staff       (20)     1679 2019-10-13 12:34:24.000000 jmetalpy-1.5.5/jmetal/util/test/test_distance.py
--rw-r--r--   0 benhid     (501) staff       (20)     2892 2020-01-08 13:20:59.000000 jmetalpy-1.5.5/jmetal/util/test/test_evaluator.py
--rw-r--r--   0 benhid     (501) staff       (20)    10564 2020-02-17 16:14:45.000000 jmetalpy-1.5.5/jmetal/util/test/test_neighborhood.py
--rw-r--r--   0 benhid     (501) staff       (20)     1144 2019-10-13 12:34:24.000000 jmetalpy-1.5.5/jmetal/util/test/test_point.py
--rw-r--r--   0 benhid     (501) staff       (20)     9074 2019-10-13 12:34:24.000000 jmetalpy-1.5.5/jmetal/util/test/test_ranking.py
--rw-r--r--   0 benhid     (501) staff       (20)     6804 2019-10-13 12:34:24.000000 jmetalpy-1.5.5/jmetal/util/test/test_replacement.py
-drwxr-xr-x   0 benhid     (501) staff       (20)        0 2020-04-09 12:56:49.000000 jmetalpy-1.5.5/jmetalpy.egg-info/
--rw-r--r--   0 benhid     (501) staff       (20)     7097 2020-04-09 12:56:48.000000 jmetalpy-1.5.5/jmetalpy.egg-info/PKG-INFO
--rw-r--r--   0 benhid     (501) staff       (20)     8507 2020-04-09 12:56:48.000000 jmetalpy-1.5.5/jmetalpy.egg-info/SOURCES.txt
--rw-r--r--   0 benhid     (501) staff       (20)        1 2020-04-09 12:56:48.000000 jmetalpy-1.5.5/jmetalpy.egg-info/dependency_links.txt
--rw-r--r--   0 benhid     (501) staff       (20)      681 2020-04-09 12:56:48.000000 jmetalpy-1.5.5/jmetalpy.egg-info/requires.txt
--rw-r--r--   0 benhid     (501) staff       (20)       16 2020-04-09 12:56:48.000000 jmetalpy-1.5.5/jmetalpy.egg-info/top_level.txt
--rw-r--r--   0 benhid     (501) staff       (20)       79 2020-04-09 12:56:49.000000 jmetalpy-1.5.5/setup.cfg
--rw-r--r--   0 benhid     (501) staff       (20)     1618 2020-04-09 12:56:45.000000 jmetalpy-1.5.5/setup.py
+drwxr-xr-x   0 benhid     (501) staff       (20)        0 2023-04-19 14:32:18.768884 jmetalpy-1.6.0/
+-rw-r--r--   0 benhid     (501) staff       (20)     1073 2023-04-19 14:00:52.000000 jmetalpy-1.6.0/LICENSE
+-rw-r--r--   0 benhid     (501) staff       (20)     6631 2023-04-19 14:32:18.769125 jmetalpy-1.6.0/PKG-INFO
+-rw-r--r--   0 benhid     (501) staff       (20)     5725 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/README.md
+drwxr-xr-x   0 benhid     (501) staff       (20)        0 2023-04-19 14:32:18.590495 jmetalpy-1.6.0/examples/
+-rw-r--r--   0 benhid     (501) staff       (20)        0 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/examples/__init__.py
+drwxr-xr-x   0 benhid     (501) staff       (20)        0 2023-04-19 14:32:18.592603 jmetalpy-1.6.0/examples/experiment/
+-rw-r--r--   0 benhid     (501) staff       (20)        0 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/examples/experiment/__init__.py
+-rw-r--r--   0 benhid     (501) staff       (20)     3233 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/examples/experiment/comparison.py
+-rw-r--r--   0 benhid     (501) staff       (20)      525 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/examples/experiment/generateMedianAndWilcoxonLatexTables.py
+-rw-r--r--   0 benhid     (501) staff       (20)     2781 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/examples/experiment/statistical_analysis.py
+drwxr-xr-x   0 benhid     (501) staff       (20)        0 2023-04-19 14:32:18.593321 jmetalpy-1.6.0/examples/multiobjective/
+-rw-r--r--   0 benhid     (501) staff       (20)        0 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/examples/multiobjective/__init__.py
+drwxr-xr-x   0 benhid     (501) staff       (20)        0 2023-04-19 14:32:18.596038 jmetalpy-1.6.0/examples/multiobjective/gde3/
+-rw-r--r--   0 benhid     (501) staff       (20)        0 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/examples/multiobjective/gde3/__init__.py
+-rw-r--r--   0 benhid     (501) staff       (20)      863 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/examples/multiobjective/gde3/dynamic_gde3.py
+-rw-r--r--   0 benhid     (501) staff       (20)     1050 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/examples/multiobjective/gde3/gde3_spark_evaluator.py
+-rw-r--r--   0 benhid     (501) staff       (20)      895 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/examples/multiobjective/gde3/gde3_zdt1.py
+-rw-r--r--   0 benhid     (501) staff       (20)     1165 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/examples/multiobjective/gde3/ggde3_zdt2.py
+drwxr-xr-x   0 benhid     (501) staff       (20)        0 2023-04-19 14:32:18.597034 jmetalpy-1.6.0/examples/multiobjective/hype/
+-rw-r--r--   0 benhid     (501) staff       (20)        0 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/examples/multiobjective/hype/__init__.py
+-rw-r--r--   0 benhid     (501) staff       (20)     1467 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/examples/multiobjective/hype/hype_zdt1.py
+drwxr-xr-x   0 benhid     (501) staff       (20)        0 2023-04-19 14:32:18.597956 jmetalpy-1.6.0/examples/multiobjective/ibea/
+-rw-r--r--   0 benhid     (501) staff       (20)        0 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/examples/multiobjective/ibea/__init__.py
+-rw-r--r--   0 benhid     (501) staff       (20)     1238 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/examples/multiobjective/ibea/ibea_zdt1.py
+drwxr-xr-x   0 benhid     (501) staff       (20)        0 2023-04-19 14:32:18.598951 jmetalpy-1.6.0/examples/multiobjective/mocell/
+-rw-r--r--   0 benhid     (501) staff       (20)        0 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/examples/multiobjective/mocell/__init__.py
+-rw-r--r--   0 benhid     (501) staff       (20)     1399 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/examples/multiobjective/mocell/mocell_zdt1.py
+drwxr-xr-x   0 benhid     (501) staff       (20)        0 2023-04-19 14:32:18.601769 jmetalpy-1.6.0/examples/multiobjective/moead/
+-rw-r--r--   0 benhid     (501) staff       (20)        0 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/examples/multiobjective/moead/__init__.py
+-rw-r--r--   0 benhid     (501) staff       (20)     1789 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/examples/multiobjective/moead/moead_dtlz2.py
+-rw-r--r--   0 benhid     (501) staff       (20)     1597 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/examples/multiobjective/moead/moead_iepsilon_lircmop1.py
+-rw-r--r--   0 benhid     (501) staff       (20)     1563 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/examples/multiobjective/moead/moead_lz09.py
+-rw-r--r--   0 benhid     (501) staff       (20)     1769 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/examples/multiobjective/moead/moeaddra_lz09.py
+drwxr-xr-x   0 benhid     (501) staff       (20)        0 2023-04-19 14:32:18.610682 jmetalpy-1.6.0/examples/multiobjective/nsgaii/
+-rw-r--r--   0 benhid     (501) staff       (20)        0 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/examples/multiobjective/nsgaii/__init__.py
+-rw-r--r--   0 benhid     (501) staff       (20)     1297 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/examples/multiobjective/nsgaii/distributed_nsgaii_with_dask.py
+-rw-r--r--   0 benhid     (501) staff       (20)     1333 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/examples/multiobjective/nsgaii/distributed_nsgaii_with_dask_evaluator.py
+-rw-r--r--   0 benhid     (501) staff       (20)     1344 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/examples/multiobjective/nsgaii/distributed_nsgaii_with_spark_evaluator.py
+-rw-r--r--   0 benhid     (501) staff       (20)     1157 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/examples/multiobjective/nsgaii/dynamic_nsgaii_solving_fda2.py
+-rw-r--r--   0 benhid     (501) staff       (20)     1605 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/examples/multiobjective/nsgaii/nsgaii_defining_schaffer_problem_on_the_fly.py
+-rw-r--r--   0 benhid     (501) staff       (20)     2208 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/examples/multiobjective/nsgaii/nsgaii_defining_srinivas_problem_on_the_fly.py
+-rw-r--r--   0 benhid     (501) staff       (20)     1376 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/examples/multiobjective/nsgaii/nsgaii_solving_3D_problem.py
+-rw-r--r--   0 benhid     (501) staff       (20)     1409 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/examples/multiobjective/nsgaii/nsgaii_solving_binary_problem.py
+-rw-r--r--   0 benhid     (501) staff       (20)     1386 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/examples/multiobjective/nsgaii/nsgaii_solving_constrained_srinivas_problem.py
+-rw-r--r--   0 benhid     (501) staff       (20)     1623 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/examples/multiobjective/nsgaii/nsgaii_solving_mixed_encoding_problem.py
+-rw-r--r--   0 benhid     (501) staff       (20)     2872 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/examples/multiobjective/nsgaii/nsgaii_ssp.py
+-rw-r--r--   0 benhid     (501) staff       (20)     1410 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/examples/multiobjective/nsgaii/nsgaii_standard_settings.py
+-rw-r--r--   0 benhid     (501) staff       (20)     2290 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/examples/multiobjective/nsgaii/nsgaii_standard_settings_with_real_time_plotting.py
+-rw-r--r--   0 benhid     (501) staff       (20)     1448 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/examples/multiobjective/nsgaii/nsgaii_steady_state.py
+-rw-r--r--   0 benhid     (501) staff       (20)     2387 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/examples/multiobjective/nsgaii/nsgaii_steady_state_with_real_time_plotting.py
+-rw-r--r--   0 benhid     (501) staff       (20)     1282 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/examples/multiobjective/nsgaii/parallel_nsgaii_with_multiprocess_evaluator.py
+drwxr-xr-x   0 benhid     (501) staff       (20)        0 2023-04-19 14:32:18.611562 jmetalpy-1.6.0/examples/multiobjective/nsgaiii/
+-rw-r--r--   0 benhid     (501) staff       (20)        0 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/examples/multiobjective/nsgaiii/__init__.py
+-rw-r--r--   0 benhid     (501) staff       (20)     1413 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/examples/multiobjective/nsgaiii/nsgaiii_dtlz2.py
+drwxr-xr-x   0 benhid     (501) staff       (20)        0 2023-04-19 14:32:18.613057 jmetalpy-1.6.0/examples/multiobjective/omopso/
+-rw-r--r--   0 benhid     (501) staff       (20)        0 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/examples/multiobjective/omopso/__init__.py
+-rw-r--r--   0 benhid     (501) staff       (20)     1722 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/examples/multiobjective/omopso/omopso_spark_evaluator.py
+-rw-r--r--   0 benhid     (501) staff       (20)     1550 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/examples/multiobjective/omopso/omopso_zdt1.py
+drwxr-xr-x   0 benhid     (501) staff       (20)        0 2023-04-19 14:32:18.614655 jmetalpy-1.6.0/examples/multiobjective/preferences/
+-rw-r--r--   0 benhid     (501) staff       (20)        0 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/examples/multiobjective/preferences/__init__.py
+-rw-r--r--   0 benhid     (501) staff       (20)     1922 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/examples/multiobjective/preferences/ggde3_zdt2.py
+-rw-r--r--   0 benhid     (501) staff       (20)     2494 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/examples/multiobjective/preferences/gnsgaii_solving_zdt2_with_reference_point.py
+drwxr-xr-x   0 benhid     (501) staff       (20)        0 2023-04-19 14:32:18.615662 jmetalpy-1.6.0/examples/multiobjective/random_search/
+-rw-r--r--   0 benhid     (501) staff       (20)        0 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/examples/multiobjective/random_search/__init__.py
+-rw-r--r--   0 benhid     (501) staff       (20)      851 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/examples/multiobjective/random_search/random_search_zdt1.py
+drwxr-xr-x   0 benhid     (501) staff       (20)        0 2023-04-19 14:32:18.620026 jmetalpy-1.6.0/examples/multiobjective/smpso/
+-rw-r--r--   0 benhid     (501) staff       (20)        0 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/examples/multiobjective/smpso/__init__.py
+-rw-r--r--   0 benhid     (501) staff       (20)     1283 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/examples/multiobjective/smpso/dynamic_smpso.py
+-rw-r--r--   0 benhid     (501) staff       (20)     1405 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/examples/multiobjective/smpso/smpso_schaffer_on_the_fly.py
+-rw-r--r--   0 benhid     (501) staff       (20)     1424 2023-04-19 14:01:13.000000 jmetalpy-1.6.0/examples/multiobjective/smpso/smpso_spark_evaluator.py
+-rw-r--r--   0 benhid     (501) staff       (20)     1950 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/examples/multiobjective/smpso/smpso_srinivas_on_the_fly.py
+-rw-r--r--   0 benhid     (501) staff       (20)     1428 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/examples/multiobjective/smpso/smpso_tanaka.py
+-rw-r--r--   0 benhid     (501) staff       (20)     1121 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/examples/multiobjective/smpso/smpso_zdt4.py
+-rw-r--r--   0 benhid     (501) staff       (20)     2440 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/examples/multiobjective/smpso/smpsorp_zdt4.py
+drwxr-xr-x   0 benhid     (501) staff       (20)        0 2023-04-19 14:32:18.622032 jmetalpy-1.6.0/examples/multiobjective/spea2/
+-rw-r--r--   0 benhid     (501) staff       (20)        0 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/examples/multiobjective/spea2/__init__.py
+-rw-r--r--   0 benhid     (501) staff       (20)     1305 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/examples/multiobjective/spea2/gspea2_zdt1.py
+-rw-r--r--   0 benhid     (501) staff       (20)     1149 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/examples/multiobjective/spea2/spea2_dtlz1.py
+-rw-r--r--   0 benhid     (501) staff       (20)     1147 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/examples/multiobjective/spea2/spea2_zdt1.py
+drwxr-xr-x   0 benhid     (501) staff       (20)        0 2023-04-19 14:32:18.622647 jmetalpy-1.6.0/examples/singleobjective/
+-rw-r--r--   0 benhid     (501) staff       (20)        0 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/examples/singleobjective/__init__.py
+drwxr-xr-x   0 benhid     (501) staff       (20)        0 2023-04-19 14:32:18.625342 jmetalpy-1.6.0/examples/singleobjective/evolution_strategy/
+-rw-r--r--   0 benhid     (501) staff       (20)        0 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/examples/singleobjective/evolution_strategy/__init__.py
+-rw-r--r--   0 benhid     (501) staff       (20)      893 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/examples/singleobjective/evolution_strategy/evolution_strategy_binary.py
+-rw-r--r--   0 benhid     (501) staff       (20)      909 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/examples/singleobjective/evolution_strategy/evolution_strategy_float.py
+-rw-r--r--   0 benhid     (501) staff       (20)     1008 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/examples/singleobjective/evolution_strategy/evolution_strategy_permutation.py
+drwxr-xr-x   0 benhid     (501) staff       (20)        0 2023-04-19 14:32:18.626443 jmetalpy-1.6.0/examples/singleobjective/gde3/
+-rw-r--r--   0 benhid     (501) staff       (20)        0 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/examples/singleobjective/gde3/__init__.py
+-rw-r--r--   0 benhid     (501) staff       (20)      933 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/examples/singleobjective/gde3/gde3_single_objective.py
+drwxr-xr-x   0 benhid     (501) staff       (20)        0 2023-04-19 14:32:18.631927 jmetalpy-1.6.0/examples/singleobjective/genetic_algorithm/
+-rw-r--r--   0 benhid     (501) staff       (20)        0 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/examples/singleobjective/genetic_algorithm/__init__.py
+-rw-r--r--   0 benhid     (501) staff       (20)     1087 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/examples/singleobjective/genetic_algorithm/generational_genetic_algorithm_binary.py
+-rw-r--r--   0 benhid     (501) staff       (20)     1001 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/examples/singleobjective/genetic_algorithm/generational_genetic_algorithm_float.py
+-rw-r--r--   0 benhid     (501) staff       (20)     1256 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/examples/singleobjective/genetic_algorithm/generational_genetic_algorithm_tsp.py
+-rw-r--r--   0 benhid     (501) staff       (20)     2434 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/examples/singleobjective/genetic_algorithm/generational_genetic_algorithm_tsp_with_contraints.py
+-rw-r--r--   0 benhid     (501) staff       (20)     2863 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/examples/singleobjective/genetic_algorithm/steady_state_genetic_algorithm.py
+-rw-r--r--   0 benhid     (501) staff       (20)     1182 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/examples/singleobjective/genetic_algorithm/steady_state_genetic_algorithm_with_knapsack_problem.py
+drwxr-xr-x   0 benhid     (501) staff       (20)        0 2023-04-19 14:32:18.634324 jmetalpy-1.6.0/examples/singleobjective/local_search/
+-rw-r--r--   0 benhid     (501) staff       (20)        0 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/examples/singleobjective/local_search/__init__.py
+-rw-r--r--   0 benhid     (501) staff       (20)     1300 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/examples/singleobjective/local_search/local_search_binary.py
+-rw-r--r--   0 benhid     (501) staff       (20)     1191 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/examples/singleobjective/local_search/local_search_float.py
+drwxr-xr-x   0 benhid     (501) staff       (20)        0 2023-04-19 14:32:18.636750 jmetalpy-1.6.0/examples/singleobjective/nsgaii/
+-rw-r--r--   0 benhid     (501) staff       (20)        0 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/examples/singleobjective/nsgaii/__init__.py
+-rw-r--r--   0 benhid     (501) staff       (20)     1474 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/examples/singleobjective/nsgaii/nsgaii_single_objective_binary.py
+-rw-r--r--   0 benhid     (501) staff       (20)     1384 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/examples/singleobjective/nsgaii/nsgaii_single_objective_float.py
+drwxr-xr-x   0 benhid     (501) staff       (20)        0 2023-04-19 14:32:18.640097 jmetalpy-1.6.0/examples/singleobjective/simulated_annealing/
+-rw-r--r--   0 benhid     (501) staff       (20)        0 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/examples/singleobjective/simulated_annealing/__init__.py
+-rw-r--r--   0 benhid     (501) staff       (20)     1191 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/examples/singleobjective/simulated_annealing/simulated_annealing_binary.py
+-rw-r--r--   0 benhid     (501) staff       (20)     1246 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/examples/singleobjective/simulated_annealing/simulated_annealing_float.py
+-rw-r--r--   0 benhid     (501) staff       (20)      949 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/examples/singleobjective/simulated_annealing/simulated_annealing_permutation.py
+drwxr-xr-x   0 benhid     (501) staff       (20)        0 2023-04-19 14:32:18.643088 jmetalpy-1.6.0/jmetal/
+-rw-r--r--   0 benhid     (501) staff       (20)      197 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/jmetal/__init__.py
+drwxr-xr-x   0 benhid     (501) staff       (20)        0 2023-04-19 14:32:18.644199 jmetalpy-1.6.0/jmetal/algorithm/
+-rw-r--r--   0 benhid     (501) staff       (20)        0 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/jmetal/algorithm/__init__.py
+drwxr-xr-x   0 benhid     (501) staff       (20)        0 2023-04-19 14:32:18.658401 jmetalpy-1.6.0/jmetal/algorithm/multiobjective/
+-rw-r--r--   0 benhid     (501) staff       (20)      361 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/jmetal/algorithm/multiobjective/__init__.py
+-rw-r--r--   0 benhid     (501) staff       (20)     5410 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/jmetal/algorithm/multiobjective/gde3.py
+-rw-r--r--   0 benhid     (501) staff       (20)     3673 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/jmetal/algorithm/multiobjective/hype.py
+-rw-r--r--   0 benhid     (501) staff       (20)     4691 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/jmetal/algorithm/multiobjective/ibea.py
+-rw-r--r--   0 benhid     (501) staff       (20)     5801 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/jmetal/algorithm/multiobjective/mocell.py
+-rw-r--r--   0 benhid     (501) staff       (20)    16675 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/jmetal/algorithm/multiobjective/moead.py
+-rw-r--r--   0 benhid     (501) staff       (20)    12046 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/jmetal/algorithm/multiobjective/nsgaii.py
+-rw-r--r--   0 benhid     (501) staff       (20)    14219 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/jmetal/algorithm/multiobjective/nsgaiii.py
+-rw-r--r--   0 benhid     (501) staff       (20)     7568 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/jmetal/algorithm/multiobjective/omopso.py
+-rw-r--r--   0 benhid     (501) staff       (20)     2263 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/jmetal/algorithm/multiobjective/random_search.py
+-rw-r--r--   0 benhid     (501) staff       (20)    14866 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/jmetal/algorithm/multiobjective/smpso.py
+-rw-r--r--   0 benhid     (501) staff       (20)     4190 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/jmetal/algorithm/multiobjective/spea2.py
+drwxr-xr-x   0 benhid     (501) staff       (20)        0 2023-04-19 14:32:18.663817 jmetalpy-1.6.0/jmetal/algorithm/singleobjective/
+-rw-r--r--   0 benhid     (501) staff       (20)      188 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/jmetal/algorithm/singleobjective/__init__.py
+-rw-r--r--   0 benhid     (501) staff       (20)     3128 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/jmetal/algorithm/singleobjective/evolution_strategy.py
+-rw-r--r--   0 benhid     (501) staff       (20)     4335 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/jmetal/algorithm/singleobjective/genetic_algorithm.py
+-rw-r--r--   0 benhid     (501) staff       (20)     2735 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/jmetal/algorithm/singleobjective/local_search.py
+-rw-r--r--   0 benhid     (501) staff       (20)     3237 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/jmetal/algorithm/singleobjective/simulated_annealing.py
+drwxr-xr-x   0 benhid     (501) staff       (20)        0 2023-04-19 14:32:18.665026 jmetalpy-1.6.0/jmetal/algorithm/test/
+-rw-r--r--   0 benhid     (501) staff       (20)        0 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/jmetal/algorithm/test/__init__.py
+-rw-r--r--   0 benhid     (501) staff       (20)     3079 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/jmetal/algorithm/test/ittest_algorithm.py
+-rw-r--r--   0 benhid     (501) staff       (20)     1080 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/jmetal/config.py
+drwxr-xr-x   0 benhid     (501) staff       (20)        0 2023-04-19 14:32:18.669908 jmetalpy-1.6.0/jmetal/core/
+-rw-r--r--   0 benhid     (501) staff       (20)        0 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/jmetal/core/__init__.py
+-rw-r--r--   0 benhid     (501) staff       (20)     7033 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/jmetal/core/algorithm.py
+-rw-r--r--   0 benhid     (501) staff       (20)      645 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/jmetal/core/observer.py
+-rw-r--r--   0 benhid     (501) staff       (20)     1728 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/jmetal/core/operator.py
+-rw-r--r--   0 benhid     (501) staff       (20)     5594 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/jmetal/core/problem.py
+-rw-r--r--   0 benhid     (501) staff       (20)    14055 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/jmetal/core/quality_indicator.py
+-rw-r--r--   0 benhid     (501) staff       (20)     6144 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/jmetal/core/solution.py
+drwxr-xr-x   0 benhid     (501) staff       (20)        0 2023-04-19 14:32:18.674272 jmetalpy-1.6.0/jmetal/core/test/
+-rw-r--r--   0 benhid     (501) staff       (20)        0 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/jmetal/core/test/__init__.py
+-rw-r--r--   0 benhid     (501) staff       (20)     1923 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/jmetal/core/test/test_observable.py
+-rw-r--r--   0 benhid     (501) staff       (20)     1443 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/jmetal/core/test/test_operator.py
+-rw-r--r--   0 benhid     (501) staff       (20)     2933 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/jmetal/core/test/test_problem.py
+-rw-r--r--   0 benhid     (501) staff       (20)    11178 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/jmetal/core/test/test_quality_indicator.py
+-rw-r--r--   0 benhid     (501) staff       (20)     8802 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/jmetal/core/test/test_solution.py
+drwxr-xr-x   0 benhid     (501) staff       (20)        0 2023-04-19 14:32:18.675948 jmetalpy-1.6.0/jmetal/lab/
+-rw-r--r--   0 benhid     (501) staff       (20)        0 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/jmetal/lab/__init__.py
+-rw-r--r--   0 benhid     (501) staff       (20)    30362 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/jmetal/lab/experiment.py
+drwxr-xr-x   0 benhid     (501) staff       (20)        0 2023-04-19 14:32:18.680948 jmetalpy-1.6.0/jmetal/lab/statistical_test/
+-rw-r--r--   0 benhid     (501) staff       (20)        0 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/jmetal/lab/statistical_test/__init__.py
+-rw-r--r--   0 benhid     (501) staff       (20)    13072 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/jmetal/lab/statistical_test/apv_procedures.py
+-rw-r--r--   0 benhid     (501) staff       (20)     5718 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/jmetal/lab/statistical_test/bayesian.py
+-rw-r--r--   0 benhid     (501) staff       (20)     8803 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/jmetal/lab/statistical_test/critical_distance.py
+-rw-r--r--   0 benhid     (501) staff       (20)    19952 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/jmetal/lab/statistical_test/functions.py
+drwxr-xr-x   0 benhid     (501) staff       (20)        0 2023-04-19 14:32:18.690168 jmetalpy-1.6.0/jmetal/lab/visualization/
+-rw-r--r--   0 benhid     (501) staff       (20)      293 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/jmetal/lab/visualization/__init__.py
+-rw-r--r--   0 benhid     (501) staff       (20)    13751 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/jmetal/lab/visualization/chord_plot.py
+-rw-r--r--   0 benhid     (501) staff       (20)     7307 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/jmetal/lab/visualization/interactive.py
+-rw-r--r--   0 benhid     (501) staff       (20)     7013 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/jmetal/lab/visualization/plotting.py
+-rw-r--r--   0 benhid     (501) staff       (20)     4119 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/jmetal/lab/visualization/posterior.py
+-rw-r--r--   0 benhid     (501) staff       (20)     4498 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/jmetal/lab/visualization/streaming.py
+-rw-r--r--   0 benhid     (501) staff       (20)      728 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/jmetal/logger.py
+drwxr-xr-x   0 benhid     (501) staff       (20)        0 2023-04-19 14:32:18.694820 jmetalpy-1.6.0/jmetal/operator/
+-rw-r--r--   0 benhid     (501) staff       (20)     1215 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/jmetal/operator/__init__.py
+-rw-r--r--   0 benhid     (501) staff       (20)    17781 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/jmetal/operator/crossover.py
+-rw-r--r--   0 benhid     (501) staff       (20)    10761 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/jmetal/operator/mutation.py
+-rw-r--r--   0 benhid     (501) staff       (20)    11970 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/jmetal/operator/selection.py
+drwxr-xr-x   0 benhid     (501) staff       (20)        0 2023-04-19 14:32:18.700157 jmetalpy-1.6.0/jmetal/operator/test/
+-rw-r--r--   0 benhid     (501) staff       (20)        0 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/jmetal/operator/test/__init__.py
+-rw-r--r--   0 benhid     (501) staff       (20)    18653 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/jmetal/operator/test/test_crossover.py
+-rw-r--r--   0 benhid     (501) staff       (20)    14021 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/jmetal/operator/test/test_mutation.py
+-rw-r--r--   0 benhid     (501) staff       (20)    15557 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/jmetal/operator/test/test_selection.py
+drwxr-xr-x   0 benhid     (501) staff       (20)        0 2023-04-19 14:32:18.701440 jmetalpy-1.6.0/jmetal/problem/
+-rw-r--r--   0 benhid     (501) staff       (20)      626 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/jmetal/problem/__init__.py
+drwxr-xr-x   0 benhid     (501) staff       (20)        0 2023-04-19 14:32:18.713408 jmetalpy-1.6.0/jmetal/problem/multiobjective/
+-rw-r--r--   0 benhid     (501) staff       (20)        0 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/jmetal/problem/multiobjective/__init__.py
+-rw-r--r--   0 benhid     (501) staff       (20)     5646 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/jmetal/problem/multiobjective/constrained.py
+-rw-r--r--   0 benhid     (501) staff       (20)     9739 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/jmetal/problem/multiobjective/dtlz.py
+-rw-r--r--   0 benhid     (501) staff       (20)     9749 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/jmetal/problem/multiobjective/fda.py
+-rw-r--r--   0 benhid     (501) staff       (20)    19755 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/jmetal/problem/multiobjective/lircmop.py
+-rw-r--r--   0 benhid     (501) staff       (20)    13053 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/jmetal/problem/multiobjective/lz09.py
+drwxr-xr-x   0 benhid     (501) staff       (20)        0 2023-04-19 14:32:18.722066 jmetalpy-1.6.0/jmetal/problem/multiobjective/test/
+-rw-r--r--   0 benhid     (501) staff       (20)        0 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/jmetal/problem/multiobjective/test/__init__.py
+-rw-r--r--   0 benhid     (501) staff       (20)     2851 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/jmetal/problem/multiobjective/test/test_constrained.py
+-rw-r--r--   0 benhid     (501) staff       (20)    13319 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/jmetal/problem/multiobjective/test/test_dtlz.py
+-rw-r--r--   0 benhid     (501) staff       (20)    16974 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/jmetal/problem/multiobjective/test/test_lz09.py
+-rw-r--r--   0 benhid     (501) staff       (20)     7748 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/jmetal/problem/multiobjective/test/test_unconstrained.py
+-rw-r--r--   0 benhid     (501) staff       (20)     9816 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/jmetal/problem/multiobjective/test/test_zdt.py
+-rw-r--r--   0 benhid     (501) staff       (20)     1953 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/jmetal/problem/multiobjective/uf.py
+-rw-r--r--   0 benhid     (501) staff       (20)     9772 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/jmetal/problem/multiobjective/unconstrained.py
+-rw-r--r--   0 benhid     (501) staff       (20)     5051 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/jmetal/problem/multiobjective/zdt.py
+drwxr-xr-x   0 benhid     (501) staff       (20)        0 2023-04-19 14:32:18.727069 jmetalpy-1.6.0/jmetal/problem/singleobjective/
+-rw-r--r--   0 benhid     (501) staff       (20)        0 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/jmetal/problem/singleobjective/__init__.py
+-rw-r--r--   0 benhid     (501) staff       (20)     2912 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/jmetal/problem/singleobjective/knapsack.py
+drwxr-xr-x   0 benhid     (501) staff       (20)        0 2023-04-19 14:32:18.732180 jmetalpy-1.6.0/jmetal/problem/singleobjective/test/
+-rw-r--r--   0 benhid     (501) staff       (20)        0 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/jmetal/problem/singleobjective/test/__init__.py
+-rw-r--r--   0 benhid     (501) staff       (20)     2743 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/jmetal/problem/singleobjective/test/test_knapsack.py
+-rw-r--r--   0 benhid     (501) staff       (20)     4281 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/jmetal/problem/singleobjective/test/test_unconstrained.py
+-rw-r--r--   0 benhid     (501) staff       (20)     3127 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/jmetal/problem/singleobjective/tsp.py
+-rw-r--r--   0 benhid     (501) staff       (20)     4946 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/jmetal/problem/singleobjective/unconstrained.py
+drwxr-xr-x   0 benhid     (501) staff       (20)        0 2023-04-19 14:32:18.755797 jmetalpy-1.6.0/jmetal/util/
+-rw-r--r--   0 benhid     (501) staff       (20)        0 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/jmetal/util/__init__.py
+-rw-r--r--   0 benhid     (501) staff       (20)     2213 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/jmetal/util/aggregative_function.py
+-rw-r--r--   0 benhid     (501) staff       (20)     7785 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/jmetal/util/archive.py
+-rw-r--r--   0 benhid     (501) staff       (20)     2310 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/jmetal/util/ckecking.py
+-rw-r--r--   0 benhid     (501) staff       (20)     8890 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/jmetal/util/comparator.py
+-rw-r--r--   0 benhid     (501) staff       (20)     1220 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/jmetal/util/constraint_handling.py
+-rw-r--r--   0 benhid     (501) staff       (20)     5659 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/jmetal/util/density_estimator.py
+-rw-r--r--   0 benhid     (501) staff       (20)     1365 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/jmetal/util/distance.py
+-rw-r--r--   0 benhid     (501) staff       (20)     2707 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/jmetal/util/evaluator.py
+-rw-r--r--   0 benhid     (501) staff       (20)     1108 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/jmetal/util/generator.py
+-rw-r--r--   0 benhid     (501) staff       (20)     7630 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/jmetal/util/neighborhood.py
+-rw-r--r--   0 benhid     (501) staff       (20)     1386 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/jmetal/util/observable.py
+-rw-r--r--   0 benhid     (501) staff       (20)     7852 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/jmetal/util/observer.py
+-rw-r--r--   0 benhid     (501) staff       (20)      570 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/jmetal/util/point.py
+-rw-r--r--   0 benhid     (501) staff       (20)     5882 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/jmetal/util/ranking.py
+-rw-r--r--   0 benhid     (501) staff       (20)     2827 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/jmetal/util/replacement.py
+-rw-r--r--   0 benhid     (501) staff       (20)     2776 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/jmetal/util/solution.py
+-rw-r--r--   0 benhid     (501) staff       (20)     2613 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/jmetal/util/termination_criterion.py
+drwxr-xr-x   0 benhid     (501) staff       (20)        0 2023-04-19 14:32:18.765406 jmetalpy-1.6.0/jmetal/util/test/
+-rw-r--r--   0 benhid     (501) staff       (20)        0 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/jmetal/util/test/__init__.py
+-rw-r--r--   0 benhid     (501) staff       (20)      569 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/jmetal/util/test/test_aggregativefunction.py
+-rw-r--r--   0 benhid     (501) staff       (20)    12104 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/jmetal/util/test/test_archive.py
+-rw-r--r--   0 benhid     (501) staff       (20)     1517 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/jmetal/util/test/test_checking.py
+-rw-r--r--   0 benhid     (501) staff       (20)    14917 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/jmetal/util/test/test_comparator.py
+-rw-r--r--   0 benhid     (501) staff       (20)     4470 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/jmetal/util/test/test_constraint_handling.py
+-rw-r--r--   0 benhid     (501) staff       (20)     7627 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/jmetal/util/test/test_density_estimator.py
+-rw-r--r--   0 benhid     (501) staff       (20)     1672 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/jmetal/util/test/test_distance.py
+-rw-r--r--   0 benhid     (501) staff       (20)     2895 2023-04-19 14:29:02.000000 jmetalpy-1.6.0/jmetal/util/test/test_evaluator.py
+-rw-r--r--   0 benhid     (501) staff       (20)    10653 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/jmetal/util/test/test_neighborhood.py
+-rw-r--r--   0 benhid     (501) staff       (20)     1143 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/jmetal/util/test/test_point.py
+-rw-r--r--   0 benhid     (501) staff       (20)     9003 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/jmetal/util/test/test_ranking.py
+-rw-r--r--   0 benhid     (501) staff       (20)     6420 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/jmetal/util/test/test_replacement.py
+drwxr-xr-x   0 benhid     (501) staff       (20)        0 2023-04-19 14:32:18.768516 jmetalpy-1.6.0/jmetalpy.egg-info/
+-rw-r--r--   0 benhid     (501) staff       (20)     6631 2023-04-19 14:32:18.000000 jmetalpy-1.6.0/jmetalpy.egg-info/PKG-INFO
+-rw-r--r--   0 benhid     (501) staff       (20)     9090 2023-04-19 14:32:18.000000 jmetalpy-1.6.0/jmetalpy.egg-info/SOURCES.txt
+-rw-r--r--   0 benhid     (501) staff       (20)        1 2023-04-19 14:32:18.000000 jmetalpy-1.6.0/jmetalpy.egg-info/dependency_links.txt
+-rw-r--r--   0 benhid     (501) staff       (20)        1 2023-04-19 14:32:18.000000 jmetalpy-1.6.0/jmetalpy.egg-info/not-zip-safe
+-rw-r--r--   0 benhid     (501) staff       (20)      321 2023-04-19 14:32:18.000000 jmetalpy-1.6.0/jmetalpy.egg-info/requires.txt
+-rw-r--r--   0 benhid     (501) staff       (20)       16 2023-04-19 14:32:18.000000 jmetalpy-1.6.0/jmetalpy.egg-info/top_level.txt
+-rw-r--r--   0 benhid     (501) staff       (20)      224 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/pyproject.toml
+-rw-r--r--   0 benhid     (501) staff       (20)     1296 2023-04-19 14:32:18.769950 jmetalpy-1.6.0/setup.cfg
+-rw-r--r--   0 benhid     (501) staff       (20)       68 2023-04-19 14:00:53.000000 jmetalpy-1.6.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `jmetalpy-1.5.5/PKG-INFO` & `jmetalpy-1.6.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,147 +1,155 @@
 Metadata-Version: 2.1
 Name: jmetalpy
-Version: 1.5.5
+Version: 1.6.0
 Summary: Python version of the jMetal framework
 Home-page: https://github.com/jMetal/jMetalPy
 Author: Antonio J. Nebro
 Author-email: antonio@lcc.uma.es
-Maintainer: Antonio J. Nebro, Antonio Benitez-Hidalgo
-Maintainer-email: antonio@lcc.uma.es, antonio.benitez@lcc.uma.es
 License: MIT
-Description: ![jMetalPy](docs/source/jmetalpy.png)
-        
-        [![Build Status](https://img.shields.io/travis/jMetal/jMetalPy/master.svg?style=flat-square)](https://travis-ci.org/jMetal/jMetalPy)
-        [![Documentation](https://img.shields.io/badge/docs-online-success?style=flat-square)](https://jmetal.github.io/jMetalPy/index.html)
-        [![PyPI License](https://img.shields.io/pypi/l/jMetalPy.svg?style=flat-square)]()
-        [![PyPI version](https://img.shields.io/pypi/v/jMetalPy.svg?style=flat-square)]()
-        [![PyPI Python version](https://img.shields.io/pypi/pyversions/jMetalPy.svg?style=flat-square)]()
-        
-        A paper introducing jMetalPy is available at: https://doi.org/10.1016/j.swevo.2019.100598
-        
-        ### Table of Contents
-        - [Installation](#installation)
-        - [Usage](#hello-world-)
-        - [Features](#features)
-        - [Changelog](#changelog)
-        - [License](#license)
-        
-        ## Installation
-        
-        You can install the latest version of jMetalPy with `pip`, 
-        
-        ```console
-        pip install jmetalpy  # or "jmetalpy[distributed]"
-        ```
-        
-        <details><summary><b>Notes on installing with <tt>pip</tt></b></summary>
-        <p>
-        
-        jMetalPy includes features for parallel and distributed computing based on [pySpark](https://spark.apache.org/docs/latest/api/python/index.html) and [Dask](https://dask.org/).
-        
-        These (extra) dependencies are *not* automatically installed when running `pip`, which only comprises the core functionality of the framework (enough for most users):
-        
-        ```console
-        pip install jmetalpy
-        ```
-        
-        This is the equivalent of running: 
-        
-        ```console
-        pip install "jmetalpy[core]"
-        ```
-        
-        Other supported commands are listed next:
-        
-        ```console
-        pip install "jmetalpy[docs]"  # Install requirements for building docs
-        pip install "jmetalpy[distributed]"  # Install requirements for parallel/distributed computing
-        pip install "jmetalpy[complete]"  # Install all requirements
-        ```
-        
-        </p>
-        </details>
-        
-        ## Hello, world! 👋
-        
-        Examples of configuring and running all the included algorithms are located [in the documentation](https://jmetal.github.io/jMetalPy/multiobjective.algorithms.html).
-        
-        ```python
-        from jmetal.algorithm.multiobjective import NSGAII
-        from jmetal.operator import SBXCrossover, PolynomialMutation
-        from jmetal.problem import ZDT1
-        from jmetal.util.termination_criterion import StoppingByEvaluations
-        
-        problem = ZDT1()
-        
-        algorithm = NSGAII(
-            problem=problem,
-            population_size=100,
-            offspring_population_size=100,
-            mutation=PolynomialMutation(probability=1.0 / problem.number_of_variables, distribution_index=20),
-            crossover=SBXCrossover(probability=1.0, distribution_index=20),
-            termination_criterion=StoppingByEvaluations(max_evaluations=25000)
-        )
-        
-        algorithm.run()
-        ```
-        
-        We can then proceed to explore the results:
-        
-        ```python
-        from jmetal.util.solution import get_non_dominated_solutions, print_function_values_to_file, \ 
-            print_variables_to_file
-        
-        front = get_non_dominated_solutions(algorithm.get_result())
-        
-        # save to files
-        print_function_values_to_file(front, 'FUN.NSGAII.ZDT1')
-        print_variables_to_file(front, 'VAR.NSGAII.ZDT1')
-        ```
-        
-        Or visualize the Pareto front approximation produced by the algorithm:
-        
-        ```python
-        from jmetal.lab.visualization import Plot
-        
-        plot_front = Plot(title='Pareto front approximation', axis_labels=['x', 'y'])
-        plot_front.plot(front, label='NSGAII-ZDT1', filename='NSGAII-ZDT1', format='png')
-        ```
-        
-        <img src=docs/source/_static/NSGAII-ZDT1.png width=450 alt="Pareto front approximation">
-        
-        ## Features
-        The current release of jMetalPy (v1.5.5) contains the following components:
-        
-        * Algorithms: local search, genetic algorithm, evolution strategy, simulated annealing, random search, NSGA-II, NSGA-III, SMPSO, OMOPSO, MOEA/D, MOEA/D-DRA, MOEA/D-IEpsilon, GDE3, SPEA2, HYPE, IBEA. Preference articulation-based algorithms (G-NSGA-II, G-GDE3, G-SPEA2, SMPSO/RP); Dynamic versions of NSGA-II, SMPSO, and GDE3.
-        * Parallel computing based on Apache Spark and Dask.
-        * Benchmark problems: ZDT1-6, DTLZ1-2, FDA, LZ09, LIR-CMOP, unconstrained (Kursawe, Fonseca, Schaffer, Viennet2), constrained (Srinivas, Tanaka).
-        * Encodings: real, binary, permutations.
-        * Operators: selection (binary tournament, ranking and crowding distance, random, nary random, best solution), crossover (single-point, SBX), mutation (bit-blip, polynomial, uniform, random).
-        * Quality indicators: hypervolume, additive epsilon, GD, IGD.
-        * Pareto front approximation plotting in real-time, static or interactive.
-        * Experiment class for performing studies either alone or alongside [jMetal](https://github.com/jMetal/jMetal).
-        * Pairwise and multiple hypothesis testing for statistical analysis, including several frequentist and Bayesian testing methods, critical distance plots and posterior diagrams.
-        
-        | ![Scatter plot 2D](docs/source/_static/2D.gif) | ![Scatter plot 3D](docs/source/_static/3D.gif) |
-        |-------------- | ----------------  |
-        | ![Parallel coordinates](docs/source/_static/p-c.gif) | ![Interactive chord plot](docs/source/_static/chordplot.gif) |
-        
-        ## Changelog
-        
-        * [v1.5.5] Minor bug fixes.
-        * [v1.5.4] Refactored quality indicators to accept numpy array as input parameter.
-        * [v1.5.4] Added [CompositeSolution](https://github.com/jMetal/jMetalPy/blob/master/jmetal/core/solution.py#L111) class to support mixed combinatorial problems. [#69](https://github.com/jMetal/jMetalPy/issues/69)
-        
-        ## License
-        This project is licensed under the terms of the MIT - see the [LICENSE](LICENSE) file for details.
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Project-URL: Source, https://github.com/jMetal/jMetalPy
+Project-URL: Tracker, https://github.com/jMetal/jMetalPy/issues
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Programming Language :: Python :: 3.6
-Description-Content-Type: text/markdown
-Provides-Extra: core
-Provides-Extra: docs
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown; charset=UTF-8
 Provides-Extra: distributed
-Provides-Extra: complete
+Provides-Extra: dev
+Provides-Extra: test
+Provides-Extra: all
+License-File: LICENSE
+
+![jMetalPy](docs/source/jmetalpy.png)
+
+[![CI](https://github.com/jMetal/jMetalPy/actions/workflows/ci.yml/badge.svg)](https://github.com/jMetal/jMetalPy/actions/workflows/ci.yml)
+[![PyPI Python version](https://img.shields.io/pypi/pyversions/jMetalPy.svg)]()
+[![DOI](https://img.shields.io/badge/DOI-10.1016%2Fj.swevo.2019.100598-blue)](https://doi.org/10.1016/j.swevo.2019.100598)
+[![PyPI License](https://img.shields.io/pypi/l/jMetalPy.svg)]()
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+A paper introducing jMetalPy is available at: https://doi.org/10.1016/j.swevo.2019.100598
+
+### Table of Contents
+- [Installation](#installation)
+- [Usage](#hello-world-)
+- [Features](#features)
+- [Changelog](#changelog)
+- [License](#license)
+
+## Installation
+
+You can install the latest version of jMetalPy with `pip`, 
+
+```console
+pip install jmetalpy  # or "jmetalpy[distributed]"
+```
+
+<details><summary><b>Notes on installing with <tt>pip</tt></b></summary>
+<p>
+
+jMetalPy includes features for parallel and distributed computing based on [pySpark](https://spark.apache.org/docs/latest/api/python/index.html) and [Dask](https://dask.org/).
+
+These (extra) dependencies are *not* automatically installed when running `pip`, which only comprises the core functionality of the framework (enough for most users):
+
+```console
+pip install jmetalpy
+```
+
+This is the equivalent of running: 
+
+```console
+pip install "jmetalpy[core]"
+```
+
+Other supported commands are listed next:
+
+```console
+pip install "jmetalpy[dev]"  # Install requirements for development
+pip install "jmetalpy[distributed]"  # Install requirements for parallel/distributed computing
+pip install "jmetalpy[complete]"  # Install all requirements
+```
+
+</p>
+</details>
+
+## Hello, world! 👋
+
+Examples of configuring and running all the included algorithms are located [in the documentation](https://jmetal.github.io/jMetalPy/multiobjective.algorithms.html).
+
+```python
+from jmetal.algorithm.multiobjective import NSGAII
+from jmetal.operator import SBXCrossover, PolynomialMutation
+from jmetal.problem import ZDT1
+from jmetal.util.termination_criterion import StoppingByEvaluations
+
+problem = ZDT1()
+
+algorithm = NSGAII(
+    problem=problem,
+    population_size=100,
+    offspring_population_size=100,
+    mutation=PolynomialMutation(probability=1.0 / problem.number_of_variables, distribution_index=20),
+    crossover=SBXCrossover(probability=1.0, distribution_index=20),
+    termination_criterion=StoppingByEvaluations(max_evaluations=25000)
+)
+
+algorithm.run()
+```
+
+We can then proceed to explore the results:
+
+```python
+from jmetal.util.solution import get_non_dominated_solutions, print_function_values_to_file, \ 
+    print_variables_to_file
+
+front = get_non_dominated_solutions(algorithm.get_result())
+
+# save to files
+print_function_values_to_file(front, 'FUN.NSGAII.ZDT1')
+print_variables_to_file(front, 'VAR.NSGAII.ZDT1')
+```
+
+Or visualize the Pareto front approximation produced by the algorithm:
+
+```python
+from jmetal.lab.visualization import Plot
+
+plot_front = Plot(title='Pareto front approximation', axis_labels=['x', 'y'])
+plot_front.plot(front, label='NSGAII-ZDT1', filename='NSGAII-ZDT1', format='png')
+```
+
+<img src=docs/source/_static/NSGAII-ZDT1.png width=450 alt="Pareto front approximation">
+
+## Features
+The current release of jMetalPy (v1.5.7) contains the following components:
+
+* Algorithms: local search, genetic algorithm, evolution strategy, simulated annealing, random search, NSGA-II, NSGA-III, SMPSO, OMOPSO, MOEA/D, MOEA/D-DRA, MOEA/D-IEpsilon, GDE3, SPEA2, HYPE, IBEA. Preference articulation-based algorithms (G-NSGA-II, G-GDE3, G-SPEA2, SMPSO/RP); Dynamic versions of NSGA-II, SMPSO, and GDE3.
+* Parallel computing based on Apache Spark and Dask.
+* Benchmark problems: ZDT1-6, DTLZ1-2, FDA, LZ09, LIR-CMOP, unconstrained (Kursawe, Fonseca, Schaffer, Viennet2), constrained (Srinivas, Tanaka).
+* Encodings: real, binary, permutations.
+* Operators: selection (binary tournament, ranking and crowding distance, random, nary random, best solution), crossover (single-point, SBX), mutation (bit-blip, polynomial, uniform, random).
+* Quality indicators: hypervolume, additive epsilon, GD, IGD.
+* Pareto front approximation plotting in real-time, static or interactive.
+* Experiment class for performing studies either alone or alongside [jMetal](https://github.com/jMetal/jMetal).
+* Pairwise and multiple hypothesis testing for statistical analysis, including several frequentist and Bayesian testing methods, critical distance plots and posterior diagrams.
+
+| ![Scatter plot 2D](docs/source/_static/2D.gif) | ![Scatter plot 3D](docs/source/_static/3D.gif) |
+|-------------- | ----------------  |
+| ![Parallel coordinates](docs/source/_static/p-c.gif) | ![Interactive chord plot](docs/source/_static/chordplot.gif) |
+
+## Changelog
+
+* [v1.6.0] Refactor class Problem, the single-objective genetic algorithm can solve constrained problems, performance improvements in NSGA-II, generation of Latex tables summarizing the results of the Wilcoxon rank sum test, added a notebook folder with examples.
+* [v1.5.7] Use of linters for catching errors and formatters to fix style, minor bug fixes.
+* [v1.5.6] Removed warnings when using Python 3.8.
+* [v1.5.5] Minor bug fixes.
+* [v1.5.4] Refactored quality indicators to accept numpy array as input parameter.
+* [v1.5.4] Added [CompositeSolution](https://github.com/jMetal/jMetalPy/blob/master/jmetal/core/solution.py#L111) class to support mixed combinatorial problems. [#69](https://github.com/jMetal/jMetalPy/issues/69)
+
+## License
+
+This project is licensed under the terms of the MIT - see the [LICENSE](LICENSE) file for details.
```

### Comparing `jmetalpy-1.5.5/README.md` & `jmetalpy-1.6.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ![jMetalPy](docs/source/jmetalpy.png)
 
-[![Build Status](https://img.shields.io/travis/jMetal/jMetalPy/master.svg?style=flat-square)](https://travis-ci.org/jMetal/jMetalPy)
-[![Documentation](https://img.shields.io/badge/docs-online-success?style=flat-square)](https://jmetal.github.io/jMetalPy/index.html)
-[![PyPI License](https://img.shields.io/pypi/l/jMetalPy.svg?style=flat-square)]()
-[![PyPI version](https://img.shields.io/pypi/v/jMetalPy.svg?style=flat-square)]()
-[![PyPI Python version](https://img.shields.io/pypi/pyversions/jMetalPy.svg?style=flat-square)]()
+[![CI](https://github.com/jMetal/jMetalPy/actions/workflows/ci.yml/badge.svg)](https://github.com/jMetal/jMetalPy/actions/workflows/ci.yml)
+[![PyPI Python version](https://img.shields.io/pypi/pyversions/jMetalPy.svg)]()
+[![DOI](https://img.shields.io/badge/DOI-10.1016%2Fj.swevo.2019.100598-blue)](https://doi.org/10.1016/j.swevo.2019.100598)
+[![PyPI License](https://img.shields.io/pypi/l/jMetalPy.svg)]()
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 A paper introducing jMetalPy is available at: https://doi.org/10.1016/j.swevo.2019.100598
 
 ### Table of Contents
 - [Installation](#installation)
 - [Usage](#hello-world-)
 - [Features](#features)
@@ -39,15 +39,15 @@
 ```console
 pip install "jmetalpy[core]"
 ```
 
 Other supported commands are listed next:
 
 ```console
-pip install "jmetalpy[docs]"  # Install requirements for building docs
+pip install "jmetalpy[dev]"  # Install requirements for development
 pip install "jmetalpy[distributed]"  # Install requirements for parallel/distributed computing
 pip install "jmetalpy[complete]"  # Install all requirements
 ```
 
 </p>
 </details>
 
@@ -96,15 +96,15 @@
 plot_front = Plot(title='Pareto front approximation', axis_labels=['x', 'y'])
 plot_front.plot(front, label='NSGAII-ZDT1', filename='NSGAII-ZDT1', format='png')
 ```
 
 <img src=docs/source/_static/NSGAII-ZDT1.png width=450 alt="Pareto front approximation">
 
 ## Features
-The current release of jMetalPy (v1.5.5) contains the following components:
+The current release of jMetalPy (v1.5.7) contains the following components:
 
 * Algorithms: local search, genetic algorithm, evolution strategy, simulated annealing, random search, NSGA-II, NSGA-III, SMPSO, OMOPSO, MOEA/D, MOEA/D-DRA, MOEA/D-IEpsilon, GDE3, SPEA2, HYPE, IBEA. Preference articulation-based algorithms (G-NSGA-II, G-GDE3, G-SPEA2, SMPSO/RP); Dynamic versions of NSGA-II, SMPSO, and GDE3.
 * Parallel computing based on Apache Spark and Dask.
 * Benchmark problems: ZDT1-6, DTLZ1-2, FDA, LZ09, LIR-CMOP, unconstrained (Kursawe, Fonseca, Schaffer, Viennet2), constrained (Srinivas, Tanaka).
 * Encodings: real, binary, permutations.
 * Operators: selection (binary tournament, ranking and crowding distance, random, nary random, best solution), crossover (single-point, SBX), mutation (bit-blip, polynomial, uniform, random).
 * Quality indicators: hypervolume, additive epsilon, GD, IGD.
@@ -114,13 +114,17 @@
 
 | ![Scatter plot 2D](docs/source/_static/2D.gif) | ![Scatter plot 3D](docs/source/_static/3D.gif) |
 |-------------- | ----------------  |
 | ![Parallel coordinates](docs/source/_static/p-c.gif) | ![Interactive chord plot](docs/source/_static/chordplot.gif) |
 
 ## Changelog
 
+* [v1.6.0] Refactor class Problem, the single-objective genetic algorithm can solve constrained problems, performance improvements in NSGA-II, generation of Latex tables summarizing the results of the Wilcoxon rank sum test, added a notebook folder with examples.
+* [v1.5.7] Use of linters for catching errors and formatters to fix style, minor bug fixes.
+* [v1.5.6] Removed warnings when using Python 3.8.
 * [v1.5.5] Minor bug fixes.
 * [v1.5.4] Refactored quality indicators to accept numpy array as input parameter.
 * [v1.5.4] Added [CompositeSolution](https://github.com/jMetal/jMetalPy/blob/master/jmetal/core/solution.py#L111) class to support mixed combinatorial problems. [#69](https://github.com/jMetal/jMetalPy/issues/69)
 
 ## License
+
 This project is licensed under the terms of the MIT - see the [LICENSE](LICENSE) file for details.
```

### Comparing `jmetalpy-1.5.5/examples/experiment/comparison.py` & `jmetalpy-1.6.0/examples/experiment/comparison.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,66 +17,68 @@
         for problem_tag, problem in problems.items():
             jobs.append(
                 Job(
                     algorithm=NSGAII(
                         problem=problem,
                         population_size=100,
                         offspring_population_size=100,
-                        mutation=PolynomialMutation(probability=1.0 / problem.number_of_variables,
-                                                    distribution_index=20),
+                        mutation=PolynomialMutation(
+                            probability=1.0 / problem.number_of_variables, distribution_index=20
+                        ),
                         crossover=SBXCrossover(probability=1.0, distribution_index=20),
-                        termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations)
+                        termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations),
                     ),
-                    algorithm_tag='NSGAII',
+                    algorithm_tag="NSGAII",
                     problem_tag=problem_tag,
                     run=run,
                 )
             )
             jobs.append(
                 Job(
                     algorithm=GDE3(
                         problem=problem,
                         population_size=100,
                         cr=0.5,
                         f=0.5,
-                        termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations)
+                        termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations),
                     ),
-                    algorithm_tag='GDE3',
+                    algorithm_tag="GDE3",
                     problem_tag=problem_tag,
                     run=run,
                 )
             )
             jobs.append(
                 Job(
                     algorithm=SMPSO(
                         problem=problem,
                         swarm_size=100,
-                        mutation=PolynomialMutation(probability=1.0 / problem.number_of_variables,
-                                                    distribution_index=20),
+                        mutation=PolynomialMutation(
+                            probability=1.0 / problem.number_of_variables, distribution_index=20
+                        ),
                         leaders=CrowdingDistanceArchive(100),
-                        termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations)
+                        termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations),
                     ),
-                    algorithm_tag='SMPSO',
+                    algorithm_tag="SMPSO",
                     problem_tag=problem_tag,
                     run=run,
                 )
             )
 
     return jobs
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     # Configure the experiments
-    jobs = configure_experiment(problems={'ZDT1': ZDT1(), 'ZDT2': ZDT2(), 'ZDT3': ZDT3()}, n_run=25)
+    jobs = configure_experiment(problems={"ZDT1": ZDT1(), "ZDT2": ZDT2(), "ZDT3": ZDT3()}, n_run=2)
 
     # Run the study
-    output_directory = 'data'
+    output_directory = "data"
 
     experiment = Experiment(output_dir=output_directory, jobs=jobs)
     experiment.run()
 
     # Generate summary file
     generate_summary_from_experiment(
         input_dir=output_directory,
-        reference_fronts='resources/reference_front',
-        quality_indicators=[GenerationalDistance(), EpsilonIndicator(), HyperVolume([1.0, 1.0])]
+        reference_fronts="resources/reference_front",
+        quality_indicators=[GenerationalDistance(), EpsilonIndicator(), HyperVolume([1.0, 1.0])],
     )
```

### Comparing `jmetalpy-1.5.5/examples/experiment/statistical_analysis.py` & `jmetalpy-1.6.0/examples/experiment/statistical_analysis.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,68 +1,75 @@
-from jmetal.lab.experiment import generate_boxplot, generate_latex_tables, compute_mean_indicator, compute_wilcoxon
+from jmetal.lab.experiment import (
+    compute_mean_indicator,
+    compute_wilcoxon,
+    generate_boxplot,
+    generate_latex_tables,
+)
 from jmetal.lab.statistical_test.bayesian import *
 from jmetal.lab.statistical_test.functions import *
 from jmetal.lab.visualization import CDplot, plot_posterior
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     # Generate Median & IQR tables
-    generate_latex_tables(filename='QualityIndicatorSummary.csv')
+    generate_latex_tables(filename="QualityIndicatorSummary.csv")
 
     # Generate boxplots
-    generate_boxplot(filename='QualityIndicatorSummary.csv')
+    generate_boxplot(filename="QualityIndicatorSummary.csv")
 
     # Wilcoxon
-    compute_wilcoxon(filename='QualityIndicatorSummary.csv')
+    compute_wilcoxon(filename="QualityIndicatorSummary.csv")
 
     # Statistical lab
 
-    avg = compute_mean_indicator(filename='QualityIndicatorSummary.csv', indicator_name='HV')
+    avg = compute_mean_indicator(filename="QualityIndicatorSummary.csv", indicator_name="HV")
     print(avg)
 
     # Non-parametric test
-    print('-------- Sign Test --------')
-    print(sign_test(avg[['NSGAII', 'SMPSO']]))
-    print('-------- Friedman Test --------')
+    print("-------- Sign Test --------")
+    print(sign_test(avg[["NSGAII", "SMPSO"]]))
+    print("-------- Friedman Test --------")
     print(friedman_test(avg))
-    print('-------- Friedman Aligned Rank Test --------')
+    print("-------- Friedman Aligned Rank Test --------")
     print(friedman_aligned_rank_test(avg))
-    print('-------- Quade Test --------')
+    print("-------- Quade Test --------")
     print(quade_test(avg))
 
     # Post-hoc tests
-    print('-------- Friedman Post-Hoc Test --------')
-    z, p_val, adj_pval = friedman_ph_test(avg, control=0, apv_procedure='Bonferroni')
-    print('z values \n', z)
-    print('p-values \n', p_val)
-    print('adjusted p-values \n', adj_pval)
-    print('-------- Friedman Aligned Rank Post-Hoc Test --------')
-    z, p_val, adj_pval = friedman_aligned_ph_test(avg, apv_procedure='Shaffer')
-    print('z values \n', z)
-    print('p-values \n', p_val)
-    print('adjusted p-values \n', adj_pval)
-    print('-------- QuadeTest Post-Hoc Test --------')
-    z, p_val, adj_pval = quade_ph_test(avg, apv_procedure='Holm')
-    print('z values \n', z)
-    print('p-values \n', p_val)
-    print('adjusted p-values \n', adj_pval)
+    print("-------- Friedman Post-Hoc Test --------")
+    z, p_val, adj_pval = friedman_ph_test(avg, control=0, apv_procedure="Bonferroni")
+    print("z values \n", z)
+    print("p-values \n", p_val)
+    print("adjusted p-values \n", adj_pval)
+    print("-------- Friedman Aligned Rank Post-Hoc Test --------")
+    z, p_val, adj_pval = friedman_aligned_ph_test(avg, apv_procedure="Shaffer")
+    print("z values \n", z)
+    print("p-values \n", p_val)
+    print("adjusted p-values \n", adj_pval)
+    print("-------- QuadeTest Post-Hoc Test --------")
+    z, p_val, adj_pval = quade_ph_test(avg, apv_procedure="Holm")
+    print("z values \n", z)
+    print("p-values \n", p_val)
+    print("adjusted p-values \n", adj_pval)
 
     # Plot critical distance
 
     CDplot(avg.T, alpha=0.15, higher_is_better=True)
 
-    print('-------- Bayesian Sign Test --------')
-    bst, DProcess = bayesian_sign_test(avg[['NSGAII', 'SMPSO']], rope_limits=[-0.002, 0.002],
-                                       prior_strength=0.5, return_sample=True)
-    plot_posterior(DProcess, higher_is_better=True, alg_names=['NSGAII', 'SMPSO'])
-
-    print('Pr(NSGAII < SMPSO) = %.3f' % bst[0])
-    print('Pr(NSGAII ~= SMPSO) = %.3f' % bst[1])
-    print('Pr(NSGAII > SMPSO) = %.3f' % bst[2])
-
-    print('-------- Bayesian Signed Rank Test --------')
-    bst, DProcess = bayesian_signed_rank_test(avg[['NSGAII', 'SMPSO']], rope_limits=[-0.002, 0.002],
-                                              prior_strength=0.5, return_sample=True)
-    plot_posterior(DProcess, higher_is_better=True, alg_names=['NSGAII', 'SMPSO'])
-
-    print('Pr(NSGAII < SMPSO) = %.3f' % bst[0])
-    print('Pr(NSGAII ~= SMPSO) = %.3f' % bst[1])
-    print('Pr(NSGAII > SMPSO) = %.3f' % bst[2])
+    print("-------- Bayesian Sign Test --------")
+    bst, DProcess = bayesian_sign_test(
+        avg[["NSGAII", "SMPSO"]], rope_limits=[-0.002, 0.002], prior_strength=0.5, return_sample=True
+    )
+    plot_posterior(DProcess, higher_is_better=True, alg_names=["NSGAII", "SMPSO"])
+
+    print("Pr(NSGAII < SMPSO) = %.3f" % bst[0])
+    print("Pr(NSGAII ~= SMPSO) = %.3f" % bst[1])
+    print("Pr(NSGAII > SMPSO) = %.3f" % bst[2])
+
+    print("-------- Bayesian Signed Rank Test --------")
+    bst, DProcess = bayesian_signed_rank_test(
+        avg[["NSGAII", "SMPSO"]], rope_limits=[-0.002, 0.002], prior_strength=0.5, return_sample=True
+    )
+    plot_posterior(DProcess, higher_is_better=True, alg_names=["NSGAII", "SMPSO"])
+
+    print("Pr(NSGAII < SMPSO) = %.3f" % bst[0])
+    print("Pr(NSGAII ~= SMPSO) = %.3f" % bst[1])
+    print("Pr(NSGAII > SMPSO) = %.3f" % bst[2])
```

### Comparing `jmetalpy-1.5.5/examples/multiobjective/gde3/dynamic_gde3.py` & `jmetalpy-1.6.0/examples/multiobjective/gde3/dynamic_gde3.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from jmetal.algorithm.multiobjective.gde3 import DynamicGDE3
 from jmetal.problem.multiobjective.fda import FDA2
 from jmetal.util.observable import TimeCounter
-from jmetal.util.observer import WriteFrontToFileObserver, PlotFrontToFileObserver
+from jmetal.util.observer import PlotFrontToFileObserver, WriteFrontToFileObserver
 from jmetal.util.termination_criterion import StoppingByEvaluations
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     problem = FDA2()
 
     time_counter = TimeCounter(delay=1)
     time_counter.observable.register(problem)
     time_counter.start()
 
     algorithm = DynamicGDE3(
         problem=problem,
         population_size=100,
         cr=0.5,
         f=0.5,
-        termination_criterion=StoppingByEvaluations(max_evaluations=500)
+        termination_criterion=StoppingByEvaluations(max_evaluations=500),
     )
 
-    algorithm.observable.register(observer=PlotFrontToFileObserver('dynamic_front_vis'))
-    algorithm.observable.register(observer=WriteFrontToFileObserver('dynamic_front'))
+    algorithm.observable.register(observer=PlotFrontToFileObserver("dynamic_front_vis"))
+    algorithm.observable.register(observer=WriteFrontToFileObserver("dynamic_front"))
 
     algorithm.run()
```

### Comparing `jmetalpy-1.5.5/examples/multiobjective/gde3/gde3_spark_evaluator.py` & `jmetalpy-1.6.0/examples/multiobjective/gde3/gde3_spark_evaluator.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from jmetal.algorithm.multiobjective.gde3 import GDE3
 from jmetal.problem.multiobjective.zdt import ZDT1Modified
 from jmetal.util.evaluator import SparkEvaluator
 from jmetal.util.solution import print_function_values_to_file, print_variables_to_file
 from jmetal.util.termination_criterion import StoppingByEvaluations
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     problem = ZDT1Modified()
 
     algorithm = GDE3(
         problem=problem,
         population_size=10,
         cr=0.5,
         f=0.5,
         termination_criterion=StoppingByEvaluations(max_evaluations=100),
-        population_evaluator=SparkEvaluator()
+        population_evaluator=SparkEvaluator(),
     )
 
     algorithm.run()
     front = algorithm.get_result()
 
     # Save results to file
-    print_function_values_to_file(front, 'FUN.' + algorithm.get_name() + "." + problem.get_name())
-    print_variables_to_file(front, 'VAR.' + algorithm.get_name() + "." + problem.get_name())
+    print_function_values_to_file(front, "FUN." + algorithm.get_name() + "." + problem.name())
+    print_variables_to_file(front, "VAR." + algorithm.get_name() + "." + problem.name())
 
-    print('Algorithm (continuous problem): ' + algorithm.get_name())
-    print('Problem: ' + problem.get_name())
-    print('Computing time: ' + str(algorithm.total_computing_time))
+    print(f"Algorithm (continuous problem): {algorithm.get_name()}")
+    print(f"Problem: {problem.name()}")
+    print(f"Computing time: {algorithm.total_computing_time}")
```

### Comparing `jmetalpy-1.5.5/examples/multiobjective/gde3/gde3_zdt1.py` & `jmetalpy-1.6.0/examples/multiobjective/gde3/gde3_zdt1.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 from jmetal.algorithm.multiobjective.gde3 import GDE3
 from jmetal.problem import ZDT1
-from jmetal.util.solution import read_solutions, print_function_values_to_file, print_variables_to_file
+from jmetal.util.solution import (
+    print_function_values_to_file,
+    print_variables_to_file,
+    read_solutions,
+)
 from jmetal.util.termination_criterion import StoppingByKeyboard
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     problem = ZDT1()
-    problem.reference_front = read_solutions(filename='resources/reference_front/ZDT1.pf')
+    problem.reference_front = read_solutions(filename="resources/reference_front/ZDT1.pf")
 
-    algorithm = GDE3(
-        problem=problem,
-        population_size=100,
-        cr=0.5,
-        f=0.5,
-        termination_criterion=StoppingByKeyboard()
-    )
+    algorithm = GDE3(problem=problem, population_size=100, cr=0.5, f=0.5, termination_criterion=StoppingByKeyboard())
 
     algorithm.run()
     front = algorithm.get_result()
 
     # Save results to file
-    print_function_values_to_file(front, 'FUN.' + algorithm.label)
-    print_variables_to_file(front, 'VAR.'+ algorithm.label)
+    print_function_values_to_file(front, "FUN." + algorithm.label)
+    print_variables_to_file(front, "VAR." + algorithm.label)
 
-    print(f'Algorithm: ${algorithm.get_name()}')
-    print(f'Problem: ${problem.get_name()}')
-    print(f'Computing time: ${algorithm.total_computing_time}')
+    print(f"Algorithm: {algorithm.get_name()}")
+    print(f"Problem: {problem.name()}")
+    print(f"Computing time: {algorithm.total_computing_time}")
```

### Comparing `jmetalpy-1.5.5/examples/multiobjective/gde3/ggde3_zdt2.py` & `jmetalpy-1.6.0/examples/multiobjective/gde3/ggde3_zdt2.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 from jmetal.algorithm.multiobjective.gde3 import GDE3
 from jmetal.problem import ZDT2
 from jmetal.util.comparator import GDominanceComparator
-from jmetal.util.solution import read_solutions, print_function_values_to_file, print_variables_to_file
+from jmetal.util.solution import (
+    print_function_values_to_file,
+    print_variables_to_file,
+    read_solutions,
+)
 from jmetal.util.termination_criterion import StoppingByEvaluations
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     problem = ZDT2()
-    problem.reference_front = read_solutions(filename='resources/reference_front/ZDT2.pf')
+    problem.reference_front = read_solutions(filename="resources/reference_front/ZDT2.pf")
 
     max_evaluations = 25000
     reference_point = [0.2, 0.5]
 
     algorithm = GDE3(
         problem=problem,
         population_size=100,
         cr=0.5,
         f=0.5,
         termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations),
-        dominance_comparator=GDominanceComparator(reference_point)
+        dominance_comparator=GDominanceComparator(reference_point),
     )
 
     algorithm.run()
     front = algorithm.get_result()
 
     # Save results to file
-    print_function_values_to_file(front, 'FUN.' + algorithm.label)
-    print_variables_to_file(front, 'VAR.'+ algorithm.label)
+    print_function_values_to_file(front, "FUN." + algorithm.label)
+    print_variables_to_file(front, "VAR." + algorithm.label)
 
-    print(f'Algorithm: ${algorithm.get_name()}')
-    print(f'Problem: ${problem.get_name()}')
-    print(f'Computing time: ${algorithm.total_computing_time}')
+    print(f"Algorithm: {algorithm.get_name()}")
+    print(f"Problem: {problem.name()}")
+    print(f"Computing time: {algorithm.total_computing_time}")
```

### Comparing `jmetalpy-1.5.5/examples/multiobjective/hype/hype_zdt1.py` & `jmetalpy-1.6.0/examples/multiobjective/spea2/gspea2_zdt1.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,36 @@
-from jmetal.algorithm.multiobjective.hype import HYPE
-from jmetal.core.solution import FloatSolution
-from jmetal.operator import SBXCrossover, PolynomialMutation
+from jmetal.algorithm.multiobjective.spea2 import SPEA2
+from jmetal.operator import PolynomialMutation, SBXCrossover
 from jmetal.problem import ZDT1
-from jmetal.util.solution import read_solutions, print_function_values_to_file, print_variables_to_file
+from jmetal.util.comparator import GDominanceComparator
+from jmetal.util.solution import (
+    print_function_values_to_file,
+    print_variables_to_file,
+)
 from jmetal.util.termination_criterion import StoppingByEvaluations
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     problem = ZDT1()
-    problem.reference_front = read_solutions(filename='resources/reference_front/ZDT1.pf')
 
-    reference_point = FloatSolution([0], [1], problem.number_of_objectives, )
-    reference_point.objectives = [1., 1.]  # Mandatory for HYPE
+    reference_point = [0.4, 0.6]
 
-    algorithm = HYPE(
+    max_evaluations = 25000
+    algorithm = SPEA2(
         problem=problem,
-        reference_point=reference_point,
-        population_size=100,
-        offspring_population_size=100,
-        mutation=PolynomialMutation(probability=1.0 / problem.number_of_variables, distribution_index=20),
+        population_size=40,
+        offspring_population_size=40,
+        mutation=PolynomialMutation(probability=1.0 / problem.number_of_variables(), distribution_index=20),
         crossover=SBXCrossover(probability=1.0, distribution_index=20),
-        termination_criterion=StoppingByEvaluations(25000)
+        termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations),
+        dominance_comparator=GDominanceComparator(reference_point),
     )
 
     algorithm.run()
     front = algorithm.get_result()
 
     # Save results to file
-    print_function_values_to_file(front, 'FUN.' + algorithm.label)
-    print_variables_to_file(front, 'VAR.'+ algorithm.label)
+    print_function_values_to_file(front, "FUN." + algorithm.label)
+    print_variables_to_file(front, "VAR." + algorithm.label)
 
-    print(f'Algorithm: ${algorithm.get_name()}')
-    print(f'Problem: ${problem.get_name()}')
-    print(f'Computing time: ${algorithm.total_computing_time}')
+    print(f"Algorithm: {algorithm.get_name()}")
+    print(f"Problem: {problem.name()}")
+    print(f"Computing time: {algorithm.total_computing_time}")
```

### Comparing `jmetalpy-1.5.5/examples/multiobjective/ibea/ibea_zdt1.py` & `jmetalpy-1.6.0/examples/multiobjective/nsgaiii/nsgaiii_dtlz2.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,39 @@
-from jmetal.algorithm.multiobjective.ibea import IBEA
-from jmetal.operator import SBXCrossover, PolynomialMutation
-from jmetal.problem import ZDT1
-from jmetal.util.solution import read_solutions, print_function_values_to_file, print_variables_to_file
+from jmetal.algorithm.multiobjective.nsgaiii import (
+    NSGAIII,
+    UniformReferenceDirectionFactory,
+)
+from jmetal.operator import PolynomialMutation, SBXCrossover
+from jmetal.problem import DTLZ2
+from jmetal.util.solution import (
+    get_non_dominated_solutions,
+    print_function_values_to_file,
+    print_variables_to_file,
+    read_solutions,
+)
 from jmetal.util.termination_criterion import StoppingByEvaluations
 
-if __name__ == '__main__':
-    problem = ZDT1()
-    problem.reference_front = read_solutions(filename='resources/reference_front/ZDT1.pf')
+if __name__ == "__main__":
+    problem = DTLZ2()
+    reference_front = read_solutions(filename="resources/reference_front/DTLZ2.3D.pf")
 
-    algorithm = IBEA(
+    max_evaluations = 25000
+
+    algorithm = NSGAIII(
         problem=problem,
-        kappa=1.,
-        population_size=100,
-        offspring_population_size=100,
-        mutation=PolynomialMutation(probability=1.0 / problem.number_of_variables, distribution_index=20),
-        crossover=SBXCrossover(probability=1.0, distribution_index=20),
-        termination_criterion=StoppingByEvaluations(max_evaluations=25000)
+        population_size=92,
+        reference_directions=UniformReferenceDirectionFactory(3, n_points=91),
+        mutation=PolynomialMutation(probability=1.0 / problem.number_of_variables(), distribution_index=20),
+        crossover=SBXCrossover(probability=1.0, distribution_index=30),
+        termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations),
     )
 
     algorithm.run()
-    front = algorithm.get_result()
+    front = get_non_dominated_solutions(algorithm.get_result())
 
     # Save results to file
-    print_function_values_to_file(front, 'FUN.' + algorithm.label)
-    print_variables_to_file(front, 'VAR.'+ algorithm.label)
+    print_function_values_to_file(front, "FUN." + algorithm.label)
+    print_variables_to_file(front, "VAR." + algorithm.label)
 
-    print(f'Algorithm: ${algorithm.get_name()}')
-    print(f'Problem: ${problem.get_name()}')
-    print(f'Computing time: ${algorithm.total_computing_time}')
+    print(f"Algorithm: {algorithm.get_name()}")
+    print(f"Problem: {problem.name()}")
+    print(f"Computing time: {algorithm.total_computing_time}")
```

### Comparing `jmetalpy-1.5.5/examples/multiobjective/mocell/mocell_zdt1.py` & `jmetalpy-1.6.0/examples/multiobjective/omopso/omopso_zdt1.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,42 @@
-from jmetal.util.solution_list import print_function_values_to_file, print_variables_to_file
-
-from jmetal.algorithm.multiobjective.mocell import MOCell
-from jmetal.operator import SBXCrossover, PolynomialMutation
+from jmetal.algorithm.multiobjective.omopso import OMOPSO
+from jmetal.operator import UniformMutation
+from jmetal.operator.mutation import NonUniformMutation
 from jmetal.problem import ZDT1
 from jmetal.util.archive import CrowdingDistanceArchive
-from jmetal.util.neighborhood import C9
-from jmetal.util.solution import read_solutions
+from jmetal.util.solution import (
+    print_function_values_to_file,
+    print_variables_to_file,
+    read_solutions,
+)
 from jmetal.util.termination_criterion import StoppingByEvaluations
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     problem = ZDT1()
-    problem.reference_front = read_solutions(filename='resources/reference_front/ZDT4.pf')
+    problem.reference_front = read_solutions(filename="resources/reference_front/ZDT1.pf")
 
+    mutation_probability = 1.0 / problem.number_of_variables()
     max_evaluations = 25000
-    algorithm = MOCell(
+    swarm_size = 100
+
+    algorithm = OMOPSO(
         problem=problem,
-        population_size=100,
-        neighborhood=C9(10, 10),
-        archive=CrowdingDistanceArchive(100),
-        mutation=PolynomialMutation(probability=1.0 / problem.number_of_variables, distribution_index=20),
-        crossover=SBXCrossover(probability=1.0, distribution_index=20),
-        termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations)
+        swarm_size=swarm_size,
+        epsilon=0.0075,
+        uniform_mutation=UniformMutation(probability=mutation_probability, perturbation=0.5),
+        non_uniform_mutation=NonUniformMutation(
+            mutation_probability, perturbation=0.5, max_iterations=int(max_evaluations / swarm_size)
+        ),
+        leaders=CrowdingDistanceArchive(100),
+        termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations),
     )
 
     algorithm.run()
     front = algorithm.get_result()
 
     # Save results to file
-    print_function_values_to_file(front, 'FUN.' + algorithm.label)
-    print_variables_to_file(front, 'VAR.'+ algorithm.label)
+    print_function_values_to_file(front, "FUN." + algorithm.label)
+    print_variables_to_file(front, "VAR." + algorithm.label)
 
-    print(f'Algorithm: ${algorithm.get_name()}')
-    print(f'Problem: ${problem.get_name()}')
-    print(f'Computing time: ${algorithm.total_computing_time}')
+    print(f"Algorithm: {algorithm.get_name()}")
+    print(f"Problem: {problem.name()}")
+    print(f"Computing time: {algorithm.total_computing_time}")
```

### Comparing `jmetalpy-1.5.5/examples/multiobjective/moead/moead_dtlz2.py` & `jmetalpy-1.6.0/examples/multiobjective/moead/moeaddra_lz09.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,44 @@
-from jmetal.algorithm.multiobjective.moead import MOEAD
-from jmetal.core.quality_indicator import HyperVolume, InvertedGenerationalDistance
-from jmetal.operator import PolynomialMutation, DifferentialEvolutionCrossover
-from jmetal.problem import DTLZ2
+from jmetal.algorithm.multiobjective.moead import MOEAD_DRA
+from jmetal.core.quality_indicator import HyperVolume
+from jmetal.operator import DifferentialEvolutionCrossover, PolynomialMutation
+from jmetal.problem.multiobjective.uf import UF1
 from jmetal.util.aggregative_function import Tschebycheff
-from jmetal.util.solution import read_solutions, print_function_values_to_file, print_variables_to_file
+from jmetal.util.solution import (
+    print_function_values_to_file,
+    print_variables_to_file,
+    read_solutions,
+)
 from jmetal.util.termination_criterion import StoppingByEvaluations
 
-if __name__ == '__main__':
-    problem = DTLZ2()
-    problem.reference_front = read_solutions(filename='resources/reference_front/DTLZ2.3D.pf')
+if __name__ == "__main__":
+    problem = UF1()
+    problem.reference_front = read_solutions(filename="resources/reference_front/UF1.pf")
 
-    max_evaluations = 50000
+    max_evaluations = 300000
 
-    algorithm = MOEAD(
+    algorithm = MOEAD_DRA(
         problem=problem,
-        population_size=300,
+        population_size=600,
         crossover=DifferentialEvolutionCrossover(CR=1.0, F=0.5),
         mutation=PolynomialMutation(probability=1.0 / problem.number_of_variables, distribution_index=20),
         aggregative_function=Tschebycheff(dimension=problem.number_of_objectives),
         neighbor_size=20,
         neighbourhood_selection_probability=0.9,
         max_number_of_replaced_solutions=2,
-        weight_files_path='resources/MOEAD_weights',
-        termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations)
+        weight_files_path="resources/MOEAD_weights",
+        termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations),
     )
 
     algorithm.run()
     front = algorithm.get_result()
 
-    hypervolume = HyperVolume([1.0, 1.0, 1.0])
+    hypervolume = HyperVolume([2.0, 2.0])
     print("Hypervolume: " + str(hypervolume.compute([front[i].objectives for i in range(len(front))])))
 
     # Save results to file
-    print_function_values_to_file(front, 'FUN.' + algorithm.label)
-    print_variables_to_file(front, 'VAR.'+ algorithm.label)
+    print_function_values_to_file(front, "FUN." + algorithm.label)
+    print_variables_to_file(front, "VAR." + algorithm.label)
 
-    print(f'Algorithm: ${algorithm.get_name()}')
-    print(f'Problem: ${problem.get_name()}')
-    print(f'Computing time: ${algorithm.total_computing_time}')
+    print(f"Algorithm: {algorithm.get_name()}")
+    print(f"Problem: {problem.name()}")
+    print(f"Computing time: {algorithm.total_computing_time}")
```

### Comparing `jmetalpy-1.5.5/examples/multiobjective/moead/moead_iepsilon_lircmop1.py` & `jmetalpy-1.6.0/examples/multiobjective/moead/moead_iepsilon_lircmop1.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 from jmetal.algorithm.multiobjective.moead import MOEADIEpsilon
-from jmetal.operator import PolynomialMutation, DifferentialEvolutionCrossover
+from jmetal.operator import DifferentialEvolutionCrossover, PolynomialMutation
 from jmetal.problem.multiobjective.lircmop import LIRCMOP2
 from jmetal.util.aggregative_function import Tschebycheff
-from jmetal.util.solution import read_solutions, print_function_values_to_file, print_variables_to_file
+from jmetal.util.solution import (
+    print_function_values_to_file,
+    print_variables_to_file,
+    read_solutions,
+)
 from jmetal.util.termination_criterion import StoppingByEvaluations
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     problem = LIRCMOP2()
 
-    problem.reference_front = read_solutions(filename='resources/reference_front/LIRCMOP2.pf')
+    problem.reference_front = read_solutions(filename="resources/reference_front/LIRCMOP2.pf")
 
     max_evaluations = 300000
 
     algorithm = MOEADIEpsilon(
         problem=problem,
         population_size=300,
         crossover=DifferentialEvolutionCrossover(CR=1.0, F=0.5),
         mutation=PolynomialMutation(probability=1.0 / problem.number_of_variables, distribution_index=20),
         aggregative_function=Tschebycheff(dimension=problem.number_of_objectives),
         neighbor_size=20,
         neighbourhood_selection_probability=0.9,
         max_number_of_replaced_solutions=2,
-        weight_files_path='resources/MOEAD_weights',
-        termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations)
+        weight_files_path="resources/MOEAD_weights",
+        termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations),
     )
 
     algorithm.run()
     front = algorithm.get_result()
 
     # Save results to file
-    print_function_values_to_file(front, 'FUN.' + algorithm.label)
-    print_variables_to_file(front, 'VAR.'+ algorithm.label)
+    print_function_values_to_file(front, "FUN." + algorithm.label)
+    print_variables_to_file(front, "VAR." + algorithm.label)
 
-    print(f'Algorithm: ${algorithm.get_name()}')
-    print(f'Problem: ${problem.get_name()}')
-    print(f'Computing time: ${algorithm.total_computing_time}')
+    print(f"Algorithm: {algorithm.get_name()}")
+    print(f"Problem: {problem.name()}")
+    print(f"Computing time: {algorithm.total_computing_time}")
```

### Comparing `jmetalpy-1.5.5/examples/multiobjective/moead/moead_lz09.py` & `jmetalpy-1.6.0/examples/multiobjective/moead/moead_lz09.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 from jmetal.algorithm.multiobjective.moead import MOEAD
-from jmetal.operator import PolynomialMutation, DifferentialEvolutionCrossover
+from jmetal.operator import DifferentialEvolutionCrossover, PolynomialMutation
 from jmetal.problem import LZ09_F2
 from jmetal.util.aggregative_function import Tschebycheff
-from jmetal.util.solution import read_solutions, print_function_values_to_file, print_variables_to_file
+from jmetal.util.solution import (
+    print_function_values_to_file,
+    print_variables_to_file,
+    read_solutions,
+)
 from jmetal.util.termination_criterion import StoppingByEvaluations
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     problem = LZ09_F2()
 
-    problem.reference_front = read_solutions(filename='resources/reference_front/LZ09_F2.pf')
+    problem.reference_front = read_solutions(filename="resources/reference_front/LZ09_F2.pf")
 
     max_evaluations = 150000
 
     algorithm = MOEAD(
         problem=problem,
         population_size=300,
         crossover=DifferentialEvolutionCrossover(CR=1.0, F=0.5),
-        mutation=PolynomialMutation(probability=1.0 / problem.number_of_variables, distribution_index=20),
-        aggregative_function=Tschebycheff(dimension=problem.number_of_objectives),
+        mutation=PolynomialMutation(probability=1.0 / problem.number_of_variables(), distribution_index=20),
+        aggregative_function=Tschebycheff(dimension=problem.number_of_objectives()),
         neighbor_size=20,
         neighbourhood_selection_probability=0.9,
         max_number_of_replaced_solutions=2,
-        weight_files_path='resources/MOEAD_weights',
-        termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations)
+        weight_files_path="resources/MOEAD_weights",
+        termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations),
     )
 
     algorithm.run()
     front = algorithm.get_result()
 
     # Save results to file
-    print_function_values_to_file(front, 'FUN.' + algorithm.label)
-    print_variables_to_file(front, 'VAR.'+ algorithm.label)
+    print_function_values_to_file(front, "FUN." + algorithm.label)
+    print_variables_to_file(front, "VAR." + algorithm.label)
 
-    print(f'Algorithm: ${algorithm.get_name()}')
-    print(f'Problem: ${problem.get_name()}')
-    print(f'Computing time: ${algorithm.total_computing_time}')
+    print(f"Algorithm: {algorithm.get_name()}")
+    print(f"Problem: {problem.get_name()}")
+    print(f"Computing time: {algorithm.total_computing_time}")
```

### Comparing `jmetalpy-1.5.5/examples/multiobjective/moead/moeaddra_lz09.py` & `jmetalpy-1.6.0/examples/multiobjective/moead/moead_dtlz2.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,44 @@
-from jmetal.algorithm.multiobjective.moead import MOEAD_DRA
-from jmetal.operator import PolynomialMutation, DifferentialEvolutionCrossover
-from jmetal.problem import LZ09_F2
-from jmetal.problem.multiobjective.uf import UF1
-from jmetal.util.aggregative_function import Tschebycheff
-from jmetal.util.solution import read_solutions, print_function_values_to_file, print_variables_to_file
+from jmetal.algorithm.multiobjective.moead import MOEAD
+from jmetal.core.quality_indicator import HyperVolume
+from jmetal.operator import DifferentialEvolutionCrossover, PolynomialMutation
+from jmetal.problem import DTLZ2
+from jmetal.util.aggregative_function import PenaltyBoundaryIntersection
+from jmetal.util.solution import (
+    print_function_values_to_file,
+    print_variables_to_file,
+    read_solutions,
+)
 from jmetal.util.termination_criterion import StoppingByEvaluations
-from jmetal.core.quality_indicator import HyperVolume, InvertedGenerationalDistance
 
-if __name__ == '__main__':
-    problem = UF1()
-    problem.reference_front = read_solutions(filename='resources/reference_front/UF1.pf')
+if __name__ == "__main__":
+    problem = DTLZ2()
+    problem.reference_front = read_solutions(filename="resources/reference_front/DTLZ2.3D.pf")
 
-    max_evaluations = 300000
+    max_evaluations = 50000
 
-    algorithm = MOEAD_DRA(
+    algorithm = MOEAD(
         problem=problem,
-        population_size=600,
+        population_size=91,
         crossover=DifferentialEvolutionCrossover(CR=1.0, F=0.5),
-        mutation=PolynomialMutation(probability=1.0 / problem.number_of_variables, distribution_index=20),
-        aggregative_function=Tschebycheff(dimension=problem.number_of_objectives),
+        mutation=PolynomialMutation(probability=1.0 / problem.number_of_variables(), distribution_index=20),
+        aggregative_function=PenaltyBoundaryIntersection(dimension=problem.number_of_objectives()),
         neighbor_size=20,
         neighbourhood_selection_probability=0.9,
         max_number_of_replaced_solutions=2,
-        weight_files_path='resources/MOEAD_weights',
-        termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations)
+        weight_files_path="resources/MOEAD_weights",
+        termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations),
     )
 
     algorithm.run()
     front = algorithm.get_result()
 
-    hypervolume = HyperVolume([2.0, 2.0])
+    hypervolume = HyperVolume([1.0, 1.0, 1.0])
     print("Hypervolume: " + str(hypervolume.compute([front[i].objectives for i in range(len(front))])))
 
     # Save results to file
-    print_function_values_to_file(front, 'FUN.' + algorithm.label)
-    print_variables_to_file(front, 'VAR.'+ algorithm.label)
-
-    print(f'Algorithm: ${algorithm.get_name()}')
-    print(f'Problem: ${problem.get_name()}')
-    print(f'Computing time: ${algorithm.total_computing_time}')
-
+    print_function_values_to_file(front, "FUN." + algorithm.label)
+    print_variables_to_file(front, "VAR." + algorithm.label)
 
+    print(f"Algorithm: {algorithm.get_name()}")
+    print(f"Problem: {problem.name()}")
+    print(f"Computing time: {algorithm.total_computing_time}")
```

### Comparing `jmetalpy-1.5.5/examples/multiobjective/nsgaii/distributed_nsgaii_with_dask.py` & `jmetalpy-1.6.0/examples/multiobjective/nsgaii/distributed_nsgaii_with_dask.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,36 +6,35 @@
 from jmetal.problem.multiobjective.zdt import ZDT1Modified
 from jmetal.util.termination_criterion import StoppingByEvaluations
 
 """ 
 Distributed (asynchronous) version of NSGA-II using Dask.
 """
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     problem = ZDT1Modified()
 
     # setup Dask client
     client = Client(LocalCluster(n_workers=24))
 
     ncores = sum(client.ncores().values())
-    print(f'{ncores} cores available')
+    print(f"{ncores} cores available")
 
     # creates the algorithm
     max_evaluations = 25000
 
     algorithm = DistributedNSGAII(
         problem=problem,
         population_size=100,
         mutation=PolynomialMutation(probability=1.0 / problem.number_of_variables, distribution_index=20),
         crossover=SBXCrossover(probability=1.0, distribution_index=20),
         termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations),
         number_of_cores=ncores,
-        client=client
+        client=client,
     )
 
     algorithm.run()
     front = algorithm.get_result()
 
-    print('Algorithm: ' + algorithm.get_name())
-    print('Problem: ' + problem.get_name())
-    print('Computing time: ' + str(algorithm.total_computing_time))
-
+    print(f"Algorithm: {algorithm.get_name()}")
+    print(f"Problem: {problem.get_name()}")
+    print(f"Computing time: {algorithm.total_computing_time}")
```

### Comparing `jmetalpy-1.5.5/examples/multiobjective/nsgaii/distributed_nsgaii_with_dask_evaluator.py` & `jmetalpy-1.6.0/examples/multiobjective/nsgaii/distributed_nsgaii_with_dask_evaluator.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 from jmetal.algorithm.multiobjective.nsgaii import NSGAII
-from jmetal.operator import SBXCrossover, PolynomialMutation
+from jmetal.operator import PolynomialMutation, SBXCrossover
 from jmetal.problem.multiobjective.zdt import ZDT1Modified
 from jmetal.util.evaluator import DaskEvaluator
 from jmetal.util.solution import print_function_values_to_file, print_variables_to_file
 from jmetal.util.termination_criterion import StoppingByEvaluations
 
 """ 
 Distributed (synchronous) version of NSGA-II using Dask.
 """
-if __name__ == '__main__':
+if __name__ == "__main__":
     problem = ZDT1Modified()
 
     max_evaluations = 100
 
     algorithm = NSGAII(
         problem=problem,
         population_size=10,
         offspring_population_size=10,
         mutation=PolynomialMutation(probability=1.0 / problem.number_of_variables, distribution_index=20),
         crossover=SBXCrossover(probability=1.0, distribution_index=20),
         population_evaluator=DaskEvaluator(),
-        termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations)
+        termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations),
     )
 
     algorithm.run()
     front = algorithm.get_result()
 
     # Save results to file
-    print_function_values_to_file(front, 'FUN.' + algorithm.label)
-    print_variables_to_file(front, 'VAR.'+ algorithm.label)
-
-    print(f'Algorithm: ${algorithm.get_name()}')
-    print(f'Problem: ${problem.get_name()}')
-    print(f'Computing time: ${algorithm.total_computing_time}')
+    print_function_values_to_file(front, "FUN." + algorithm.label)
+    print_variables_to_file(front, "VAR." + algorithm.label)
 
+    print(f"Algorithm: {algorithm.get_name()}")
+    print(f"Problem: {problem.get_name()}")
+    print(f"Computing time: {algorithm.total_computing_time}")
```

### Comparing `jmetalpy-1.5.5/examples/multiobjective/nsgaii/distributed_nsgaii_with_spark_evaluator.py` & `jmetalpy-1.6.0/examples/multiobjective/nsgaii/parallel_nsgaii_with_multiprocess_evaluator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,32 @@
 from jmetal.algorithm.multiobjective.nsgaii import NSGAII
-from jmetal.operator import SBXCrossover, PolynomialMutation
+from jmetal.operator import PolynomialMutation, SBXCrossover
 from jmetal.problem.multiobjective.zdt import ZDT1Modified
-from jmetal.util.evaluator import SparkEvaluator
+from jmetal.util.evaluator import MultiprocessEvaluator
 from jmetal.util.solution import print_function_values_to_file, print_variables_to_file
 from jmetal.util.termination_criterion import StoppingByEvaluations
 
-""" 
-Distributed (synchronous) version of NSGA-II using Apache Spark.
-"""
-
-if __name__ == '__main__':
+if __name__ == "__main__":
     problem = ZDT1Modified()
 
     max_evaluations = 100
 
     algorithm = NSGAII(
+        population_evaluator=MultiprocessEvaluator(8),
         problem=problem,
         population_size=10,
         offspring_population_size=10,
-        mutation=PolynomialMutation(probability=1.0 / problem.number_of_variables, distribution_index=20),
+        mutation=PolynomialMutation(probability=1.0 / problem.number_of_variables(), distribution_index=20),
         crossover=SBXCrossover(probability=1.0, distribution_index=20),
-        population_evaluator=SparkEvaluator(),
-        termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations)
+        termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations),
     )
 
     algorithm.run()
     front = algorithm.get_result()
 
     # Save results to file
-    print_function_values_to_file(front, 'FUN.' + algorithm.label)
-    print_variables_to_file(front, 'VAR.'+ algorithm.label)
+    print_function_values_to_file(front, "FUN." + algorithm.label)
+    print_variables_to_file(front, "VAR." + algorithm.label)
 
-    print(f'Algorithm: ${algorithm.get_name()}')
-    print(f'Problem: ${problem.get_name()}')
-    print(f'Computing time: ${algorithm.total_computing_time}')
+    print(f"Algorithm: {algorithm.get_name()}")
+    print(f"Problem: {problem.name()}")
+    print(f"Computing time: {algorithm.total_computing_time}")
```

### Comparing `jmetalpy-1.5.5/examples/multiobjective/nsgaii/dynamic_nsgaii_solving_fda2.py` & `jmetalpy-1.6.0/examples/multiobjective/nsgaii/dynamic_nsgaii_solving_fda2.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from jmetal.algorithm.multiobjective.nsgaii import DynamicNSGAII
 from jmetal.operator import PolynomialMutation, SBXCrossover
 from jmetal.problem.multiobjective.fda import FDA2
 from jmetal.util.observable import TimeCounter
 from jmetal.util.observer import PlotFrontToFileObserver, WriteFrontToFileObserver
 from jmetal.util.termination_criterion import StoppingByEvaluations
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     problem = FDA2()
 
     time_counter = TimeCounter(delay=1)
     time_counter.observable.register(problem)
     time_counter.start()
 
     max_evaluations = 25000
     algorithm = DynamicNSGAII(
         problem=problem,
         population_size=100,
         offspring_population_size=100,
         mutation=PolynomialMutation(probability=1.0 / problem.number_of_variables, distribution_index=20),
         crossover=SBXCrossover(probability=1.0, distribution_index=20),
-        termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations)
+        termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations),
     )
 
-    algorithm.observable.register(observer=PlotFrontToFileObserver('dynamic_front_vis'))
-    algorithm.observable.register(observer=WriteFrontToFileObserver('dynamic_front'))
+    algorithm.observable.register(observer=PlotFrontToFileObserver("dynamic_front_vis"))
+    algorithm.observable.register(observer=WriteFrontToFileObserver("dynamic_front"))
 
     algorithm.run()
```

### Comparing `jmetalpy-1.5.5/examples/multiobjective/nsgaii/gnsgaii_solving_zdt2_with_reference_point.py` & `jmetalpy-1.6.0/examples/multiobjective/preferences/gnsgaii_solving_zdt2_with_reference_point.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,55 +1,66 @@
 from jmetal.algorithm.multiobjective.nsgaii import NSGAII
-from jmetal.lab.visualization import Plot, InteractivePlot
-from jmetal.operator import SBXCrossover, PolynomialMutation
+from jmetal.lab.visualization import InteractivePlot, Plot
+from jmetal.operator import PolynomialMutation, SBXCrossover
 from jmetal.problem import ZDT2
 from jmetal.util.comparator import GDominanceComparator
 from jmetal.util.observer import ProgressBarObserver, VisualizerObserver
-from jmetal.util.solution import print_function_values_to_file, print_variables_to_file, read_solutions
+from jmetal.util.solution import (
+    print_function_values_to_file,
+    print_variables_to_file,
+    read_solutions,
+)
 from jmetal.util.termination_criterion import StoppingByEvaluations
 
 """  
 Program to configure and run G-NSGA-II (NSGA-II with G-Dominance) to solve problem ZDT2 with 
 reference point = [0.2, 0.5].
 """
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     problem = ZDT2()
-    problem.reference_front = read_solutions(filename='resources/reference_front/ZDT2.pf')
+    reference_front = read_solutions(filename="resources/reference_front/ZDT2.pf")
 
-    reference_point = [0.2, 0.5]
+    reference_point = [0.3, 0.5]
 
     max_evaluations = 25000
     algorithm = NSGAII(
         problem=problem,
         population_size=100,
         offspring_population_size=100,
-        mutation=PolynomialMutation(probability=1.0 / problem.number_of_variables, distribution_index=20),
+        mutation=PolynomialMutation(probability=1.0 / problem.number_of_variables(), distribution_index=20),
         crossover=SBXCrossover(probability=1.0, distribution_index=20),
         dominance_comparator=GDominanceComparator(reference_point),
-        termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations)
+        termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations),
     )
 
     algorithm.observable.register(observer=ProgressBarObserver(max=max_evaluations))
     algorithm.observable.register(
-        observer=VisualizerObserver(reference_front=problem.reference_front, reference_point=reference_point))
+        observer=VisualizerObserver(reference_front=reference_front, reference_point=reference_point)
+    )
 
     algorithm.run()
     front = algorithm.get_result()
 
     # Plot front
-    plot_front = Plot(title='Pareto front approximation. Problem: ' + problem.get_name(),
-                      reference_front=problem.reference_front, axis_labels=problem.obj_labels)
+    plot_front = Plot(
+        title="Pareto front approximation. Problem: " + problem.name(),
+        reference_front=reference_front,
+        axis_labels=problem.obj_labels,
+    )
     plot_front.plot(front, label=algorithm.label, filename=algorithm.get_name())
 
     # Plot interactive front
-    plot_front = InteractivePlot(title='Pareto front approximation. Problem: ' + problem.get_name(),
-                                 reference_front=problem.reference_front, axis_labels=problem.obj_labels)
+    plot_front = InteractivePlot(
+        title="Pareto front approximation. Problem: " + problem.name(),
+        reference_front=reference_front,
+        axis_labels=problem.obj_labels,
+    )
     plot_front.plot(front, label=algorithm.label, filename=algorithm.get_name())
 
     # Save results to file
-    print_function_values_to_file(front, 'FUN.' + algorithm.label)
-    print_variables_to_file(front, 'VAR.' + algorithm.label)
+    print_function_values_to_file(front, "FUN." + algorithm.label)
+    print_variables_to_file(front, "VAR." + algorithm.label)
 
-    print('Algorithm (continuous problem): ' + algorithm.get_name())
-    print('Problem: ' + problem.get_name())
-    print('Computing time: ' + str(algorithm.total_computing_time))
+    print(f"Algorithm: {algorithm.get_name()}")
+    print(f"Problem: {problem.name()}")
+    print(f"Computing time: {algorithm.total_computing_time}")
```

### Comparing `jmetalpy-1.5.5/examples/multiobjective/nsgaii/nsgaii_defining_schaffer_problem_on_the_fly.py` & `jmetalpy-1.6.0/examples/multiobjective/nsgaii/nsgaii_defining_srinivas_problem_on_the_fly.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,49 +1,64 @@
 from jmetal.algorithm.multiobjective.nsgaii import NSGAII
 from jmetal.core.problem import OnTheFlyFloatProblem
-from jmetal.operator import SBXCrossover, PolynomialMutation
-from jmetal.util.solution import get_non_dominated_solutions, read_solutions, print_function_values_to_file, \
-    print_variables_to_file
+from jmetal.operator import PolynomialMutation, SBXCrossover
+from jmetal.util.comparator import DominanceWithConstraintsComparator
+from jmetal.util.solution import (
+    get_non_dominated_solutions,
+    print_function_values_to_file,
+    print_variables_to_file,
+    read_solutions,
+)
 from jmetal.util.termination_criterion import StoppingByEvaluations
 
 """  
 Program to  configure and run the NSGA-II algorithm configured with standard settings.
 """
 
-if __name__ == '__main__':
-    # Defining problem Schaffer on the fly
+if __name__ == "__main__":
+    # Defining problem Srinivas on the fly
     def f1(x: [float]):
-        return x[0] * x[0]
+        return 2.0 + (x[0] - 2.0) * (x[0] - 2.0) + (x[1] - 1.0) * (x[1] - 1.0)
 
     def f2(x: [float]):
-        return (x[0] - 2) * (x[0] - 2)
+        return 9.0 * x[0] - (x[1] - 1.0) * (x[1] - 1.0)
 
-    problem = OnTheFlyFloatProblem()
-    problem \
-        .set_name('Schaffer') \
-        .add_variable(-10000.0, 10000.0) \
-        .add_function(f1) \
+    def c1(x: [float]):
+        return 1.0 - (x[0] * x[0] + x[1] * x[1]) / 225.0
+
+    def c2(x: [float]):
+        return (3.0 * x[1] - x[0]) / 10.0 - 1.0
+
+    problem = (
+        OnTheFlyFloatProblem()
+        .set_name("Srinivas")
+        .add_variable(-20.0, 20.0)
+        .add_variable(-20.0, 20.0)
+        .add_function(f1)
         .add_function(f2)
+        .add_constraint(c1)
+        .add_constraint(c2)
+    )
 
-    problem.reference_front = read_solutions(filename='resources/reference_front/ZDT1.pf')
+    problem.reference_front = read_solutions(filename="resources/reference_front/Srinivas.pf")
 
     max_evaluations = 25000
     algorithm = NSGAII(
         problem=problem,
         population_size=100,
         offspring_population_size=100,
-        mutation=PolynomialMutation(probability=1.0 / problem.number_of_variables, distribution_index=20),
+        mutation=PolynomialMutation(probability=1.0 / problem.number_of_variables(), distribution_index=20),
         crossover=SBXCrossover(probability=1.0, distribution_index=20),
-        termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations)
+        termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations),
+        dominance_comparator=DominanceWithConstraintsComparator()
     )
 
     algorithm.run()
     front = get_non_dominated_solutions(algorithm.get_result())
 
     # Save results to file
-    print_function_values_to_file(front, 'FUN.' + algorithm.label)
-    print_variables_to_file(front, 'VAR.'+ algorithm.label)
-
-    print('Algorithm (continuous problem): ' + algorithm.get_name())
-    print('Problem: ' + problem.get_name())
-    print('Computing time: ' + str(algorithm.total_computing_time))
+    print_function_values_to_file(front, "FUN." + algorithm.label)
+    print_variables_to_file(front, "VAR." + algorithm.label)
 
+    print(f"Algorithm: {algorithm.get_name()}")
+    print(f"Problem: {problem.name()}")
+    print(f"Computing time: {algorithm.total_computing_time}")
```

### Comparing `jmetalpy-1.5.5/examples/multiobjective/nsgaii/nsgaii_defining_srinivas_problem_on_the_fly.py` & `jmetalpy-1.6.0/examples/multiobjective/nsgaii/nsgaii_standard_settings.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,61 +1,38 @@
 from jmetal.algorithm.multiobjective.nsgaii import NSGAII
-from jmetal.core.problem import OnTheFlyFloatProblem
-from jmetal.operator import SBXCrossover, PolynomialMutation
-from jmetal.util.solution import get_non_dominated_solutions, read_solutions, print_function_values_to_file, \
-    print_variables_to_file
+from jmetal.operator import PolynomialMutation, SBXCrossover
+from jmetal.problem import Fonseca
+from jmetal.util.solution import (
+    get_non_dominated_solutions,
+    print_function_values_to_file,
+    print_variables_to_file,
+)
 from jmetal.util.termination_criterion import StoppingByEvaluations
 
 """  
 Program to  configure and run the NSGA-II algorithm configured with standard settings.
 """
 
-if __name__ == '__main__':
-    # Defining problem Srinivas on the fly
-    def f1(x: [float]):
-        return 2.0 + (x[0] - 2.0) * (x[0] - 2.0) + (x[1] - 1.0) * (x[1] - 1.0)
-
-
-    def f2(x: [float]):
-        return 9.0 * x[0] - (x[1] - 1.0) * (x[1] - 1.0)
-
-
-    def c1(x: [float]):
-        return 1.0 - (x[0] * x[0] + x[1] * x[1]) / 225.0
-
-
-    def c2(x: [float]):
-        return (3.0 * x[1] - x[0]) / 10.0 - 1.0
-
-
-    problem = OnTheFlyFloatProblem() \
-        .set_name('Srinivas') \
-        .add_variable(-20.0, 20.0) \
-        .add_variable(-20.0, 20.0) \
-        .add_function(f1) \
-        .add_function(f2) \
-        .add_constraint(c1) \
-        .add_constraint(c2)
-
-    problem.reference_front = read_solutions(filename='resources/reference_front/Srinivas.pf')
+if __name__ == "__main__":
+    problem = Fonseca()
+    #problem.reference_front = read_solutions(filename="resources/reference_front/ZDT1.pf")
 
     max_evaluations = 25000
     algorithm = NSGAII(
         problem=problem,
         population_size=100,
         offspring_population_size=100,
-        mutation=PolynomialMutation(probability=1.0 / problem.number_of_variables, distribution_index=20),
+        mutation=PolynomialMutation(probability=1.0 / problem.number_of_variables(), distribution_index=20),
         crossover=SBXCrossover(probability=1.0, distribution_index=20),
-        termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations)
+        termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations),
     )
 
     algorithm.run()
     front = get_non_dominated_solutions(algorithm.get_result())
 
     # Save results to file
-    print_function_values_to_file(front, 'FUN.' + algorithm.label)
-    print_variables_to_file(front, 'VAR.'+ algorithm.label)
-
-    print('Algorithm (continuous problem): ' + algorithm.get_name())
-    print('Problem: ' + problem.get_name())
-    print('Computing time: ' + str(algorithm.total_computing_time))
+    print_function_values_to_file(front, "FUN." + algorithm.label)
+    print_variables_to_file(front, "VAR." + algorithm.label)
 
+    print(f"Algorithm: {algorithm.get_name()}")
+    print(f"Problem: {problem.name()}")
+    print(f"Computing time: {algorithm.total_computing_time}")
```

### Comparing `jmetalpy-1.5.5/examples/multiobjective/nsgaii/nsgaii_solving_3D_problem.py` & `jmetalpy-1.6.0/examples/multiobjective/nsgaii/distributed_nsgaii_with_spark_evaluator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 from jmetal.algorithm.multiobjective.nsgaii import NSGAII
-from jmetal.operator import SBXCrossover, PolynomialMutation
-from jmetal.problem import DTLZ2
-from jmetal.util.comparator import DominanceComparator
-from jmetal.util.solution import print_function_values_to_file, print_variables_to_file, read_solutions
+from jmetal.operator import PolynomialMutation, SBXCrossover
+from jmetal.problem.multiobjective.zdt import ZDT1Modified
+from jmetal.util.evaluator import SparkEvaluator
+from jmetal.util.solution import print_function_values_to_file, print_variables_to_file
 from jmetal.util.termination_criterion import StoppingByEvaluations
 
-if __name__ == '__main__':
-    problem = DTLZ2()
-    problem.reference_front = read_solutions(filename='resources/reference_front/DTLZ2.3D.pf')
+""" 
+Distributed (synchronous) version of NSGA-II using Apache Spark.
+"""
+
+if __name__ == "__main__":
+    problem = ZDT1Modified()
+
+    max_evaluations = 100
 
-    max_evaluations = 25000
     algorithm = NSGAII(
         problem=problem,
-        population_size=100,
-        offspring_population_size=100,
+        population_size=10,
+        offspring_population_size=10,
         mutation=PolynomialMutation(probability=1.0 / problem.number_of_variables, distribution_index=20),
         crossover=SBXCrossover(probability=1.0, distribution_index=20),
+        population_evaluator=SparkEvaluator(),
         termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations),
-        dominance_comparator=DominanceComparator()
     )
 
     algorithm.run()
     front = algorithm.get_result()
 
     # Save results to file
-    print_function_values_to_file(front, 'FUN.' + algorithm.label)
-    print_variables_to_file(front, 'VAR.'+ algorithm.label)
+    print_function_values_to_file(front, "FUN." + algorithm.label)
+    print_variables_to_file(front, "VAR." + algorithm.label)
 
-    print(f'Algorithm: ${algorithm.get_name()}')
-    print(f'Problem: ${problem.get_name()}')
-    print(f'Computing time: ${algorithm.total_computing_time}')
+    print(f"Algorithm: {algorithm.get_name()}")
+    print(f"Problem: {problem.get_name()}")
+    print(f"Computing time: {algorithm.total_computing_time}")
```

### Comparing `jmetalpy-1.5.5/examples/multiobjective/nsgaii/nsgaii_solving_binary_problem.py` & `jmetalpy-1.6.0/examples/multiobjective/nsgaii/nsgaii_solving_binary_problem.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,31 +5,31 @@
 from jmetal.util.termination_criterion import StoppingByEvaluations
 
 """  
 Program to  configure and run the NSGA-II algorithm configured to solve a binary problem, OneZeroMax, which is 
 multiobjective version of the ONE_MAX problem where the numbers of 1s and 0s have to be maximized at the same time.
 """
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     binary_string_length = 512
     problem = OneZeroMax(binary_string_length)
 
-    max_evaluations = 50000
+    max_evaluations = 30000
     algorithm = NSGAII(
         problem=problem,
         population_size=100,
         offspring_population_size=100,
         mutation=BitFlipMutation(probability=1.0 / binary_string_length),
         crossover=SPXCrossover(probability=1.0),
-        termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations)
+        termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations),
     )
 
     algorithm.run()
     front = algorithm.get_result()
 
     # Save results to file
-    print_function_values_to_file(front, 'FUN.' + algorithm.label)
-    print_variables_to_file(front, 'VAR.'+ algorithm.label)
+    print_function_values_to_file(front, "FUN." + algorithm.label)
+    print_variables_to_file(front, "VAR." + algorithm.label)
 
-    print(f'Algorithm: ${algorithm.get_name()}')
-    print(f'Problem: ${problem.get_name()}')
-    print(f'Computing time: ${algorithm.total_computing_time}')
+    print(f"Algorithm: {algorithm.get_name()}")
+    print(f"Problem: {problem.name()}")
+    print(f"Computing time: {algorithm.total_computing_time}")
```

### Comparing `jmetalpy-1.5.5/examples/multiobjective/nsgaii/nsgaii_solving_constrained_srinivas_problem.py` & `jmetalpy-1.6.0/examples/multiobjective/smpso/smpso_spark_evaluator.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,36 @@
-from jmetal.algorithm.multiobjective import NSGAII
-from jmetal.operator import SBXCrossover, PolynomialMutation
-from jmetal.problem import Srinivas
-from jmetal.util.comparator import DominanceComparator
-from jmetal.util.solution import read_solutions, print_function_values_to_file, print_variables_to_file
+from examples.multiobjective.zdt1_modified import ZDT1Modified
+from jmetal.algorithm.multiobjective.smpso import SMPSO
+from jmetal.operator import PolynomialMutation
+from jmetal.util.archive import CrowdingDistanceArchive
+from jmetal.util.evaluator import SparkEvaluator
+from jmetal.util.solution import (
+    print_function_values_to_file,
+    print_variables_to_file,
+    read_solutions,
+)
 from jmetal.util.termination_criterion import StoppingByEvaluations
 
-if __name__ == '__main__':
-    problem = Srinivas()
-    problem.reference_front = read_solutions(filename='resources/reference_front/Srinivas.pf')
+if __name__ == "__main__":
+    problem = ZDT1Modified()
+    problem.reference_front = read_solutions(filename="resources/reference_front/ZDT1.pf")
 
-    max_evaluations = 25000
-    algorithm = NSGAII(
+    max_evaluations = 100
+    algorithm = SMPSO(
         problem=problem,
-        population_size=100,
-        offspring_population_size=100,
+        swarm_size=10,
         mutation=PolynomialMutation(probability=1.0 / problem.number_of_variables, distribution_index=20),
-        crossover=SBXCrossover(probability=1.0, distribution_index=20),
+        leaders=CrowdingDistanceArchive(10),
         termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations),
-        dominance_comparator=DominanceComparator()
+        swarm_evaluator=SparkEvaluator(),
     )
 
     algorithm.run()
     front = algorithm.get_result()
 
     # Save results to file
-    print_function_values_to_file(front, 'FUN.' + algorithm.label)
-    print_variables_to_file(front, 'VAR.'+ algorithm.label)
+    print_function_values_to_file(front, "FUN." + algorithm.get_name() + "." + problem.get_name())
+    print_variables_to_file(front, "VAR." + algorithm.get_name() + "." + problem.get_name())
 
-    print(f'Algorithm: ${algorithm.get_name()}')
-    print(f'Problem: ${problem.get_name()}')
-    print(f'Computing time: ${algorithm.total_computing_time}')
+    print(f"Algorithm: {algorithm.get_name()}")
+    print(f"Problem: {problem.get_name()}")
+    print(f"Computing time: {algorithm.total_computing_time}")
```

### Comparing `jmetalpy-1.5.5/examples/multiobjective/nsgaii/nsgaii_solving_mixed_encoding_problem.py` & `jmetalpy-1.6.0/examples/multiobjective/nsgaii/nsgaii_solving_mixed_encoding_problem.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,40 @@
 from jmetal.algorithm.multiobjective.nsgaii import NSGAII
-from jmetal.operator import SBXCrossover, PolynomialMutation, IntegerPolynomialMutation
+from jmetal.operator import IntegerPolynomialMutation, PolynomialMutation, SBXCrossover
 from jmetal.operator.crossover import CompositeCrossover, IntegerSBXCrossover
 from jmetal.operator.mutation import CompositeMutation
 from jmetal.problem.multiobjective.unconstrained import MixedIntegerFloatProblem
-from jmetal.util.solution import get_non_dominated_solutions, print_function_values_to_file, \
-    print_variables_to_file
+from jmetal.util.solution import (
+    get_non_dominated_solutions,
+    print_function_values_to_file,
+    print_variables_to_file,
+)
 from jmetal.util.termination_criterion import StoppingByEvaluations
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     problem = MixedIntegerFloatProblem(10, 10, 100, -100, -1000, 1000)
 
     max_evaluations = 25000
     algorithm = NSGAII(
         problem=problem,
         population_size=100,
         offspring_population_size=100,
         mutation=CompositeMutation([IntegerPolynomialMutation(0.01, 20), PolynomialMutation(0.01, 20.0)]),
-        crossover=CompositeCrossover([IntegerSBXCrossover(probability=1.0, distribution_index=20),
-                                      SBXCrossover(probability=1.0, distribution_index=20)]),
-        termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations)
+        crossover=CompositeCrossover(
+            [
+                IntegerSBXCrossover(probability=1.0, distribution_index=20),
+                SBXCrossover(probability=1.0, distribution_index=20),
+            ]
+        ),
+        termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations),
     )
 
     algorithm.run()
     front = get_non_dominated_solutions(algorithm.get_result())
 
     # Save results to file
-    print_function_values_to_file(front, 'FUN.' + algorithm.label)
-    print_variables_to_file(front, 'VAR.' + algorithm.label)
+    print_function_values_to_file(front, "FUN." + algorithm.label)
+    print_variables_to_file(front, "VAR." + algorithm.label)
 
-    print('Algorithm (continuous problem): ' + algorithm.get_name())
-    print('Problem: ' + problem.get_name())
-    print('Computing time: ' + str(algorithm.total_computing_time))
+    print(f"Algorithm: {algorithm.get_name()}")
+    print(f"Problem: {problem.name()}")
+    print(f"Computing time: {algorithm.total_computing_time}")
```

### Comparing `jmetalpy-1.5.5/examples/multiobjective/nsgaii/nsgaii_ssp.py` & `jmetalpy-1.6.0/examples/multiobjective/nsgaii/nsgaii_standard_settings_with_real_time_plotting.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,45 +1,59 @@
 from jmetal.algorithm.multiobjective.nsgaii import NSGAII
-from jmetal.operator import BitFlipMutation, SPXCrossover
-from jmetal.problem.multiobjective.unconstrained import SubsetSum
-from jmetal.util.solution import print_function_values_to_file, print_variables_to_file
+from jmetal.lab.visualization import InteractivePlot, Plot
+from jmetal.operator import PolynomialMutation, SBXCrossover
+from jmetal.problem import ZDT6, ZDT1
+from jmetal.util.observer import ProgressBarObserver, VisualizerObserver
+from jmetal.util.solution import (
+    print_function_values_to_file,
+    print_variables_to_file,
+    read_solutions,
+)
 from jmetal.util.termination_criterion import StoppingByEvaluations
 
-if __name__ == '__main__':
-    C = 300500
-    W = [2902, 5235, 357, 6058, 4846, 8280, 1295, 181, 3264,
-         7285, 8806, 2344, 9203, 6806, 1511, 2172, 843, 4697,
-         3348, 1866, 5800, 4094, 2751, 64, 7181, 9167, 5579,
-         9461, 3393, 4602, 1796, 8174, 1691, 8854, 5902, 4864,
-         5488, 1129, 1111, 7597, 5406, 2134, 7280, 6465, 4084,
-         8564, 2593, 9954, 4731, 1347, 8984, 5057, 3429, 7635,
-         1323, 1146, 5192, 6547, 343, 7584, 3765, 8660, 9318,
-         5098, 5185, 9253, 4495, 892, 5080, 5297, 9275, 7515,
-         9729, 6200, 2138, 5480, 860, 8295, 8327, 9629, 4212,
-         3087, 5276, 9250, 1835, 9241, 1790, 1947, 8146, 8328,
-         973, 1255, 9733, 4314, 6912, 8007, 8911, 6802, 5102,
-         5451, 1026, 8029, 6628, 8121, 5509, 3603, 6094, 4447,
-         683, 6996, 3304, 3130, 2314, 7788, 8689, 3253, 5920,
-         3660, 2489, 8153, 2822, 6132, 7684, 3032, 9949, 59,
-         6669, 6334]
-
-    problem = SubsetSum(C, W)
+"""  
+Program to  configure and run the NSGA-II algorithm configured with standard settings.
+"""
+
+if __name__ == "__main__":
+    problem = ZDT1()
+    problem.reference_front = read_solutions(filename="resources/reference_front/ZDT1.pf")
 
+    max_evaluations = 10000
     algorithm = NSGAII(
         problem=problem,
         population_size=100,
         offspring_population_size=100,
-        mutation=BitFlipMutation(probability=0.5),
-        crossover=SPXCrossover(probability=0.8),
-        termination_criterion=StoppingByEvaluations(max_evaluations=25000)
+        mutation=PolynomialMutation(probability=1.0 / problem.number_of_variables(), distribution_index=20),
+        crossover=SBXCrossover(probability=1.0, distribution_index=20),
+        termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations),
     )
 
+    algorithm.observable.register(observer=ProgressBarObserver(max=max_evaluations))
+    algorithm.observable.register(observer=VisualizerObserver(reference_front=problem.reference_front))
+
     algorithm.run()
     front = algorithm.get_result()
 
+    # Plot front
+    plot_front = Plot(
+        title="Pareto front approximation. Problem: " + problem.name(),
+        reference_front=problem.reference_front,
+        axis_labels=problem.obj_labels,
+    )
+    plot_front.plot(front, label=algorithm.label, filename=algorithm.get_name())
+
+    # Plot interactive front
+    plot_front = InteractivePlot(
+        title="Pareto front approximation. Problem: " + problem.name(),
+        reference_front=problem.reference_front,
+        axis_labels=problem.obj_labels,
+    )
+    plot_front.plot(front, label=algorithm.label, filename=algorithm.get_name())
+
     # Save results to file
-    print_function_values_to_file(front, 'FUN.' + algorithm.label)
-    print_variables_to_file(front, 'VAR.'+ algorithm.label)
+    print_function_values_to_file(front, "FUN." + algorithm.label)
+    print_variables_to_file(front, "VAR." + algorithm.label)
 
-    print(f'Algorithm: ${algorithm.get_name()}')
-    print(f'Problem: ${problem.get_name()}')
-    print(f'Computing time: ${algorithm.total_computing_time}')
+    print(f"Algorithm: {algorithm.get_name()}")
+    print(f"Problem: {problem.name()}")
+    print(f"Computing time: {algorithm.total_computing_time}")
```

### Comparing `jmetalpy-1.5.5/examples/multiobjective/nsgaii/nsgaii_standard_settings.py` & `jmetalpy-1.6.0/examples/multiobjective/nsgaii/nsgaii_steady_state.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 from jmetal.algorithm.multiobjective.nsgaii import NSGAII
-from jmetal.operator import SBXCrossover, PolynomialMutation
+from jmetal.operator import PolynomialMutation, SBXCrossover
 from jmetal.problem import ZDT1
-from jmetal.util.solution import get_non_dominated_solutions, read_solutions, print_function_values_to_file, \
-    print_variables_to_file
+from jmetal.util.solution import (
+    get_non_dominated_solutions,
+    print_function_values_to_file,
+    print_variables_to_file,
+    read_solutions,
+)
 from jmetal.util.termination_criterion import StoppingByEvaluations
 
-
 """  
-Program to  configure and run the NSGA-II algorithm configured with standard settings.
+Program to configure and run a steady-state version of the NSGA-II algorithm (configured with standard settings).
 """
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     problem = ZDT1()
-    problem.reference_front = read_solutions(filename='resources/reference_front/ZDT1.pf')
+    problem.reference_front = read_solutions(filename="resources/reference_front/ZDT1.pf")
 
     max_evaluations = 25000
     algorithm = NSGAII(
         problem=problem,
         population_size=100,
-        offspring_population_size=100,
-        mutation=PolynomialMutation(probability=1.0 / problem.number_of_variables, distribution_index=20),
+        offspring_population_size=1,
+        mutation=PolynomialMutation(probability=1.0 / problem.number_of_variables(), distribution_index=20),
         crossover=SBXCrossover(probability=1.0, distribution_index=20),
-        termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations)
+        termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations),
     )
 
     algorithm.run()
     front = get_non_dominated_solutions(algorithm.get_result())
 
     # Save results to file
-    print_function_values_to_file(front, 'FUN.' + algorithm.label)
-    print_variables_to_file(front, 'VAR.'+ algorithm.label)
-
-    print('Algorithm (continuous problem): ' + algorithm.get_name())
-    print('Problem: ' + problem.get_name())
-    print('Computing time: ' + str(algorithm.total_computing_time))
+    print_function_values_to_file(front, "FUN." + algorithm.label)
+    print_variables_to_file(front, "VAR." + algorithm.label)
 
+    print(f"Algorithm: {algorithm.get_name()}")
+    print(f"Problem: {problem.name()}")
+    print(f"Computing time: {algorithm.total_computing_time}")
```

### Comparing `jmetalpy-1.5.5/examples/multiobjective/nsgaii/nsgaii_standard_settings_with_real_time_plotting.py` & `jmetalpy-1.6.0/examples/multiobjective/preferences/ggde3_zdt2.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,48 +1,51 @@
-from jmetal.algorithm.multiobjective.nsgaii import NSGAII
-from jmetal.lab.visualization import Plot, InteractivePlot
-from jmetal.operator import SBXCrossover, PolynomialMutation
-from jmetal.problem import ZDT1
-from jmetal.util.observer import ProgressBarObserver, VisualizerObserver
-from jmetal.util.solution import read_solutions, print_function_values_to_file, \
-    print_variables_to_file
+
+from jmetal.algorithm.multiobjective.gde3 import GDE3
+from jmetal.lab.visualization import InteractivePlot, Plot
+from jmetal.problem import ZDT2
+from jmetal.util.comparator import GDominanceComparator
+from jmetal.util.observer import VisualizerObserver
+from jmetal.util.solution import read_solutions, print_function_values_to_file, print_variables_to_file
 from jmetal.util.termination_criterion import StoppingByEvaluations
 
-"""  
-Program to  configure and run the NSGA-II algorithm configured with standard settings.
-"""
-
-if __name__ == '__main__':
-    problem = ZDT1()
-    problem.reference_front = read_solutions(filename='resources/reference_front/ZDT1.pf')
+if __name__ == "__main__":
+    problem = ZDT2()
+    reference_front = read_solutions(filename="resources/reference_front/{}.pf".format(problem.name()))
 
     max_evaluations = 25000
-    algorithm = NSGAII(
+    reference_point = [0.4, 0.6]
+
+    algorithm = GDE3(
         problem=problem,
         population_size=100,
-        offspring_population_size=100,
-        mutation=PolynomialMutation(probability=1.0 / problem.number_of_variables, distribution_index=20),
-        crossover=SBXCrossover(probability=1.0, distribution_index=20),
-        termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations)
+        cr=0.5,
+        f=0.5,
+        termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations),
+        dominance_comparator=GDominanceComparator(reference_point),
     )
 
-    algorithm.observable.register(observer=ProgressBarObserver(max=max_evaluations))
-    algorithm.observable.register(observer=VisualizerObserver(reference_front=problem.reference_front))
+    algorithm.observable.register(
+        observer=VisualizerObserver(reference_front=reference_front, reference_point=reference_point)
+    )
 
     algorithm.run()
     front = algorithm.get_result()
 
     # Plot front
-    plot_front = Plot(title='Pareto front approximation. Problem: ' + problem.get_name(), reference_front=problem.reference_front, axis_labels=problem.obj_labels)
+    plot_front = Plot(
+        plot_title="Pareto front approximation", reference_front=reference_front, axis_labels=problem.obj_labels
+    )
     plot_front.plot(front, label=algorithm.label, filename=algorithm.get_name())
 
     # Plot interactive front
-    plot_front = InteractivePlot(title='Pareto front approximation. Problem: ' + problem.get_name(), reference_front=problem.reference_front, axis_labels=problem.obj_labels)
+    plot_front = InteractivePlot(
+        plot_title="Pareto front approximation", reference_front=reference_front, axis_labels=problem.obj_labels
+    )
     plot_front.plot(front, label=algorithm.label, filename=algorithm.get_name())
 
     # Save results to file
-    print_function_values_to_file(front, 'FUN.' + algorithm.label)
-    print_variables_to_file(front, 'VAR.'+ algorithm.label)
+    print_function_values_to_file(front, "FUN." + algorithm.label)
+    print_variables_to_file(front, "VAR." + algorithm.label)
 
-    print('Algorithm (continuous problem): ' + algorithm.get_name())
-    print('Problem: ' + problem.get_name())
-    print('Computing time: ' + str(algorithm.total_computing_time))
+    print(f"Algorithm: {algorithm.get_name()}")
+    print(f"Problem: {problem.name()}")
+    print(f"Computing time: {algorithm.total_computing_time}")
```

### Comparing `jmetalpy-1.5.5/examples/multiobjective/nsgaii/nsgaii_steady_state.py` & `jmetalpy-1.6.0/examples/multiobjective/ibea/ibea_zdt1.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,34 @@
-from jmetal.algorithm.multiobjective.nsgaii import NSGAII
-from jmetal.operator import SBXCrossover, PolynomialMutation
+from jmetal.algorithm.multiobjective.ibea import IBEA
+from jmetal.operator import PolynomialMutation, SBXCrossover
 from jmetal.problem import ZDT1
-from jmetal.util.solution import get_non_dominated_solutions, read_solutions, print_function_values_to_file, \
-    print_variables_to_file
+from jmetal.util.solution import (
+    print_function_values_to_file,
+    print_variables_to_file,
+    read_solutions,
+)
 from jmetal.util.termination_criterion import StoppingByEvaluations
 
-"""  
-Program to configure and run a steady-state version of the NSGA-II algorithm (configured with standard settings).
-"""
-
-if __name__ == '__main__':
+if __name__ == "__main__":
     problem = ZDT1()
-    problem.reference_front = read_solutions(filename='resources/reference_front/ZDT1.pf')
+    problem.reference_front = read_solutions(filename="resources/reference_front/ZDT1.pf")
 
-    max_evaluations = 25000
-    algorithm = NSGAII(
+    algorithm = IBEA(
         problem=problem,
+        kappa=1.0,
         population_size=100,
-        offspring_population_size=1,
-        mutation=PolynomialMutation(probability=1.0 / problem.number_of_variables, distribution_index=20),
+        offspring_population_size=100,
+        mutation=PolynomialMutation(probability=1.0 / problem.number_of_variables(), distribution_index=20),
         crossover=SBXCrossover(probability=1.0, distribution_index=20),
-        termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations)
+        termination_criterion=StoppingByEvaluations(max_evaluations=25000),
     )
 
     algorithm.run()
-    front = get_non_dominated_solutions(algorithm.get_result())
+    front = algorithm.get_result()
 
     # Save results to file
-    print_function_values_to_file(front, 'FUN.' + algorithm.label)
-    print_variables_to_file(front, 'VAR.'+ algorithm.label)
-
-    print('Algorithm (continuous problem): ' + algorithm.get_name())
-    print('Problem: ' + problem.get_name())
-    print('Computing time: ' + str(algorithm.total_computing_time))
+    print_function_values_to_file(front, "FUN." + algorithm.label)
+    print_variables_to_file(front, "VAR." + algorithm.label)
 
+    print(f"Algorithm: {algorithm.get_name()}")
+    print(f"Problem: {problem.name()}")
+    print(f"Computing time: {algorithm.total_computing_time}")
```

### Comparing `jmetalpy-1.5.5/examples/multiobjective/nsgaii/nsgaii_steady_state_with_real_time_plotting.py` & `jmetalpy-1.6.0/examples/multiobjective/nsgaii/nsgaii_steady_state_with_real_time_plotting.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,54 +1,62 @@
 from jmetal.algorithm.multiobjective.nsgaii import NSGAII
 from jmetal.lab.visualization import InteractivePlot, Plot
-from jmetal.operator import SBXCrossover, PolynomialMutation
+from jmetal.operator import PolynomialMutation, SBXCrossover
 from jmetal.problem import ZDT1
 from jmetal.util.observer import ProgressBarObserver, VisualizerObserver
-from jmetal.util.solution import read_solutions, print_function_values_to_file, \
-    print_variables_to_file
+from jmetal.util.solution import (
+    print_function_values_to_file,
+    print_variables_to_file,
+    read_solutions,
+)
 from jmetal.util.termination_criterion import StoppingByEvaluations
 
 """
 Program to configure and run the steady-state NSGA-II algorithm with a real-time plotting observer. The display 
 update frequency is set to 100 evaluations.
 """
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     problem = ZDT1()
-    problem.reference_front = read_solutions(filename='resources/reference_front/ZDT1.pf')
+    problem.reference_front = read_solutions(filename="resources/reference_front/ZDT1.pf")
 
     max_evaluations = 25000
     algorithm = NSGAII(
         problem=problem,
         population_size=100,
         offspring_population_size=1,
-        mutation=PolynomialMutation(probability=1.0 / problem.number_of_variables, distribution_index=20),
+        mutation=PolynomialMutation(probability=1.0 / problem.number_of_variables(), distribution_index=20),
         crossover=SBXCrossover(probability=1.0, distribution_index=20),
-        termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations)
+        termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations),
     )
 
     algorithm.observable.register(observer=ProgressBarObserver(max=max_evaluations))
     algorithm.observable.register(
-        observer=VisualizerObserver(reference_front=problem.reference_front, display_frequency=100))
+        observer=VisualizerObserver(reference_front=problem.reference_front, display_frequency=100)
+    )
 
     algorithm.run()
     front = algorithm.get_result()
 
     # Plot front
-    plot_front = Plot(title='Pareto front approximation. Problem: ' + problem.get_name(),
-                      reference_front=problem.reference_front,
-                      axis_labels=problem.obj_labels)
+    plot_front = Plot(
+        title="Pareto front approximation. Problem: " + problem.name(),
+        reference_front=problem.reference_front,
+        axis_labels=problem.obj_labels,
+    )
     plot_front.plot(front, label=algorithm.label, filename=algorithm.get_name())
 
     # Plot interactive front
-    plot_front = InteractivePlot(title='Pareto front approximation. Problem: ' + problem.get_name(),
-                                 reference_front=problem.reference_front,
-                                 axis_labels=problem.obj_labels)
+    plot_front = InteractivePlot(
+        title="Pareto front approximation. Problem: " + problem.name(),
+        reference_front=problem.reference_front,
+        axis_labels=problem.obj_labels,
+    )
     plot_front.plot(front, label=algorithm.label, filename=algorithm.get_name())
 
     # Save results to file
-    print_function_values_to_file(front, 'FUN.' + algorithm.label)
-    print_variables_to_file(front, 'VAR.' + algorithm.label)
+    print_function_values_to_file(front, "FUN." + algorithm.label)
+    print_variables_to_file(front, "VAR." + algorithm.label)
 
-    print('Algorithm (continuous problem): ' + algorithm.get_name())
-    print('Problem: ' + problem.get_name())
-    print('Computing time: ' + str(algorithm.total_computing_time))
+    print(f"Algorithm: {algorithm.get_name()}")
+    print(f"Problem: {problem.name()}")
+    print(f"Computing time: {algorithm.total_computing_time}")
```

### Comparing `jmetalpy-1.5.5/examples/multiobjective/nsgaii/parallel_nsgaii_with_multiprocess_evaluator.py` & `jmetalpy-1.6.0/examples/singleobjective/nsgaii/nsgaii_single_objective_binary.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 from jmetal.algorithm.multiobjective.nsgaii import NSGAII
-from jmetal.operator import SBXCrossover, PolynomialMutation
-from jmetal.problem.multiobjective.zdt import ZDT1Modified
-from jmetal.util.evaluator import MultiprocessEvaluator
+from jmetal.operator import BitFlipMutation, SPXCrossover
+from jmetal.problem import OneMax
+from jmetal.util.comparator import DominanceComparator
+from jmetal.util.observer import ProgressBarObserver
 from jmetal.util.solution import print_function_values_to_file, print_variables_to_file
 from jmetal.util.termination_criterion import StoppingByEvaluations
 
-if __name__ == '__main__':
-    problem = ZDT1Modified()
+if __name__ == "__main__":
+    binary_string_length = 512
+    problem = OneMax(binary_string_length)
 
-    max_evaluations = 100
+    max_evaluations = 20000
 
     algorithm = NSGAII(
-        population_evaluator=MultiprocessEvaluator(8),
         problem=problem,
-        population_size=10,
-        offspring_population_size=10,
-        mutation=PolynomialMutation(probability=1.0 / problem.number_of_variables, distribution_index=20),
-        crossover=SBXCrossover(probability=1.0, distribution_index=20),
-        termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations)
+        population_size=100,
+        offspring_population_size=100,
+        mutation=BitFlipMutation(probability=1.0 / binary_string_length),
+        crossover=SPXCrossover(probability=1.0),
+        termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations),
+        dominance_comparator=DominanceComparator(),
     )
 
+    algorithm.observable.register(observer=ProgressBarObserver(max=max_evaluations))
+
     algorithm.run()
     front = algorithm.get_result()
 
     # Save results to file
-    print_function_values_to_file(front, 'FUN.' + algorithm.label)
-    print_variables_to_file(front, 'VAR.'+ algorithm.label)
-
-    print(f'Algorithm: ${algorithm.get_name()}')
-    print(f'Problem: ${problem.get_name()}')
-    print(f'Computing time: ${algorithm.total_computing_time}')
+    print_function_values_to_file(front, "FUN." + algorithm.get_name() + "-" + problem.get_name())
+    print_variables_to_file(front, "VAR." + algorithm.get_name() + "-" + problem.get_name())
 
+    print("Algorithm (continuous problem): " + algorithm.get_name())
+    print("Problem: " + problem.get_name())
+    print("Computing time: " + str(algorithm.total_computing_time))
```

### Comparing `jmetalpy-1.5.5/examples/multiobjective/nsgaiii/nsgaiii_dtlz2.py` & `jmetalpy-1.6.0/examples/singleobjective/local_search/local_search_float.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,29 @@
-from jmetal.algorithm.multiobjective.nsgaiii import NSGAIII, UniformReferenceDirectionFactory
-from jmetal.operator import SBXCrossover, PolynomialMutation
-from jmetal.problem import DTLZ2
-from jmetal.util.solution import read_solutions, print_function_values_to_file, print_variables_to_file
+from jmetal.algorithm.singleobjective.local_search import LocalSearch
+from jmetal.operator import PolynomialMutation
+from jmetal.problem.singleobjective.unconstrained import Rastrigin
+from jmetal.util.solution import print_function_values_to_file, print_variables_to_file
 from jmetal.util.termination_criterion import StoppingByEvaluations
 
-if __name__ == '__main__':
-    problem = DTLZ2()
-    problem.reference_front = read_solutions(filename='resources/reference_front/DTLZ2.3D.pf')
+if __name__ == "__main__":
+    problem = Rastrigin(10)
 
-    max_evaluations = 25000
+    max_evaluations = 100000
 
-    algorithm = NSGAIII(
+    algorithm = LocalSearch(
         problem=problem,
-        population_size=92,
-        reference_directions=UniformReferenceDirectionFactory(3, n_points=91),
-        mutation=PolynomialMutation(probability=1.0 / problem.number_of_variables, distribution_index=20),
-        crossover=SBXCrossover(probability=1.0, distribution_index=30),
-        termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations)
+        mutation=PolynomialMutation(1.0 / problem.number_of_variables, 20.0),
+        termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations),
     )
 
     algorithm.run()
-    front = algorithm.get_result()
+    result = algorithm.get_result()
 
     # Save results to file
-    print_function_values_to_file(front, 'FUN.' + algorithm.label)
-    print_variables_to_file(front, 'VAR.'+ algorithm.label)
+    print_function_values_to_file(result, "FUN." + algorithm.get_name() + "." + problem.get_name())
+    print_variables_to_file(result, "VAR." + algorithm.get_name() + "." + problem.get_name())
 
-    print(f'Algorithm: ${algorithm.get_name()}')
-    print(f'Problem: ${problem.get_name()}')
-    print(f'Computing time: ${algorithm.total_computing_time}')
+    print("Algorithm: " + algorithm.get_name())
+    print("Problem: " + problem.get_name())
+    print("Solution: " + str(result.variables))
+    print("Fitness:  " + str(result.objectives[0]))
+    print("Computing time: " + str(algorithm.total_computing_time))
```

### Comparing `jmetalpy-1.5.5/examples/multiobjective/omopso/omopso_spark_evaluator.py` & `jmetalpy-1.6.0/examples/multiobjective/omopso/omopso_spark_evaluator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,43 @@
 from jmetal.algorithm.multiobjective.omopso import OMOPSO
 from jmetal.operator import UniformMutation
 from jmetal.operator.mutation import NonUniformMutation
 from jmetal.problem.multiobjective.zdt import ZDT1Modified
 from jmetal.util.archive import CrowdingDistanceArchive
 from jmetal.util.evaluator import SparkEvaluator
-from jmetal.util.solution import print_function_values_to_file, print_variables_to_file, read_solutions
+from jmetal.util.solution import (
+    print_function_values_to_file,
+    print_variables_to_file,
+    read_solutions,
+)
 from jmetal.util.termination_criterion import StoppingByEvaluations
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     problem = ZDT1Modified()
-    problem.reference_front = read_solutions(filename='resources/reference_front/ZDT1.pf')
-    mutation_probability = 1.0 / problem.number_of_variables
+    problem.reference_front = read_solutions(filename="resources/reference_front/ZDT1.pf")
+    mutation_probability = 1.0 / problem.number_of_variables()
 
     max_evaluations = 100
     swarm_size = 10
     algorithm = OMOPSO(
         problem=problem,
         swarm_size=swarm_size,
         epsilon=0.0075,
         uniform_mutation=UniformMutation(probability=mutation_probability, perturbation=0.5),
-        non_uniform_mutation=NonUniformMutation(mutation_probability, perturbation=0.5,
-                                                max_iterations=max_evaluations / swarm_size),
+        non_uniform_mutation=NonUniformMutation(
+            mutation_probability, perturbation=0.5, max_iterations=max_evaluations / swarm_size
+        ),
         leaders=CrowdingDistanceArchive(10),
         termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations),
         swarm_evaluator=SparkEvaluator(),
     )
 
     algorithm.run()
     front = algorithm.get_result()
 
     # Save results to file
-    print_function_values_to_file(front, 'FUN.' + algorithm.get_name() + "." + problem.get_name())
-    print_variables_to_file(front, 'VAR.' + algorithm.get_name() + "." + problem.get_name())
+    print_function_values_to_file(front, "FUN." + algorithm.get_name() + "." + problem.name())
+    print_variables_to_file(front, "VAR." + algorithm.get_name() + "." + problem.name())
 
-    print('Algorithm (continuous problem): ' + algorithm.get_name())
-    print('Problem: ' + problem.get_name())
-    print('Computing time: ' + str(algorithm.total_computing_time))
+    print(f"Algorithm: {algorithm.get_name()}")
+    print(f"Problem: {problem.name()}")
+    print(f"Computing time: {algorithm.total_computing_time}")
```

### Comparing `jmetalpy-1.5.5/examples/multiobjective/omopso/omopso_zdt1.py` & `jmetalpy-1.6.0/examples/multiobjective/nsgaii/nsgaii_solving_3D_problem.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,36 @@
-from jmetal.algorithm.multiobjective.omopso import OMOPSO
-from jmetal.operator import UniformMutation
-from jmetal.operator.mutation import NonUniformMutation
-from jmetal.problem import ZDT1
-from jmetal.util.archive import CrowdingDistanceArchive
-from jmetal.util.solution import print_function_values_to_file, print_variables_to_file
-from jmetal.util.solution import read_solutions
+from jmetal.algorithm.multiobjective.nsgaii import NSGAII
+from jmetal.operator import PolynomialMutation, SBXCrossover
+from jmetal.problem import DTLZ2
+from jmetal.util.comparator import DominanceComparator
+from jmetal.util.solution import (
+    print_function_values_to_file,
+    print_variables_to_file,
+    read_solutions,
+)
 from jmetal.util.termination_criterion import StoppingByEvaluations
 
-if __name__ == '__main__':
-    problem = ZDT1()
-    problem.reference_front = read_solutions(filename='resources/reference_front/ZDT1.pf')
+if __name__ == "__main__":
+    problem = DTLZ2()
+    problem.reference_front = read_solutions(filename="resources/reference_front/DTLZ2.3D.pf")
 
-    mutation_probability = 1.0 / problem.number_of_variables
     max_evaluations = 25000
-    swarm_size = 100
-
-    algorithm = OMOPSO(
+    algorithm = NSGAII(
         problem=problem,
-        swarm_size=swarm_size,
-        epsilon=0.0075,
-        uniform_mutation=UniformMutation(probability=mutation_probability, perturbation=0.5),
-        non_uniform_mutation=NonUniformMutation(mutation_probability, perturbation=0.5,
-                                                max_iterations=int(max_evaluations / swarm_size)),
-        leaders=CrowdingDistanceArchive(100),
-        termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations)
+        population_size=100,
+        offspring_population_size=100,
+        mutation=PolynomialMutation(probability=1.0 / problem.number_of_variables(), distribution_index=20),
+        crossover=SBXCrossover(probability=1.0, distribution_index=20),
+        termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations),
+        dominance_comparator=DominanceComparator(),
     )
 
     algorithm.run()
     front = algorithm.get_result()
 
     # Save results to file
-    print_function_values_to_file(front, 'FUN.' + algorithm.label)
-    print_variables_to_file(front, 'VAR.'+ algorithm.label)
+    print_function_values_to_file(front, "FUN." + algorithm.label)
+    print_variables_to_file(front, "VAR." + algorithm.label)
 
-    print(f'Algorithm: ${algorithm.get_name()}')
-    print(f'Problem: ${problem.get_name()}')
-    print(f'Computing time: ${algorithm.total_computing_time}')
+    print(f"Algorithm: {algorithm.get_name()}")
+    print(f"Problem: {problem.name()}")
+    print(f"Computing time: {algorithm.total_computing_time}")
```

### Comparing `jmetalpy-1.5.5/examples/multiobjective/random_search/random_search_zdt1.py` & `jmetalpy-1.6.0/examples/multiobjective/random_search/random_search_zdt1.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from jmetal.algorithm.multiobjective.random_search import RandomSearch
 from jmetal.problem import ZDT1
-from jmetal.util.solution import read_solutions, print_function_values_to_file, print_variables_to_file
+from jmetal.util.solution import (
+    print_function_values_to_file,
+    print_variables_to_file,
+)
 from jmetal.util.termination_criterion import StoppingByEvaluations
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     problem = ZDT1()
-    problem.reference_front = read_solutions(filename='resources/reference_front/ZDT1.pf')
 
     max_evaluations = 1000
     algorithm = RandomSearch(
-        problem=problem,
-        termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations)
+        problem=problem, termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations)
     )
 
     algorithm.run()
     front = algorithm.get_result()
 
     # Save results to file
-    print_function_values_to_file(front, 'FUN.' + algorithm.label)
-    print_variables_to_file(front, 'VAR.'+ algorithm.label)
+    print_function_values_to_file(front, "FUN." + algorithm.label)
+    print_variables_to_file(front, "VAR." + algorithm.label)
 
-    print(f'Algorithm: ${algorithm.get_name()}')
-    print(f'Problem: ${problem.get_name()}')
-    print(f'Computing time: ${algorithm.total_computing_time}')
+    print(f"Algorithm: {algorithm.get_name()}")
+    print(f"Problem: {problem.name()}")
+    print(f"Computing time: {algorithm.total_computing_time}")
```

### Comparing `jmetalpy-1.5.5/examples/multiobjective/smpso/dynamic_smpso.py` & `jmetalpy-1.6.0/examples/multiobjective/smpso/dynamic_smpso.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 from jmetal.algorithm.multiobjective.smpso import DynamicSMPSO
 from jmetal.operator import PolynomialMutation
 from jmetal.problem.multiobjective.fda import FDA2
 from jmetal.util.archive import CrowdingDistanceArchive
 from jmetal.util.observable import TimeCounter
-<<<<<<< HEAD
 from jmetal.util.observer import PlotFrontToFileObserver, WriteFrontToFileObserver
-=======
-
->>>>>>> master
 from jmetal.util.termination_criterion import StoppingByEvaluations
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     problem = FDA2()
 
     time_counter = TimeCounter(delay=15)
     time_counter.observable.register(problem)
     time_counter.start()
 
     max_evaluations = 25000
     algorithm = DynamicSMPSO(
         problem=problem,
         swarm_size=100,
         mutation=PolynomialMutation(probability=1.0 / problem.number_of_variables, distribution_index=20),
         leaders=CrowdingDistanceArchive(100),
-        termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations)
+        termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations),
     )
 
-    algorithm.observable.register(observer=PlotFrontToFileObserver('dynamic_front_vis'))
-    algorithm.observable.register(observer=WriteFrontToFileObserver('dynamic_front'))
+    algorithm.observable.register(observer=PlotFrontToFileObserver("dynamic_front_vis"))
+    algorithm.observable.register(observer=WriteFrontToFileObserver("dynamic_front"))
 
     algorithm.run()
+
+    print(f"Algorithm: {algorithm.get_name()}")
+    print(f"Problem: {problem.get_name()}")
+    print(f"Computing time: {algorithm.total_computing_time}")
```

### Comparing `jmetalpy-1.5.5/examples/multiobjective/smpso/smpso_schaffer_on_the_fly.py` & `jmetalpy-1.6.0/examples/multiobjective/nsgaii/nsgaii_defining_schaffer_problem_on_the_fly.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,45 @@
-from jmetal.algorithm.multiobjective.smpso import SMPSO
+from jmetal.algorithm.multiobjective.nsgaii import NSGAII
 from jmetal.core.problem import OnTheFlyFloatProblem
-from jmetal.operator import PolynomialMutation
-from jmetal.util.archive import CrowdingDistanceArchive
-from jmetal.util.solution import print_function_values_to_file, print_variables_to_file
+from jmetal.operator import PolynomialMutation, SBXCrossover
+from jmetal.util.solution import (
+    get_non_dominated_solutions,
+    print_function_values_to_file,
+    print_variables_to_file,
+)
 from jmetal.util.termination_criterion import StoppingByEvaluations
 
-if __name__ == '__main__':
-    # Defining problem Schaffer on the fly
+"""  
+Program to  configure and run the NSGA-II algorithm configured with standard settings.
+"""
 
+if __name__ == "__main__":
+    # Defining problem Schaffer on the fly
     def f1(x: [float]):
         return x[0] * x[0]
 
     def f2(x: [float]):
         return (x[0] - 2) * (x[0] - 2)
 
     problem = OnTheFlyFloatProblem()
-    problem \
-        .set_name('Schaffer') \
-        .add_variable(-10000.0, 10000.0) \
-        .add_function(f1) \
-        .add_function(f2)
+    problem.set_name("Schaffer").add_variable(-1000.0, 1000.0).add_function(f1).add_function(f2)
 
     max_evaluations = 25000
-
-    algorithm = SMPSO(
+    algorithm = NSGAII(
         problem=problem,
-        swarm_size=100,
-        mutation=PolynomialMutation(probability=1.0 / problem.number_of_variables, distribution_index=20),
-        leaders=CrowdingDistanceArchive(100),
-        termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations)
+        population_size=100,
+        offspring_population_size=100,
+        mutation=PolynomialMutation(probability=1.0 / problem.number_of_variables(), distribution_index=20),
+        crossover=SBXCrossover(probability=1.0, distribution_index=20),
+        termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations),
     )
 
     algorithm.run()
-    front = algorithm.get_result()
+    front = get_non_dominated_solutions(algorithm.get_result())
 
     # Save results to file
-    print_function_values_to_file(front, 'FUN.' + algorithm.label)
-    print_variables_to_file(front, 'VAR.'+ algorithm.label)
+    print_function_values_to_file(front, "FUN." + algorithm.label)
+    print_variables_to_file(front, "VAR." + algorithm.label)
 
-    print(f'Algorithm: ${algorithm.get_name()}')
-    print(f'Problem: ${problem.get_name()}')
-    print(f'Computing time: ${algorithm.total_computing_time}')
+    print(f"Algorithm: {algorithm.get_name()}")
+    print(f"Problem: {problem.name()}")
+    print(f"Computing time: {algorithm.total_computing_time}")
```

### Comparing `jmetalpy-1.5.5/examples/multiobjective/smpso/smpso_spark_evaluator.py` & `jmetalpy-1.6.0/examples/multiobjective/mocell/mocell_zdt1.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,37 @@
-from examples.multiobjective.zdt1_modified import ZDT1Modified
-
-from jmetal.algorithm.multiobjective.smpso import SMPSO
-from jmetal.operator import PolynomialMutation
+from jmetal.algorithm.multiobjective.mocell import MOCell
+from jmetal.operator import PolynomialMutation, SBXCrossover
+from jmetal.problem import ZDT1
 from jmetal.util.archive import CrowdingDistanceArchive
-from jmetal.util.evaluator import SparkEvaluator
-from jmetal.util.solution import print_function_values_to_file, print_variables_to_file
-from jmetal.util.solution import read_solutions
+from jmetal.util.neighborhood import C9
+from jmetal.util.solution import (
+    print_function_values_to_file,
+    print_variables_to_file,
+    read_solutions,
+)
 from jmetal.util.termination_criterion import StoppingByEvaluations
 
-if __name__ == '__main__':
-    problem = ZDT1Modified()
-    problem.reference_front = read_solutions(filename='resources/reference_front/ZDT1.pf')
+if __name__ == "__main__":
+    problem = ZDT1()
+    problem.reference_front = read_solutions(filename="resources/reference_front/ZDT1.pf")
 
-    max_evaluations = 100
-    algorithm = SMPSO(
+    max_evaluations = 25000
+    algorithm = MOCell(
         problem=problem,
-        swarm_size=10,
-        mutation=PolynomialMutation(probability=1.0 / problem.number_of_variables, distribution_index=20),
-        leaders=CrowdingDistanceArchive(10),
+        population_size=100,
+        neighborhood=C9(10, 10),
+        archive=CrowdingDistanceArchive(100),
+        mutation=PolynomialMutation(probability=1.0 / problem.number_of_variables(), distribution_index=20),
+        crossover=SBXCrossover(probability=1.0, distribution_index=20),
         termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations),
-        swarm_evaluator=SparkEvaluator(),
     )
 
     algorithm.run()
     front = algorithm.get_result()
 
     # Save results to file
-    print_function_values_to_file(front, 'FUN.' + algorithm.get_name() + "." + problem.get_name())
-    print_variables_to_file(front, 'VAR.'+ algorithm.get_name() + "." + problem.get_name())
+    print_function_values_to_file(front, "FUN." + algorithm.label)
+    print_variables_to_file(front, "VAR." + algorithm.label)
 
-    print('Algorithm (continuous problem): ' + algorithm.get_name())
-    print('Problem: ' + problem.get_name())
-    print('Computing time: ' + str(algorithm.total_computing_time))
+    print(f"Algorithm: {algorithm.get_name()}")
+    print(f"Problem: {problem.name()}")
+    print(f"Computing time: {algorithm.total_computing_time}")
```

### Comparing `jmetalpy-1.5.5/examples/multiobjective/smpso/smpso_srinivas.py` & `jmetalpy-1.6.0/examples/multiobjective/smpso/smpso_schaffer_on_the_fly.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,39 @@
 from jmetal.algorithm.multiobjective.smpso import SMPSO
+from jmetal.core.problem import OnTheFlyFloatProblem
 from jmetal.operator import PolynomialMutation
-from jmetal.problem import Srinivas
 from jmetal.util.archive import CrowdingDistanceArchive
 from jmetal.util.solution import print_function_values_to_file, print_variables_to_file
-from jmetal.util.solution import read_solutions
 from jmetal.util.termination_criterion import StoppingByEvaluations
 
-if __name__ == '__main__':
-    problem = Srinivas()
-    problem.reference_front = read_solutions(filename='resources/reference_front/Srinivas.pf')
+if __name__ == "__main__":
+    # Defining problem Schaffer on the fly
+
+    def f1(x: [float]):
+        return x[0] * x[0]
+
+    def f2(x: [float]):
+        return (x[0] - 2) * (x[0] - 2)
+
+    problem = OnTheFlyFloatProblem()
+    problem.set_name("Schaffer").add_variable(-10000.0, 10000.0).add_function(f1).add_function(f2)
 
     max_evaluations = 25000
+
     algorithm = SMPSO(
         problem=problem,
         swarm_size=100,
-        mutation=PolynomialMutation(probability=1.0 / problem.number_of_variables, distribution_index=20),
+        mutation=PolynomialMutation(probability=1.0 / problem.number_of_variables(), distribution_index=20),
         leaders=CrowdingDistanceArchive(100),
-        termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations)
+        termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations),
     )
 
     algorithm.run()
     front = algorithm.get_result()
 
     # Save results to file
-    print_function_values_to_file(front, 'FUN.' + algorithm.label)
-    print_variables_to_file(front, 'VAR.'+ algorithm.label)
+    print_function_values_to_file(front, "FUN." + algorithm.label)
+    print_variables_to_file(front, "VAR." + algorithm.label)
 
-    print(f'Algorithm: ${algorithm.get_name()}')
-    print(f'Problem: ${problem.get_name()}')
-    print(f'Computing time: ${algorithm.total_computing_time}')
+    print(f"Algorithm: {algorithm.get_name()}")
+    print(f"Problem: {problem.name()}")
+    print(f"Computing time: {algorithm.total_computing_time}")
```

### Comparing `jmetalpy-1.5.5/examples/multiobjective/smpso/smpso_zdt4.py` & `jmetalpy-1.6.0/examples/multiobjective/smpso/smpso_tanaka.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 from jmetal.algorithm.multiobjective.smpso import SMPSO
 from jmetal.operator import PolynomialMutation
-from jmetal.problem import ZDT4
+from jmetal.problem import Tanaka
 from jmetal.util.archive import CrowdingDistanceArchive
-from jmetal.util.solution import print_function_values_to_file, print_variables_to_file
-from jmetal.util.solution import read_solutions
+from jmetal.util.comparator import DominanceWithConstraintsComparator
+from jmetal.util.solution import (
+    print_function_values_to_file,
+    print_variables_to_file,
+    read_solutions,
+)
 from jmetal.util.termination_criterion import StoppingByEvaluations
 
-if __name__ == '__main__':
-    problem = ZDT4()
-    problem.reference_front = read_solutions(filename='resources/reference_front/ZDT4.pf')
+if __name__ == "__main__":
+    problem = Tanaka()
+    reference_front = read_solutions(filename="resources/reference_front/Tanaka.pf")
 
     max_evaluations = 25000
     algorithm = SMPSO(
         problem=problem,
         swarm_size=100,
-        mutation=PolynomialMutation(probability=1.0 / problem.number_of_variables, distribution_index=20),
-        leaders=CrowdingDistanceArchive(100),
-        termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations)
+        mutation=PolynomialMutation(probability=1.0 / problem.number_of_variables(), distribution_index=20),
+        leaders=CrowdingDistanceArchive(100, dominance_comparator = DominanceWithConstraintsComparator()),
+        dominance_comparator=DominanceWithConstraintsComparator(),
+        termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations),
     )
 
     algorithm.run()
     front = algorithm.get_result()
 
     # Save results to file
-    print_function_values_to_file(front, 'FUN.' + algorithm.label)
-    print_variables_to_file(front, 'VAR.'+ algorithm.label)
+    print_function_values_to_file(front, "FUN." + algorithm.label)
+    print_variables_to_file(front, "VAR." + algorithm.label)
 
-    print(f'Algorithm: ${algorithm.get_name()}')
-    print(f'Problem: ${problem.get_name()}')
-    print(f'Computing time: ${algorithm.total_computing_time}')
+    print(f"Algorithm: {algorithm.get_name()}")
+    print(f"Problem: {problem.name()}")
+    print(f"Computing time: {algorithm.total_computing_time}")
```

### Comparing `jmetalpy-1.5.5/examples/multiobjective/smpso/smpsorp_zdt4.py` & `jmetalpy-1.6.0/examples/multiobjective/smpso/smpsorp_zdt4.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,59 +1,67 @@
-from jmetal.lab.visualization import Plot, InteractivePlot
-from jmetal.util.observer import ProgressBarObserver, VisualizerObserver
-from jmetal.util.solution import print_function_values_to_file, print_variables_to_file, read_solutions
-
-from jmetal.util.termination_criterion import StoppingByEvaluations
-
 from jmetal.algorithm.multiobjective.smpso import SMPSORP
+from jmetal.lab.visualization import InteractivePlot, Plot
 from jmetal.operator import PolynomialMutation
-from jmetal.problem import ZDT4, ZDT1
+from jmetal.problem import ZDT1
 from jmetal.util.archive import CrowdingDistanceArchiveWithReferencePoint
+from jmetal.util.observer import VisualizerObserver
+from jmetal.util.solution import (
+    print_function_values_to_file,
+    print_variables_to_file,
+    read_solutions,
+)
+from jmetal.util.termination_criterion import StoppingByEvaluations
 
-
-if __name__ == '__main__':
+if __name__ == "__main__":
     problem = ZDT1()
-    problem.reference_front = read_solutions(filename='resources/reference_front/ZDT1.pf')
+    reference_front = read_solutions(filename="resources/reference_front/ZDT1.pf")
 
     swarm_size = 100
 
-    reference_point = [[0.1, 0.8],[0.6, 0.1]]
+    reference_point = [[0.1, 0.8], [0.6, 0.1]]
     archives_with_reference_points = []
 
     for point in reference_point:
         archives_with_reference_points.append(
             CrowdingDistanceArchiveWithReferencePoint(int(swarm_size / len(reference_point)), point)
         )
 
     max_evaluations = 50000
     algorithm = SMPSORP(
         problem=problem,
         swarm_size=swarm_size,
-        mutation=PolynomialMutation(probability=1.0 / problem.number_of_variables, distribution_index=20),
+        mutation=PolynomialMutation(probability=1.0 / problem.number_of_variables(), distribution_index=20),
         reference_points=reference_point,
         leaders=archives_with_reference_points,
-        termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations)
+        termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations),
     )
 
     algorithm.observable.register(
-        observer=VisualizerObserver(reference_front=problem.reference_front, reference_point=reference_point))
+        observer=VisualizerObserver(reference_front=reference_front, reference_point=reference_point)
+    )
 
     algorithm.run()
     front = algorithm.get_result()
 
     # Plot front
-    plot_front = Plot(title='Pareto front approximation. Problem: ' + problem.get_name(),
-                      reference_front=problem.reference_front, axis_labels=problem.obj_labels)
+    plot_front = Plot(
+        title="Pareto front approximation. Problem: " + problem.name(),
+        reference_front=reference_front,
+        axis_labels=problem.obj_labels,
+    )
     plot_front.plot(front, label=algorithm.label, filename=algorithm.get_name())
 
     # Plot interactive front
-    plot_front = InteractivePlot(title='Pareto front approximation. Problem: ' + problem.get_name(),
-                                 reference_front=problem.reference_front, axis_labels=problem.obj_labels)
+    plot_front = InteractivePlot(
+        title="Pareto front approximation. Problem: " + problem.name(),
+        reference_front=reference_front,
+        axis_labels=problem.obj_labels,
+    )
     plot_front.plot(front, label=algorithm.label, filename=algorithm.get_name())
 
     # Save results to file
-    print_function_values_to_file(front, 'FUN.' + algorithm.label)
-    print_variables_to_file(front, 'VAR.' + algorithm.label)
+    print_function_values_to_file(front, "FUN." + algorithm.label)
+    print_variables_to_file(front, "VAR." + algorithm.label)
 
-    print('Algorithm (continuous problem): ' + algorithm.get_name())
-    print('Problem: ' + problem.get_name())
-    print('Computing time: ' + str(algorithm.total_computing_time))
+    print(f"Algorithm: {algorithm.get_name()}")
+    print(f"Problem: {problem.name()}")
+    print(f"Computing time: {algorithm.total_computing_time}")
```

### Comparing `jmetalpy-1.5.5/examples/multiobjective/spea2/gspea2_zdt1.py` & `jmetalpy-1.6.0/examples/singleobjective/nsgaii/nsgaii_single_objective_float.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,31 @@
-from jmetal.algorithm.multiobjective.spea2 import SPEA2
-from jmetal.operator import SBXCrossover, PolynomialMutation
-from jmetal.problem import ZDT1
-from jmetal.util.comparator import GDominanceComparator
-from jmetal.util.solution import print_function_values_to_file, print_variables_to_file, read_solutions
+from jmetal.algorithm.multiobjective.nsgaii import NSGAII
+from jmetal.operator import PolynomialMutation, SBXCrossover
+from jmetal.problem.singleobjective.unconstrained import Rastrigin
+from jmetal.util.comparator import DominanceComparator
+from jmetal.util.solution import print_function_values_to_file, print_variables_to_file
 from jmetal.util.termination_criterion import StoppingByEvaluations
 
-if __name__ == '__main__':
-    problem = ZDT1()
-    problem.reference_front = read_solutions(filename='resources/reference_front/ZDT1.pf')
+if __name__ == "__main__":
+    problem = Rastrigin(10)
 
-    reference_point = [0.4, 0.6]
-
-    max_evaluations = 25000
-    algorithm = SPEA2(
+    max_evaluations = 50000
+    algorithm = NSGAII(
         problem=problem,
-        population_size=40,
-        offspring_population_size=40,
-        mutation=PolynomialMutation(probability=1.0 / problem.number_of_variables, distribution_index=20),
-        crossover=SBXCrossover(probability=1.0, distribution_index=20),
+        population_size=100,
+        offspring_population_size=100,
+        mutation=PolynomialMutation(probability=1.0 / problem.number_of_variables, distribution_index=20.0),
+        crossover=SBXCrossover(probability=0.9, distribution_index=20.0),
         termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations),
-        dominance_comparator=GDominanceComparator(reference_point)
+        dominance_comparator=DominanceComparator(),
     )
 
     algorithm.run()
     front = algorithm.get_result()
 
     # Save results to file
-    print_function_values_to_file(front, 'FUN.' + algorithm.label)
-    print_variables_to_file(front, 'VAR.'+ algorithm.label)
+    print_function_values_to_file(front, "FUN." + algorithm.get_name() + "-" + problem.get_name())
+    print_variables_to_file(front, "VAR." + algorithm.get_name() + "-" + problem.get_name())
 
-    print(f'Algorithm: ${algorithm.get_name()}')
-    print(f'Problem: ${problem.get_name()}')
-    print(f'Computing time: ${algorithm.total_computing_time}')
+    print("Algorithm (continuous problem): " + algorithm.get_name())
+    print("Problem: " + problem.get_name())
+    print("Computing time: " + str(algorithm.total_computing_time))
```

### Comparing `jmetalpy-1.5.5/examples/multiobjective/spea2/spea2_dtlz1.py` & `jmetalpy-1.6.0/examples/singleobjective/local_search/local_search_binary.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,31 @@
-from jmetal.algorithm.multiobjective.spea2 import SPEA2
-from jmetal.operator import SBXCrossover, PolynomialMutation
-from jmetal.problem import DTLZ2
-from jmetal.util.solution import read_solutions, print_function_values_to_file, print_variables_to_file
+from jmetal.algorithm.singleobjective.local_search import LocalSearch
+from jmetal.operator import BitFlipMutation
+from jmetal.problem import OneMax
+from jmetal.util.observer import PrintObjectivesObserver
+from jmetal.util.solution import print_function_values_to_file, print_variables_to_file
 from jmetal.util.termination_criterion import StoppingByEvaluations
 
-if __name__ == '__main__':
-    problem = DTLZ2()
-    problem.reference_front = read_solutions(filename='resources/reference_front/DTLZ2.3D.pf')
+if __name__ == "__main__":
+    problem = OneMax(number_of_bits=512)
 
-    max_evaluations = 20000
-    algorithm = SPEA2(
+    max_evaluations = 10000
+    algorithm = LocalSearch(
         problem=problem,
-        population_size=20,
-        offspring_population_size=20,
-        mutation=PolynomialMutation(probability=1.0 / problem.number_of_variables, distribution_index=20),
-        crossover=SBXCrossover(probability=1.0, distribution_index=20),
-        termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations)
+        mutation=BitFlipMutation(probability=1.0 / problem.number_of_bits),
+        termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations),
     )
 
+    algorithm.observable.register(observer=PrintObjectivesObserver(100))
+
     algorithm.run()
-    front = algorithm.get_result()
+    result = algorithm.get_result()
 
     # Save results to file
-    print_function_values_to_file(front, 'FUN.' + algorithm.label)
-    print_variables_to_file(front, 'VAR.'+ algorithm.label)
+    print_function_values_to_file(result, "FUN." + algorithm.get_name() + "." + problem.get_name())
+    print_variables_to_file(result, "VAR." + algorithm.get_name() + "." + problem.get_name())
 
-    print(f'Algorithm: ${algorithm.get_name()}')
-    print(f'Problem: ${problem.get_name()}')
-    print(f'Computing time: ${algorithm.total_computing_time}')
+    print("Algorithm: " + algorithm.get_name())
+    print("Problem: " + problem.get_name())
+    print("Solution: " + result.get_binary_string())
+    print("Fitness:  " + str(result.objectives[0]))
+    print("Computing time: " + str(algorithm.total_computing_time))
```

### Comparing `jmetalpy-1.5.5/examples/multiobjective/spea2/spea2_zdt1.py` & `jmetalpy-1.6.0/examples/multiobjective/nsgaii/nsgaii_solving_constrained_srinivas_problem.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,35 @@
-from jmetal.algorithm.multiobjective.spea2 import SPEA2
-from jmetal.operator import SBXCrossover, PolynomialMutation
-from jmetal.problem import ZDT1
-from jmetal.util.solution import read_solutions, print_function_values_to_file, print_variables_to_file
+from jmetal.algorithm.multiobjective import NSGAII
+from jmetal.operator import PolynomialMutation, SBXCrossover
+from jmetal.problem import Srinivas
+from jmetal.util.comparator import DominanceWithConstraintsComparator
+from jmetal.util.solution import (
+    print_function_values_to_file,
+    print_variables_to_file,
+)
 from jmetal.util.termination_criterion import StoppingByEvaluations
 
-if __name__ == '__main__':
-    problem = ZDT1()
-    problem.reference_front = read_solutions(filename='resources/reference_front/ZDT1.pf')
+if __name__ == "__main__":
+    problem = Srinivas()
+    #problem.reference_front = read_solutions(filename="resources/reference_front/Srinivas.pf")
 
-    max_evaluations = 20000
-    algorithm = SPEA2(
+    max_evaluations = 25000
+    algorithm = NSGAII(
         problem=problem,
-        population_size=40,
-        offspring_population_size=40,
-        mutation=PolynomialMutation(probability=1.0 / problem.number_of_variables, distribution_index=20),
+        population_size=100,
+        offspring_population_size=100,
+        mutation=PolynomialMutation(probability=1.0 / problem.number_of_variables(), distribution_index=20),
         crossover=SBXCrossover(probability=1.0, distribution_index=20),
-        termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations)
+        termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations),
+        dominance_comparator=DominanceWithConstraintsComparator(),
     )
 
     algorithm.run()
     front = algorithm.get_result()
 
     # Save results to file
-    print_function_values_to_file(front, 'FUN.' + algorithm.label)
-    print_variables_to_file(front, 'VAR.' + algorithm.label)
+    print_function_values_to_file(front, "FUN." + algorithm.label)
+    print_variables_to_file(front, "VAR." + algorithm.label)
 
-    print(f'Algorithm: ${algorithm.get_name()}')
-    print(f'Problem: ${problem.get_name()}')
-    print(f'Computing time: ${algorithm.total_computing_time}')
+    print(f"Algorithm: {algorithm.get_name()}")
+    print(f"Problem: {problem.name()}")
+    print(f"Computing time: {algorithm.total_computing_time}")
```

### Comparing `jmetalpy-1.5.5/examples/singleobjective/evolution_strategy/evolution_strategy_binary.py` & `jmetalpy-1.6.0/examples/singleobjective/evolution_strategy/evolution_strategy_binary.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from jmetal.algorithm.singleobjective.evolution_strategy import EvolutionStrategy
 from jmetal.operator import BitFlipMutation
 from jmetal.problem import OneMax
 from jmetal.util.termination_criterion import StoppingByEvaluations
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     problem = OneMax(number_of_bits=512)
 
     algorithm = EvolutionStrategy(
         problem=problem,
         mu=1,
         lambda_=10,
         mutation=BitFlipMutation(probability=1.0 / problem.number_of_bits),
         elitist=True,
-        termination_criterion=StoppingByEvaluations(max_evaluations=25000)
+        termination_criterion=StoppingByEvaluations(max_evaluations=25000),
     )
 
     algorithm.run()
     result = algorithm.get_result()
 
-    print('Algorithm: ' + algorithm.get_name())
-    print('Problem: ' + problem.get_name())
-    print('Solution: ' + str(result.variables[0]))
-    print('Fitness:  ' + str(result.objectives[0]))
-    print('Computing time: ' + str(algorithm.total_computing_time))
+    print("Algorithm: " + algorithm.get_name())
+    print("Problem: " + problem.get_name())
+    print("Solution: " + str(result.variables[0]))
+    print("Fitness:  " + str(result.objectives[0]))
+    print("Computing time: " + str(algorithm.total_computing_time))
```

### Comparing `jmetalpy-1.5.5/examples/singleobjective/evolution_strategy/evolution_strategy_float.py` & `jmetalpy-1.6.0/examples/singleobjective/evolution_strategy/evolution_strategy_float.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from jmetal.algorithm.singleobjective.evolution_strategy import EvolutionStrategy
 from jmetal.operator import PolynomialMutation
 from jmetal.problem import Sphere
 from jmetal.util.termination_criterion import StoppingByEvaluations
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     problem = Sphere(number_of_variables=10)
 
     algorithm = EvolutionStrategy(
         problem=problem,
         mu=10,
         lambda_=10,
         elitist=True,
         mutation=PolynomialMutation(probability=1.0 / problem.number_of_variables),
-        termination_criterion=StoppingByEvaluations(max_evaluations=25000)
+        termination_criterion=StoppingByEvaluations(max_evaluations=25000),
     )
 
     algorithm.run()
     result = algorithm.get_result()
 
-    print('Algorithm: ' + algorithm.get_name())
-    print('Problem: ' + problem.get_name())
-    print('Solution: ' + str(result.variables[0]))
-    print('Fitness:  ' + str(result.objectives[0]))
-    print('Computing time: ' + str(algorithm.total_computing_time))
+    print("Algorithm: " + algorithm.get_name())
+    print("Problem: " + problem.get_name())
+    print("Solution: " + str(result.variables[0]))
+    print("Fitness:  " + str(result.objectives[0]))
+    print("Computing time: " + str(algorithm.total_computing_time))
```

### Comparing `jmetalpy-1.5.5/examples/singleobjective/gde3/gde3_single_objective.py` & `jmetalpy-1.6.0/examples/singleobjective/gde3/gde3_single_objective.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 from jmetal.algorithm.multiobjective.gde3 import GDE3
 from jmetal.problem.singleobjective.unconstrained import Rastrigin
 from jmetal.util.solution import print_function_values_to_file, print_variables_to_file
 from jmetal.util.termination_criterion import StoppingByEvaluations
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     problem = Rastrigin(10)
 
     algorithm = GDE3(
-        problem=problem,
-        population_size=100,
-        cr=0.5,
-        f=0.5,
-        termination_criterion=StoppingByEvaluations(50000)
+        problem=problem, population_size=100, cr=0.5, f=0.5, termination_criterion=StoppingByEvaluations(100000)
     )
 
     algorithm.run()
     front = algorithm.get_result()
 
     # Save results to file
-    print_function_values_to_file(front, 'FUN.' + algorithm.get_name() + "." + problem.get_name())
-    print_variables_to_file(front, 'VAR.' + algorithm.get_name() + "." + problem.get_name())
+    print_function_values_to_file(front, "FUN." + algorithm.get_name() + "." + problem.get_name())
+    print_variables_to_file(front, "VAR." + algorithm.get_name() + "." + problem.get_name())
 
-    print('Algorithm (continuous problem): ' + algorithm.get_name())
-    print('Problem: ' + problem.get_name())
-    print('Computing time: ' + str(algorithm.total_computing_time))
+    print("Algorithm (continuous problem): " + algorithm.get_name())
+    print("Problem: " + problem.get_name())
+    print("Computing time: " + str(algorithm.total_computing_time))
```

### Comparing `jmetalpy-1.5.5/examples/singleobjective/genetic_algorithm/generational_genetic_algorithm_binary.py` & `jmetalpy-1.6.0/examples/singleobjective/genetic_algorithm/generational_genetic_algorithm_binary.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from jmetal.algorithm.singleobjective.genetic_algorithm import GeneticAlgorithm
-from jmetal.operator import BitFlipMutation, SPXCrossover, BinaryTournamentSelection
+from jmetal.operator import BitFlipMutation, SPXCrossover
 from jmetal.problem import OneMax
+from jmetal.util.observer import PrintObjectivesObserver
 from jmetal.util.termination_criterion import StoppingByEvaluations
 
-if __name__ == '__main__':
-    problem = OneMax(number_of_bits=1024)
+if __name__ == "__main__":
+    problem = OneMax(number_of_bits=512)
 
     algorithm = GeneticAlgorithm(
         problem=problem,
-        population_size=100,
-        offspring_population_size=100,
+        population_size=40,
+        offspring_population_size=40,
         mutation=BitFlipMutation(1.0 / problem.number_of_bits),
         crossover=SPXCrossover(1.0),
-        selection=BinaryTournamentSelection(),
-        termination_criterion=StoppingByEvaluations(max_evaluations=20000)
+        termination_criterion=StoppingByEvaluations(max_evaluations=20000),
     )
 
+    algorithm.observable.register(observer=PrintObjectivesObserver(100))
+
     algorithm.run()
     result = algorithm.get_result()
 
-    print('Algorithm: {}'.format(algorithm.get_name()))
-    print('Problem: {}'.format(problem.get_name()))
-    print('Solution: ' + result.get_binary_string())
-    print('Fitness:  ' + str(result.objectives[0]))
-    print('Computing time: {}'.format(algorithm.total_computing_time))
+    print("Algorithm: {}".format(algorithm.get_name()))
+    print("Problem: {}".format(problem.name()))
+    print("Solution: " + result.get_binary_string())
+    print("Fitness:  " + str(result.objectives[0]))
+    print("Computing time: {}".format(algorithm.total_computing_time))
```

### Comparing `jmetalpy-1.5.5/examples/singleobjective/genetic_algorithm/generational_genetic_algorithm_float.py` & `jmetalpy-1.6.0/examples/singleobjective/genetic_algorithm/steady_state_genetic_algorithm_with_knapsack_problem.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from jmetal.algorithm.singleobjective.genetic_algorithm import GeneticAlgorithm
-from jmetal.operator import BinaryTournamentSelection, PolynomialMutation, SBXCrossover
-from jmetal.problem.singleobjective.unconstrained import Rastrigin
+from jmetal.operator import BinaryTournamentSelection, BitFlipMutation, SPXCrossover
+from jmetal.problem.singleobjective.knapsack import Knapsack
 from jmetal.util.termination_criterion import StoppingByEvaluations
 
-if __name__ == '__main__':
-    problem = Rastrigin(10)
+if __name__ == "__main__":
+    problem = Knapsack(from_file=True, filename="resources/Knapsack_instances/KnapsackInstance_50_0_0.kp")
 
     algorithm = GeneticAlgorithm(
         problem=problem,
         population_size=100,
-        offspring_population_size=100,
-        mutation=PolynomialMutation(1.0 / problem.number_of_variables, 20.0),
-        crossover=SBXCrossover(0.9, 20.0),
+        offspring_population_size=1,
+        mutation=BitFlipMutation(probability=0.1),
+        crossover=SPXCrossover(probability=0.8),
         selection=BinaryTournamentSelection(),
-        termination_criterion=StoppingByEvaluations(max_evaluations=500000)
+        termination_criterion=StoppingByEvaluations(max_evaluations=25000),
     )
 
     algorithm.run()
-    result = algorithm.get_result()
+    subset = algorithm.get_result()
 
-    print('Algorithm: {}'.format(algorithm.get_name()))
-    print('Problem: {}'.format(problem.get_name()))
-    print('Solution: {}'.format(result.variables))
-    print('Fitness: {}'.format(result.objectives[0]))
-    print('Computing time: {}'.format(algorithm.total_computing_time))
+    print("Algorithm: {}".format(algorithm.get_name()))
+    print("Problem: {}".format(problem.name()))
+    print("Solution: {}".format(subset.variables))
+    print("Fitness: {}".format(-subset.objectives[0]))
+    print("Computing time: {}".format(algorithm.total_computing_time))
+    print(f"Problem Maximum Capacity: {problem.capacity}")
```

### Comparing `jmetalpy-1.5.5/examples/singleobjective/genetic_algorithm/generational_genetic_algorithm_tsp.py` & `jmetalpy-1.6.0/examples/multiobjective/spea2/spea2_zdt1.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,32 @@
-from jmetal.algorithm.singleobjective.genetic_algorithm import GeneticAlgorithm
-from jmetal.operator import BinaryTournamentSelection
-from jmetal.operator.crossover import PMXCrossover
-from jmetal.operator.mutation import PermutationSwapMutation
-from jmetal.problem.singleobjective.tsp import TSP
-from jmetal.util.comparator import MultiComparator
-from jmetal.util.density_estimator import CrowdingDistance
-from jmetal.util.ranking import FastNonDominatedRanking
+from jmetal.algorithm.multiobjective.spea2 import SPEA2
+from jmetal.operator import PolynomialMutation, SBXCrossover
+from jmetal.problem import ZDT1
+from jmetal.util.solution import (
+    print_function_values_to_file,
+    print_variables_to_file,
+)
 from jmetal.util.termination_criterion import StoppingByEvaluations
 
-if __name__ == '__main__':
-    problem = TSP(instance='resources/TSP_instances/kroA100.tsp')
+if __name__ == "__main__":
+    problem = ZDT1()
 
-    print('Cities: ', problem.number_of_variables)
-
-    algorithm = GeneticAlgorithm(
+    max_evaluations = 20000
+    algorithm = SPEA2(
         problem=problem,
-        population_size=100,
-        offspring_population_size=100,
-        mutation=PermutationSwapMutation(1.0 / problem.number_of_variables),
-        crossover=PMXCrossover(0.8),
-        selection=BinaryTournamentSelection(
-            MultiComparator([FastNonDominatedRanking.get_comparator(),
-                             CrowdingDistance.get_comparator()])),
-        termination_criterion=StoppingByEvaluations(max_evaluations=2500000)
+        population_size=40,
+        offspring_population_size=40,
+        mutation=PolynomialMutation(probability=1.0 / problem.number_of_variables(), distribution_index=20),
+        crossover=SBXCrossover(probability=1.0, distribution_index=20),
+        termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations),
     )
 
     algorithm.run()
-    result = algorithm.get_result()
+    front = algorithm.get_result()
+
+    # Save results to file
+    print_function_values_to_file(front, "FUN." + algorithm.label)
+    print_variables_to_file(front, "VAR." + algorithm.label)
 
-    print('Algorithm: {}'.format(algorithm.get_name()))
-    print('Problem: {}'.format(problem.get_name()))
-    print('Solution: {}'.format(result.variables))
-    print('Fitness: {}'.format(result.objectives[0]))
-    print('Computing time: {}'.format(algorithm.total_computing_time))
+    print(f"Algorithm: {algorithm.get_name()}")
+    print(f"Problem: {problem.name()}")
+    print(f"Computing time: {algorithm.total_computing_time}")
```

### Comparing `jmetalpy-1.5.5/examples/singleobjective/local_search/local_search_float.py` & `jmetalpy-1.6.0/examples/singleobjective/simulated_annealing/simulated_annealing_float.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-from jmetal.algorithm.singleobjective.local_search import LocalSearch
+from jmetal.algorithm.singleobjective.simulated_annealing import SimulatedAnnealing
 from jmetal.operator import PolynomialMutation
-from jmetal.problem.singleobjective.unconstrained import Sphere
+from jmetal.problem.singleobjective.unconstrained import Rastrigin
 from jmetal.util.solution import print_function_values_to_file, print_variables_to_file
 from jmetal.util.termination_criterion import StoppingByEvaluations
 
-if __name__ == '__main__':
-    problem = Sphere(10)
+if __name__ == "__main__":
+    problem = Rastrigin(10)
 
-    max_evaluations = 1000000
+    max_evaluations = 100000
 
-    algorithm = LocalSearch(
+    algorithm = SimulatedAnnealing(
         problem=problem,
-        mutation=PolynomialMutation(1.0 / problem.number_of_variables, 20.0),
-        termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations)
+        mutation=PolynomialMutation(probability=1.0 / problem.number_of_variables, distribution_index=20.0),
+        termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations),
     )
 
     algorithm.run()
     result = algorithm.get_result()
 
     # Save results to file
-    print_function_values_to_file(result, 'FUN.'+ algorithm.get_name() + "." + problem.get_name())
-    print_variables_to_file(result, 'VAR.' + algorithm.get_name() + "." + problem.get_name())
+    print_function_values_to_file(result, "FUN." + algorithm.get_name() + "." + problem.get_name())
+    print_variables_to_file(result, "VAR." + algorithm.get_name() + "." + problem.get_name())
 
-    print('Algorithm: ' + algorithm.get_name())
-    print('Problem: ' + problem.get_name())
-    print('Solution: ' + str(result.variables))
-    print('Fitness:  ' + str(result.objectives[0]))
-    print('Computing time: ' + str(algorithm.total_computing_time))
+    print("Algorithm: " + algorithm.get_name())
+    print("Problem: " + problem.get_name())
+    print("Solution: " + str(result.variables[0]))
+    print("Fitness:  " + str(result.objectives[0]))
+    print("Computing time: " + str(algorithm.total_computing_time))
```

### Comparing `jmetalpy-1.5.5/examples/singleobjective/nsgaii/nsgaii_single_objective_binary.py` & `jmetalpy-1.6.0/examples/singleobjective/simulated_annealing/simulated_annealing_binary.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,29 @@
-from jmetal.algorithm.multiobjective.nsgaii import NSGAII
-from jmetal.operator import BitFlipMutation, SPXCrossover
+from jmetal.algorithm.singleobjective.simulated_annealing import SimulatedAnnealing
+from jmetal.operator import BitFlipMutation
 from jmetal.problem import OneMax
-from jmetal.util.comparator import DominanceComparator
 from jmetal.util.solution import print_function_values_to_file, print_variables_to_file
 from jmetal.util.termination_criterion import StoppingByEvaluations
 
-if __name__ == '__main__':
-    binary_string_length = 512
-    problem = OneMax(binary_string_length)
+if __name__ == "__main__":
+    problem = OneMax(number_of_bits=512)
 
-    max_evaluations = 20000
+    max_evaluations = 10000
 
-    algorithm = NSGAII(
+    algorithm = SimulatedAnnealing(
         problem=problem,
-        population_size=100,
-        offspring_population_size=1,
-        mutation=BitFlipMutation(probability=1.0 / binary_string_length),
-        crossover=SPXCrossover(probability=1.0),
+        mutation=BitFlipMutation(probability=1.0 / problem.number_of_bits),
         termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations),
-        dominance_comparator=DominanceComparator()
     )
 
     algorithm.run()
-    front = algorithm.get_result()
+    result = algorithm.get_result()
 
     # Save results to file
-    print_function_values_to_file(front, 'FUN.'+ algorithm.get_name()+"-"+problem.get_name())
-    print_variables_to_file(front, 'VAR.' + algorithm.get_name()+"-"+problem.get_name())
+    print_function_values_to_file(result, "FUN." + algorithm.get_name() + "." + problem.get_name())
+    print_variables_to_file(result, "VAR." + algorithm.get_name() + "." + problem.get_name())
 
-    print('Algorithm (continuous problem): ' + algorithm.get_name())
-    print('Problem: ' + problem.get_name())
-    print('Computing time: ' + str(algorithm.total_computing_time))
+    print("Algorithm: " + algorithm.get_name())
+    print("Problem: " + problem.get_name())
+    print("Solution: " + result.get_binary_string())
+    print("Fitness:  " + str(result.objectives[0]))
+    print("Computing time: " + str(algorithm.total_computing_time))
```

### Comparing `jmetalpy-1.5.5/examples/singleobjective/simulated_annealing/simulated_annealing_binary.py` & `jmetalpy-1.6.0/examples/singleobjective/simulated_annealing/simulated_annealing_permutation.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,24 @@
 from jmetal.algorithm.singleobjective.simulated_annealing import SimulatedAnnealing
-from jmetal.operator import BitFlipMutation
-from jmetal.problem import OneMax
-from jmetal.util.solution import print_function_values_to_file, print_variables_to_file
-from jmetal.util.termination_criterion import StoppingByEvaluations
+from jmetal.operator import ScrambleMutation
+from jmetal.problem import TSP
+from jmetal.util.termination_criterion import StoppingByTime
 
-if __name__ == '__main__':
-    problem = OneMax(number_of_bits=1024)
+if __name__ == "__main__":
+    problem = TSP(instance="resources/TSP_instances/kroA100.tsp")
 
-    max_evaluations = 20000
+    print(f"Solving TSP problem with {problem.number_of_cities} cities.")
 
     algorithm = SimulatedAnnealing(
         problem=problem,
-        mutation=BitFlipMutation(probability=1.0 / problem.number_of_bits),
-        termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations)
+        mutation=ScrambleMutation(probability=1.0 / problem.number_of_cities),
+        termination_criterion=StoppingByTime(max_seconds=10),
     )
 
     algorithm.run()
     result = algorithm.get_result()
 
-    # Save results to file
-    print_function_values_to_file(result, 'FUN.'+ algorithm.get_name() + "." + problem.get_name())
-    print_variables_to_file(result, 'VAR.' + algorithm.get_name() + "." + problem.get_name())
-
-    print('Algorithm: ' + algorithm.get_name())
-    print('Problem: ' + problem.get_name())
-    print('Solution: ' + result.get_binary_string())
-    print('Fitness:  ' + str(result.objectives[0]))
-    print('Computing time: ' + str(algorithm.total_computing_time))
+    print(f"Algorithm: {algorithm.get_name()}")
+    print(f"Solution: {result.variables}")
+    print(f"The shortest path length:  {str(result.objectives[0])}")
+    print(f"Computing time: {str(algorithm.total_computing_time)}")
+    print(f"Problem evaluations: {str(algorithm.evaluations)}")
```

### Comparing `jmetalpy-1.5.5/examples/singleobjective/simulated_annealing/simulated_annealing_float.py` & `jmetalpy-1.6.0/examples/multiobjective/hype/hype_zdt1.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,42 @@
-from jmetal.algorithm.singleobjective.simulated_annealing import SimulatedAnnealing
-from jmetal.operator import PolynomialMutation
-from jmetal.problem.singleobjective.unconstrained import Rastrigin
-from jmetal.util.solution import print_function_values_to_file, print_variables_to_file
+from jmetal.algorithm.multiobjective.hype import HYPE
+from jmetal.core.solution import FloatSolution
+from jmetal.operator import PolynomialMutation, SBXCrossover
+from jmetal.problem import ZDT1
+from jmetal.util.solution import (
+    print_function_values_to_file,
+    print_variables_to_file,
+    read_solutions,
+)
 from jmetal.util.termination_criterion import StoppingByEvaluations
 
-if __name__ == '__main__':
-    problem = Rastrigin(10)
-
-    max_evaluations = 250000
+if __name__ == "__main__":
+    problem = ZDT1()
+    problem.reference_front = read_solutions(filename="resources/reference_front/ZDT1.pf")
+
+    reference_point = FloatSolution(
+        [0],
+        [1],
+        problem.number_of_objectives(),
+    )
+    reference_point.objectives = [1.0, 1.0]  # Mandatory for HYPE
 
-    algorithm = SimulatedAnnealing(
+    algorithm = HYPE(
         problem=problem,
-        mutation=PolynomialMutation(probability=1.0 / problem.number_of_variables, distribution_index=20.0),
-        termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations)
+        reference_point=reference_point,
+        population_size=100,
+        offspring_population_size=100,
+        mutation=PolynomialMutation(probability=1.0 / problem.number_of_variables(), distribution_index=20),
+        crossover=SBXCrossover(probability=1.0, distribution_index=20),
+        termination_criterion=StoppingByEvaluations(25000),
     )
 
     algorithm.run()
-    result = algorithm.get_result()
+    front = algorithm.get_result()
 
     # Save results to file
-    print_function_values_to_file(result, 'FUN.'+ algorithm.get_name() + "." + problem.get_name())
-    print_variables_to_file(result, 'VAR.' + algorithm.get_name() + "." + problem.get_name())
+    print_function_values_to_file(front, "FUN." + algorithm.label)
+    print_variables_to_file(front, "VAR." + algorithm.label)
 
-    print('Algorithm: ' + algorithm.get_name())
-    print('Problem: ' + problem.get_name())
-    print('Solution: ' + str(result.variables[0]))
-    print('Fitness:  ' + str(result.objectives[0]))
-    print('Computing time: ' + str(algorithm.total_computing_time))
+    print(f"Algorithm: {algorithm.get_name()}")
+    print(f"Problem: {problem.name()}")
+    print(f"Computing time: {algorithm.total_computing_time}")
```

### Comparing `jmetalpy-1.5.5/jmetal/algorithm/multiobjective/gde3.py` & `jmetalpy-1.6.0/jmetal/algorithm/multiobjective/gde3.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,43 @@
-from typing import TypeVar, List
+from typing import List, TypeVar
 
 from jmetal.config import store
-from jmetal.core.algorithm import EvolutionaryAlgorithm, DynamicAlgorithm
-from jmetal.core.problem import Problem, DynamicProblem
+from jmetal.core.algorithm import DynamicAlgorithm, EvolutionaryAlgorithm
+from jmetal.core.problem import DynamicProblem, Problem
 from jmetal.core.solution import FloatSolution
-from jmetal.operator import DifferentialEvolutionCrossover, RankingAndCrowdingDistanceSelection
+from jmetal.operator import (
+    DifferentialEvolutionCrossover,
+    RankingAndCrowdingDistanceSelection,
+)
 from jmetal.operator.selection import DifferentialEvolutionSelection
 from jmetal.util.comparator import Comparator, DominanceComparator
 from jmetal.util.evaluator import Evaluator
 from jmetal.util.generator import Generator
 from jmetal.util.termination_criterion import TerminationCriterion
 
-S = TypeVar('S')
+S = TypeVar("S")
 R = List[S]
 
 
 class GDE3(EvolutionaryAlgorithm[FloatSolution, FloatSolution]):
-
-    def __init__(self,
-                 problem: Problem,
-                 population_size: int,
-                 cr: float,
-                 f: float,
-                 termination_criterion: TerminationCriterion = store.default_termination_criteria,
-                 k: float = 0.5,
-                 population_generator: Generator = store.default_generator,
-                 population_evaluator: Evaluator = store.default_evaluator,
-                 dominance_comparator: Comparator = store.default_comparator):
+    def __init__(
+        self,
+        problem: Problem,
+        population_size: int,
+        cr: float,
+        f: float,
+        termination_criterion: TerminationCriterion = store.default_termination_criteria,
+        k: float = 0.5,
+        population_generator: Generator = store.default_generator,
+        population_evaluator: Evaluator = store.default_evaluator,
+        dominance_comparator: Comparator = store.default_comparator,
+    ):
         super(GDE3, self).__init__(
-            problem=problem,
-            population_size=population_size,
-            offspring_population_size=population_size)
+            problem=problem, population_size=population_size, offspring_population_size=population_size
+        )
         self.dominance_comparator = dominance_comparator
         self.selection_operator = DifferentialEvolutionSelection()
         self.crossover_operator = DifferentialEvolutionCrossover(cr, f, k)
 
         self.population_generator = population_generator
         self.population_evaluator = population_evaluator
 
@@ -53,15 +56,15 @@
 
     def reproduction(self, mating_pool: List[S]) -> List[S]:
         offspring_population = []
         first_parent_index = 0
 
         for solution in self.solutions:
             self.crossover_operator.current_individual = solution
-            parents = mating_pool[first_parent_index:first_parent_index + 3]
+            parents = mating_pool[first_parent_index : first_parent_index + 3]
             first_parent_index += 3
 
             offspring_population.append(self.crossover_operator.execute(parents)[0])
 
         return offspring_population
 
     def replacement(self, population: List[S], offspring_population: List[FloatSolution]) -> List[List[FloatSolution]]:
@@ -92,50 +95,59 @@
     def stopping_condition_is_met(self) -> bool:
         return self.termination_criterion.is_met
 
     def get_result(self) -> List[FloatSolution]:
         return self.solutions
 
     def get_name(self) -> str:
-        return 'GDE3'
+        return "GDE3"
 
 
 class DynamicGDE3(GDE3, DynamicAlgorithm):
-
-    def __init__(self,
-                 problem: DynamicProblem,
-                 population_size: int,
-                 cr: float,
-                 f: float,
-                 termination_criterion: TerminationCriterion,
-                 k: float = 0.5,
-                 population_generator: Generator = store.default_generator,
-                 population_evaluator: Evaluator = store.default_evaluator,
-                 dominance_comparator: Comparator = DominanceComparator()):
+    def __init__(
+        self,
+        problem: DynamicProblem,
+        population_size: int,
+        cr: float,
+        f: float,
+        termination_criterion: TerminationCriterion,
+        k: float = 0.5,
+        population_generator: Generator = store.default_generator,
+        population_evaluator: Evaluator = store.default_evaluator,
+        dominance_comparator: Comparator = DominanceComparator(),
+    ):
         super(DynamicGDE3, self).__init__(
-            problem, population_size, cr, f, termination_criterion, k,
-            population_generator, population_evaluator, dominance_comparator)
+            problem,
+            population_size,
+            cr,
+            f,
+            termination_criterion,
+            k,
+            population_generator,
+            population_evaluator,
+            dominance_comparator,
+        )
 
         self.completed_iterations = 0
 
     def restart(self) -> None:
         pass
 
     def update_progress(self):
         if self.problem.the_problem_has_changed():
             self.restart()
             self.problem.clear_changed()
 
-        observable_data = self.get_observable_data()
+        observable_data = self.observable_data()
         self.observable.notify_all(**observable_data)
 
         self.evaluations += self.offspring_population_size
 
     def stopping_condition_is_met(self):
         if self.termination_criterion.is_met:
-            observable_data = self.get_observable_data()
+            observable_data = self.observable_data()
             self.observable.notify_all(**observable_data)
 
             self.restart()
             self.init_progress()
 
             self.completed_iterations += 1
```

### Comparing `jmetalpy-1.5.5/jmetal/algorithm/multiobjective/hype.py` & `jmetalpy-1.6.0/jmetal/algorithm/multiobjective/hype.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-from typing import TypeVar, List
+from typing import List, TypeVar
 
 from jmetal.algorithm.singleobjective.genetic_algorithm import GeneticAlgorithm
 from jmetal.config import store
-from jmetal.core.operator import Mutation, Crossover
+from jmetal.core.operator import Crossover, Mutation
 from jmetal.core.problem import Problem
 from jmetal.core.solution import Solution
 from jmetal.operator import BinaryTournamentSelection
 from jmetal.operator.selection import RankingAndFitnessSelection
-from jmetal.util.comparator import Comparator
-from jmetal.util.comparator import SolutionAttributeComparator
+from jmetal.util.comparator import Comparator, SolutionAttributeComparator
 from jmetal.util.evaluator import Evaluator
 from jmetal.util.generator import Generator
 from jmetal.util.termination_criterion import TerminationCriterion
 
-S = TypeVar('S')
-R = TypeVar('R')
+S = TypeVar("S")
+R = TypeVar("R")
 
 
 class HYPE(GeneticAlgorithm[S, R]):
-
-    def __init__(self,
-                 problem: Problem,
-                 reference_point: Solution,
-                 population_size: int,
-                 offspring_population_size: int,
-                 mutation: Mutation,
-                 crossover: Crossover,
-                 termination_criterion: TerminationCriterion = store.default_termination_criteria,
-                 population_generator: Generator = store.default_generator,
-                 population_evaluator: Evaluator = store.default_evaluator,
-                 dominance_comparator: Comparator = store.default_comparator):
-        """ This is an implementation of the Hypervolume Estimation Algorithm for Multi-objective Optimization
+    def __init__(
+        self,
+        problem: Problem,
+        reference_point: Solution,
+        population_size: int,
+        offspring_population_size: int,
+        mutation: Mutation,
+        crossover: Crossover,
+        termination_criterion: TerminationCriterion = store.default_termination_criteria,
+        population_generator: Generator = store.default_generator,
+        population_evaluator: Evaluator = store.default_evaluator,
+        dominance_comparator: Comparator = store.default_comparator,
+    ):
+        """This is an implementation of the Hypervolume Estimation Algorithm for Multi-objective Optimization
         proposed in:
 
         * J. Bader and E. Zitzler. HypE: An Algorithm for Fast Hypervolume-Based Many-Objective
         Optimization. TIK Report 286, Computer Engineering and Networks Laboratory (TIK), ETH
         Zurich, November 2008.
 
         It uses the Exact Hypervolume-based indicator formulation, which once computed, guides both
@@ -45,41 +45,43 @@
 
         problem = ZDT1()
         reference_point = FloatSolution(problem.number_of_variables,problem.number_of_objectives, [0], [1])
         reference_point.objectives = [1., 1.]
         """
 
         selection = BinaryTournamentSelection(
-            comparator=SolutionAttributeComparator(key='fitness', lowest_is_best=False))
-        self.ranking_fitness = RankingAndFitnessSelection(population_size,
-                                                          dominance_comparator=dominance_comparator,
-                                                          reference_point=reference_point)
+            comparator=SolutionAttributeComparator(key="fitness", lowest_is_best=False)
+        )
+        self.ranking_fitness = RankingAndFitnessSelection(
+            population_size, dominance_comparator=dominance_comparator, reference_point=reference_point
+        )
         self.reference_point = reference_point
         self.dominance_comparator = dominance_comparator
 
         super(HYPE, self).__init__(
             problem=problem,
             population_size=population_size,
             offspring_population_size=offspring_population_size,
             mutation=mutation,
             crossover=crossover,
             selection=selection,
             termination_criterion=termination_criterion,
             population_evaluator=population_evaluator,
-            population_generator=population_generator
+            population_generator=population_generator,
         )
 
     def evaluate(self, population: List[S]):
         population = self.population_evaluator.evaluate(population, self.problem)
-        population = self.ranking_fitness.compute_hypervol_fitness_values(population, self.reference_point,
-                                                                          len(population))
+        population = self.ranking_fitness.compute_hypervol_fitness_values(
+            population, self.reference_point, len(population)
+        )
         return population
 
     def replacement(self, population: List[S], offspring_population: List[S]) -> List[List[S]]:
         join_population = population + offspring_population
         return self.ranking_fitness.execute(join_population)
 
     def get_result(self) -> R:
         return self.solutions
 
     def get_name(self) -> str:
-        return 'HYPE'
+        return "HYPE"
```

### Comparing `jmetalpy-1.5.5/jmetal/algorithm/multiobjective/ibea.py` & `jmetalpy-1.6.0/jmetal/algorithm/multiobjective/ibea.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,40 @@
-from typing import TypeVar, List
+from typing import List, TypeVar
 
 import numpy as np
 
 from jmetal.algorithm.singleobjective.genetic_algorithm import GeneticAlgorithm
 from jmetal.config import store
-from jmetal.core.operator import Mutation, Crossover
+from jmetal.core.operator import Crossover, Mutation
 from jmetal.core.problem import Problem
 from jmetal.core.quality_indicator import EpsilonIndicator
 from jmetal.operator import BinaryTournamentSelection
 from jmetal.util.comparator import SolutionAttributeComparator
 from jmetal.util.evaluator import Evaluator
 from jmetal.util.generator import Generator
 from jmetal.util.termination_criterion import TerminationCriterion
 
-S = TypeVar('S')
-R = TypeVar('R')
+S = TypeVar("S")
+R = TypeVar("R")
 
 
 class IBEA(GeneticAlgorithm[S, R]):
-
-    def __init__(self,
-                 problem: Problem,
-                 population_size: int,
-                 offspring_population_size: int,
-                 mutation: Mutation,
-                 crossover: Crossover,
-                 kappa: float,
-                 termination_criterion: TerminationCriterion = store.default_termination_criteria,
-                 population_generator: Generator = store.default_generator,
-                 population_evaluator: Evaluator = store.default_evaluator):
-        """  Epsilon IBEA implementation as described in
+    def __init__(
+        self,
+        problem: Problem,
+        population_size: int,
+        offspring_population_size: int,
+        mutation: Mutation,
+        crossover: Crossover,
+        kappa: float,
+        termination_criterion: TerminationCriterion = store.default_termination_criteria,
+        population_generator: Generator = store.default_generator,
+        population_evaluator: Evaluator = store.default_evaluator,
+    ):
+        """Epsilon IBEA implementation as described in
 
         * Zitzler, Eckart, and Simon Künzli. "Indicator-based selection in multiobjective search."
         In International Conference on Parallel Problem Solving from Nature, pp. 832-842. Springer,
         Berlin, Heidelberg, 2004.
 
         https://link.springer.com/chapter/10.1007/978-3-540-30217-9_84
 
@@ -46,61 +47,67 @@
         :param population_size: Size of the population.
         :param mutation: Mutation operator (see :py:mod:`jmetal.operator.mutation`).
         :param crossover: Crossover operator (see :py:mod:`jmetal.operator.crossover`).
         :param kappa: Weight in the fitness computation.
         """
 
         selection = BinaryTournamentSelection(
-            comparator=SolutionAttributeComparator(key='fitness', lowest_is_best=False))
+            comparator=SolutionAttributeComparator(key="fitness", lowest_is_best=False)
+        )
         self.kappa = kappa
 
         super(IBEA, self).__init__(
             problem=problem,
             population_size=population_size,
             offspring_population_size=offspring_population_size,
             mutation=mutation,
             crossover=crossover,
             selection=selection,
             termination_criterion=termination_criterion,
             population_evaluator=population_evaluator,
-            population_generator=population_generator
+            population_generator=population_generator,
         )
 
     def compute_fitness_values(self, population: List[S], kappa: float) -> List[S]:
         for i in range(len(population)):
-            population[i].attributes['fitness'] = 0
+            population[i].attributes["fitness"] = 0
 
             for j in range(len(population)):
                 if j != i:
-                    population[i].attributes['fitness'] += -np.exp(
-                        -EpsilonIndicator([population[i].objectives]).compute([population[j].objectives]) / self.kappa)
+                    population[i].attributes["fitness"] += -np.exp(
+                        -EpsilonIndicator([population[i].objectives]).compute([population[j].objectives]) / self.kappa
+                    )
         return population
 
     def create_initial_solutions(self) -> List[S]:
         population = [self.population_generator.new(self.problem) for _ in range(self.population_size)]
         population = self.compute_fitness_values(population, self.kappa)
 
         return population
 
     def replacement(self, population: List[S], offspring_population: List[S]) -> List[List[S]]:
         join_population = population + offspring_population
         join_population_size = len(join_population)
         join_population = self.compute_fitness_values(join_population, self.kappa)
 
         while join_population_size > self.population_size:
-            current_fitnesses = [individual.attributes['fitness'] for individual in join_population]
+            current_fitnesses = [individual.attributes["fitness"] for individual in join_population]
             index_worst = current_fitnesses.index(min(current_fitnesses))
 
             for i in range(join_population_size):
-                join_population[i].attributes['fitness'] += np.exp(
-                    - EpsilonIndicator([join_population[i].objectives]).compute([join_population[index_worst].objectives]) / self.kappa)
+                join_population[i].attributes["fitness"] += np.exp(
+                    -EpsilonIndicator([join_population[i].objectives]).compute(
+                        [join_population[index_worst].objectives]
+                    )
+                    / self.kappa
+                )
 
             join_population.pop(index_worst)
             join_population_size = join_population_size - 1
 
         return join_population
 
     def get_result(self) -> R:
         return self.solutions
 
     def get_name(self) -> str:
-        return 'Epsilon-IBEA'
+        return "Epsilon-IBEA"
```

### Comparing `jmetalpy-1.5.5/jmetal/algorithm/multiobjective/mocell.py` & `jmetalpy-1.6.0/jmetal/algorithm/multiobjective/mocell.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,52 +1,53 @@
 import copy
 from functools import cmp_to_key
-from typing import TypeVar, List
+from typing import List, TypeVar
 
 from jmetal.algorithm.singleobjective.genetic_algorithm import GeneticAlgorithm
 from jmetal.config import store
-from jmetal.core.operator import Mutation, Crossover, Selection
+from jmetal.core.operator import Crossover, Mutation, Selection
 from jmetal.core.problem import Problem
 from jmetal.operator import BinaryTournamentSelection
 from jmetal.util.archive import BoundedArchive
 from jmetal.util.comparator import Comparator, MultiComparator
 from jmetal.util.density_estimator import CrowdingDistance, DensityEstimator
 from jmetal.util.evaluator import Evaluator
 from jmetal.util.generator import Generator
 from jmetal.util.neighborhood import Neighborhood
 from jmetal.util.ranking import FastNonDominatedRanking, Ranking
 from jmetal.util.termination_criterion import TerminationCriterion
 
-S = TypeVar('S')
-R = TypeVar('R')
+S = TypeVar("S")
+R = TypeVar("R")
 
 """
 .. module:: MOCell
    :platform: Unix, Windows
    :synopsis: MOCell (Multi-Objective Cellular evolutionary algorithm) implementation
 .. moduleauthor:: Antonio J. Nebro <antonio@lcc.uma.es>
 """
 
 
 class MOCell(GeneticAlgorithm[S, R]):
-
-    def __init__(self,
-                 problem: Problem,
-                 population_size: int,
-                 neighborhood: Neighborhood,
-                 archive: BoundedArchive,
-                 mutation: Mutation,
-                 crossover: Crossover,
-                 selection: Selection = BinaryTournamentSelection(
-                     MultiComparator([FastNonDominatedRanking.get_comparator(),
-                                      CrowdingDistance.get_comparator()])),
-                 termination_criterion: TerminationCriterion = store.default_termination_criteria,
-                 population_generator: Generator = store.default_generator,
-                 population_evaluator: Evaluator = store.default_evaluator,
-                 dominance_comparator: Comparator = store.default_comparator):
+    def __init__(
+        self,
+        problem: Problem,
+        population_size: int,
+        neighborhood: Neighborhood,
+        archive: BoundedArchive,
+        mutation: Mutation,
+        crossover: Crossover,
+        selection: Selection = BinaryTournamentSelection(
+            MultiComparator([FastNonDominatedRanking.get_comparator(), CrowdingDistance.get_comparator()])
+        ),
+        termination_criterion: TerminationCriterion = store.default_termination_criteria,
+        population_generator: Generator = store.default_generator,
+        population_evaluator: Evaluator = store.default_evaluator,
+        dominance_comparator: Comparator = store.default_comparator,
+    ):
         """
         MOCEll implementation as described in:
 
         :param problem: The problem to solve.
         :param population_size: Size of the population.
         :param mutation: Mutation operator (see :py:mod:`jmetal.operator.mutation`).
         :param crossover: Crossover operator (see :py:mod:`jmetal.operator.crossover`).
@@ -57,24 +58,23 @@
             population_size=population_size,
             offspring_population_size=1,
             mutation=mutation,
             crossover=crossover,
             selection=selection,
             termination_criterion=termination_criterion,
             population_evaluator=population_evaluator,
-            population_generator=population_generator
+            population_generator=population_generator,
         )
         self.dominance_comparator = dominance_comparator
         self.neighborhood = neighborhood
         self.archive = archive
         self.current_individual = 0
         self.current_neighbors = []
 
-        self.comparator = MultiComparator([FastNonDominatedRanking.get_comparator(),
-                                           CrowdingDistance.get_comparator()])
+        self.comparator = MultiComparator([FastNonDominatedRanking.get_comparator(), CrowdingDistance.get_comparator()])
 
     def init_progress(self) -> None:
         super().init_progress()
         for solution in self.solutions:
             self.archive.add(copy.copy(solution))
 
     def update_progress(self) -> None:
@@ -95,27 +95,27 @@
 
         return parents
 
     def reproduction(self, mating_population: List[S]) -> List[S]:
         number_of_parents_to_combine = self.crossover_operator.get_number_of_parents()
 
         if len(mating_population) % number_of_parents_to_combine != 0:
-            raise Exception('Wrong number of parents')
+            raise Exception("Wrong number of parents")
 
         offspring_population = self.crossover_operator.execute(mating_population)
-        self.mutation_operator.execute(offspring_population[0])
+        offspring_population[0] = self.mutation_operator.execute(offspring_population[0])
 
         return [offspring_population[0]]
 
     def replacement(self, population: List[S], offspring_population: List[S]) -> List[List[S]]:
         result = self.dominance_comparator.compare(population[self.current_individual], offspring_population[0])
 
         if result == 1:  # the offspring individual dominates the current one
             population[self.current_individual] = offspring_population[0]
-            self.archive.add(offspring_population[0])
+            self.archive.add(copy.deepcopy(offspring_population[0]))
         elif result == 0:  # the offspring and current individuals are non-dominated
             new_individual = offspring_population[0]
 
             self.current_neighbors.append(new_individual)
 
             ranking: Ranking = FastNonDominatedRanking()
             ranking.compute_ranking(self.current_neighbors)
@@ -123,18 +123,18 @@
             density_estimator: DensityEstimator = CrowdingDistance()
             for i in range(ranking.get_number_of_subfronts()):
                 density_estimator.compute_density_estimator(ranking.get_subfront(i))
 
             self.current_neighbors.sort(key=cmp_to_key(self.comparator.compare))
             worst_solution = self.current_neighbors[-1]
 
-            self.archive.add(new_individual)
+            self.archive.add(copy.deepcopy(new_individual))
             if worst_solution != new_individual:
                 population[self.current_individual] = new_individual
 
         return population
 
     def get_result(self) -> R:
         return self.archive.solution_list
 
     def get_name(self) -> str:
-        return 'MOCell'
+        return "MOCell"
```

### Comparing `jmetalpy-1.5.5/jmetal/algorithm/multiobjective/moead.py` & `jmetalpy-1.6.0/jmetal/algorithm/multiobjective/moead.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,91 +1,98 @@
 import copy
 import random
 from math import ceil
-from typing import TypeVar, List, Generator
+from typing import Generator, List, TypeVar
 
 import numpy as np
 
 from jmetal.algorithm.singleobjective.genetic_algorithm import GeneticAlgorithm
 from jmetal.config import store
 from jmetal.core.operator import Mutation
 from jmetal.core.problem import Problem
 from jmetal.operator import DifferentialEvolutionCrossover, NaryRandomSolutionSelection
 from jmetal.util.aggregative_function import AggregativeFunction
-from jmetal.util.constraint_handling import feasibility_ratio, \
-    overall_constraint_violation_degree, is_feasible
+from jmetal.util.constraint_handling import (
+    feasibility_ratio,
+    is_feasible,
+    overall_constraint_violation_degree,
+)
 from jmetal.util.density_estimator import CrowdingDistance
 from jmetal.util.evaluator import Evaluator
 from jmetal.util.neighborhood import WeightVectorNeighborhood
 from jmetal.util.ranking import FastNonDominatedRanking
-from jmetal.util.termination_criterion import TerminationCriterion, StoppingByEvaluations
+from jmetal.util.termination_criterion import (
+    StoppingByEvaluations,
+    TerminationCriterion,
+)
 
-S = TypeVar('S')
+S = TypeVar("S")
 R = List[S]
 
 
 class MOEAD(GeneticAlgorithm):
-
-    def __init__(self,
-                 problem: Problem,
-                 population_size: int,
-                 mutation: Mutation,
-                 crossover: DifferentialEvolutionCrossover,
-                 aggregative_function: AggregativeFunction,
-                 neighbourhood_selection_probability: float,
-                 max_number_of_replaced_solutions: int,
-                 neighbor_size: int,
-                 weight_files_path: str,
-                 termination_criterion: TerminationCriterion = store.default_termination_criteria,
-                 population_generator: Generator = store.default_generator,
-                 population_evaluator: Evaluator = store.default_evaluator):
+    def __init__(
+        self,
+        problem: Problem,
+        population_size: int,
+        mutation: Mutation,
+        crossover: DifferentialEvolutionCrossover,
+        aggregative_function: AggregativeFunction,
+        neighbourhood_selection_probability: float,
+        max_number_of_replaced_solutions: int,
+        neighbor_size: int,
+        weight_files_path: str,
+        termination_criterion: TerminationCriterion = store.default_termination_criteria,
+        population_generator: Generator = store.default_generator,
+        population_evaluator: Evaluator = store.default_evaluator,
+    ):
         """
         :param max_number_of_replaced_solutions: (eta in Zhang & Li paper).
         :param neighbourhood_selection_probability: Probability of mating with a solution in the neighborhood rather
                than the entire population (Delta in Zhang & Li paper).
         """
         super(MOEAD, self).__init__(
             problem=problem,
             population_size=population_size,
             offspring_population_size=1,
             mutation=mutation,
             crossover=crossover,
             selection=NaryRandomSolutionSelection(2),
             population_evaluator=population_evaluator,
             population_generator=population_generator,
-            termination_criterion=termination_criterion
+            termination_criterion=termination_criterion,
         )
         self.max_number_of_replaced_solutions = max_number_of_replaced_solutions
         self.fitness_function = aggregative_function
         self.neighbourhood = WeightVectorNeighborhood(
             number_of_weight_vectors=population_size,
             neighborhood_size=neighbor_size,
-            weight_vector_size=problem.number_of_objectives,
-            weights_path=weight_files_path
+            weight_vector_size=problem.number_of_objectives(),
+            weights_path=weight_files_path,
         )
         self.neighbourhood_selection_probability = neighbourhood_selection_probability
         self.permutation = None
         self.current_subproblem = 0
         self.neighbor_type = None
 
     def init_progress(self) -> None:
         self.evaluations = self.population_size
         for solution in self.solutions:
             self.fitness_function.update(solution.objectives)
 
         self.permutation = Permutation(self.population_size)
 
-        observable_data = self.get_observable_data()
+        observable_data = self.observable_data()
         self.observable.notify_all(**observable_data)
 
     def selection(self, population: List[S]):
         self.current_subproblem = self.permutation.get_next_value()
         self.neighbor_type = self.choose_neighbor_type()
 
-        if self.neighbor_type == 'NEIGHBOR':
+        if self.neighbor_type == "NEIGHBOR":
             neighbors = self.neighbourhood.get_neighbors(self.current_subproblem, population)
             mating_population = self.selection_operator.execute(neighbors)
         else:
             mating_population = self.selection_operator.execute(population)
 
         mating_population.append(population[self.current_subproblem])
 
@@ -124,50 +131,69 @@
 
             if replacements >= self.max_number_of_replaced_solutions:
                 break
 
         return population
 
     def generate_permutation_of_neighbors(self, subproblem_id):
-        if self.neighbor_type == 'NEIGHBOR':
+        if self.neighbor_type == "NEIGHBOR":
             neighbors = self.neighbourhood.get_neighborhood()[subproblem_id]
             permuted_array = copy.deepcopy(neighbors.tolist())
         else:
             permuted_array = Permutation(self.population_size).get_permutation()
 
         return permuted_array
 
     def choose_neighbor_type(self):
         rnd = random.random()
 
         if rnd < self.neighbourhood_selection_probability:
-            neighbor_type = 'NEIGHBOR'
+            neighbor_type = "NEIGHBOR"
         else:
-            neighbor_type = 'POPULATION'
+            neighbor_type = "POPULATION"
 
         return neighbor_type
 
     def get_name(self):
-        return 'MOEAD'
+        return "MOEAD"
 
     def get_result(self):
         return self.solutions
 
 
 class MOEAD_DRA(MOEAD):
-    def __init__(self, problem, population_size, mutation, crossover, aggregative_function,
-                 neighbourhood_selection_probability, max_number_of_replaced_solutions, neighbor_size,
-                 weight_files_path, termination_criterion=store.default_termination_criteria,
-                 population_generator=store.default_generator, population_evaluator=store.default_evaluator):
-        super(MOEAD_DRA, self).__init__(problem, population_size, mutation, crossover, aggregative_function,
-                                        neighbourhood_selection_probability, max_number_of_replaced_solutions,
-                                        neighbor_size, weight_files_path,
-                                        termination_criterion=termination_criterion,
-                                        population_generator=population_generator,
-                                        population_evaluator=population_evaluator)
+    def __init__(
+        self,
+        problem,
+        population_size,
+        mutation,
+        crossover,
+        aggregative_function,
+        neighbourhood_selection_probability,
+        max_number_of_replaced_solutions,
+        neighbor_size,
+        weight_files_path,
+        termination_criterion=store.default_termination_criteria,
+        population_generator=store.default_generator,
+        population_evaluator=store.default_evaluator,
+    ):
+        super(MOEAD_DRA, self).__init__(
+            problem,
+            population_size,
+            mutation,
+            crossover,
+            aggregative_function,
+            neighbourhood_selection_probability,
+            max_number_of_replaced_solutions,
+            neighbor_size,
+            weight_files_path,
+            termination_criterion=termination_criterion,
+            population_generator=population_generator,
+            population_evaluator=population_evaluator,
+        )
 
         self.saved_values = []
         self.utility = [1.0 for _ in range(population_size)]
         self.frequency = [0.0 for _ in range(population_size)]
         self.generation_counter = 0
         self.order = []
         self.current_order_index = 0
@@ -179,15 +205,15 @@
         self.evaluations = self.population_size
         for solution in self.solutions:
             self.fitness_function.update(solution.objectives)
 
         self.order = self.__tour_selection(10)
         self.current_order_index = 0
 
-        observable_data = self.get_observable_data()
+        observable_data = self.observable_data()
         self.observable.notify_all(**observable_data)
 
     def update_progress(self):
         super().update_progress()
 
         self.current_order_index += 1
         if self.current_order_index == (len(self.order)):
@@ -201,26 +227,26 @@
     def selection(self, population: List[S]):
         self.current_subproblem = self.order[self.current_order_index]
         self.current_order_index += 1
         self.frequency[self.current_subproblem] += 1
 
         self.neighbor_type = self.choose_neighbor_type()
 
-        if self.neighbor_type == 'NEIGHBOR':
+        if self.neighbor_type == "NEIGHBOR":
             neighbors = self.neighbourhood.get_neighbors(self.current_subproblem, population)
             mating_population = self.selection_operator.execute(neighbors)
         else:
             mating_population = self.selection_operator.execute(population)
 
         mating_population.append(population[self.current_subproblem])
 
         return mating_population
 
     def get_name(self):
-        return 'MOEAD-DRA'
+        return "MOEAD-DRA"
 
     def __utility_function(self):
         for i in range(len(self.solutions)):
             f1 = self.fitness_function.compute(self.solutions[i].objectives, self.neighbourhood.weight_vectors[i])
             f2 = self.fitness_function.compute(self.saved_values[i].objectives, self.neighbourhood.weight_vectors[i])
             delta = f2 - f1
             if delta > 0.001:
@@ -247,27 +273,29 @@
             selected.append(best_sub)
             del candidate[best_idd]
 
         return selected
 
 
 class MOEADIEpsilon(MOEAD):
-    def __init__(self,
-                 problem: Problem,
-                 population_size: int,
-                 mutation: Mutation,
-                 crossover: DifferentialEvolutionCrossover,
-                 aggregative_function: AggregativeFunction,
-                 neighbourhood_selection_probability: float,
-                 max_number_of_replaced_solutions: int,
-                 neighbor_size: int,
-                 weight_files_path: str,
-                 termination_criterion: TerminationCriterion = StoppingByEvaluations(300000),
-                 population_generator: Generator = store.default_generator,
-                 population_evaluator: Evaluator = store.default_evaluator):
+    def __init__(
+        self,
+        problem: Problem,
+        population_size: int,
+        mutation: Mutation,
+        crossover: DifferentialEvolutionCrossover,
+        aggregative_function: AggregativeFunction,
+        neighbourhood_selection_probability: float,
+        max_number_of_replaced_solutions: int,
+        neighbor_size: int,
+        weight_files_path: str,
+        termination_criterion: TerminationCriterion = StoppingByEvaluations(300000),
+        population_generator: Generator = store.default_generator,
+        population_evaluator: Evaluator = store.default_evaluator,
+    ):
         """
         :param max_number_of_replaced_solutions: (eta in Zhang & Li paper).
         :param neighbourhood_selection_probability: Probability of mating with a solution in the neighborhood rather
                than the entire population (Delta in Zhang & Li paper).
         """
         super(MOEADIEpsilon, self).__init__(
             problem=problem,
@@ -277,15 +305,15 @@
             aggregative_function=aggregative_function,
             neighbourhood_selection_probability=neighbourhood_selection_probability,
             max_number_of_replaced_solutions=max_number_of_replaced_solutions,
             neighbor_size=neighbor_size,
             weight_files_path=weight_files_path,
             population_evaluator=population_evaluator,
             population_generator=population_generator,
-            termination_criterion=termination_criterion
+            termination_criterion=termination_criterion,
         )
         self.constraints = []
         self.epsilon_k = 0
         self.phi_max = -1e30
         self.epsilon_zero = 0
         self.tc = 800
         self.tao = 0.05
@@ -294,16 +322,17 @@
         self.archive = []
 
     def init_progress(self) -> None:
         super().init_progress()
 
         # for i in range(self.population_size):
         #    self.constraints[i] = get_overall_constraint_violation_degree(self.permutation[i])
-        self.constraints = [overall_constraint_violation_degree(self.solutions[i])
-                            for i in range(0, self.population_size)]
+        self.constraints = [
+            overall_constraint_violation_degree(self.solutions[i]) for i in range(0, self.population_size)
+        ]
 
         sorted(self.constraints)
         self.epsilon_zero = abs(self.constraints[int(ceil(0.05 * self.population_size))])
 
         if self.phi_max < abs(self.constraints[0]):
             self.phi_max = abs(self.constraints[0])
 
@@ -374,28 +403,28 @@
                 self.archive = []
                 for solution in first_rank_solutions:
                     self.archive.append(copy.deepcopy(solution))
             else:
                 crowding_distance = CrowdingDistance()
                 while len(first_rank_solutions) > self.population_size:
                     crowding_distance.compute_density_estimator(first_rank_solutions)
-                    first_rank_solutions = sorted(first_rank_solutions, key=lambda x: x.attributes['crowding_distance'],
-                                                  reverse=True)
+                    first_rank_solutions = sorted(
+                        first_rank_solutions, key=lambda x: x.attributes["crowding_distance"], reverse=True
+                    )
                     first_rank_solutions.pop()
 
                 self.archive = []
                 for solution in first_rank_solutions:
                     self.archive.append(copy.deepcopy(solution))
 
     def get_result(self):
         return self.archive
 
 
 class Permutation:
-
     def __init__(self, length: int):
         self.counter = 0
         self.length = length
         self.permutation = np.random.permutation(length)
 
     def get_next_value(self):
         next_value = self.permutation[self.counter]
```

### Comparing `jmetalpy-1.5.5/jmetal/algorithm/multiobjective/nsgaii.py` & `jmetalpy-1.6.0/jmetal/algorithm/multiobjective/nsgaii.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,56 +1,60 @@
 import time
-from typing import TypeVar, List, Generator
+from typing import Generator, List, TypeVar
 
 try:
     import dask
-    from distributed import as_completed, Client
+    from distributed import Client, as_completed
 except ImportError:
     pass
 
 from jmetal.algorithm.singleobjective.genetic_algorithm import GeneticAlgorithm
 from jmetal.config import store
-from jmetal.core.algorithm import DynamicAlgorithm, Algorithm
-from jmetal.core.operator import Mutation, Crossover, Selection
-from jmetal.core.problem import Problem, DynamicProblem
+from jmetal.core.algorithm import Algorithm, DynamicAlgorithm
+from jmetal.core.operator import Crossover, Mutation, Selection
+from jmetal.core.problem import DynamicProblem, Problem
 from jmetal.operator import BinaryTournamentSelection
+from jmetal.util.comparator import Comparator, DominanceComparator, MultiComparator
 from jmetal.util.density_estimator import CrowdingDistance
 from jmetal.util.evaluator import Evaluator
 from jmetal.util.ranking import FastNonDominatedRanking
-from jmetal.util.replacement import RankingAndDensityEstimatorReplacement, RemovalPolicyType
-from jmetal.util.comparator import DominanceComparator, Comparator, MultiComparator
+from jmetal.util.replacement import (
+    RankingAndDensityEstimatorReplacement,
+    RemovalPolicyType,
+)
 from jmetal.util.termination_criterion import TerminationCriterion
 
-S = TypeVar('S')
-R = TypeVar('R')
+S = TypeVar("S")
+R = TypeVar("R")
 
 """
 .. module:: NSGA-II
    :platform: Unix, Windows
    :synopsis: NSGA-II (Non-dominance Sorting Genetic Algorithm II) implementation.
 
 .. moduleauthor:: Antonio J. Nebro <antonio@lcc.uma.es>, Antonio Benítez-Hidalgo <antonio.b@uma.es>
 """
 
 
 class NSGAII(GeneticAlgorithm[S, R]):
-
-    def __init__(self,
-                 problem: Problem,
-                 population_size: int,
-                 offspring_population_size: int,
-                 mutation: Mutation,
-                 crossover: Crossover,
-                 selection: Selection = BinaryTournamentSelection(
-                     MultiComparator([FastNonDominatedRanking.get_comparator(),
-                                      CrowdingDistance.get_comparator()])),
-                 termination_criterion: TerminationCriterion = store.default_termination_criteria,
-                 population_generator: Generator = store.default_generator,
-                 population_evaluator: Evaluator = store.default_evaluator,
-                 dominance_comparator: Comparator = store.default_comparator):
+    def __init__(
+        self,
+        problem: Problem,
+        population_size: int,
+        offspring_population_size: int,
+        mutation: Mutation,
+        crossover: Crossover,
+        selection: Selection = BinaryTournamentSelection(
+            MultiComparator([FastNonDominatedRanking.get_comparator(), CrowdingDistance.get_comparator()])
+        ),
+        termination_criterion: TerminationCriterion = store.default_termination_criteria,
+        population_generator: Generator = store.default_generator,
+        population_evaluator: Evaluator = store.default_evaluator,
+        dominance_comparator: Comparator = store.default_comparator,
+    ):
         """
         NSGA-II implementation as described in
 
         * K. Deb, A. Pratap, S. Agarwal and T. Meyarivan, "A fast and elitist
           multiobjective genetic algorithm: NSGA-II," in IEEE Transactions on Evolutionary Computation,
           vol. 6, no. 2, pp. 182-197, Apr 2002. doi: 10.1109/4235.996017
 
@@ -60,31 +64,30 @@
 
         .. note:: A steady-state version of this algorithm can be run by setting the offspring size to 1.
 
         :param problem: The problem to solve.
         :param population_size: Size of the population.
         :param mutation: Mutation operator (see :py:mod:`jmetal.operator.mutation`).
         :param crossover: Crossover operator (see :py:mod:`jmetal.operator.crossover`).
-        :param selection: Selection operator (see :py:mod:`jmetal.operator.selection`).
         """
         super(NSGAII, self).__init__(
             problem=problem,
             population_size=population_size,
             offspring_population_size=offspring_population_size,
             mutation=mutation,
             crossover=crossover,
             selection=selection,
             termination_criterion=termination_criterion,
             population_evaluator=population_evaluator,
-            population_generator=population_generator
+            population_generator=population_generator,
         )
         self.dominance_comparator = dominance_comparator
 
     def replacement(self, population: List[S], offspring_population: List[S]) -> List[List[S]]:
-        """ This method joins the current and offspring populations to produce the population of the next generation
+        """This method joins the current and offspring populations to produce the population of the next generation
         by applying the ranking and crowding distance selection.
 
         :param population: Parent population.
         :param offspring_population: Offspring population.
         :return: New population after ranking and crowding distance selection is applied.
         """
         ranking = FastNonDominatedRanking(self.dominance_comparator)
@@ -95,86 +98,89 @@
 
         return solutions
 
     def get_result(self) -> R:
         return self.solutions
 
     def get_name(self) -> str:
-        return 'NSGAII'
+        return "NSGAII"
 
 
 class DynamicNSGAII(NSGAII[S, R], DynamicAlgorithm):
-
-    def __init__(self,
-                 problem: DynamicProblem[S],
-                 population_size: int,
-                 offspring_population_size: int,
-                 mutation: Mutation,
-                 crossover: Crossover,
-                 selection: Selection = BinaryTournamentSelection(
-                     MultiComparator([FastNonDominatedRanking.get_comparator(),
-                                      CrowdingDistance.get_comparator()])),
-                 termination_criterion: TerminationCriterion = store.default_termination_criteria,
-                 population_generator: Generator = store.default_generator,
-                 population_evaluator: Evaluator = store.default_evaluator,
-                 dominance_comparator: DominanceComparator = DominanceComparator()):
+    def __init__(
+        self,
+        problem: DynamicProblem[S],
+        population_size: int,
+        offspring_population_size: int,
+        mutation: Mutation,
+        crossover: Crossover,
+        selection: Selection = BinaryTournamentSelection(
+            MultiComparator([FastNonDominatedRanking.get_comparator(), CrowdingDistance.get_comparator()])
+        ),
+        termination_criterion: TerminationCriterion = store.default_termination_criteria,
+        population_generator: Generator = store.default_generator,
+        population_evaluator: Evaluator = store.default_evaluator,
+        dominance_comparator: DominanceComparator = DominanceComparator(),
+    ):
         super(DynamicNSGAII, self).__init__(
             problem=problem,
             population_size=population_size,
             offspring_population_size=offspring_population_size,
             mutation=mutation,
             crossover=crossover,
             selection=selection,
             population_evaluator=population_evaluator,
             population_generator=population_generator,
             termination_criterion=termination_criterion,
-            dominance_comparator=dominance_comparator)
+            dominance_comparator=dominance_comparator,
+        )
         self.completed_iterations = 0
         self.start_computing_time = 0
         self.total_computing_time = 0
 
     def restart(self):
         self.solutions = self.evaluate(self.solutions)
 
     def update_progress(self):
         if self.problem.the_problem_has_changed():
             self.restart()
             self.problem.clear_changed()
 
-        observable_data = self.get_observable_data()
+        observable_data = self.observable_data()
         self.observable.notify_all(**observable_data)
 
         self.evaluations += self.offspring_population_size
 
     def stopping_condition_is_met(self):
         if self.termination_criterion.is_met:
-            observable_data = self.get_observable_data()
-            observable_data['TERMINATION_CRITERIA_IS_MET'] = True
+            observable_data = self.observable_data()
+            observable_data["TERMINATION_CRITERIA_IS_MET"] = True
             self.observable.notify_all(**observable_data)
 
             self.restart()
             self.init_progress()
 
             self.completed_iterations += 1
 
 
 class DistributedNSGAII(Algorithm[S, R]):
-
-    def __init__(self,
-                 problem: Problem,
-                 population_size: int,
-                 mutation: Mutation,
-                 crossover: Crossover,
-                 number_of_cores: int,
-                 client,
-                 selection: Selection = BinaryTournamentSelection(
-                     MultiComparator([FastNonDominatedRanking.get_comparator(),
-                                      CrowdingDistance.get_comparator()])),
-                 termination_criterion: TerminationCriterion = store.default_termination_criteria,
-                 dominance_comparator: DominanceComparator = DominanceComparator()):
+    def __init__(
+        self,
+        problem: Problem,
+        population_size: int,
+        mutation: Mutation,
+        crossover: Crossover,
+        number_of_cores: int,
+        client,
+        selection: Selection = BinaryTournamentSelection(
+            MultiComparator([FastNonDominatedRanking.get_comparator(), CrowdingDistance.get_comparator()])
+        ),
+        termination_criterion: TerminationCriterion = store.default_termination_criteria,
+        dominance_comparator: DominanceComparator = DominanceComparator(),
+    ):
         super(DistributedNSGAII, self).__init__()
         self.problem = problem
         self.population_size = population_size
         self.mutation_operator = mutation
         self.crossover_operator = crossover
         self.selection_operator = selection
         self.dominance_comparator = dominance_comparator
@@ -190,37 +196,39 @@
 
     def evaluate(self, solutions: List[S]) -> List[S]:
         return self.client.map(self.problem.evaluate, solutions)
 
     def stopping_condition_is_met(self) -> bool:
         return self.termination_criterion.is_met
 
-    def get_observable_data(self) -> dict:
+    def observable_data(self) -> dict:
         ctime = time.time() - self.start_computing_time
 
-        return {'PROBLEM': self.problem,
-                'EVALUATIONS': self.evaluations,
-                'SOLUTIONS': self.get_result(),
-                'COMPUTING_TIME': ctime}
+        return {
+            "PROBLEM": self.problem,
+            "EVALUATIONS": self.evaluations,
+            "SOLUTIONS": self.get_result(),
+            "COMPUTING_TIME": ctime,
+        }
 
     def init_progress(self) -> None:
         self.evaluations = self.number_of_cores
 
-        observable_data = self.get_observable_data()
+        observable_data = self.observable_data()
         self.observable.notify_all(**observable_data)
 
     def step(self) -> None:
         pass
 
     def update_progress(self):
-        observable_data = self.get_observable_data()
+        observable_data = self.observable_data()
         self.observable.notify_all(**observable_data)
 
     def run(self):
-        """ Execute the algorithm. """
+        """Execute the algorithm."""
         self.start_computing_time = time.time()
 
         create_solution = dask.delayed(self.problem.create_solution)
         evaluate_solution = dask.delayed(self.problem.evaluate)
 
         task_pool = as_completed([], with_results=True)
 
@@ -269,16 +277,17 @@
                 # selection
                 mating_population = []
                 for _ in range(2):
                     solution = self.selection_operator.execute(auxiliar_population)
                     mating_population.append(solution)
 
                 # Reproduction and evaluation
-                new_task = self.client.submit(reproduction, mating_population, self.problem,
-                                              self.crossover_operator, self.mutation_operator)
+                new_task = self.client.submit(
+                    reproduction, mating_population, self.problem, self.crossover_operator, self.mutation_operator
+                )
                 task_pool.add(new_task)
 
                 # update progress
                 self.evaluations += 1
                 self.solutions = auxiliar_population
 
                 self.update_progress()
@@ -292,15 +301,15 @@
         for future, _ in task_pool:
             future.cancel()
 
     def get_result(self) -> R:
         return self.solutions
 
     def get_name(self) -> str:
-        return 'dNSGA-II'
+        return "dNSGA-II"
 
 
 def reproduction(mating_population: List[S], problem, crossover_operator, mutation_operator) -> S:
     offspring_pool = []
     for parents in zip(*[iter(mating_population)] * 2):
         offspring_pool.append(crossover_operator.execute(parents))
```

### Comparing `jmetalpy-1.5.5/jmetal/algorithm/multiobjective/nsgaiii.py` & `jmetalpy-1.6.0/jmetal/algorithm/multiobjective/nsgaiii.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,39 @@
-from abc import abstractmethod, ABC
-from typing import TypeVar, List
+from abc import ABC, abstractmethod
+from typing import List, TypeVar
 
 import numpy as np
 from numpy.linalg import LinAlgError
 from scipy import special
 
 from jmetal.algorithm.multiobjective.nsgaii import NSGAII
 from jmetal.config import store
-from jmetal.core.operator import Mutation, Crossover, Selection
+from jmetal.core.operator import Crossover, Mutation, Selection
 from jmetal.core.problem import Problem
 from jmetal.operator import BinaryTournamentSelection
 from jmetal.util.comparator import Comparator, MultiComparator
 from jmetal.util.density_estimator import CrowdingDistance
 from jmetal.util.evaluator import Evaluator
 from jmetal.util.generator import Generator
 from jmetal.util.ranking import FastNonDominatedRanking
 from jmetal.util.termination_criterion import TerminationCriterion
 
-S = TypeVar('S')
-R = TypeVar('R')
+S = TypeVar("S")
+R = TypeVar("R")
 
 """
 .. module:: NSGA-III
    :platform: Unix, Windows
    :synopsis: NSGA-III (Non-dominance Sorting Genetic Algorithm III) implementation.
 
 .. moduleauthor:: Antonio Benítez-Hidalgo <antonio.b@uma.es>, Julian Blank <blankjul@egr.msu.edu>
 """
 
 
 class ReferenceDirectionFactory(ABC):
-
     def __init__(self, n_dim: int, scaling=None) -> None:
         self.n_dim = n_dim
         self.scaling = scaling
 
     def compute(self):
         if self.n_dim == 1:
             return np.array([[1.0]])
@@ -46,15 +45,14 @@
 
     @abstractmethod
     def _compute(self):
         pass
 
 
 class UniformReferenceDirectionFactory(ReferenceDirectionFactory):
-
     def __init__(self, n_dim: int, scaling=None, n_points: int = None, n_partitions: int = None) -> None:
         super().__init__(n_dim, scaling)
         if n_points is not None:
             self.n_partitions = self.get_partition_closest_to_points(n_points, n_dim)
         else:
             if n_partitions is None:
                 raise Exception("Either provide number of partitions or number of points.")
@@ -73,16 +71,15 @@
     def __uniform_reference_directions(self, ref_dirs, ref_dir, n_partitions: int, beta: int, depth: int):
         if depth == len(ref_dir) - 1:
             ref_dir[depth] = beta / (1.0 * n_partitions)
             ref_dirs.append(ref_dir[None, :])
         else:
             for i in range(beta + 1):
                 ref_dir[depth] = 1.0 * i / (1.0 * n_partitions)
-                self.__uniform_reference_directions(ref_dirs, np.copy(ref_dir), n_partitions, beta - i,
-                                                    depth + 1)
+                self.__uniform_reference_directions(ref_dirs, np.copy(ref_dir), n_partitions, beta - i, depth + 1)
 
     @staticmethod
     def get_partition_closest_to_points(n_points, n_dim):
         # in this case the do method will always return one values anyway
         if n_dim == 1:
             return 0
 
@@ -96,15 +93,15 @@
 
     @staticmethod
     def get_n_points(n_partitions, n_dim):
         return int(special.binom(n_dim + n_partitions - 1, n_partitions))
 
 
 def get_extreme_points(F, n_objs, ideal_point, extreme_points=None):
-    """ Calculate the Achievement Scalarization Function which is used for the extreme point decomposition. """
+    """Calculate the Achievement Scalarization Function which is used for the extreme point decomposition."""
     asf = np.eye(n_objs)
     asf[asf == 0] = 1e6
 
     # add the old extreme points to never loose them for normalization
     _F = F
     if extreme_points is not None:
         _F = np.concatenate([extreme_points, _F], axis=0)
@@ -118,15 +115,15 @@
     idx = np.argmin(F_asf, axis=1)
     extreme_points = _F[idx, :]
 
     return extreme_points
 
 
 def get_nadir_point(extreme_points, ideal_point, worst_point, worst_of_front, worst_of_population):
-    """ Calculate the axis intersects for a set of individuals and its extremes (construct hyperplane). """
+    """Calculate the axis intersects for a set of individuals and its extremes (construct hyperplane)."""
     try:
         # find the intercepts using gaussian elimination
         M = extreme_points - ideal_point
         b = np.ones(extreme_points.shape[1])
         plane = np.linalg.solve(M, b)
         intercepts = 1 / plane
 
@@ -177,25 +174,25 @@
             else:
                 # already randomized through shuffling
                 next_ind = next_ind[0]
                 is_closest = False
 
             # add the selected individual to the survivors
             mask[next_ind] = False
-            pop[next_ind].attributes['is_closest'] = is_closest
+            pop[next_ind].attributes["is_closest"] = is_closest
             survivors.append(int(next_ind))
 
             # increase the corresponding niche count
             niche_count[next_niche] += 1
 
     return survivors
 
 
 def associate_to_niches(F, niches, ideal_point, nadir_point, utopian_epsilon: float = 0.0):
-    """ Associate each solution to a reference point. """
+    """Associate each solution to a reference point."""
     utopian_point = ideal_point - utopian_epsilon
 
     denom = nadir_point - utopian_point
     denom[denom == 0] = 1e-12
 
     # normalize by ideal point and intercepts
     N = (F - utopian_point) / denom
@@ -226,54 +223,55 @@
     index, count = np.unique(niche_of_individuals, return_counts=True)
     niche_count[index] = count
 
     return niche_count
 
 
 class NSGAIII(NSGAII):
-
-    def __init__(self,
-                 reference_directions,
-                 problem: Problem,
-                 mutation: Mutation,
-                 crossover: Crossover,
-                 population_size: int = None,
-                 selection: Selection = BinaryTournamentSelection(
-                     MultiComparator([FastNonDominatedRanking.get_comparator(),
-                                      CrowdingDistance.get_comparator()])),
-                 termination_criterion: TerminationCriterion = store.default_termination_criteria,
-                 population_generator: Generator = store.default_generator,
-                 population_evaluator: Evaluator = store.default_evaluator,
-                 dominance_comparator: Comparator = store.default_comparator):
+    def __init__(
+        self,
+        reference_directions,
+        problem: Problem,
+        mutation: Mutation,
+        crossover: Crossover,
+        population_size: int = None,
+        selection: Selection = BinaryTournamentSelection(
+            MultiComparator([FastNonDominatedRanking.get_comparator(), CrowdingDistance.get_comparator()])
+        ),
+        termination_criterion: TerminationCriterion = store.default_termination_criteria,
+        population_generator: Generator = store.default_generator,
+        population_evaluator: Evaluator = store.default_evaluator,
+        dominance_comparator: Comparator = store.default_comparator,
+    ):
         self.reference_directions = reference_directions.compute()
 
         if not population_size:
             population_size = len(self.reference_directions)
-        if self.reference_directions.shape[1] != problem.number_of_objectives:
-            raise Exception('Dimensionality of reference points must be equal to the number of objectives')
+        if self.reference_directions.shape[1] != problem.number_of_objectives():
+            raise Exception("Dimensionality of reference points must be equal to the number of objectives")
 
         super(NSGAIII, self).__init__(
             problem=problem,
             population_size=population_size,
             offspring_population_size=population_size,
             mutation=mutation,
             crossover=crossover,
             selection=selection,
             termination_criterion=termination_criterion,
             population_evaluator=population_evaluator,
             population_generator=population_generator,
-            dominance_comparator=dominance_comparator
+            dominance_comparator=dominance_comparator,
         )
 
         self.extreme_points = None
-        self.ideal_point = np.full(self.problem.number_of_objectives, np.inf)
-        self.worst_point = np.full(self.problem.number_of_objectives, -np.inf)
+        self.ideal_point = np.full(self.problem.number_of_objectives(), np.inf)
+        self.worst_point = np.full(self.problem.number_of_objectives(), -np.inf)
 
     def replacement(self, population: List[S], offspring_population: List[S]) -> List[S]:
-        """ Implements NSGA-III environmental selection based on reference points as described in:
+        """Implements NSGA-III environmental selection based on reference points as described in:
 
         * Deb, K., & Jain, H. (2014). An Evolutionary Many-Objective Optimization
           Algorithm Using Reference-Point-Based Nondominated Sorting Approach,
           Part I: Solving Problems With Box Constraints. IEEE Transactions on
           Evolutionary Computation, 18(4), 577–601. doi:10.1109/TEVC.2013.2281535.
         """
         F = np.array([s.objectives for s in population])
@@ -286,74 +284,80 @@
         # calculate the fronts of the population
         ranking = FastNonDominatedRanking(self.dominance_comparator)
         ranking.compute_ranking(population + offspring_population, k=self.population_size)
 
         fronts, non_dominated = ranking.ranked_sublists, ranking.get_subfront(0)
 
         # find the extreme points for normalization
-        self.extreme_points = get_extreme_points(F=np.array([s.objectives for s in non_dominated]),
-                                                 n_objs=self.problem.number_of_objectives,
-                                                 ideal_point=self.ideal_point,
-                                                 extreme_points=self.extreme_points)
+        self.extreme_points = get_extreme_points(
+            F=np.array([s.objectives for s in non_dominated]),
+            n_objs=self.problem.number_of_objectives(),
+            ideal_point=self.ideal_point,
+            extreme_points=self.extreme_points,
+        )
 
         # find the intercepts for normalization and do backup if gaussian elimination fails
         worst_of_population = np.max(F, axis=0)
         worst_of_front = np.max(np.array([s.objectives for s in non_dominated]), axis=0)
 
-        nadir_point = get_nadir_point(extreme_points=self.extreme_points,
-                                      ideal_point=self.ideal_point,
-                                      worst_point=self.worst_point,
-                                      worst_of_population=worst_of_population,
-                                      worst_of_front=worst_of_front)
+        nadir_point = get_nadir_point(
+            extreme_points=self.extreme_points,
+            ideal_point=self.ideal_point,
+            worst_point=self.worst_point,
+            worst_of_population=worst_of_population,
+            worst_of_front=worst_of_front,
+        )
 
         #  consider only the population until we come to the splitting front
         pop = np.concatenate(ranking.ranked_sublists)
         F = np.array([s.objectives for s in pop])
 
         # update the front indices for the current population
         counter = 0
         for i in range(len(fronts)):
             for j in range(len(fronts[i])):
                 fronts[i][j] = counter
                 counter += 1
         last_front = np.array(fronts[-1])
 
         # associate individuals to niches
-        niche_of_individuals, dist_to_niche = associate_to_niches(F=F,
-                                                                  niches=self.reference_directions,
-                                                                  ideal_point=self.ideal_point,
-                                                                  nadir_point=nadir_point)
+        niche_of_individuals, dist_to_niche = associate_to_niches(
+            F=F, niches=self.reference_directions, ideal_point=self.ideal_point, nadir_point=nadir_point
+        )
 
         # if we need to select individuals to survive
         if len(pop) > self.population_size:
             # if there is only one front
             if len(fronts) == 1:
                 until_last_front = np.array([], dtype=np.int)
                 niche_count = np.zeros(len(self.reference_directions), dtype=np.int)
                 n_remaining = self.population_size
             # if some individuals already survived
             else:
                 until_last_front = np.concatenate(fronts[:-1])
-                niche_count = compute_niche_count(len(self.reference_directions),
-                                                  niche_of_individuals[until_last_front])
+                niche_count = compute_niche_count(
+                    len(self.reference_directions), niche_of_individuals[until_last_front]
+                )
                 n_remaining = self.population_size - len(until_last_front)
 
-            S_idx = niching(pop=pop[last_front],
-                            n_remaining=n_remaining,
-                            niche_count=niche_count,
-                            niche_of_individuals=niche_of_individuals[last_front],
-                            dist_to_niche=dist_to_niche[last_front])
+            S_idx = niching(
+                pop=pop[last_front],
+                n_remaining=n_remaining,
+                niche_count=niche_count,
+                niche_of_individuals=niche_of_individuals[last_front],
+                dist_to_niche=dist_to_niche[last_front],
+            )
 
             survivors_idx = np.concatenate((until_last_front, last_front[S_idx].tolist()))
             pop = pop[survivors_idx]
 
         return list(pop)
 
     def get_result(self):
-        """ Return only non dominated solutions."""
+        """Return only non dominated solutions."""
         ranking = FastNonDominatedRanking(self.dominance_comparator)
         ranking.compute_ranking(self.solutions, k=self.population_size)
 
         return ranking.get_subfront(0)
 
     def get_name(self) -> str:
-        return 'NSGAIII'
+        return "NSGAIII"
```

### Comparing `jmetalpy-1.5.5/jmetal/algorithm/multiobjective/omopso.py` & `jmetalpy-1.6.0/jmetal/algorithm/multiobjective/omopso.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import random
 from copy import copy
-from math import sqrt
-from typing import TypeVar, List, Optional
+from typing import List, Optional, TypeVar
 
 import numpy
 
 from jmetal.config import store
 from jmetal.core.algorithm import ParticleSwarmOptimization
 from jmetal.core.problem import FloatProblem
 from jmetal.core.solution import FloatSolution
@@ -13,52 +12,51 @@
 from jmetal.operator.mutation import NonUniformMutation
 from jmetal.util.archive import BoundedArchive, NonDominatedSolutionsArchive
 from jmetal.util.comparator import DominanceComparator, EpsilonDominanceComparator
 from jmetal.util.evaluator import Evaluator
 from jmetal.util.generator import Generator
 from jmetal.util.termination_criterion import TerminationCriterion
 
-R = TypeVar('R')
+R = TypeVar("R")
 
 """
 .. module:: OMOPSO
    :platform: Unix, Windows
    :synopsis: Implementation of SMPSO.
 
 .. moduleauthor:: Antonio J. Nebro <antonio@lcc.uma.es>
 """
 
 
 class OMOPSO(ParticleSwarmOptimization):
-
-    def __init__(self,
-                 problem: FloatProblem,
-                 swarm_size: int,
-                 uniform_mutation: UniformMutation,
-                 non_uniform_mutation: NonUniformMutation,
-                 leaders: Optional[BoundedArchive],
-                 epsilon: float,
-                 termination_criterion: TerminationCriterion,
-                 swarm_generator: Generator = store.default_generator,
-                 swarm_evaluator: Evaluator = store.default_evaluator):
-        """ This class implements the OMOPSO algorithm as described in
+    def __init__(
+        self,
+        problem: FloatProblem,
+        swarm_size: int,
+        uniform_mutation: UniformMutation,
+        non_uniform_mutation: NonUniformMutation,
+        leaders: Optional[BoundedArchive],
+        epsilon: float,
+        termination_criterion: TerminationCriterion,
+        swarm_generator: Generator = store.default_generator,
+        swarm_evaluator: Evaluator = store.default_evaluator,
+    ):
+        """This class implements the OMOPSO algorithm as described in
 
         todo Update this reference
         * SMPSO: A new PSO-based metaheuristic for multi-objective optimization
 
         The implementation of OMOPSO provided in jMetalPy follows the algorithm template described in the algorithm
         templates section of the documentation.
 
         :param problem: The problem to solve.
         :param swarm_size: Size of the swarm.
         :param leaders: Archive for leaders.
         """
-        super(OMOPSO, self).__init__(
-            problem=problem,
-            swarm_size=swarm_size)
+        super(OMOPSO, self).__init__(problem=problem, swarm_size=swarm_size)
         self.swarm_generator = swarm_generator
         self.swarm_evaluator = swarm_evaluator
 
         self.termination_criterion = termination_criterion
         self.observable.register(termination_criterion)
 
         self.uniform_mutation = uniform_mutation
@@ -80,15 +78,15 @@
         self.weight_min = 0.1
         self.weight_max = 0.5
         self.change_velocity1 = -1
         self.change_velocity2 = -1
 
         self.dominance_comparator = DominanceComparator()
 
-        self.speed = numpy.zeros((self.swarm_size, self.problem.number_of_variables), dtype=float)
+        self.speed = numpy.zeros((self.swarm_size, self.problem.number_of_variables()), dtype=float)
 
     def create_initial_solutions(self) -> List[FloatSolution]:
         return [self.swarm_generator.new(self.problem) for _ in range(self.swarm_size)]
 
     def evaluate(self, solution_list: List[FloatSolution]):
         return self.swarm_evaluator.evaluate(solution_list, self.problem)
 
@@ -98,36 +96,38 @@
     def initialize_global_best(self, swarm: List[FloatSolution]) -> None:
         for particle in swarm:
             if self.leaders.add(particle):
                 self.epsilon_archive.add(copy(particle))
 
     def initialize_particle_best(self, swarm: List[FloatSolution]) -> None:
         for particle in swarm:
-            particle.attributes['local_best'] = copy(particle)
+            particle.attributes["local_best"] = copy(particle)
 
     def initialize_velocity(self, swarm: List[FloatSolution]) -> None:
         for i in range(self.swarm_size):
-            for j in range(self.problem.number_of_variables):
+            for j in range(self.problem.number_of_variables()):
                 self.speed[i][j] = 0.0
 
     def update_velocity(self, swarm: List[FloatSolution]) -> None:
         for i in range(self.swarm_size):
-            best_particle = copy(swarm[i].attributes['local_best'])
+            best_particle = copy(swarm[i].attributes["local_best"])
             best_global = self.select_global_best()
 
             r1 = round(random.uniform(self.r1_min, self.r1_max), 1)
             r2 = round(random.uniform(self.r2_min, self.r2_max), 1)
             c1 = round(random.uniform(self.c1_min, self.c1_max), 1)
             c2 = round(random.uniform(self.c2_min, self.c2_max), 1)
             w = round(random.uniform(self.weight_min, self.weight_max), 1)
 
             for var in range(swarm[i].number_of_variables):
-                self.speed[i][var] = w * self.speed[i][var] \
-                                     + (c1 * r1 * (best_particle.variables[var] - swarm[i].variables[var])) \
-                                     + (c2 * r2 * (best_global.variables[var] - swarm[i].variables[var]))
+                self.speed[i][var] = (
+                    w * self.speed[i][var]
+                    + (c1 * r1 * (best_particle.variables[var] - swarm[i].variables[var]))
+                    + (c2 * r2 * (best_global.variables[var] - swarm[i].variables[var]))
+                )
 
     def update_position(self, swarm: List[FloatSolution]) -> None:
         for i in range(self.swarm_size):
             particle = swarm[i]
 
             for j in range(particle.number_of_variables):
                 particle.variables[j] += self.speed[i][j]
@@ -143,19 +143,17 @@
     def update_global_best(self, swarm: List[FloatSolution]) -> None:
         for particle in swarm:
             if self.leaders.add(copy(particle)):
                 self.epsilon_archive.add(copy(particle))
 
     def update_particle_best(self, swarm: List[FloatSolution]) -> None:
         for i in range(self.swarm_size):
-            flag = self.dominance_comparator.compare(
-                swarm[i],
-                swarm[i].attributes['local_best'])
+            flag = self.dominance_comparator.compare(swarm[i], swarm[i].attributes["local_best"])
             if flag != 1:
-                swarm[i].attributes['local_best'] = copy(swarm[i])
+                swarm[i].attributes["local_best"] = copy(swarm[i])
 
     def perturbation(self, swarm: List[FloatSolution]) -> None:
         self.non_uniform_mutation.set_current_iteration(self.evaluations / self.swarm_size)
         for i in range(self.swarm_size):
             if (i % 3) == 0:
                 self.non_uniform_mutation.execute(swarm[i])
             else:
@@ -172,49 +170,28 @@
             else:
                 best_global = copy(particles[1])
         else:
             best_global = copy(self.leaders.solution_list[0])
 
         return best_global
 
-    def __velocity_constriction(self, value: float, delta_max: [], delta_min: [], variable_index: int) -> float:
-        result = value
-        if value > delta_max[variable_index]:
-            result = delta_max[variable_index]
-        if value < delta_min[variable_index]:
-            result = delta_min[variable_index]
-
-        return result
-
-    def __inertia_weight(self, wmax: float):
-        return wmax
-
-    def __constriction_coefficient(self, c1: float, c2: float) -> float:
-        rho = c1 + c2
-        if rho <= 4:
-            result = 1.0
-        else:
-            result = 2.0 / (2.0 - rho - sqrt(pow(rho, 2.0) - 4.0 * rho))
-
-        return result
-
     def init_progress(self) -> None:
         self.evaluations = self.swarm_size
         self.leaders.compute_density_estimator()
 
         self.initialize_velocity(self.solutions)
         self.initialize_particle_best(self.solutions)
         self.initialize_global_best(self.solutions)
 
     def update_progress(self) -> None:
         self.evaluations += self.swarm_size
         self.leaders.compute_density_estimator()
 
-        observable_data = self.get_observable_data()
-        observable_data['SOLUTIONS'] = self.epsilon_archive.solution_list
+        observable_data = self.observable_data()
+        observable_data["SOLUTIONS"] = self.epsilon_archive.solution_list
         self.observable.notify_all(**observable_data)
 
     def get_result(self) -> List[FloatSolution]:
         return self.epsilon_archive.solution_list
 
     def get_name(self) -> str:
-        return 'OMOPSO'
+        return "OMOPSO"
```

### Comparing `jmetalpy-1.5.5/jmetal/algorithm/multiobjective/random_search.py` & `jmetalpy-1.6.0/jmetal/algorithm/multiobjective/random_search.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,73 +1,76 @@
 import time
-from typing import TypeVar, List
+from typing import List, TypeVar
 
 from jmetal.config import store
 from jmetal.core.algorithm import Algorithm
 from jmetal.core.problem import Problem
 from jmetal.util.archive import NonDominatedSolutionsArchive
 from jmetal.util.termination_criterion import TerminationCriterion
 
-S = TypeVar('S')
-R = TypeVar('R')
+S = TypeVar("S")
+R = TypeVar("R")
 
 """
 .. module:: RamdomSearch
    :platform: Unix, Windows
    :synopsis: Simple random_search search algorithms.
 
 .. moduleauthor:: Antonio J. Nebro <antonio@lcc.uma.es>
 """
 
 
 class RandomSearch(Algorithm[S, R]):
-
-    def __init__(self,
-                 problem: Problem[S],
-                 termination_criterion: TerminationCriterion = store.default_termination_criteria):
+    def __init__(
+        self, problem: Problem[S], termination_criterion: TerminationCriterion = store.default_termination_criteria
+    ):
         super().__init__()
         self.problem = problem
         self.termination_criterion = termination_criterion
         self.observable.register(termination_criterion)
 
         self.archive = NonDominatedSolutionsArchive()
 
-    def get_observable_data(self) -> dict:
+    def observable_data(self) -> dict:
         ctime = time.time() - self.start_computing_time
-        return {'PROBLEM': self.problem, 'EVALUATIONS': self.evaluations, 'SOLUTIONS': self.get_result(),
-                'COMPUTING_TIME': ctime}
+        return {
+            "PROBLEM": self.problem,
+            "EVALUATIONS": self.evaluations,
+            "SOLUTIONS": self.get_result(),
+            "COMPUTING_TIME": ctime,
+        }
 
     def create_initial_solutions(self) -> List[S]:
         return [self.problem.create_solution()]
 
     def evaluate(self, solution_list: List[S]) -> List[S]:
         return [self.problem.evaluate(solution_list[0])]
 
     def init_progress(self) -> None:
         self.evaluations = 1
 
-        observable_data = self.get_observable_data()
+        observable_data = self.observable_data()
         self.observable.notify_all(**observable_data)
 
     def stopping_condition_is_met(self) -> bool:
         return self.termination_criterion.is_met
 
     def step(self) -> None:
         new_solution = self.problem.create_solution()
         self.problem.evaluate(new_solution)
         self.archive.add(new_solution)
 
     def update_progress(self) -> None:
         self.evaluations += 1
 
-        observable_data = self.get_observable_data()
+        observable_data = self.observable_data()
         self.observable.notify_all(**observable_data)
 
     def get_result(self) -> List[S]:
         return self.archive.solution_list
 
     def get_name(self) -> str:
-        return 'Random Search'
+        return "Random Search"
 
     @property
     def label(self) -> str:
-        return f'{self.get_name()}.{self.problem.get_name()}'
+        return f"{self.get_name()}.{self.problem.name()}"
```

### Comparing `jmetalpy-1.5.5/jmetal/algorithm/multiobjective/smpso.py` & `jmetalpy-1.6.0/jmetal/algorithm/multiobjective/smpso.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,64 +1,64 @@
 import random
 import threading
 from copy import copy
 from math import sqrt
-from typing import TypeVar, List, Optional
+from typing import List, Optional, TypeVar
 
 import numpy
 
 from jmetal.config import store
-from jmetal.core.algorithm import ParticleSwarmOptimization, DynamicAlgorithm
+from jmetal.core.algorithm import DynamicAlgorithm, ParticleSwarmOptimization
 from jmetal.core.operator import Mutation
-from jmetal.core.problem import FloatProblem, DynamicProblem
+from jmetal.core.problem import DynamicProblem, FloatProblem
 from jmetal.core.solution import FloatSolution
-from jmetal.util.archive import BoundedArchive, ArchiveWithReferencePoint
-from jmetal.util.comparator import DominanceComparator
+from jmetal.util.archive import ArchiveWithReferencePoint, BoundedArchive
+from jmetal.util.comparator import DominanceComparator, Comparator
 from jmetal.util.evaluator import Evaluator
 from jmetal.util.generator import Generator
 from jmetal.util.termination_criterion import TerminationCriterion
 
-R = TypeVar('R')
+R = TypeVar("R")
 
 """
 .. module:: SMPSO
    :platform: Unix, Windows
    :synopsis: Implementation of SMPSO.
 
 .. moduleauthor:: Antonio Benítez-Hidalgo <antonio.b@uma.es>
 """
 
 
 class SMPSO(ParticleSwarmOptimization):
-
-    def __init__(self,
-                 problem: FloatProblem,
-                 swarm_size: int,
-                 mutation: Mutation,
-                 leaders: Optional[BoundedArchive],
-                 termination_criterion: TerminationCriterion = store.default_termination_criteria,
-                 swarm_generator: Generator = store.default_generator,
-                 swarm_evaluator: Evaluator = store.default_evaluator):
-        """ This class implements the SMPSO algorithm as described in
+    def __init__(
+        self,
+        problem: FloatProblem,
+        swarm_size: int,
+        mutation: Mutation,
+        leaders: Optional[BoundedArchive],
+        dominance_comparator: Comparator = DominanceComparator(),
+        termination_criterion: TerminationCriterion = store.default_termination_criteria,
+        swarm_generator: Generator = store.default_generator,
+        swarm_evaluator: Evaluator = store.default_evaluator,
+    ):
+        """This class implements the SMPSO algorithm as described in
 
         * SMPSO: A new PSO-based metaheuristic for multi-objective optimization
         * MCDM 2009. DOI: `<http://dx.doi.org/10.1109/MCDM.2009.4938830/>`_.
 
         The implementation of SMPSO provided in jMetalPy follows the algorithm template described in the algorithm
         templates section of the documentation.
 
         :param problem: The problem to solve.
         :param swarm_size: Size of the swarm.
         :param max_evaluations: Maximum number of evaluations/iterations.
         :param mutation: Mutation operator (see :py:mod:`jmetal.operator.mutation`).
         :param leaders: Archive for leaders.
         """
-        super(SMPSO, self).__init__(
-            problem=problem,
-            swarm_size=swarm_size)
+        super(SMPSO, self).__init__(problem=problem, swarm_size=swarm_size)
         self.swarm_generator = swarm_generator
         self.swarm_evaluator = swarm_evaluator
         self.termination_criterion = termination_criterion
         self.observable.register(termination_criterion)
         self.mutation_operator = mutation
         self.leaders = leaders
 
@@ -71,19 +71,21 @@
         self.r2_min = 0.0
         self.r2_max = 1.0
         self.min_weight = 0.1
         self.max_weight = 0.1
         self.change_velocity1 = -1
         self.change_velocity2 = -1
 
-        self.dominance_comparator = DominanceComparator()
+        self.dominance_comparator = dominance_comparator
 
-        self.speed = numpy.zeros((self.swarm_size, self.problem.number_of_variables), dtype=float)
-        self.delta_max, self.delta_min = numpy.empty(problem.number_of_variables), \
-                                         numpy.empty(problem.number_of_variables)
+        self.speed = numpy.zeros((self.swarm_size, self.problem.number_of_variables()), dtype=float)
+        self.delta_max, self.delta_min = (
+            numpy.empty(problem.number_of_variables()),
+            numpy.empty(problem.number_of_variables()),
+        )
 
     def create_initial_solutions(self) -> List[FloatSolution]:
         return [self.swarm_generator.new(self.problem) for _ in range(self.swarm_size)]
 
     def evaluate(self, solution_list: List[FloatSolution]):
         return self.swarm_evaluator.evaluate(solution_list, self.problem)
 
@@ -92,44 +94,46 @@
 
     def initialize_global_best(self, swarm: List[FloatSolution]) -> None:
         for particle in swarm:
             self.leaders.add(copy(particle))
 
     def initialize_particle_best(self, swarm: List[FloatSolution]) -> None:
         for particle in swarm:
-            particle.attributes['local_best'] = copy(particle)
+            particle.attributes["local_best"] = copy(particle)
 
     def initialize_velocity(self, swarm: List[FloatSolution]) -> None:
-        for i in range(self.problem.number_of_variables):
+        for i in range(self.problem.number_of_variables()):
             self.delta_max[i] = (self.problem.upper_bound[i] - self.problem.lower_bound[i]) / 2.0
 
         self.delta_min = -1.0 * self.delta_max
 
     def update_velocity(self, swarm: List[FloatSolution]) -> None:
         for i in range(self.swarm_size):
-            best_particle = copy(swarm[i].attributes['local_best'])
+            best_particle = copy(swarm[i].attributes["local_best"])
             best_global = self.select_global_best()
 
             r1 = round(random.uniform(self.r1_min, self.r1_max), 1)
             r2 = round(random.uniform(self.r2_min, self.r2_max), 1)
             c1 = round(random.uniform(self.c1_min, self.c1_max), 1)
             c2 = round(random.uniform(self.c2_min, self.c2_max), 1)
             wmax = self.max_weight
             wmin = self.min_weight
 
             for var in range(swarm[i].number_of_variables):
-                self.speed[i][var] = \
-                    self.__velocity_constriction(
-                        self.__constriction_coefficient(c1, c2) *
-                        ((self.__inertia_weight(wmax)
-                          * self.speed[i][var])
-                         + (c1 * r1 * (best_particle.variables[var] - swarm[i].variables[var]))
-                         + (c2 * r2 * (best_global.variables[var] - swarm[i].variables[var]))
-                         ),
-                        self.delta_max, self.delta_min, var)
+                self.speed[i][var] = self.__velocity_constriction(
+                    self.__constriction_coefficient(c1, c2)
+                    * (
+                        (self.__inertia_weight(wmax) * self.speed[i][var])
+                        + (c1 * r1 * (best_particle.variables[var] - swarm[i].variables[var]))
+                        + (c2 * r2 * (best_global.variables[var] - swarm[i].variables[var]))
+                    ),
+                    self.delta_max,
+                    self.delta_min,
+                    var,
+                )
 
     def update_position(self, swarm: List[FloatSolution]) -> None:
         for i in range(self.swarm_size):
             particle = swarm[i]
 
             for j in range(particle.number_of_variables):
                 particle.variables[j] += self.speed[i][j]
@@ -144,19 +148,17 @@
 
     def update_global_best(self, swarm: List[FloatSolution]) -> None:
         for particle in swarm:
             self.leaders.add(copy(particle))
 
     def update_particle_best(self, swarm: List[FloatSolution]) -> None:
         for i in range(self.swarm_size):
-            flag = self.dominance_comparator.compare(
-                swarm[i],
-                swarm[i].attributes['local_best'])
+            flag = self.dominance_comparator.compare(swarm[i], swarm[i].attributes["local_best"])
             if flag != 1:
-                swarm[i].attributes['local_best'] = copy(swarm[i])
+                swarm[i].attributes["local_best"] = copy(swarm[i])
 
     def perturbation(self, swarm: List[FloatSolution]) -> None:
         for i in range(self.swarm_size):
             if (i % 6) == 0:
                 self.mutation_operator.execute(swarm[i])
 
     def select_global_best(self) -> FloatSolution:
@@ -203,43 +205,45 @@
         self.initialize_particle_best(self.solutions)
         self.initialize_global_best(self.solutions)
 
     def update_progress(self) -> None:
         self.evaluations += self.swarm_size
         self.leaders.compute_density_estimator()
 
-        observable_data = self.get_observable_data()
-        observable_data['SOLUTIONS'] = self.leaders.solution_list
+        observable_data = self.observable_data()
+        observable_data["SOLUTIONS"] = self.leaders.solution_list
         self.observable.notify_all(**observable_data)
 
     def get_result(self) -> List[FloatSolution]:
         return self.leaders.solution_list
 
     def get_name(self) -> str:
-        return 'SMPSO'
+        return "SMPSO"
 
 
 class DynamicSMPSO(SMPSO, DynamicAlgorithm):
-
-    def __init__(self,
-                 problem: DynamicProblem[FloatSolution],
-                 swarm_size: int,
-                 mutation: Mutation,
-                 leaders: BoundedArchive,
-                 termination_criterion: TerminationCriterion = store.default_termination_criteria,
-                 swarm_generator: Generator = store.default_generator,
-                 swarm_evaluator: Evaluator = store.default_evaluator):
+    def __init__(
+        self,
+        problem: DynamicProblem[FloatSolution],
+        swarm_size: int,
+        mutation: Mutation,
+        leaders: BoundedArchive,
+        termination_criterion: TerminationCriterion = store.default_termination_criteria,
+        swarm_generator: Generator = store.default_generator,
+        swarm_evaluator: Evaluator = store.default_evaluator,
+    ):
         super(DynamicSMPSO, self).__init__(
             problem=problem,
             swarm_size=swarm_size,
             mutation=mutation,
             leaders=leaders,
             termination_criterion=termination_criterion,
             swarm_generator=swarm_generator,
-            swarm_evaluator=swarm_evaluator)
+            swarm_evaluator=swarm_evaluator,
+        )
         self.completed_iterations = 0
 
     def restart(self) -> None:
         self.solutions = self.create_initial_solutions()
         self.solutions = self.evaluate(self.solutions)
 
         self.leaders.__init__(self.leaders.maximum_size)
@@ -251,58 +255,60 @@
         self.init_progress()
 
     def update_progress(self):
         if self.problem.the_problem_has_changed():
             self.restart()
             self.problem.clear_changed()
 
-        observable_data = self.get_observable_data()
+        observable_data = self.observable_data()
         self.observable.notify_all(**observable_data)
 
         self.evaluations += self.swarm_size
         self.leaders.compute_density_estimator()
 
     def stopping_condition_is_met(self):
         if self.termination_criterion.is_met:
-            observable_data = self.get_observable_data()
-            observable_data['termination_criterion_is_met'] = True
+            observable_data = self.observable_data()
+            observable_data["termination_criterion_is_met"] = True
             self.observable.notify_all(**observable_data)
 
             self.restart()
             self.init_progress()
             self.completed_iterations += 1
 
 
 class SMPSORP(SMPSO):
-
-    def __init__(self,
-                 problem: FloatProblem,
-                 swarm_size: int,
-                 mutation: Mutation,
-                 reference_points: List[List[float]],
-                 leaders: List[ArchiveWithReferencePoint],
-                 termination_criterion: TerminationCriterion,
-                 swarm_generator: Generator = store.default_generator,
-                 swarm_evaluator: Evaluator = store.default_evaluator):
-        """ This class implements the SMPSORP algorithm.
+    def __init__(
+        self,
+        problem: FloatProblem,
+        swarm_size: int,
+        mutation: Mutation,
+        reference_points: List[List[float]],
+        leaders: List[ArchiveWithReferencePoint],
+        termination_criterion: TerminationCriterion,
+        swarm_generator: Generator = store.default_generator,
+        swarm_evaluator: Evaluator = store.default_evaluator,
+    ):
+        """This class implements the SMPSORP algorithm.
 
         :param problem: The problem to solve.
         :param swarm_size:
         :param mutation:
         :param leaders: List of bounded archives.
         :param swarm_evaluator: An evaluator object to evaluate the solutions in the population.
         """
         super(SMPSORP, self).__init__(
             problem=problem,
             swarm_size=swarm_size,
             mutation=mutation,
             leaders=None,
             swarm_generator=swarm_generator,
             swarm_evaluator=swarm_evaluator,
-            termination_criterion=termination_criterion)
+            termination_criterion=termination_criterion,
+        )
         self.leaders = leaders
         self.reference_points = reference_points
         self.lock = threading.Lock()
 
         thread = threading.Thread(target=_change_reference_point, args=(self,))
         thread.start()
 
@@ -352,16 +358,16 @@
     def update_progress(self) -> None:
         self.evaluations += self.swarm_size
 
         for leader in self.leaders:
             leader.filter()
             leader.compute_density_estimator()
 
-        observable_data = self.get_observable_data()
-        observable_data['REFERENCE_POINT'] = self.get_reference_point()
+        observable_data = self.observable_data()
+        observable_data["REFERENCE_POINT"] = self.get_reference_point()
         self.observable.notify_all(**observable_data)
 
     def update_reference_point(self, new_reference_points: list):
         with self.lock:
             self.reference_points = new_reference_points
 
             for index, archive in enumerate(self.leaders):
@@ -377,26 +383,25 @@
         for leader in self.leaders:
             for solution in leader.solution_list:
                 result.append(solution)
 
         return result
 
     def get_name(self) -> str:
-        return 'SMPSO/RP'
+        return "SMPSO/RP"
 
 
 def _change_reference_point(algorithm: SMPSORP):
-    """ Auxiliar function to read new reference points from the keyboard for the SMPSO/RP algorithm
-    """
+    """Auxiliar function to read new reference points from the keyboard for the SMPSO/RP algorithm"""
     number_of_reference_points = len(algorithm.reference_points)
     number_of_objectives = algorithm.problem.number_of_objectives
 
     while True:
-        print(f'Enter {number_of_reference_points}-points of dimension {number_of_objectives}: ')
+        print(f"Enter {number_of_reference_points}-points of dimension {number_of_objectives}: ")
         read = [float(x) for x in input().split()]
 
         # Update reference points
         reference_points = []
         for i in range(0, len(read), number_of_objectives):
-            reference_points.append(read[i:i + number_of_objectives])
+            reference_points.append(read[i : i + number_of_objectives])
 
         algorithm.update_reference_point(reference_points)
```

### Comparing `jmetalpy-1.5.5/jmetal/algorithm/multiobjective/spea2.py` & `jmetalpy-1.6.0/jmetal/algorithm/multiobjective/spea2.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,27 @@
-from typing import TypeVar, List
+from typing import List, TypeVar
 
 from jmetal.algorithm.singleobjective.genetic_algorithm import GeneticAlgorithm
 from jmetal.config import store
-from jmetal.core.operator import Mutation, Crossover
+from jmetal.core.operator import Crossover, Mutation
 from jmetal.core.problem import Problem
 from jmetal.operator import BinaryTournamentSelection
 from jmetal.util.comparator import Comparator, MultiComparator
 from jmetal.util.density_estimator import KNearestNeighborDensityEstimator
 from jmetal.util.evaluator import Evaluator
 from jmetal.util.generator import Generator
 from jmetal.util.ranking import StrengthRanking
-from jmetal.util.replacement import RankingAndDensityEstimatorReplacement, RemovalPolicyType
+from jmetal.util.replacement import (
+    RankingAndDensityEstimatorReplacement,
+    RemovalPolicyType,
+)
 from jmetal.util.termination_criterion import TerminationCriterion
 
-S = TypeVar('S')
-R = TypeVar('R')
+S = TypeVar("S")
+R = TypeVar("R")
 
 """
 .. module:: SPEA2
    :platform: Unix, Windows
    :synopsis: SPEA2  implementation. Note that we do not follow the structure of the original SPEA2 code. We consider
    SPEA2 as a genetic algorithm with binary tournament selection, with a comparator based on the strength fitness and 
    the KNN distance, and a sequential replacement strategy based in iteratively (sequentially) 
@@ -29,50 +32,52 @@
    density estimator).
 
 .. moduleauthor:: Antonio J. Nebro <antonio@lcc.uma.es>
 """
 
 
 class SPEA2(GeneticAlgorithm[S, R]):
-
-    def __init__(self,
-                 problem: Problem,
-                 population_size: int,
-                 offspring_population_size: int,
-                 mutation: Mutation,
-                 crossover: Crossover,
-                 termination_criterion: TerminationCriterion = store.default_termination_criteria,
-                 population_generator: Generator = store.default_generator,
-                 population_evaluator: Evaluator = store.default_evaluator,
-                 dominance_comparator: Comparator = store.default_comparator):
+    def __init__(
+        self,
+        problem: Problem,
+        population_size: int,
+        offspring_population_size: int,
+        mutation: Mutation,
+        crossover: Crossover,
+        termination_criterion: TerminationCriterion = store.default_termination_criteria,
+        population_generator: Generator = store.default_generator,
+        population_evaluator: Evaluator = store.default_evaluator,
+        dominance_comparator: Comparator = store.default_comparator,
+    ):
         """
         :param problem: The problem to solve.
         :param population_size: Size of the population.
         :param mutation: Mutation operator (see :py:mod:`jmetal.operator.mutation`).
         :param crossover: Crossover operator (see :py:mod:`jmetal.operator.crossover`).
         """
-        multi_comparator = MultiComparator([StrengthRanking.get_comparator(),
-                                            KNearestNeighborDensityEstimator.get_comparator()])
+        multi_comparator = MultiComparator(
+            [StrengthRanking.get_comparator(), KNearestNeighborDensityEstimator.get_comparator()]
+        )
         selection = BinaryTournamentSelection(comparator=multi_comparator)
 
         super(SPEA2, self).__init__(
             problem=problem,
             population_size=population_size,
             offspring_population_size=offspring_population_size,
             mutation=mutation,
             crossover=crossover,
             selection=selection,
             termination_criterion=termination_criterion,
             population_evaluator=population_evaluator,
-            population_generator=population_generator
+            population_generator=population_generator,
         )
         self.dominance_comparator = dominance_comparator
 
     def replacement(self, population: List[S], offspring_population: List[S]) -> List[List[S]]:
-        """ This method joins the current and offspring populations to produce the population of the next generation
+        """This method joins the current and offspring populations to produce the population of the next generation
         by applying the ranking and crowding distance selection.
 
         :param population: Parent population.
         :param offspring_population: Offspring population.
         :return: New population after ranking and crowding distance selection is applied.
         """
         ranking = StrengthRanking(self.dominance_comparator)
@@ -83,8 +88,8 @@
 
         return solutions
 
     def get_result(self) -> R:
         return self.solutions
 
     def get_name(self) -> str:
-        return 'SPEA2'
+        return "SPEA2"
```

### Comparing `jmetalpy-1.5.5/jmetal/algorithm/singleobjective/evolution_strategy.py` & `jmetalpy-1.6.0/jmetal/algorithm/singleobjective/evolution_strategy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,60 +1,57 @@
 from copy import copy
-from typing import TypeVar, List
+from typing import List, TypeVar
 
 from jmetal.core.algorithm import EvolutionaryAlgorithm
 from jmetal.core.operator import Mutation
 from jmetal.core.problem import Problem
+from jmetal.util.constraint_handling import overall_constraint_violation_degree
 from jmetal.util.evaluator import Evaluator, SequentialEvaluator
 from jmetal.util.generator import Generator, RandomGenerator
 from jmetal.util.termination_criterion import TerminationCriterion
-from jmetal.util.constraint_handling import overall_constraint_violation_degree
 
-S = TypeVar('S')
-R = TypeVar('R')
+S = TypeVar("S")
+R = TypeVar("R")
 
 """
 .. module:: evolutionary_algorithm
    :platform: Unix, Windows
    :synopsis: Implementation of Evolutionary Algorithms.
 
 .. moduleauthor:: Antonio J. Nebro <antonio@lcc.uma.es>, Antonio Benítez-Hidalgo <antonio.b@uma.es>
 """
 
 
 class EvolutionStrategy(EvolutionaryAlgorithm[S, R]):
-
-    def __init__(self,
-                 problem: Problem,
-                 mu: int,
-                 lambda_: int,
-                 elitist: bool,
-                 mutation: Mutation,
-                 termination_criterion: TerminationCriterion,
-                 population_generator: Generator = RandomGenerator(),
-                 population_evaluator: Evaluator = SequentialEvaluator()):
-        super(EvolutionStrategy, self).__init__(
-            problem=problem,
-            population_size=mu,
-            offspring_population_size=lambda_)
+    def __init__(
+        self,
+        problem: Problem,
+        mu: int,
+        lambda_: int,
+        elitist: bool,
+        mutation: Mutation,
+        termination_criterion: TerminationCriterion,
+        population_generator: Generator = RandomGenerator(),
+        population_evaluator: Evaluator = SequentialEvaluator(),
+    ):
+        super(EvolutionStrategy, self).__init__(problem=problem, population_size=mu, offspring_population_size=lambda_)
         self.mu = mu
         self.lambda_ = lambda_
         self.elitist = elitist
 
         self.mutation_operator = mutation
 
         self.population_generator = population_generator
         self.population_evaluator = population_evaluator
 
         self.termination_criterion = termination_criterion
         self.observable.register(termination_criterion)
 
     def create_initial_solutions(self) -> List[S]:
-        return [self.population_generator.new(self.problem)
-                for _ in range(self.population_size)]
+        return [self.population_generator.new(self.problem) for _ in range(self.population_size)]
 
     def evaluate(self, solution_list: List[S]):
         return self.population_evaluator.evaluate(solution_list, self.problem)
 
     def stopping_condition_is_met(self) -> bool:
         return self.termination_criterion.is_met
 
@@ -87,8 +84,8 @@
 
         return new_population
 
     def get_result(self) -> R:
         return self.solutions[0]
 
     def get_name(self) -> str:
-        return 'Elitist evolution Strategy'
+        return "Elitist evolution Strategy"
```

### Comparing `jmetalpy-1.5.5/jmetal/algorithm/singleobjective/genetic_algorithm.py` & `jmetalpy-1.6.0/jmetal/algorithm/singleobjective/genetic_algorithm.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,85 +1,92 @@
-from typing import TypeVar, List
+from functools import cmp_to_key
+from typing import List, TypeVar
 
 from jmetal.config import store
 from jmetal.core.algorithm import EvolutionaryAlgorithm
-from jmetal.core.operator import Mutation, Crossover, Selection
+from jmetal.core.operator import Crossover, Mutation, Selection
 from jmetal.core.problem import Problem
+from jmetal.operator import BinaryTournamentSelection
+from jmetal.util.comparator import Comparator, ObjectiveComparator
 from jmetal.util.evaluator import Evaluator
 from jmetal.util.generator import Generator
 from jmetal.util.termination_criterion import TerminationCriterion
 
-S = TypeVar('S')
-R = TypeVar('R')
+S = TypeVar("S")
+R = TypeVar("R")
 
 """
 .. module:: genetic_algorithm
    :platform: Unix, Windows
    :synopsis: Implementation of Genetic Algorithms.
 .. moduleauthor:: Antonio J. Nebro <antonio@lcc.uma.es>, Antonio Benítez-Hidalgo <antonio.b@uma.es>
 """
 
 
 class GeneticAlgorithm(EvolutionaryAlgorithm[S, R]):
-
-    def __init__(self,
-                 problem: Problem,
-                 population_size: int,
-                 offspring_population_size: int,
-                 mutation: Mutation,
-                 crossover: Crossover,
-                 selection: Selection,
-                 termination_criterion: TerminationCriterion = store.default_termination_criteria,
-                 population_generator: Generator = store.default_generator,
-                 population_evaluator: Evaluator = store.default_evaluator):
+    def __init__(
+        self,
+        problem: Problem,
+        population_size: int,
+        offspring_population_size: int,
+        mutation: Mutation,
+        crossover: Crossover,
+        selection: Selection = BinaryTournamentSelection(ObjectiveComparator(0)),
+        termination_criterion: TerminationCriterion = store.default_termination_criteria,
+        population_generator: Generator = store.default_generator,
+        population_evaluator: Evaluator = store.default_evaluator,
+            solution_comparator: Comparator = ObjectiveComparator(0)
+    ):
         super(GeneticAlgorithm, self).__init__(
-            problem=problem,
-            population_size=population_size,
-            offspring_population_size=offspring_population_size)
+            problem=problem, population_size=population_size, offspring_population_size=offspring_population_size
+        )
         self.mutation_operator = mutation
         self.crossover_operator = crossover
+        self.solution_comparator = solution_comparator
+
         self.selection_operator = selection
 
         self.population_generator = population_generator
         self.population_evaluator = population_evaluator
 
         self.termination_criterion = termination_criterion
         self.observable.register(termination_criterion)
 
-        self.mating_pool_size = \
-            self.offspring_population_size * \
-            self.crossover_operator.get_number_of_parents() // self.crossover_operator.get_number_of_children()
+        self.mating_pool_size = (
+            self.offspring_population_size
+            * self.crossover_operator.get_number_of_parents()
+            // self.crossover_operator.get_number_of_children()
+        )
 
         if self.mating_pool_size < self.crossover_operator.get_number_of_children():
             self.mating_pool_size = self.crossover_operator.get_number_of_children()
 
     def create_initial_solutions(self) -> List[S]:
-        return [self.population_generator.new(self.problem)
-                for _ in range(self.population_size)]
+        return [self.population_generator.new(self.problem) for _ in range(self.population_size)]
 
     def evaluate(self, population: List[S]):
         return self.population_evaluator.evaluate(population, self.problem)
 
     def stopping_condition_is_met(self) -> bool:
         return self.termination_criterion.is_met
 
     def selection(self, population: List[S]):
         mating_population = []
 
-        for i in range(self.mating_pool_size):
+        for _ in range(self.mating_pool_size):
             solution = self.selection_operator.execute(population)
             mating_population.append(solution)
 
         return mating_population
 
     def reproduction(self, mating_population: List[S]) -> List[S]:
         number_of_parents_to_combine = self.crossover_operator.get_number_of_parents()
 
         if len(mating_population) % number_of_parents_to_combine != 0:
-            raise Exception('Wrong number of parents')
+            raise Exception("Wrong number of parents")
 
         offspring_population = []
         for i in range(0, self.offspring_population_size, number_of_parents_to_combine):
             parents = []
             for j in range(number_of_parents_to_combine):
                 parents.append(mating_population[i + j])
 
@@ -92,16 +99,16 @@
                     break
 
         return offspring_population
 
     def replacement(self, population: List[S], offspring_population: List[S]) -> List[S]:
         population.extend(offspring_population)
 
-        population.sort(key=lambda s: s.objectives[0])
+        population.sort(key=cmp_to_key(self.solution_comparator.compare))
 
-        return population[:self.population_size]
+        return population[: self.population_size]
 
     def get_result(self) -> R:
         return self.solutions[0]
 
     def get_name(self) -> str:
-        return 'Genetic algorithm'
+        return "Genetic algorithm"
```

### Comparing `jmetalpy-1.5.5/jmetal/algorithm/singleobjective/local_search.py` & `jmetalpy-1.6.0/jmetal/algorithm/singleobjective/local_search.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 import copy
 import random
 import threading
 import time
-from typing import TypeVar, List
+from typing import List, TypeVar
 
 from jmetal.config import store
 from jmetal.core.algorithm import Algorithm
 from jmetal.core.operator import Mutation
 from jmetal.core.problem import Problem
 from jmetal.core.solution import Solution
 from jmetal.util.comparator import Comparator
 from jmetal.util.termination_criterion import TerminationCriterion
 
-S = TypeVar('S')
-R = TypeVar('R')
+S = TypeVar("S")
+R = TypeVar("R")
 
 """
 .. module:: local_search
    :platform: Unix, Windows
    :synopsis: Implementation of Local search.
 
 .. moduleauthor:: Antonio J. Nebro <antonio@lcc.uma.es>, Antonio Benítez-Hidalgo <antonio.b@uma.es>
 """
 
 
 class LocalSearch(Algorithm[S, R], threading.Thread):
-
-    def __init__(self,
-                 problem: Problem[S],
-                 mutation: Mutation,
-                 termination_criterion: TerminationCriterion = store.default_termination_criteria,
-                 comparator: Comparator = store.default_comparator):
+    def __init__(
+        self,
+        problem: Problem[S],
+        mutation: Mutation,
+        termination_criterion: TerminationCriterion = store.default_termination_criteria,
+        comparator: Comparator = store.default_comparator,
+    ):
         super(LocalSearch, self).__init__()
         self.comparator = comparator
         self.problem = problem
         self.mutation = mutation
         self.termination_criterion = termination_criterion
         self.observable.register(termination_criterion)
 
@@ -64,20 +65,24 @@
         else:
             if random.random() < 0.5:
                 self.solutions[0] = mutated_solution
 
     def update_progress(self) -> None:
         self.evaluations += 1
 
-        observable_data = self.get_observable_data()
+        observable_data = self.observable_data()
         self.observable.notify_all(**observable_data)
 
-    def get_observable_data(self) -> dict:
+    def observable_data(self) -> dict:
         ctime = time.time() - self.start_computing_time
-        return {'PROBLEM': self.problem, 'EVALUATIONS': self.evaluations, 'SOLUTIONS': self.get_result(),
-                'COMPUTING_TIME': ctime}
+        return {
+            "PROBLEM": self.problem,
+            "EVALUATIONS": self.evaluations,
+            "SOLUTIONS": self.get_result(),
+            "COMPUTING_TIME": ctime,
+        }
 
     def get_result(self) -> R:
         return self.solutions[0]
 
     def get_name(self) -> str:
-        return 'LS'
+        return "LS"
```

### Comparing `jmetalpy-1.5.5/jmetal/algorithm/singleobjective/simulated_annealing.py` & `jmetalpy-1.6.0/jmetal/algorithm/singleobjective/simulated_annealing.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 import copy
 import random
 import threading
 import time
-from typing import TypeVar, List
+from typing import List, TypeVar
 
 import numpy
 
 from jmetal.config import store
 from jmetal.core.algorithm import Algorithm
 from jmetal.core.operator import Mutation
 from jmetal.core.problem import Problem
 from jmetal.core.solution import Solution
 from jmetal.util.generator import Generator
 from jmetal.util.termination_criterion import TerminationCriterion
 
-S = TypeVar('S')
-R = TypeVar('R')
+S = TypeVar("S")
+R = TypeVar("R")
 
 """
 .. module:: simulated_annealing
    :platform: Unix, Windows
    :synopsis: Implementation of Simulated Annealing.
 
 .. moduleauthor:: Antonio J. Nebro <antonio@lcc.uma.es>, Antonio Benítez-Hidalgo <antonio.b@uma.es>
 """
 
 
 class SimulatedAnnealing(Algorithm[S, R], threading.Thread):
-
-    def __init__(self,
-                 problem: Problem[S],
-                 mutation: Mutation,
-                 termination_criterion: TerminationCriterion,
-                 solution_generator: Generator = store.default_generator):
+    def __init__(
+        self,
+        problem: Problem[S],
+        mutation: Mutation,
+        termination_criterion: TerminationCriterion,
+        solution_generator: Generator = store.default_generator,
+    ):
         super(SimulatedAnnealing, self).__init__()
         self.problem = problem
         self.mutation = mutation
         self.termination_criterion = termination_criterion
         self.solution_generator = solution_generator
         self.observable.register(termination_criterion)
         self.temperature = 1.0
@@ -58,17 +59,16 @@
 
     def step(self) -> None:
         mutated_solution = copy.deepcopy(self.solutions[0])
         mutated_solution: Solution = self.mutation.execute(mutated_solution)
         mutated_solution = self.evaluate([mutated_solution])[0]
 
         acceptance_probability = self.compute_acceptance_probability(
-            self.solutions[0].objectives[0],
-            mutated_solution.objectives[0],
-            self.temperature)
+            self.solutions[0].objectives[0], mutated_solution.objectives[0], self.temperature
+        )
 
         if acceptance_probability > random.random():
             self.solutions[0] = mutated_solution
 
         self.temperature *= self.alpha
 
     def compute_acceptance_probability(self, current: float, new: float, temperature: float) -> float:
@@ -78,20 +78,24 @@
             t = temperature if temperature > self.minimum_temperature else self.minimum_temperature
             value = (new - current) / t
             return numpy.exp(-1.0 * value)
 
     def update_progress(self) -> None:
         self.evaluations += 1
 
-        observable_data = self.get_observable_data()
+        observable_data = self.observable_data()
         self.observable.notify_all(**observable_data)
 
-    def get_observable_data(self) -> dict:
+    def observable_data(self) -> dict:
         ctime = time.time() - self.start_computing_time
-        return {'PROBLEM': self.problem, 'EVALUATIONS': self.evaluations, 'SOLUTIONS': self.get_result(),
-                'COMPUTING_TIME': ctime}
+        return {
+            "PROBLEM": self.problem,
+            "EVALUATIONS": self.evaluations,
+            "SOLUTIONS": self.get_result(),
+            "COMPUTING_TIME": ctime,
+        }
 
     def get_result(self) -> R:
         return self.solutions[0]
 
     def get_name(self) -> str:
-        return 'Simulated Annealing'
+        return "Simulated Annealing"
```

### Comparing `jmetalpy-1.5.5/jmetal/algorithm/test/ittest_algorithm.py` & `jmetalpy-1.6.0/jmetal/algorithm/test/ittest_algorithm.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from jmetal.operator import PolynomialMutation, SBXCrossover
 from jmetal.problem import ZDT1
 from jmetal.util.archive import CrowdingDistanceArchive
 from jmetal.util.termination_criterion import StoppingByEvaluations
 
 
 class RunningAlgorithmsTestCases(unittest.TestCase):
-
     def setUp(self):
         self.problem = ZDT1()
         self.population_size = 100
         self.offspring_size = 100
         self.mating_pool_size = 100
         self.max_evaluations = 100
         self.mutation = PolynomialMutation(probability=1.0 / self.problem.number_of_variables, distribution_index=20)
@@ -23,41 +22,40 @@
     def test_NSGAII(self):
         NSGAII(
             problem=self.problem,
             population_size=self.population_size,
             offspring_population_size=self.offspring_size,
             mutation=self.mutation,
             crossover=self.crossover,
-            termination_criterion=StoppingByEvaluations(max_evaluations=1000)
+            termination_criterion=StoppingByEvaluations(max_evaluations=1000),
         ).run()
 
     def test_SMPSO(self):
         SMPSO(
             problem=self.problem,
             swarm_size=self.population_size,
             mutation=self.mutation,
             leaders=CrowdingDistanceArchive(100),
-            termination_criterion=StoppingByEvaluations(max_evaluations=1000)
+            termination_criterion=StoppingByEvaluations(max_evaluations=1000),
         ).run()
 
 
 class IntegrationTestCases(unittest.TestCase):
-
     def test_should_NSGAII_work_when_solving_problem_ZDT1_with_standard_settings(self):
         problem = ZDT1()
 
         max_evaluations = 25000
 
         algorithm = NSGAII(
             problem=problem,
             population_size=100,
             offspring_population_size=100,
             mutation=PolynomialMutation(probability=1.0 / problem.number_of_variables, distribution_index=20),
             crossover=SBXCrossover(probability=1.0, distribution_index=20),
-            termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations)
+            termination_criterion=StoppingByEvaluations(max_evaluations=max_evaluations),
         )
 
         algorithm.run()
         front = algorithm.get_result()
 
         hv = HyperVolume(reference_point=[1, 1])
         value = hv.compute([front[i].objectives for i in range(len(front))])
@@ -68,21 +66,21 @@
         problem = ZDT1()
 
         algorithm = SMPSO(
             problem=problem,
             swarm_size=100,
             mutation=PolynomialMutation(probability=1.0 / problem.number_of_variables, distribution_index=20),
             leaders=CrowdingDistanceArchive(100),
-            termination_criterion=StoppingByEvaluations(max_evaluations=25000)
+            termination_criterion=StoppingByEvaluations(max_evaluations=25000),
         )
 
         algorithm.run()
         front = algorithm.get_result()
 
         hv = HyperVolume(reference_point=[1, 1])
         value = hv.compute([front[i].objectives for i in range(len(front))])
 
         self.assertTrue(value >= 0.655)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `jmetalpy-1.5.5/jmetal/config.py` & `jmetalpy-1.6.0/jmetal/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from jmetal.operator import PolynomialMutation, BitFlipMutation
+from jmetal.core.observer import Observable
+from jmetal.operator import BitFlipMutation, PolynomialMutation
 from jmetal.util.comparator import DominanceComparator
-from jmetal.util.evaluator import SequentialEvaluator
+from jmetal.util.evaluator import Evaluator, SequentialEvaluator
 from jmetal.util.generator import RandomGenerator
 from jmetal.util.observable import DefaultObservable
 from jmetal.util.termination_criterion import StoppingByEvaluations
 
 
 class _Store:
-
     @property
-    def default_observable(self):
+    def default_observable(self) -> Observable:
         return DefaultObservable()
 
     @property
-    def default_evaluator(self):
+    def default_evaluator(self) -> Evaluator:
         return SequentialEvaluator()
 
     @property
     def default_generator(self):
         return RandomGenerator()
 
     @property
@@ -26,14 +26,11 @@
 
     @property
     def default_comparator(self):
         return DominanceComparator()
 
     @property
     def default_mutation(self):
-        return {
-            'real': PolynomialMutation(probability=0.15, distribution_index=20),
-            'binary': BitFlipMutation(0.15)
-        }
+        return {"real": PolynomialMutation(probability=0.15, distribution_index=20), "binary": BitFlipMutation(0.15)}
 
 
 store = _Store()
```

### Comparing `jmetalpy-1.5.5/jmetal/core/algorithm.py` & `jmetalpy-1.6.0/jmetal/core/algorithm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,172 +1,170 @@
-import logging
 import threading
 import time
-from abc import abstractmethod, ABC
-from typing import TypeVar, Generic, List
+from abc import ABC, abstractmethod
+from typing import Generic, List, TypeVar
 
 from jmetal.config import store
 from jmetal.core.problem import Problem
 from jmetal.core.solution import FloatSolution
+from jmetal.logger import get_logger
 
-LOGGER = logging.getLogger('jmetal')
+logger = get_logger(__name__)
 
-S = TypeVar('S')
-R = TypeVar('R')
+S = TypeVar("S")
+R = TypeVar("R")
 
 """
 .. module:: algorithm
    :platform: Unix, Windows
    :synopsis: Templates for algorithms.
 
 .. moduleauthor:: Antonio J. Nebro <antonio@lcc.uma.es>, Antonio Benítez-Hidalgo <antonio.b@uma.es>
 """
 
 
 class Algorithm(Generic[S, R], threading.Thread, ABC):
-
     def __init__(self):
         threading.Thread.__init__(self)
 
         self.solutions: List[S] = []
         self.evaluations = 0
         self.start_computing_time = 0
         self.total_computing_time = 0
 
         self.observable = store.default_observable
 
     @abstractmethod
     def create_initial_solutions(self) -> List[S]:
-        """ Creates the initial list of solutions of a metaheuristic. """
+        """Creates the initial list of solutions of a metaheuristic."""
         pass
 
     @abstractmethod
     def evaluate(self, solution_list: List[S]) -> List[S]:
-        """ Evaluates a solution list. """
+        """Evaluates a solution list."""
         pass
 
     @abstractmethod
     def init_progress(self) -> None:
-        """ Initialize the algorithm. """
+        """Initialize the algorithm."""
         pass
 
     @abstractmethod
     def stopping_condition_is_met(self) -> bool:
-        """ The stopping condition is met or not. """
+        """The stopping condition is met or not."""
         pass
 
     @abstractmethod
     def step(self) -> None:
-        """ Performs one iteration/step of the algorithm's loop. """
+        """Performs one iteration/step of the algorithm's loop."""
         pass
 
     @abstractmethod
     def update_progress(self) -> None:
-        """ Update the progress after each iteration. """
+        """Update the progress after each iteration."""
         pass
 
     @abstractmethod
-    def get_observable_data(self) -> dict:
-        """ Get observable data, with the information that will be send to all observers each time. """
+    def observable_data(self) -> dict:
+        """Get observable data, with the information that will be seng to all observers each time."""
         pass
 
     def run(self):
-        """ Execute the algorithm. """
+        """Execute the algorithm."""
         self.start_computing_time = time.time()
 
+        logger.debug("Creating initial set of solutions...")
         self.solutions = self.create_initial_solutions()
+
+        logger.debug("Evaluating solutions...")
         self.solutions = self.evaluate(self.solutions)
 
-        LOGGER.debug('Initializing progress')
+        logger.debug("Initializing progress...")
         self.init_progress()
 
-        LOGGER.debug('Running main loop until termination criteria is met')
+        logger.debug("Running main loop until termination criteria is met")
         while not self.stopping_condition_is_met():
             self.step()
             self.update_progress()
 
+        logger.debug("Finished!")
+
         self.total_computing_time = time.time() - self.start_computing_time
 
     @abstractmethod
     def get_result(self) -> R:
         pass
 
     @abstractmethod
     def get_name(self) -> str:
         pass
 
 
 class DynamicAlgorithm(Algorithm[S, R], ABC):
-
     @abstractmethod
     def restart(self) -> None:
         pass
 
 
 class EvolutionaryAlgorithm(Algorithm[S, R], ABC):
-
-    def __init__(self,
-                 problem: Problem[S],
-                 population_size: int,
-                 offspring_population_size: int):
+    def __init__(self, problem: Problem[S], population_size: int, offspring_population_size: int):
         super(EvolutionaryAlgorithm, self).__init__()
         self.problem = problem
         self.population_size = population_size
         self.offspring_population_size = offspring_population_size
 
     @abstractmethod
     def selection(self, population: List[S]) -> List[S]:
-        """ Select the best-fit individuals for reproduction (parents). """
+        """Select the best-fit individuals for reproduction (parents)."""
         pass
 
     @abstractmethod
     def reproduction(self, population: List[S]) -> List[S]:
-        """ Breed new individuals through crossover and mutation operations to give birth to offspring. """
+        """Breed new individuals through crossover and mutation operations to give birth to offspring."""
         pass
 
     @abstractmethod
     def replacement(self, population: List[S], offspring_population: List[S]) -> List[S]:
-        """ Replace least-fit population with new individuals. """
+        """Replace least-fit population with new individuals."""
         pass
 
-    def get_observable_data(self) -> dict:
-        return {'PROBLEM': self.problem,
-                'EVALUATIONS': self.evaluations,
-                'SOLUTIONS': self.get_result(),
-                'COMPUTING_TIME': time.time() - self.start_computing_time}
+    def observable_data(self) -> dict:
+        return {
+            "PROBLEM": self.problem,
+            "EVALUATIONS": self.evaluations,
+            "SOLUTIONS": self.get_result(),
+            "COMPUTING_TIME": time.time() - self.start_computing_time,
+        }
 
     def init_progress(self) -> None:
         self.evaluations = self.population_size
 
-        observable_data = self.get_observable_data()
+        observable_data = self.observable_data()
         self.observable.notify_all(**observable_data)
 
     def step(self):
         mating_population = self.selection(self.solutions)
         offspring_population = self.reproduction(mating_population)
         offspring_population = self.evaluate(offspring_population)
 
         self.solutions = self.replacement(self.solutions, offspring_population)
 
     def update_progress(self) -> None:
         self.evaluations += self.offspring_population_size
 
-        observable_data = self.get_observable_data()
+        observable_data = self.observable_data()
         self.observable.notify_all(**observable_data)
 
     @property
     def label(self) -> str:
-        return f'{self.get_name()}.{self.problem.get_name()}'
+        return f"{self.get_name()}.{self.problem.name()}"
 
 
 class ParticleSwarmOptimization(Algorithm[FloatSolution, List[FloatSolution]], ABC):
-
-    def __init__(self,
-                 problem: Problem[S],
-                 swarm_size: int):
+    def __init__(self, problem: Problem[S], swarm_size: int):
         super(ParticleSwarmOptimization, self).__init__()
         self.problem = problem
         self.swarm_size = swarm_size
 
     @abstractmethod
     def initialize_velocity(self, swarm: List[FloatSolution]) -> None:
         pass
@@ -195,40 +193,42 @@
     def update_position(self, swarm: List[FloatSolution]) -> None:
         pass
 
     @abstractmethod
     def perturbation(self, swarm: List[FloatSolution]) -> None:
         pass
 
-    def get_observable_data(self) -> dict:
-        return {'PROBLEM': self.problem,
-                'EVALUATIONS': self.evaluations,
-                'SOLUTIONS': self.get_result(),
-                'COMPUTING_TIME': time.time() - self.start_computing_time}
+    def observable_data(self) -> dict:
+        return {
+            "PROBLEM": self.problem,
+            "EVALUATIONS": self.evaluations,
+            "SOLUTIONS": self.get_result(),
+            "COMPUTING_TIME": time.time() - self.start_computing_time,
+        }
 
     def init_progress(self) -> None:
         self.evaluations = self.swarm_size
 
         self.initialize_velocity(self.solutions)
         self.initialize_particle_best(self.solutions)
         self.initialize_global_best(self.solutions)
 
-        observable_data = self.get_observable_data()
+        observable_data = self.observable_data()
         self.observable.notify_all(**observable_data)
 
     def step(self):
         self.update_velocity(self.solutions)
         self.update_position(self.solutions)
         self.perturbation(self.solutions)
         self.solutions = self.evaluate(self.solutions)
         self.update_global_best(self.solutions)
         self.update_particle_best(self.solutions)
 
     def update_progress(self) -> None:
         self.evaluations += self.swarm_size
 
-        observable_data = self.get_observable_data()
+        observable_data = self.observable_data()
         self.observable.notify_all(**observable_data)
 
     @property
     def label(self) -> str:
-        return f'{self.get_name()}.{self.problem.get_name()}'
+        return f"{self.get_name()}.{self.problem.name()}"
```

### Comparing `jmetalpy-1.5.5/jmetal/core/observer.py` & `jmetalpy-1.6.0/jmetal/core/observer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,26 @@
-from abc import abstractmethod, ABC
+from abc import ABC, abstractmethod
 
 """
 .. module:: Observable
    :platform: Unix, Windows
    :synopsis: Implementation of the observer-observable pattern.
 
 .. moduleauthor:: Antonio J. Nebro <antonio@lcc.uma.es>
 """
 
 
 class Observer(ABC):
-
     @abstractmethod
     def update(self, *args, **kwargs):
-        """ Update method.
-        """
+        """Update method."""
         pass
 
 
 class Observable(ABC):
-
     @abstractmethod
     def register(self, observer):
         pass
 
     @abstractmethod
     def deregister(self, observer):
         pass
@@ -31,9 +28,7 @@
     @abstractmethod
     def deregister_all(self):
         pass
 
     @abstractmethod
     def notify_all(self, *args, **kwargs):
         pass
-
-
```

### Comparing `jmetalpy-1.5.5/jmetal/core/operator.py` & `jmetalpy-1.6.0/jmetal/core/operator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,56 +1,59 @@
 from abc import ABC, abstractmethod
-from typing import TypeVar, Generic, List
+from typing import Generic, List, TypeVar
 
-S = TypeVar('S')
-R = TypeVar('R')
+from jmetal.core.solution import Solution
+
+S = TypeVar("S", bound=Solution)
+R = TypeVar("R", bound=Solution)
 
 """
 .. module:: Operator
    :platform: Unix, Windows
    :synopsis: Templates for operators.
 
 .. moduleauthor:: Antonio J. Nebro <antonio@lcc.uma.es>, Antonio Benítez-Hidalgo <antonio.b@uma.es>
 """
 
 
 class Operator(Generic[S, R], ABC):
-    """ Class representing operator """
+    """Class representing operator"""
 
     @abstractmethod
     def execute(self, source: S) -> R:
         pass
 
     @abstractmethod
     def get_name(self) -> str:
         pass
 
 
 def check_valid_probability_value(func):
     def func_wrapper(self, probability: float):
         if probability > 1.0:
-            raise Exception('The probability is greater than one: {}'.format(probability))
+            raise Exception("The probability is greater than one: {}".format(probability))
         elif probability < 0.0:
-            raise Exception('The probability is lower than zero: {}'.format(probability))
+            raise Exception("The probability is lower than zero: {}".format(probability))
 
         res = func(self, probability)
         return res
+
     return func_wrapper
 
 
 class Mutation(Operator[S, S], ABC):
-    """ Class representing mutation operator. """
+    """Class representing mutation operator."""
 
     @check_valid_probability_value
     def __init__(self, probability: float):
         self.probability = probability
 
 
 class Crossover(Operator[List[S], List[R]], ABC):
-    """ Class representing crossover operator. """
+    """Class representing crossover operator."""
 
     @check_valid_probability_value
     def __init__(self, probability: float):
         self.probability = probability
 
     @abstractmethod
     def get_number_of_parents(self) -> int:
@@ -58,11 +61,11 @@
 
     @abstractmethod
     def get_number_of_children(self) -> int:
         pass
 
 
 class Selection(Operator[S, R], ABC):
-    """ Class representing selection operator. """
+    """Class representing selection operator."""
 
     def __init__(self):
         pass
```

### Comparing `jmetalpy-1.5.5/jmetal/core/problem.py` & `jmetalpy-1.6.0/jmetal/core/problem.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,118 +1,134 @@
-import logging
 import random
 from abc import ABC, abstractmethod
-from typing import Generic, TypeVar, List
+from typing import Generic, List, TypeVar
 
 from jmetal.core.observer import Observer
-from jmetal.core.solution import BinarySolution, FloatSolution, IntegerSolution, PermutationSolution
+from jmetal.core.solution import (
+    BinarySolution,
+    FloatSolution,
+    IntegerSolution,
+    PermutationSolution,
+)
+from jmetal.logger import get_logger
 
-LOGGER = logging.getLogger('jmetal')
+logger = get_logger(__name__)
 
-S = TypeVar('S')
+S = TypeVar("S")
 
 
 class Problem(Generic[S], ABC):
-    """ Class representing problems. """
+    """Class representing problems."""
 
     MINIMIZE = -1
     MAXIMIZE = 1
 
     def __init__(self):
-        self.number_of_variables: int = 0
-        self.number_of_objectives: int = 0
-        self.number_of_constraints: int = 0
-
-        self.reference_front: List[S] = []
+        #self.reference_front: List[S] = []
 
         self.directions: List[int] = []
         self.labels: List[str] = []
 
     @abstractmethod
+    def number_of_variables(self) -> int:
+        pass
+
+    @abstractmethod
+    def number_of_objectives(self) -> int:
+        pass
+
+    @abstractmethod
+    def number_of_constraints(self) -> int:
+        pass
+
+    @abstractmethod
     def create_solution(self) -> S:
-        """ Creates a random_search solution to the problem.
+        """Creates a random_search solution to the problem.
 
-        :return: Solution. """
+        :return: Solution."""
         pass
 
     @abstractmethod
     def evaluate(self, solution: S) -> S:
-        """ Evaluate a solution. For any new problem inheriting from :class:`Problem`, this method should be
-        replaced. Note that this framework ASSUMES minimization, thus solutions must be evaluated in consequence.
+        """Evaluate a solution. For any new problem inheriting from :class:`Problem`, this method should be replaced.
+        Note that this framework ASSUMES minimization, thus solutions must be evaluated in consequence.
 
-        :return: Evaluated solution. """
+        :return: Evaluated solution."""
         pass
 
     @abstractmethod
-    def get_name(self) -> str:
+    def name(self) -> str:
         pass
 
 
 class DynamicProblem(Problem[S], Observer, ABC):
-
     @abstractmethod
     def the_problem_has_changed(self) -> bool:
         pass
 
     @abstractmethod
     def clear_changed(self) -> None:
         pass
 
 
 class BinaryProblem(Problem[BinarySolution], ABC):
-    """ Class representing binary problems. """
+    """Class representing binary problems."""
 
     def __init__(self):
         super(BinaryProblem, self).__init__()
 
 
 class FloatProblem(Problem[FloatSolution], ABC):
-    """ Class representing float problems. """
+    """Class representing float problems."""
 
     def __init__(self):
         super(FloatProblem, self).__init__()
         self.lower_bound = []
         self.upper_bound = []
 
+    def number_of_variables(self) -> int:
+        return len(self.lower_bound)
+
     def create_solution(self) -> FloatSolution:
         new_solution = FloatSolution(
-            self.lower_bound,
-            self.upper_bound,
-            self.number_of_objectives,
-            self.number_of_constraints)
-        new_solution.variables = \
-            [random.uniform(self.lower_bound[i] * 1.0, self.upper_bound[i] * 1.0) for i in
-             range(self.number_of_variables)]
+            self.lower_bound, self.upper_bound, self.number_of_objectives(), self.number_of_constraints()
+        )
+        new_solution.variables = [
+            random.uniform(self.lower_bound[i] * 1.0, self.upper_bound[i] * 1.0)
+            for i in range(self.number_of_variables())
+        ]
 
         return new_solution
 
 
 class IntegerProblem(Problem[IntegerSolution], ABC):
-    """ Class representing integer problems. """
+    """Class representing integer problems."""
 
     def __init__(self):
         super(IntegerProblem, self).__init__()
-        self.lower_bound = None
-        self.upper_bound = None
+        self.lower_bound = []
+        self.upper_bound = []
+
+    def number_of_variables(self) -> int:
+        return len(self.lower_bound)
 
     def create_solution(self) -> IntegerSolution:
         new_solution = IntegerSolution(
-            self.lower_bound,
-            self.upper_bound,
-            self.number_of_objectives,
-            self.number_of_constraints)
-        new_solution.variables = \
-            [int(random.uniform(self.lower_bound[i] * 1.0, self.upper_bound[i] * 1.0))
-             for i in range(self.number_of_variables)]
+            self.lower_bound, self.upper_bound, self.number_of_objectives(), self.number_of_constraints()
+        )
+        new_solution.variables = [
+            round(random.uniform(self.lower_bound[i] * 1.0, self.upper_bound[i] * 1.0))
+            for i in range(self.number_of_variables())
+        ]
 
         return new_solution
 
 
 class PermutationProblem(Problem[PermutationSolution], ABC):
-    """ Class representing permutation problems. """
+    """Class representing permutation problems."""
 
     def __init__(self):
         super(PermutationProblem, self).__init__()
 
 
 class OnTheFlyFloatProblem(FloatProblem):
     """ Class for defining float problems on the fly.
@@ -142,42 +158,45 @@
             .add_constraint(c2)
     """
 
     def __init__(self):
         super(OnTheFlyFloatProblem, self).__init__()
         self.functions = []
         self.constraints = []
-        self.name = None
+        self.problem_name = None
 
-    def set_name(self, name):
-        self.name = name
+    def set_name(self, name) -> "OnTheFlyFloatProblem":
+        self.problem_name = name
 
         return self
 
-    def add_function(self, function):
+    def add_function(self, function) -> "OnTheFlyFloatProblem":
         self.functions.append(function)
-        self.number_of_objectives += 1
 
         return self
 
-    def add_constraint(self, constraint):
+    def add_constraint(self, constraint) -> "OnTheFlyFloatProblem":
         self.constraints.append(constraint)
-        self.number_of_constraints += 1
 
         return self
 
-    def add_variable(self, lower_bound, upper_bound):
+    def add_variable(self, lower_bound, upper_bound) -> "OnTheFlyFloatProblem":
         self.lower_bound.append(lower_bound)
         self.upper_bound.append(upper_bound)
-        self.number_of_variables += 1
 
         return self
 
-    def evaluate(self, solution: FloatSolution):
-        for i in range(self.number_of_objectives):
+    def number_of_objectives(self) -> int:
+        return len(self.functions)
+
+    def number_of_constraints(self) -> int:
+        return len(self.constraints)
+
+    def evaluate(self, solution: FloatSolution) -> None:
+        for i in range(self.number_of_objectives()):
             solution.objectives[i] = self.functions[i](solution.variables)
 
-        for i in range(self.number_of_constraints):
+        for i in range(self.number_of_constraints()):
             solution.constraints[i] = self.constraints[i](solution.variables)
 
-    def get_name(self) -> str:
-        return self.name
+    def name(self) -> str:
+        return self.problem_name
```

### Comparing `jmetalpy-1.5.5/jmetal/core/quality_indicator.py` & `jmetalpy-1.6.0/jmetal/core/quality_indicator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from abc import ABC, abstractmethod
+from typing import Iterable
 
 import numpy as np
 from scipy import spatial
 
 
 class QualityIndicator(ABC):
-
     def __init__(self, is_minimization: bool):
         self.is_minimization = is_minimization
 
     @abstractmethod
     def compute(self, solutions: np.array):
         """
         :param solutions: [m, n] bi-dimensional numpy array, being m the number of solutions and n the dimension of
@@ -36,82 +36,81 @@
             mean = np.mean([s.objectives for s in solutions])
         else:
             mean = -np.mean([s.objectives for s in solutions])
 
         return mean
 
     def get_name(self) -> str:
-        return 'Fitness'
+        return "Fitness"
 
     def get_short_name(self) -> str:
-        return 'Fitness'
+        return "Fitness"
 
 
 class GenerationalDistance(QualityIndicator):
     def __init__(self, reference_front: np.array = None):
         """
         * Van Veldhuizen, D.A., Lamont, G.B.: Multiobjective Evolutionary Algorithm Research: A History and Analysis.
           Technical Report TR-98-03, Dept. Elec. Comput. Eng., Air Force. Inst. Technol. (1998)
         """
         super(GenerationalDistance, self).__init__(is_minimization=True)
         self.reference_front = reference_front
 
     def compute(self, solutions: np.array):
         if self.reference_front is None:
-            raise Exception('Reference front is none')
+            raise Exception("Reference front is none")
 
         distances = spatial.distance.cdist(solutions, self.reference_front)
 
         return np.mean(np.min(distances, axis=1))
 
     def get_short_name(self) -> str:
-        return 'GD'
+        return "GD"
 
     def get_name(self) -> str:
-        return 'Generational Distance'
+        return "Generational Distance"
 
 
 class InvertedGenerationalDistance(QualityIndicator):
     def __init__(self, reference_front: np.array = None):
         super(InvertedGenerationalDistance, self).__init__(is_minimization=True)
         self.reference_front = reference_front
 
     def compute(self, solutions: np.array):
         if self.reference_front is None:
-            raise Exception('Reference front is none')
+            raise Exception("Reference front is none")
 
         distances = spatial.distance.cdist(self.reference_front, solutions)
 
         return np.mean(np.min(distances, axis=1))
 
     def get_short_name(self) -> str:
-        return 'IGD'
+        return "IGD"
 
     def get_name(self) -> str:
-        return 'Inverted Generational Distance'
+        return "Inverted Generational Distance"
 
 
 class EpsilonIndicator(QualityIndicator):
     def __init__(self, reference_front: np.array = None):
         super(EpsilonIndicator, self).__init__(is_minimization=True)
         self.reference_front = reference_front
 
     def compute(self, front: np.array) -> float:
-        return max([min(
-            [max([s2[k] - s1[k] for k in range(len(s2))]) for s2 in front]) for s1 in self.reference_front])
+        return max([min([max([s2[k] - s1[k] for k in range(len(s2))]) for s2 in front]) for s1 in self.reference_front])
 
     def get_short_name(self) -> str:
-        return 'EP'
+        return "EP"
 
     def get_name(self) -> str:
         return "Additive Epsilon"
 
 
 class HyperVolume(QualityIndicator):
-    """ Hypervolume computation based on variant 3 of the algorithm in the paper:
+    """Hypervolume computation based on variant 3 of the algorithm in the paper:
 
     * C. M. Fonseca, L. Paquete, and M. Lopez-Ibanez. An improved dimension-sweep
       algorithm for the hypervolume indicator. In IEEE Congress on Evolutionary
       Computation, pages 1157-1163, Vancouver, Canada, July 2006.
 
     Minimization is implicitly assumed here!
     """
@@ -188,28 +187,30 @@
             q = p.prev[dim_index]
             while q.cargo is not None:
                 if q.ignore < dim_index:
                     q.ignore = 0
                 q = q.prev[dim_index]
             q = p.prev[dim_index]
             while length > 1 and (
-                    q.cargo[dim_index] > bounds[dim_index] or q.prev[dim_index].cargo[dim_index] >= bounds[dim_index]):
+                q.cargo[dim_index] > bounds[dim_index] or q.prev[dim_index].cargo[dim_index] >= bounds[dim_index]
+            ):
                 p = q
                 remove(p, dim_index, bounds)
                 q = p.prev[dim_index]
                 length -= 1
             q_area = q.area
             q_cargo = q.cargo
             q_prev_dim_index = q.prev[dim_index]
             if length > 1:
                 hvol = q_prev_dim_index.volume[dim_index] + q_prev_dim_index.area[dim_index] * (
-                        q_cargo[dim_index] - q_prev_dim_index.cargo[dim_index])
+                    q_cargo[dim_index] - q_prev_dim_index.cargo[dim_index]
+                )
             else:
                 q_area[0] = 1
-                q_area[1:dim_index + 1] = [q_area[i] * -q_cargo[i] for i in range(dim_index)]
+                q_area[1 : dim_index + 1] = [q_area[i] * -q_cargo[i] for i in range(dim_index)]
             q.volume[dim_index] = hvol
             if q.ignore >= dim_index:
                 q_area[dim_index] = q_prev_dim_index.area[dim_index]
             else:
                 q_area[dim_index] = hv_recursive(dim_index - 1, length, bounds)
                 if q_area[dim_index] <= q_prev_dim_index.area[dim_index]:
                     q.ignore = dim_index
@@ -247,43 +248,41 @@
         decorated = [(node.cargo[i], node) for node in nodes]
         # sort by this value
         decorated.sort(key=lambda n: n[0])
         # write back to original list
         nodes[:] = [node for (_, node) in decorated]
 
     def get_short_name(self) -> str:
-        return 'HV'
+        return "HV"
 
     def get_name(self) -> str:
         return "Hypervolume (Fonseca et al. implementation)"
 
 
 class MultiList:
     """A special front structure needed by FonsecaHyperVolume.
 
     It consists of several doubly linked lists that share common nodes. So,
     every node has multiple predecessors and successors, one in every list.
     """
 
     class Node:
-
         def __init__(self, number_lists, cargo=None):
             self.cargo = cargo
             self.next = [None] * number_lists
             self.prev = [None] * number_lists
             self.ignore = 0
             self.area = [0.0] * number_lists
             self.volume = [0.0] * number_lists
 
         def __str__(self):
             return str(self.cargo)
 
     def __init__(self, number_lists):
-        """ Builds 'numberLists' doubly linked lists.
-        """
+        """Builds 'numberLists' doubly linked lists."""
         self.number_lists = number_lists
         self.sentinel = MultiList.Node(number_lists)
         self.sentinel.next = [self.sentinel] * number_lists
         self.sentinel.prev = [self.sentinel] * number_lists
 
     def __str__(self):
         strings = []
@@ -310,47 +309,77 @@
         node = sentinel.next[i]
         while node != sentinel:
             length += 1
             node = node.next[i]
         return length
 
     def append(self, node, index):
-        """ Appends a node to the end of the list at the given index."""
+        """Appends a node to the end of the list at the given index."""
         last_but_one = self.sentinel.prev[index]
         node.next[index] = self.sentinel
         node.prev[index] = last_but_one
         # set the last element as the new one
         self.sentinel.prev[index] = node
         last_but_one.next[index] = node
 
     def extend(self, nodes, index):
-        """ Extends the list at the given index with the nodes."""
+        """Extends the list at the given index with the nodes."""
         sentinel = self.sentinel
         for node in nodes:
             last_but_one = sentinel.prev[index]
             node.next[index] = sentinel
             node.prev[index] = last_but_one
             # set the last element as the new one
             sentinel.prev[index] = node
             last_but_one.next[index] = node
 
     def remove(self, node, index, bounds):
-        """ Removes and returns 'node' from all lists in [0, 'index'[."""
+        """Removes and returns 'node' from all lists in [0, 'index'[."""
         for i in range(index):
             predecessor = node.prev[i]
             successor = node.next[i]
             predecessor.next[i] = successor
             successor.prev[i] = predecessor
             if bounds[i] > node.cargo[i]:
                 bounds[i] = node.cargo[i]
         return node
 
     def reinsert(self, node, index, bounds):
-        """ Inserts 'node' at the position it had in all lists in [0, 'index'[
+        """Inserts 'node' at the position it had in all lists in [0, 'index'[
         before it was removed. This method assumes that the next and previous
         nodes of the node that is reinserted are in the list.
         """
         for i in range(index):
             node.prev[i].next[i] = node
             node.next[i].prev[i] = node
             if bounds[i] > node.cargo[i]:
                 bounds[i] = node.cargo[i]
+
+
+class NormalizedHyperVolume(QualityIndicator):
+    """Implementation of the normalized hypervolume, which is calculated as follows:
+
+    relative hypervolume = 1 - (HV of the front / HV of the reference front).
+
+    Minimization is implicitly assumed here!
+    """
+
+    def __init__(self, reference_point: Iterable[float], reference_front: np.array):
+        """Delegates the computation of the HyperVolume to `jMetal.core.quality_indicator.HyperVolume`.
+
+        Fails if the HV of the reference front is zero."""
+        self.reference_point = reference_point
+        self._hv = HyperVolume(reference_point=reference_point)
+        self._reference_hypervolume = self._hv.compute(reference_front)
+
+        assert self._reference_hypervolume != 0, "Hypervolume of reference front is zero"
+
+    def compute(self, solutions: np.array) -> float:
+        hv = self._hv.compute(solutions=solutions)
+
+        return 1 - (hv / self._reference_hypervolume)
+
+    def get_short_name(self) -> str:
+        return "NHV"
+
+    def get_name(self) -> str:
+        return "Normalized Hypervolume"
```

### Comparing `jmetalpy-1.5.5/jmetal/core/solution.py` & `jmetalpy-1.6.0/jmetal/core/solution.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from abc import ABC
-from typing import List, Generic, TypeVar
+from typing import Generic, List, TypeVar
 
 from jmetal.util.ckecking import Check
 
 BitSet = List[bool]
-S = TypeVar('S')
+S = TypeVar("S")
 
 
 class Solution(Generic[S], ABC):
-    """ Class representing solutions """
+    """Class representing solutions"""
 
     def __init__(self, number_of_variables: int, number_of_objectives: int, number_of_constraints: int = 0):
         self.number_of_variables = number_of_variables
         self.number_of_objectives = number_of_objectives
         self.number_of_constraints = number_of_constraints
         self.variables = [[] for _ in range(self.number_of_variables)]
         self.objectives = [0.0 for _ in range(self.number_of_objectives)]
@@ -21,28 +21,27 @@
 
     def __eq__(self, solution) -> bool:
         if isinstance(solution, self.__class__):
             return self.variables == solution.variables
         return False
 
     def __str__(self) -> str:
-        return 'Solution(variables={},objectives={},constraints={})'.format(self.variables, self.objectives,
-                                                                            self.constraints)
+        return "Solution(variables={},objectives={},constraints={})".format(
+            self.variables, self.objectives, self.constraints
+        )
 
 
 class BinarySolution(Solution[BitSet]):
-    """ Class representing float solutions """
+    """Class representing float solutions"""
 
     def __init__(self, number_of_variables: int, number_of_objectives: int, number_of_constraints: int = 0):
         super(BinarySolution, self).__init__(number_of_variables, number_of_objectives, number_of_constraints)
 
     def __copy__(self):
-        new_solution = BinarySolution(
-            self.number_of_variables,
-            self.number_of_objectives)
+        new_solution = BinarySolution(self.number_of_variables, self.number_of_objectives)
         new_solution.objectives = self.objectives[:]
         new_solution.variables = self.variables[:]
 
         new_solution.attributes = self.attributes.copy()
 
         return new_solution
 
@@ -52,110 +51,115 @@
             total += len(var)
 
         return total
 
     def get_binary_string(self) -> str:
         string = ""
         for bit in self.variables[0]:
-            string += '1' if bit else '0'
+            string += "1" if bit else "0"
         return string
 
 
 class FloatSolution(Solution[float]):
-    """ Class representing float solutions """
+    """Class representing float solutions"""
 
-    def __init__(self, lower_bound: List[float], upper_bound: List[float], number_of_objectives: int,
-                 number_of_constraints: int = 0):
+    def __init__(
+        self,
+        lower_bound: List[float],
+        upper_bound: List[float],
+        number_of_objectives: int,
+        number_of_constraints: int = 0,
+    ):
         super(FloatSolution, self).__init__(len(lower_bound), number_of_objectives, number_of_constraints)
         self.lower_bound = lower_bound
         self.upper_bound = upper_bound
 
     def __copy__(self):
         new_solution = FloatSolution(
-            self.lower_bound,
-            self.upper_bound,
-            self.number_of_objectives,
-            self.number_of_constraints)
+            self.lower_bound, self.upper_bound, self.number_of_objectives, self.number_of_constraints
+        )
         new_solution.objectives = self.objectives[:]
         new_solution.variables = self.variables[:]
         new_solution.constraints = self.constraints[:]
 
         new_solution.attributes = self.attributes.copy()
 
         return new_solution
 
 
 class IntegerSolution(Solution[int]):
-    """ Class representing integer solutions """
+    """Class representing integer solutions"""
 
-    def __init__(self, lower_bound: List[int], upper_bound: List[int], number_of_objectives: int,
-                 number_of_constraints: int = 0):
+    def __init__(
+        self, lower_bound: List[int], upper_bound: List[int], number_of_objectives: int, number_of_constraints: int = 0
+    ):
         super(IntegerSolution, self).__init__(len(lower_bound), number_of_objectives, number_of_constraints)
         self.lower_bound = lower_bound
         self.upper_bound = upper_bound
 
     def __copy__(self):
         new_solution = IntegerSolution(
-            self.lower_bound,
-            self.upper_bound,
-            self.number_of_objectives,
-            self.number_of_constraints)
+            self.lower_bound, self.upper_bound, self.number_of_objectives, self.number_of_constraints
+        )
         new_solution.objectives = self.objectives[:]
         new_solution.variables = self.variables[:]
         new_solution.constraints = self.constraints[:]
 
         new_solution.attributes = self.attributes.copy()
 
         return new_solution
 
 
 class CompositeSolution(Solution):
-    """ Class representing solutions composed of a list of solutions. The idea is that each decision  variable can
+    """Class representing solutions composed of a list of solutions. The idea is that each decision  variable can
     be a solution of any type, so we can create mixed solutions (e.g., solutions combining any of the existing
     encodings). The adopted approach has the advantage of easing the reuse of existing variation operators, but all the
     solutions in the list will need to have the same function and constraint violation values.
 
     It is assumed that problems using instances of this class will properly manage the solutions it contains.
     """
 
     def __init__(self, solutions: List[Solution]):
-        super(CompositeSolution, self).__init__(len(solutions), solutions[0].number_of_objectives,
-                                                solutions[0].number_of_constraints)
+        super(CompositeSolution, self).__init__(
+            len(solutions), solutions[0].number_of_objectives, solutions[0].number_of_constraints
+        )
         Check.is_not_none(solutions)
         Check.collection_is_not_empty(solutions)
 
         for solution in solutions:
-            Check.that(solution.number_of_objectives == solutions[0].number_of_objectives,
-                       "The solutions in the list must have the same number of objectives: " + str(
-                           solutions[0].number_of_objectives))
-            Check.that(solution.number_of_constraints == solutions[0].number_of_constraints,
-                       "The solutions in the list must have the same number of constraints: " + str(
-                           solutions[0].number_of_constraints))
+            Check.that(
+                solution.number_of_objectives == solutions[0].number_of_objectives,
+                "The solutions in the list must have the same number of objectives: "
+                + str(solutions[0].number_of_objectives),
+            )
+            Check.that(
+                solution.number_of_constraints == solutions[0].number_of_constraints,
+                "The solutions in the list must have the same number of constraints: "
+                + str(solutions[0].number_of_constraints),
+            )
 
         self.variables = solutions
 
     def __copy__(self):
         new_solution = CompositeSolution(self.variables)
 
         new_solution.objectives = self.objectives[:]
         new_solution.constraints = self.constraints[:]
         new_solution.attributes = self.attributes.copy()
 
         return new_solution
 
 
 class PermutationSolution(Solution):
-    """ Class representing permutation solutions """
+    """Class representing permutation solutions"""
 
     def __init__(self, number_of_variables: int, number_of_objectives: int, number_of_constraints: int = 0):
         super(PermutationSolution, self).__init__(number_of_variables, number_of_objectives, number_of_constraints)
 
     def __copy__(self):
-        new_solution = PermutationSolution(
-            self.number_of_variables,
-            self.number_of_objectives)
+        new_solution = PermutationSolution(self.number_of_variables, self.number_of_objectives)
         new_solution.objectives = self.objectives[:]
         new_solution.variables = self.variables[:]
 
         new_solution.attributes = self.attributes.copy()
 
         return new_solution
```

### Comparing `jmetalpy-1.5.5/jmetal/core/test/test_observable.py` & `jmetalpy-1.6.0/jmetal/core/test/test_observable.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 import unittest
 
 from jmetal.core.observer import Observer
 from jmetal.util.observable import DefaultObservable
 
 
-class ObservableTestCases(unittest.TestCase):
-
-    class DummyObserver(Observer):
+class DummyObserver(Observer):
+    def update(self, *args, **kwargs):
+        pass
 
-        def update(self, *args, **kwargs):
-            pass
 
+class ObservableTestCases(unittest.TestCase):
     def setUp(self):
         self.observable = DefaultObservable()
-        self.observer = self.DummyObserver()
+        self.observer = DummyObserver()
 
     def test_should_register_add_one_observer(self):
         self.observable.register(self.observer)
 
         self.assertEqual(1, len(self.observable.observers))
 
     def test_should_register_add_two_observers(self):
-        observer_two = self.DummyObserver()
+        observer_two = DummyObserver()
 
         self.observable.register(self.observer)
         self.observable.register(observer_two)
 
         self.assertEqual(2, len(self.observable.observers))
 
     def test_should_deregister_remove_the_observer_if_it_is_registered(self):
-        observer_two = self.DummyObserver()
+        observer_two = DummyObserver()
 
         self.observable.register(self.observer)
         self.observable.register(observer_two)
         self.observable.deregister(self.observer)
 
         self.assertEqual(1, len(self.observable.observers))
 
     def test_should_deregister_not_remove_the_observer_if_it_is_not_registered(self):
-        observer_two = self.DummyObserver()
+        observer_two = DummyObserver()
 
         self.observable.register(self.observer)
         self.observable.deregister(observer_two)
 
         self.assertEqual(1, len(self.observable.observers))
         self.assertTrue(self.observer in self.observable.observers)
         self.assertFalse(observer_two in self.observable.observers)
```

### Comparing `jmetalpy-1.5.5/jmetal/core/test/test_operator.py` & `jmetalpy-1.6.0/jmetal/core/test/test_operator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,36 @@
 import unittest
-from typing import TypeVar
 
-from jmetal.core.operator import Mutation, Crossover
+from jmetal.core.operator import Crossover, Mutation
 from jmetal.core.solution import Solution
 
-S = TypeVar('S')
-R = TypeVar('R')
-
-
-class DummyMutation(Mutation[Solution]):
 
+class DummyMutation(Mutation):
     def __init__(self, probability: float):
         super(DummyMutation, self).__init__(probability=probability)
 
-    def execute(self, source: Solution) -> Solution:
-        return None
+    def execute(self, source: Solution) -> None:
+        pass
 
     def get_name(self) -> str:
-        return ""
+        pass
 
 
-class DummyCrossover(Crossover[Solution, Solution]):
-
+class DummyCrossover(Crossover):
     def __init__(self, probability: float):
         super(DummyCrossover, self).__init__(probability=probability)
 
-    def execute(self, source: Solution) -> Solution:
-        return None
+    def execute(self, source: Solution) -> None:
+        pass
 
     def get_name(self) -> str:
-        return ""
+        pass
 
 
 class OperatorTestCase(unittest.TestCase):
-
     def test_should_mutation_constructor_raises_an_exception_is_probability_is_negative(self) -> None:
         with self.assertRaises(Exception):
             DummyMutation(-1)
 
     def test_should_mutation_constructor_raises_an_exception_is_probability_is_higher_than_one(self) -> None:
         with self.assertRaises(Exception):
             DummyMutation(1.1)
@@ -47,9 +40,9 @@
             DummyCrossover(-1)
 
     def test_should_crossover_constructor_raises_an_exception_is_probability_is_higher_than_one(self) -> None:
         with self.assertRaises(Exception):
             DummyMutation(1.1)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `jmetalpy-1.5.5/jmetal/core/test/test_problem.py` & `jmetalpy-1.6.0/jmetal/util/test/test_evaluator.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,97 +1,87 @@
 import unittest
 
-from jmetal.core.problem import FloatProblem, IntegerProblem
-from jmetal.core.solution import FloatSolution, IntegerSolution
+from jmetal.core.problem import FloatProblem
+from jmetal.core.solution import FloatSolution
+from jmetal.util.evaluator import MapEvaluator, SequentialEvaluator
 
 
-class DummyIntegerProblem(IntegerProblem):
+class MockedProblem(FloatProblem):
+    def __init__(self, number_of_variables: int = 3):
+        super(MockedProblem, self).__init__()
 
-    def __init__(self):
-        super(DummyIntegerProblem, self).__init__()
+        self.lower_bound = [-5.0 for _ in range(number_of_variables)]
+        self.upper_bound = [5.0 for _ in range(number_of_variables)]
 
-    def evaluate(self, solution: IntegerSolution) -> IntegerSolution:
-        pass
+        FloatSolution.lower_bound = self.lower_bound
+        FloatSolution.upper_bound = self.upper_bound
 
-    def get_name(self) -> str:
-        pass
+    def number_of_objectives(self) -> int:
+        return 2
 
+    def number_of_constraints(self) -> int:
+        return 0
 
-class DummyFloatProblem(FloatProblem):
+    def evaluate(self, solution: FloatSolution):
+        solution.objectives[0] = 1.2
+        solution.objectives[1] = 2.3
 
-    def __init__(self):
-        super(DummyFloatProblem, self).__init__()
+        return solution
 
-    def evaluate(self, solution: FloatSolution) -> FloatSolution:
-        pass
+    def name(self) -> str:
+        return "Mocked problem"
 
-    def get_name(self) -> str:
-        pass
 
+class SequentialEvaluatorTestCases(unittest.TestCase):
+    def setUp(self):
+        self.evaluator = SequentialEvaluator()
+        self.problem = MockedProblem()
 
-class FloatProblemTestCases(unittest.TestCase):
+    def test_should_constructor_create_a_non_null_object(self):
+        self.assertIsNotNone(self.evaluator)
 
-    def test_should_default_constructor_create_a_valid_problem(self) -> None:
-        number_of_objectives = 2
-        number_of_constraints = 0
-        lower_bound = [-1.0]
-        upper_bound = [1.0]
+    def test_should_evaluate_a_list_of_problem_work_properly_with_a_solution(self):
+        problem_list = [self.problem.create_solution() for _ in range(1)]
 
-        problem = DummyFloatProblem()
-        problem.lower_bound = lower_bound
-        problem.upper_bound = upper_bound
-        problem.number_of_constraints = number_of_constraints
-        problem.number_of_objectives = number_of_objectives
-        problem.number_of_variables = len(lower_bound)
+        self.evaluator.evaluate(problem_list, self.problem)
 
-        self.assertEqual(1, problem.number_of_variables)
-        self.assertEqual(2, problem.number_of_objectives)
-        self.assertEqual(0, problem.number_of_constraints)
-        self.assertEqual([-1], problem.lower_bound)
-        self.assertEqual([1], problem.upper_bound)
+        self.assertEqual(1.2, problem_list[0].objectives[0])
+        self.assertEqual(2.3, problem_list[0].objectives[1])
 
-    def test_should_create_solution_create_a_valid_solution(self) -> None:
-        problem = DummyFloatProblem()
-        problem.number_of_variables = 2
-        problem.number_of_objectives = 2
-        problem.number_of_constraints = 0
-        problem.lower_bound = [-1.0, -2.0]
-        problem.upper_bound = [1.0, 2.0]
+    def test_should_evaluate_a_list_of_problem_work_properly(self):
+        problem_list = [self.problem.create_solution() for _ in range(10)]
 
-        solution = problem.create_solution()
-        self.assertNotEqual(None, solution)
-        self.assertTrue(-1.0 <= solution.variables[0] <= 1.0)
-        self.assertTrue(-2.0 <= solution.variables[1] <= 2.0)
+        self.evaluator.evaluate(problem_list, self.problem)
 
+        for i in range(10):
+            self.assertEqual(1.2, problem_list[i].objectives[0])
+            self.assertEqual(2.3, problem_list[i].objectives[1])
 
-class IntegerProblemTestCases(unittest.TestCase):
 
-    def test_should_default_constructor_create_a_valid_problem(self) -> None:
-        problem = DummyIntegerProblem()
-        problem.number_of_variables = 1
-        problem.number_of_objectives = 2
-        problem.number_of_constraints = 0
-        problem.lower_bound = [-1]
-        problem.upper_bound = [1]
+class ParallelEvaluatorTestCases(unittest.TestCase):
+    def setUp(self):
+        self.evaluator = MapEvaluator()
+        self.problem = MockedProblem()
 
-        self.assertEqual(1, problem.number_of_variables)
-        self.assertEqual(2, problem.number_of_objectives)
-        self.assertEqual(0, problem.number_of_constraints)
-        self.assertEqual([-1], problem.lower_bound)
-        self.assertEqual([1], problem.upper_bound)
+    def test_should_constructor_create_a_non_null_object(self):
+        self.assertIsNotNone(self.evaluator)
 
-    def test_should_create_solution_create_a_valid_solution(self) -> None:
-        problem = DummyIntegerProblem()
-        problem.number_of_variables = 2
-        problem.number_of_objectives = 2
-        problem.number_of_constraints = 0
-        problem.lower_bound = [-1, -2]
-        problem.upper_bound = [1, 2]
+    def test_should_evaluate_a_list_of_problem_work_properly_with_a_solution(self):
+        problem_list = [self.problem.create_solution() for _ in range(1)]
 
-        solution = problem.create_solution()
-        self.assertNotEqual(None, solution)
-        self.assertTrue(-1 <= solution.variables[0] <= 1)
-        self.assertTrue(-2 <= solution.variables[1] <= 2)
+        self.evaluator.evaluate(problem_list, self.problem)
 
+        self.assertEqual(1.2, problem_list[0].objectives[0])
+        self.assertEqual(2.3, problem_list[0].objectives[1])
 
-if __name__ == '__main__':
+    def test_should_evaluate_a_list_of_problem_work_properly(self):
+        problem_list = [self.problem.create_solution() for _ in range(10)]
+
+        self.evaluator.evaluate(problem_list, self.problem)
+
+        for i in range(10):
+            self.assertEqual(1.2, problem_list[i].objectives[0])
+            self.assertEqual(2.3, problem_list[i].objectives[1])
+
+
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `jmetalpy-1.5.5/jmetal/core/test/test_quality_indicator.py` & `jmetalpy-1.6.0/jmetal/core/test/test_quality_indicator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,22 @@
+import os
 import unittest
-from os.path import dirname, join
 from pathlib import Path
 
 import numpy as np
-from jmetal.core.quality_indicator import GenerationalDistance, InvertedGenerationalDistance, EpsilonIndicator, \
-    HyperVolume
 
+from jmetal.core.quality_indicator import (EpsilonIndicator,
+                                           GenerationalDistance, HyperVolume,
+                                           InvertedGenerationalDistance,
+                                           NormalizedHyperVolume)
+
+DIRNAME = os.path.dirname(os.path.abspath(__file__))
 
-class GenerationalDistanceTestCases(unittest.TestCase):
-    """ Class including unit tests for class GenerationalDistance
-    """
 
+class GenerationalDistanceTestCases(unittest.TestCase):
     def test_should_constructor_create_a_non_null_object(self) -> None:
         indicator = GenerationalDistance([])
         self.assertIsNotNone(indicator)
 
     def test_get_name_return_the_right_value(self):
         self.assertEqual("Generational Distance", GenerationalDistance([]).get_name())
 
@@ -128,17 +130,14 @@
         distance_of_second_point = np.sqrt(pow(2.1 - 2.2, 2) + pow(2.1 - 2.2, 2))
         distance_of_third_point = np.sqrt(pow(2.1 - 1.9, 2) + pow(2.1 - 1.9, 2))
 
         self.assertEqual((distance_of_first_point + distance_of_second_point + distance_of_third_point) / 3.0, result)
 
 
 class InvertedGenerationalDistanceTestCases(unittest.TestCase):
-    """ Class including unit tests for class InvertedGenerationalDistance
-    """
-
     def test_should_constructor_create_a_non_null_object(self) -> None:
         indicator = InvertedGenerationalDistance([])
         self.assertIsNotNone(indicator)
 
     def test_get_name_return_the_right_value(self):
         self.assertEqual("Inverted Generational Distance", InvertedGenerationalDistance([]).get_name())
 
@@ -227,51 +226,72 @@
         distance_of_first_point = np.sqrt(pow(1.0 - 1.5, 2) + pow(1.0 - 1.5, 2))
         distance_of_second_point = np.sqrt(pow(2.0 - 1.9, 2) + pow(2.0 - 1.9, 2))
 
         self.assertEqual((distance_of_first_point + distance_of_second_point) / 2.0, result)
 
 
 class EpsilonIndicatorTestCases(unittest.TestCase):
-    """ Class including unit tests for class EpsilonIndicator
-    """
-
     def test_should_constructor_create_a_non_null_object(self) -> None:
         indicator = EpsilonIndicator(np.array([[1.0, 1.0], [2.0, 2.0]]))
         self.assertIsNotNone(indicator)
 
 
 class HyperVolumeTestCases(unittest.TestCase):
-
-    def setUp(self):
-        self.file_path = dirname(join(dirname(__file__)))
-
     def test_should_hypervolume_return_5_0(self):
         reference_point = [2, 2, 2]
 
         front = np.array([[1, 0, 1], [0, 1, 0]])
 
         hv = HyperVolume(reference_point)
         value = hv.compute(front)
 
         self.assertEqual(5.0, value)
 
     def test_should_hypervolume_return_the_correct_value_when_applied_to_the_ZDT1_reference_front(self):
-        filename = 'jmetal/core/test/ZDT1.pf'
+        filepath = Path(DIRNAME, "ZDT1.pf")
         front = []
-        if Path(filename).is_file():
-            with open(filename) as file:
-                for line in file:
-                    vector = [float(x) for x in line.split()]
-                    front.append(vector)
-        else:
-            print("error")
+
+        with open(filepath) as file:
+            for line in file:
+                vector = [float(x) for x in line.split()]
+                front.append(vector)
 
         reference_point = [1, 1]
 
         hv = HyperVolume(reference_point)
         value = hv.compute(np.array(front))
 
         self.assertAlmostEqual(0.666, value, delta=0.001)
 
 
-if __name__ == '__main__':
+class NormalizedHyperVolumeTestCases(unittest.TestCase):
+    @classmethod
+    def setUpClass(cls):
+        filepath = Path(DIRNAME, "ZDT1.pf")
+        front = []
+
+        with open(filepath) as file:
+            for line in file:
+                vector = [float(x) for x in line.split()]
+                front.append(vector)
+
+        cls._front = np.array(front)
+
+    def test_should_hypervolume_return_zero_when_providing_reference_front(self):
+        reference_point = [1, 1]
+        reference_front = self._front
+
+        hv = NormalizedHyperVolume(reference_point, reference_front=reference_front)
+        value = hv.compute(reference_front)
+
+        self.assertAlmostEqual(0, value, delta=0.001)
+
+    def test_should_raise_AssertionError_when_reference_front_hv_is_zero(self):
+        reference_point = [0, 0]
+        reference_front = self._front
+
+        with self.assertRaises(AssertionError):
+            _ = NormalizedHyperVolume(reference_point, reference_front=reference_front)
+
+
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `jmetalpy-1.5.5/jmetal/core/test/test_solution.py` & `jmetalpy-1.6.0/jmetal/core/test/test_solution.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,60 +1,64 @@
 import copy
 import unittest
 
-from jmetal.core.solution import BinarySolution, FloatSolution, IntegerSolution, Solution, CompositeSolution
+from jmetal.core.solution import (
+    BinarySolution,
+    CompositeSolution,
+    FloatSolution,
+    IntegerSolution,
+    Solution,
+)
 from jmetal.util.ckecking import InvalidConditionException
 
 
 class SolutionTestCase(unittest.TestCase):
-
-    def test_should_default_constructor_create_a_valid_solution(self) -> None:
+    def test_should_default_constructor_create_a_valid_solution(self):
         solution = Solution(2, 3)
         self.assertEqual(2, solution.number_of_variables)
         self.assertEqual(3, solution.number_of_objectives)
         self.assertEqual(0, len(solution.attributes))
         self.assertEqual(2, len(solution.variables))
         self.assertEqual(3, len(solution.objectives))
 
 
 class BinarySolutionTestCase(unittest.TestCase):
-    def test_should_default_constructor_create_a_valid_solution(self) -> None:
+    def test_should_default_constructor_create_a_valid_solution(self):
         solution = BinarySolution(2, 3)
         self.assertEqual(2, solution.number_of_variables)
         self.assertEqual(3, solution.number_of_objectives)
 
-    def test_should_constructor_create_a_valid_solution(self) -> None:
+    def test_should_constructor_create_a_valid_solution(self):
         solution = BinarySolution(number_of_variables=2, number_of_objectives=3)
         solution.variables[0] = [True, False]
         solution.variables[1] = [False]
         self.assertEqual(2, solution.number_of_variables)
         self.assertEqual(3, solution.number_of_objectives)
         self.assertEqual(2, len(solution.variables))
         self.assertEqual(3, len(solution.objectives))
         self.assertEqual([True, False], solution.variables[0])
         self.assertEqual([False], solution.variables[1])
 
-    def test_should_get_total_number_of_bits_return_zero_if_the_object_variables_are_not_initialized(self) -> None:
+    def test_should_get_total_number_of_bits_return_zero_if_the_object_variables_are_not_initialized(self):
         solution = BinarySolution(number_of_variables=2, number_of_objectives=3)
         self.assertEqual(0, solution.get_total_number_of_bits())
 
     def test_should_get_total_number_of_bits_return_the_right_value(self) -> None:
         solution = BinarySolution(number_of_variables=2, number_of_objectives=3)
         solution.variables[0] = [True, False]
         solution.variables[1] = [False, True, False]
         self.assertEqual(5, solution.get_total_number_of_bits())
 
 
 class FloatSolutionTestCase(unittest.TestCase):
-
-    def test_should_constructor_create_a_non_null_object(self) -> None:
+    def test_should_constructor_create_a_non_null_object(self):
         solution = FloatSolution([], [], 2)
         self.assertIsNotNone(solution)
 
-    def test_should_default_constructor_create_a_valid_solution(self) -> None:
+    def test_should_default_constructor_create_a_valid_solution(self):
         solution = FloatSolution([0.0, 0.5], [1.0, 2.0], 3)
 
         self.assertEqual(2, solution.number_of_variables)
         self.assertEqual(3, solution.number_of_objectives)
         self.assertEqual(2, len(solution.variables))
         self.assertEqual(3, len(solution.objectives))
         self.assertEqual([0.0, 0.5], solution.lower_bound)
@@ -78,31 +82,30 @@
         self.assertEqual(solution.constraints, new_solution.constraints)
         self.assertIs(solution.lower_bound, solution.lower_bound)
         self.assertIs(solution.upper_bound, solution.upper_bound)
         self.assertEqual(solution.attributes, new_solution.attributes)
 
 
 class IntegerSolutionTestCase(unittest.TestCase):
-
-    def test_should_constructor_create_a_non_null_object(self) -> None:
+    def test_should_constructor_create_a_non_null_object(self):
         solution = IntegerSolution([], [], 2)
         self.assertIsNotNone(solution)
 
-    def test_should_default_constructor_create_a_valid_solution(self) -> None:
+    def test_should_default_constructor_create_a_valid_solution(self):
         solution = IntegerSolution([0, 5], [1, 2], 3, 0)
 
         self.assertEqual(2, solution.number_of_variables)
         self.assertEqual(3, solution.number_of_objectives)
         self.assertEqual(2, len(solution.variables))
         self.assertEqual(3, len(solution.objectives))
         self.assertEqual(0, len(solution.constraints))
         self.assertEqual([0, 5], solution.lower_bound)
         self.assertEqual([1, 2], solution.upper_bound)
 
-    def test_should_copy_work_properly(self) -> None:
+    def test_should_copy_work_properly(self):
         solution = IntegerSolution([0, 5], [1, 2], 3, 1)
         solution.variables = [1, 2]
         solution.objectives = [0.16, -2.34, 9.25]
         solution.constraints = [-5]
         solution.attributes["attr"] = "value"
 
         new_solution = copy.copy(solution)
@@ -121,27 +124,28 @@
 
 class CompositeSolutionTestCase(unittest.TestCase):
     def test_should_constructor_create_a_valid_not_none_composite_solution_composed_of_a_double_solution(self):
         composite_solution = CompositeSolution([FloatSolution([1.0], [2.0], 2)])
         self.assertIsNotNone(composite_solution)
 
     def test_should_constructor_raise_an_exception_if_the_number_of_objectives_is_not_coherent(self):
-        float_solution: FloatSolution = FloatSolution([1.0], [3.0], 3)
-        integer_solution: IntegerSolution = IntegerSolution([2], [4], 2)
+        float_solution = FloatSolution([1.0], [3.0], 3)
+        integer_solution = IntegerSolution([2], [4], 2)
 
         with self.assertRaises(InvalidConditionException):
             CompositeSolution([float_solution, integer_solution])
 
     def test_should_constructor_create_a_valid_soltion_composed_of_a_float_and_an_integer_solutions(self):
         number_of_objectives = 3
         number_of_constraints = 1
-        float_solution: FloatSolution = FloatSolution([1.0], [3.0], number_of_objectives, number_of_constraints)
-        integer_solution: IntegerSolution = IntegerSolution([2], [4], number_of_objectives, number_of_constraints)
 
-        solution: CompositeSolution = CompositeSolution([float_solution, integer_solution])
+        float_solution = FloatSolution([1.0], [3.0], number_of_objectives, number_of_constraints)
+        integer_solution = IntegerSolution([2], [4], number_of_objectives, number_of_constraints)
+
+        solution = CompositeSolution([float_solution, integer_solution])
 
         self.assertIsNotNone(solution)
         self.assertEqual(2, solution.number_of_variables)
         self.assertEqual(number_of_objectives, solution.number_of_objectives)
         self.assertEqual(number_of_constraints, solution.number_of_constraints)
         self.assertEqual(number_of_objectives, solution.variables[0].number_of_objectives)
         self.assertEqual(number_of_objectives, solution.variables[1].number_of_objectives)
@@ -149,28 +153,28 @@
         self.assertEqual(number_of_constraints, solution.variables[1].number_of_constraints)
         self.assertTrue(type(solution.variables[0] is FloatSolution))
         self.assertTrue(type(solution.variables[1] is IntegerSolution))
 
     def test_should_copy_work_properly(self):
         number_of_objectives = 3
         number_of_constraints = 1
-        float_solution: FloatSolution = FloatSolution([1.0], [3.0], number_of_objectives, number_of_constraints)
-        integer_solution: IntegerSolution = IntegerSolution([2], [4], number_of_objectives, number_of_constraints)
+        float_solution = FloatSolution([1.0], [3.0], number_of_objectives, number_of_constraints)
+        integer_solution = IntegerSolution([2], [4], number_of_objectives, number_of_constraints)
 
-        solution: CompositeSolution = CompositeSolution([float_solution, integer_solution])
-        new_solution: CompositeSolution = copy.deepcopy(solution)
+        solution = CompositeSolution([float_solution, integer_solution])
+        new_solution = copy.deepcopy(solution)
 
         self.assertEqual(solution.number_of_variables, new_solution.number_of_variables)
         self.assertEqual(solution.number_of_objectives, new_solution.number_of_objectives)
         self.assertEqual(solution.number_of_constraints, new_solution.number_of_constraints)
 
         self.assertEqual(solution.variables[0].number_of_variables, new_solution.variables[0].number_of_variables)
         self.assertEqual(solution.variables[1].number_of_variables, new_solution.variables[1].number_of_variables)
         self.assertEqual(solution.variables[0], new_solution.variables[0])
         self.assertEqual(solution.variables[1], new_solution.variables[1])
 
         self.assertEqual(solution.variables[0].variables, new_solution.variables[0].variables)
         self.assertEqual(solution.variables[1].variables, new_solution.variables[1].variables)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `jmetalpy-1.5.5/jmetal/lab/experiment.py` & `jmetalpy-1.6.0/jmetal/lab/experiment.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,62 +1,64 @@
 import io
-import logging
 import os
 from concurrent.futures import ProcessPoolExecutor
 from pathlib import Path
 from statistics import median
 from typing import List
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
-from scipy.stats import mannwhitneyu
+from scipy.stats import mannwhitneyu, iqr
 
 from jmetal.core.algorithm import Algorithm
 from jmetal.core.quality_indicator import QualityIndicator
-from jmetal.util.solution import print_function_values_to_file, print_variables_to_file, read_solutions
+from jmetal.logger import get_logger
+from jmetal.util.solution import (
+    print_function_values_to_file,
+    print_variables_to_file,
+    read_solutions,
+)
 
-LOGGER = logging.getLogger('jmetal')
+logger = get_logger(__name__)
 
 """
 .. module:: laboratory
    :platform: Unix, Windows
    :synopsis: Run experiments. WIP!
 
 .. moduleauthor:: Antonio Benítez-Hidalgo <antonio.b@uma.es>
 """
 
 
 class Job:
-
     def __init__(self, algorithm: Algorithm, algorithm_tag: str, problem_tag: str, run: int):
         self.algorithm = algorithm
         self.algorithm_tag = algorithm_tag
         self.problem_tag = problem_tag
         self.run_tag = run
 
-    def execute(self, output_path: str = ''):
+    def execute(self, output_path: str = ""):
         self.algorithm.run()
 
         if output_path:
-            file_name = os.path.join(output_path, 'FUN.{}.tsv'.format(self.run_tag))
+            file_name = os.path.join(output_path, "FUN.{}.tsv".format(self.run_tag))
             print_function_values_to_file(self.algorithm.get_result(), filename=file_name)
 
-            file_name = os.path.join(output_path, 'VAR.{}.tsv'.format(self.run_tag))
+            file_name = os.path.join(output_path, "VAR.{}.tsv".format(self.run_tag))
             print_variables_to_file(self.algorithm.get_result(), filename=file_name)
 
-            file_name = os.path.join(output_path, 'TIME.{}'.format(self.run_tag))
-            with open(file_name, 'w+') as of:
+            file_name = os.path.join(output_path, "TIME.{}".format(self.run_tag))
+            with open(file_name, "w+") as of:
                 of.write(str(self.algorithm.total_computing_time))
 
 
 class Experiment:
-
     def __init__(self, output_dir: str, jobs: List[Job], m_workers: int = 6):
-        """ Run an experiment to execute a list of jobs.
+        """Run an experiment to execute a list of jobs.
 
         :param output_dir: Base directory where each job will save its results.
         :param jobs: List of Jobs (from :py:mod:`jmetal.util.laboratory)`) to be executed.
         :param m_workers: Maximum number of workers to execute the Jobs in parallel.
         """
         self.jobs = jobs
         self.m_workers = m_workers
@@ -65,17 +67,18 @@
     def run(self) -> None:
         with ProcessPoolExecutor(max_workers=self.m_workers) as executor:
             for job in self.jobs:
                 output_path = os.path.join(self.output_dir, job.algorithm_tag, job.problem_tag)
                 executor.submit(job.execute(output_path))
 
 
-def generate_summary_from_experiment(input_dir: str, quality_indicators: List[QualityIndicator],
-                                     reference_fronts: str = ''):
-    """ Compute a list of quality indicators. The input data directory *must* met the following structure (this is generated
+def generate_summary_from_experiment(
+    input_dir: str, quality_indicators: List[QualityIndicator], reference_fronts: str = ""
+):
+    """Compute a list of quality indicators. The input data directory *must* met the following structure (this is generated
     automatically by the Experiment class):
 
     * <base_dir>
 
       * algorithm_a
 
         * problem_a
@@ -91,139 +94,140 @@
     :param quality_indicators: List of quality indicators to compute.
     :return: None.
     """
 
     if not quality_indicators:
         quality_indicators = []
 
-    with open('QualityIndicatorSummary.csv', 'w+') as of:
-        of.write('Algorithm,Problem,ExecutionId,IndicatorName,IndicatorValue\n')
+    with open("QualityIndicatorSummary.csv", "w+") as of:
+        of.write("Algorithm,Problem,ExecutionId,IndicatorName,IndicatorValue\n")
 
     for dirname, _, filenames in os.walk(input_dir):
         for filename in filenames:
             try:
                 # Linux filesystem
-                algorithm, problem = dirname.split('/')[-2:]
+                algorithm, problem = dirname.split("/")[-2:]
             except ValueError:
                 # Windows filesystem
-                algorithm, problem = dirname.split('\\')[-2:]
+                algorithm, problem = dirname.split("\\")[-2:]
 
-            if 'TIME' in filename:
-                run_tag = [s for s in filename.split('.') if s.isdigit()].pop()
+            if "TIME" in filename:
+                run_tag = [s for s in filename.split(".") if s.isdigit()].pop()
 
-                with open(os.path.join(dirname, filename), 'r') as content_file:
+                with open(os.path.join(dirname, filename), "r") as content_file:
                     content = content_file.read()
 
-                with open('QualityIndicatorSummary.csv', 'a+') as of:
-                    of.write(','.join([algorithm, problem, run_tag, 'Time', str(content)]))
-                    of.write('\n')
+                with open("QualityIndicatorSummary.csv", "a+") as of:
+                    of.write(",".join([algorithm, problem, run_tag, "Time", str(content)]))
+                    of.write("\n")
 
-            if 'FUN' in filename:
+            if "FUN" in filename:
                 solutions = read_solutions(os.path.join(dirname, filename))
-                run_tag = [s for s in filename.split('.') if s.isdigit()].pop()
+                run_tag = [s for s in filename.split(".") if s.isdigit()].pop()
                 for indicator in quality_indicators:
-                    reference_front_file = os.path.join(reference_fronts, problem + '.pf')
+                    reference_front_file = os.path.join(reference_fronts, problem + ".pf")
 
                     # Add reference front if any
-                    if hasattr(indicator, 'reference_front'):
+                    if hasattr(indicator, "reference_front"):
                         if Path(reference_front_file).is_file():
                             reference_front = []
                             with open(reference_front_file) as file:
                                 for line in file:
                                     reference_front.append([float(x) for x in line.split()])
 
                             indicator.reference_front = reference_front
                         else:
-                            LOGGER.warning('Reference front not found at', reference_front_file)
+                            logger.warning("Reference front not found at", reference_front_file)
 
                     result = indicator.compute([solutions[i].objectives for i in range(len(solutions))])
 
                     # Save quality indicator value to file
-                    with open('QualityIndicatorSummary.csv', 'a+') as of:
-                        of.write(','.join([algorithm, problem, run_tag, indicator.get_short_name(), str(result)]))
-                        of.write('\n')
+                    with open("QualityIndicatorSummary.csv", "a+") as of:
+                        of.write(",".join([algorithm, problem, run_tag, indicator.get_short_name(), str(result)]))
+                        of.write("\n")
 
 
-def generate_boxplot(filename: str, output_dir: str = 'boxplot'):
-    """ Generate boxplot diagrams.
+def generate_boxplot(filename: str, output_dir: str = "boxplot"):
+    """Generate boxplot diagrams.
 
     :param filename: Input filename (summary).
     :param output_dir: Output path.
     """
     df = pd.read_csv(filename, skipinitialspace=True)
 
     if len(set(df.columns.tolist())) != 5:
-        raise Exception('Wrong number of columns')
+        raise Exception("Wrong number of columns")
 
     if Path(output_dir).is_dir():
-        LOGGER.warning('Directory {} exists. Removing contents.'.format(output_dir))
+        logger.warning("Directory {} exists. Removing contents.".format(output_dir))
         for file in os.listdir(output_dir):
-            os.remove('{0}/{1}'.format(output_dir, file))
+            os.remove("{0}/{1}".format(output_dir, file))
     else:
-        LOGGER.warning('Directory {} does not exist. Creating it.'.format(output_dir))
+        logger.warning("Directory {} does not exist. Creating it.".format(output_dir))
         Path(output_dir).mkdir(parents=True)
 
-    algorithms = pd.unique(df['Algorithm'])
-    problems = pd.unique(df['Problem'])
-    indicators = pd.unique(df['IndicatorName'])
+    algorithms = pd.unique(df["Algorithm"])
+    problems = pd.unique(df["Problem"])
+    indicators = pd.unique(df["IndicatorName"])
 
     # We consider the quality indicator indicator_name
 
     for indicator_name in indicators:
-        data = df[df['IndicatorName'] == indicator_name]
+        data = df[df["IndicatorName"] == indicator_name]
 
         for pr in problems:
             data_to_plot = []
 
             for alg in algorithms:
-                data_to_plot.append(data['IndicatorValue'][np.logical_and(
-                    data['Algorithm'] == alg, data['Problem'] == pr)])
+                data_to_plot.append(
+                    data["IndicatorValue"][np.logical_and(data["Algorithm"] == alg, data["Problem"] == pr)]
+                )
 
             # Create a figure instance
             fig = plt.figure(1, figsize=(9, 6))
             plt.suptitle(pr, y=0.95, fontsize=18)
 
             ax = fig.add_subplot(111)
             ax.boxplot(data_to_plot)
 
             ax.set_xticklabels(algorithms)
             ax.tick_params(labelsize=20)
 
-            plt.savefig(os.path.join(output_dir, 'boxplot-{}-{}.png'.format(pr, indicator_name)), bbox_inches='tight')
-            plt.savefig(os.path.join(output_dir, 'boxplot-{}-{}.eps'.format(pr, indicator_name)), bbox_inches='tight')
+            plt.savefig(os.path.join(output_dir, "boxplot-{}-{}.png".format(pr, indicator_name)), bbox_inches="tight")
+            plt.savefig(os.path.join(output_dir, "boxplot-{}-{}.eps".format(pr, indicator_name)), bbox_inches="tight")
             plt.close(fig)
 
 
-def generate_latex_tables(filename: str, output_dir: str = 'latex/statistical'):
-    """ Computes a number of statistical values (mean, median, standard deviation, interquartile range).
+def generate_latex_tables(filename: str, output_dir: str = "latex/statistical"):
+    """Computes a number of statistical values (mean, median, standard deviation, interquartile range).
 
     :param filename: Input filename (summary).
     :param output_dir: Output path.
     """
     df = pd.read_csv(filename, skipinitialspace=True)
 
     if len(set(df.columns.tolist())) != 5:
-        raise Exception('Wrong number of columns')
+        raise Exception("Wrong number of columns")
 
     if Path(output_dir).is_dir():
-        LOGGER.warning('Directory {} exists. Removing contents.'.format(output_dir))
+        logger.warning("Directory {} exists. Removing contents.".format(output_dir))
         for file in os.listdir(output_dir):
-            os.remove('{0}/{1}'.format(output_dir, file))
+            os.remove("{0}/{1}".format(output_dir, file))
     else:
-        LOGGER.warning('Directory {} does not exist. Creating it.'.format(output_dir))
+        logger.warning("Directory {} does not exist. Creating it.".format(output_dir))
         Path(output_dir).mkdir(parents=True)
 
     # Generate median & iqr tables
     median, iqr = pd.DataFrame(), pd.DataFrame()
     mean, std = pd.DataFrame(), pd.DataFrame()
 
-    for algorithm_name, subset in df.groupby('Algorithm', sort=False):
-        subset = subset.drop('Algorithm', axis=1)
-        subset = subset.rename(columns={'IndicatorValue': algorithm_name})
-        subset = subset.set_index(['Problem', 'IndicatorName', 'ExecutionId'])
+    for algorithm_name, subset in df.groupby("Algorithm", sort=False):
+        subset = subset.drop("Algorithm", axis=1)
+        subset = subset.rename(columns={"IndicatorValue": algorithm_name})
+        subset = subset.set_index(["Problem", "IndicatorName", "ExecutionId"])
 
         # Compute Median and Interquartile range
         median_ = subset.groupby(level=[0, 1]).median()
         median = pd.concat([median, median_], axis=1)
 
         iqr_ = subset.groupby(level=[0, 1]).quantile(0.75) - subset.groupby(level=[0, 1]).quantile(0.25)
         iqr = pd.concat([iqr, iqr_], axis=1)
@@ -232,318 +236,529 @@
         mean_ = subset.groupby(level=[0, 1]).mean()
         mean = pd.concat([mean, mean_], axis=1)
 
         std_ = subset.groupby(level=[0, 1]).std()
         std = pd.concat([std, std_], axis=1)
 
     # Generate mean & std tables
-    for indicator_name, subset in std.groupby('IndicatorName', sort=False):
-        subset = median.groupby('IndicatorName', sort=False).get_group(indicator_name)
+    for indicator_name, subset in std.groupby("IndicatorName", sort=False):
+        subset = median.groupby("IndicatorName", sort=False).get_group(indicator_name)
         subset.index = subset.index.droplevel(1)
-        subset.to_csv(os.path.join(output_dir, 'Median-{}.csv'.format(indicator_name)), sep='\t', encoding='utf-8')
+        subset.to_csv(os.path.join(output_dir, "Median-{}.csv".format(indicator_name)), sep="\t", encoding="utf-8")
 
-        subset = iqr.groupby('IndicatorName', sort=False).get_group(indicator_name)
+        subset = iqr.groupby("IndicatorName", sort=False).get_group(indicator_name)
         subset.index = subset.index.droplevel(1)
-        subset.to_csv(os.path.join(output_dir, 'IQR-{}.csv'.format(indicator_name)), sep='\t', encoding='utf-8')
+        subset.to_csv(os.path.join(output_dir, "IQR-{}.csv".format(indicator_name)), sep="\t", encoding="utf-8")
 
-        subset = mean.groupby('IndicatorName', sort=False).get_group(indicator_name)
+        subset = mean.groupby("IndicatorName", sort=False).get_group(indicator_name)
         subset.index = subset.index.droplevel(1)
-        subset.to_csv(os.path.join(output_dir, 'Mean-{}.csv'.format(indicator_name)), sep='\t', encoding='utf-8')
+        subset.to_csv(os.path.join(output_dir, "Mean-{}.csv".format(indicator_name)), sep="\t", encoding="utf-8")
 
-        subset = std.groupby('IndicatorName', sort=False).get_group(indicator_name)
+        subset = std.groupby("IndicatorName", sort=False).get_group(indicator_name)
         subset.index = subset.index.droplevel(1)
-        subset.to_csv(os.path.join(output_dir, 'Std-{}.csv'.format(indicator_name)), sep='\t', encoding='utf-8')
+        subset.to_csv(os.path.join(output_dir, "Std-{}.csv".format(indicator_name)), sep="\t", encoding="utf-8")
 
     # Generate LaTeX tables
-    for indicator_name in df.groupby('IndicatorName', sort=False).groups.keys():
+    for indicator_name in df.groupby("IndicatorName", sort=False).groups.keys():
         # Median & IQR
-        md = median.groupby('IndicatorName', sort=False).get_group(indicator_name)
+        md = median.groupby("IndicatorName", sort=False).get_group(indicator_name)
         md.index = md.index.droplevel(1)
 
-        i = iqr.groupby('IndicatorName', sort=False).get_group(indicator_name)
+        i = iqr.groupby("IndicatorName", sort=False).get_group(indicator_name)
         i.index = i.index.droplevel(1)
 
-        with open(os.path.join(output_dir, 'MedianIQR-{}.tex'.format(indicator_name)), 'w') as latex:
+        with open(os.path.join(output_dir, "MedianIQR-{}.tex".format(indicator_name)), "w") as latex:
             latex.write(
                 __averages_to_latex(
                     md,
                     i,
-                    caption='Median and Interquartile Range of the {} quality indicator.'.format(indicator_name),
+                    caption="Median and Interquartile Range of the {} quality indicator.".format(indicator_name),
                     minimization=check_minimization(indicator_name),
-                    label='table:{}'.format(indicator_name)
+                    label="table:{}".format(indicator_name),
                 )
             )
 
         # Mean & Std
-        mn = mean.groupby('IndicatorName', sort=False).get_group(indicator_name)
+        mn = mean.groupby("IndicatorName", sort=False).get_group(indicator_name)
         mn.index = mn.index.droplevel(1)
 
-        s = std.groupby('IndicatorName', sort=False).get_group(indicator_name)
+        s = std.groupby("IndicatorName", sort=False).get_group(indicator_name)
         s.index = s.index.droplevel(1)
 
-        with open(os.path.join(output_dir, 'MeanStd-{}.tex'.format(indicator_name)), 'w') as latex:
+        with open(os.path.join(output_dir, "MeanStd-{}.tex".format(indicator_name)), "w") as latex:
             latex.write(
                 __averages_to_latex(
                     mn,
                     s,
-                    caption='Mean and Standard Deviation of the {} quality indicator.'.format(indicator_name),
+                    caption="Mean and Standard Deviation of the {} quality indicator.".format(indicator_name),
                     minimization=check_minimization(indicator_name),
-                    label='table:{}'.format(indicator_name)
+                    label="table:{}".format(indicator_name),
                 )
             )
 
 
-def compute_wilcoxon(filename: str, output_dir: str = 'latex/wilcoxon'):
+def compute_wilcoxon(filename: str, output_dir: str = "latex/wilcoxon"):
     """
     :param filename: Input filename (summary).
     :param output_dir: Output path.
     """
     df = pd.read_csv(filename, skipinitialspace=True)
 
     if len(set(df.columns.tolist())) != 5:
-        raise Exception('Wrong number of columns')
+        raise Exception("Wrong number of columns")
 
     if Path(output_dir).is_dir():
-        LOGGER.warning('Directory {} exists. Removing contents.'.format(output_dir))
+        logger.warning("Directory {} exists. Removing contents.".format(output_dir))
         for file in os.listdir(output_dir):
-            os.remove('{0}/{1}'.format(output_dir, file))
+            os.remove("{0}/{1}".format(output_dir, file))
     else:
-        LOGGER.warning('Directory {} does not exist. Creating it.'.format(output_dir))
+        logger.warning("Directory {} does not exist. Creating it.".format(output_dir))
         Path(output_dir).mkdir(parents=True)
 
-    algorithms = pd.unique(df['Algorithm'])
-    problems = pd.unique(df['Problem'])
-    indicators = pd.unique(df['IndicatorName'])
+    algorithms = pd.unique(df["Algorithm"])
+    problems = pd.unique(df["Problem"])
+    indicators = pd.unique(df["IndicatorName"])
 
     table = pd.DataFrame(index=algorithms[0:-1], columns=algorithms[1:])
 
     for indicator_name in indicators:
         for i, row_algorithm in enumerate(algorithms[0:-1]):
             wilcoxon = []
             for j, col_algorithm in enumerate(algorithms[1:]):
                 line = []
 
                 if i <= j:
                     for problem in problems:
-                        df1 = df[(df["Algorithm"] == row_algorithm) & (df["Problem"] == problem) & (
-                                df["IndicatorName"] == indicator_name)]
-                        df2 = df[(df["Algorithm"] == col_algorithm) & (df["Problem"] == problem) & (
-                                df["IndicatorName"] == indicator_name)]
+                        df1 = df[
+                            (df["Algorithm"] == row_algorithm)
+                            & (df["Problem"] == problem)
+                            & (df["IndicatorName"] == indicator_name)
+                        ]
+                        df2 = df[
+                            (df["Algorithm"] == col_algorithm)
+                            & (df["Problem"] == problem)
+                            & (df["IndicatorName"] == indicator_name)
+                        ]
 
                         data1 = df1["IndicatorValue"]
                         data2 = df2["IndicatorValue"]
 
                         median1 = median(data1)
                         median2 = median(data2)
 
                         stat, p = mannwhitneyu(data1, data2)
 
                         if p <= 0.05:
                             if check_minimization(indicator_name):
                                 if median1 <= median2:
-                                    line.append('+')
+                                    line.append("+")
                                 else:
-                                    line.append('o')
+                                    line.append("o")
                             else:
                                 if median1 >= median2:
-                                    line.append('+')
+                                    line.append("+")
                                 else:
-                                    line.append('o')
+                                    line.append("o")
                         else:
-                            line.append('-')
-                    wilcoxon.append(''.join(line))
+                            line.append("-")
+                    wilcoxon.append("".join(line))
 
-            if len(wilcoxon) < len(algorithms): wilcoxon = [''] * (len(algorithms) - len(wilcoxon) - 1) + wilcoxon
+            if len(wilcoxon) < len(algorithms):
+                wilcoxon = [""] * (len(algorithms) - len(wilcoxon) - 1) + wilcoxon
             table.loc[row_algorithm] = wilcoxon
 
-        table.to_csv(os.path.join(output_dir, 'Wilcoxon-{}.csv'.format(indicator_name)), sep='\t', encoding='utf-8')
+        table.to_csv(os.path.join(output_dir, "Wilcoxon-{}.csv".format(indicator_name)), sep="\t", encoding="utf-8")
 
-        with open(os.path.join(output_dir, 'Wilcoxon-{}.tex'.format(indicator_name)), 'w') as latex:
+        with open(os.path.join(output_dir, "Wilcoxon-{}.tex".format(indicator_name)), "w") as latex:
             latex.write(
                 __wilcoxon_to_latex(
                     table,
-                    caption='Wilcoxon values of the {} quality indicator ({}).'.format(indicator_name,
-                                                                                       ', '.join(problems)),
-                    label='table:{}'.format(indicator_name)
+                    caption="Wilcoxon values of the {} quality indicator ({}).".format(
+                        indicator_name, ", ".join(problems)
+                    ),
+                    label="table:{}".format(indicator_name),
                 )
             )
 
 
 def compute_mean_indicator(filename: str, indicator_name: str):
-    """ Compute the mean values of an indicator.
+    """Compute the mean values of an indicator.
     :param filename:
     :param indicator_name: Quality indicator name.
     """
     df = pd.read_csv(filename, skipinitialspace=True)
 
     if len(set(df.columns.tolist())) != 5:
-        raise Exception('Wrong number of columns')
+        raise Exception("Wrong number of columns")
 
-    algorithms = pd.unique(df['Algorithm'])
-    problems = pd.unique(df['Problem'])
+    algorithms = pd.unique(df["Algorithm"])
+    problems = pd.unique(df["Problem"])
 
     # We consider the quality indicator indicator_name
-    data = df[df['IndicatorName'] == indicator_name]
+    data = df[df["IndicatorName"] == indicator_name]
 
     # Compute for each pair algorithm/problem the average of IndicatorValue
     average_values = np.zeros((problems.size, algorithms.size))
     j = 0
     for alg in algorithms:
         i = 0
         for pr in problems:
-            average_values[i, j] = data['IndicatorValue'][np.logical_and(
-                data['Algorithm'] == alg, data['Problem'] == pr)].mean()
+            average_values[i, j] = data["IndicatorValue"][
+                np.logical_and(data["Algorithm"] == alg, data["Problem"] == pr)
+            ].mean()
             i += 1
         j += 1
 
     # Generate dataFrame from average values and order columns by name
     df = pd.DataFrame(data=average_values, index=problems, columns=algorithms)
     df = df.reindex(df.columns, axis=1)
 
     return df
 
 
-def __averages_to_latex(central_tendency: pd.DataFrame, dispersion: pd.DataFrame,
-                        caption: str, label: str, minimization=True, alignment: str = 'c'):
-    """ Convert a pandas DataFrame to a LaTeX tabular. Prints labels in bold and does use math mode.
+def generate_median_and_wilcoxon_latex_tables(filename: str, output_dir: str = "latex/meansAndWilcoxon"):
+    """Generate Latex tables including medians and IQRs. Additionally, the last algorithm is considered as the reference
+        algorithm, and the cells include a symbol indicating whether the differences with the reference algorithm
+        are significant or not according to the Wilcoxon rank sum test.
+
+    :param filename: Input filename (summary).
+    :param output_dir: Output path.
+    """
+    data = pd.read_csv(filename, skipinitialspace=True)
+
+    if len(set(data.columns.tolist())) != 5:
+        raise Exception("Wrong number of columns")
+
+    if Path(output_dir).is_dir():
+        logger.warning("Directory {} exists. Removing contents.".format(output_dir))
+        for file in os.listdir(output_dir):
+            os.remove("{0}/{1}".format(output_dir, file))
+    else:
+        logger.warning("Directory {} does not exist. Creating it.".format(output_dir))
+        Path(output_dir).mkdir(parents=True)
+
+    algorithms = pd.unique(data["Algorithm"])
+    problems = pd.unique(data["Problem"])
+    indicators = pd.unique(data["IndicatorName"])
+
+    control_algorithm = algorithms[-1]
+
+    # Compute medians and IQRs
+    medians = data.groupby(["Algorithm", "Problem", "IndicatorName"])["IndicatorValue"].median()
+    iqrs =data.groupby(["Algorithm", "Problem", "IndicatorName"])["IndicatorValue"].apply(lambda x: iqr(x))
+
+    # Create data frame to store the Wilcoxon test results
+    wilcoxon_data = pd.DataFrame(columns=["Indicator", "Algorithm", "Problem", "PValue", "Median", "TestResult"])
+
+    for indicator in indicators:
+        for algorithm in algorithms:
+            for problem in problems:
+                algorithm_data = data[(data["Problem"] == problem) & (data["Algorithm"] == algorithm) & (
+                            data["IndicatorName"] == indicator)]
+                ref_data = data[(data["Problem"] == problem) & (data["Algorithm"] == control_algorithm) & (
+                            data["IndicatorName"] == indicator)]
+                stat, p_value = mannwhitneyu(algorithm_data["IndicatorValue"], ref_data["IndicatorValue"])
+
+                test_result = ""
+                if p_value <= 0.05:
+                    if check_minimization(indicator):
+                        if medians[algorithm][problem][indicator] <= medians[control_algorithm][problem][indicator]:
+                            test_result = '+'
+                        else:
+                            test_result = '-'
+                    else:
+                        if medians[algorithm][problem][indicator] >= medians[control_algorithm][problem][indicator]:
+                            test_result = '+'
+                        else:
+                            test_result = '-'
+                else:
+                    test_result = '='
+
+
+                new_row = {'Indicator': indicator, 'Algorithm': algorithm, "Problem": problem,
+                           "PValue": p_value,
+                           "Median": medians[algorithm][problem][indicator],
+                           "IQR": iqrs[algorithm][problem][indicator],
+                           "TestResult": test_result
+                           }
+                wilcoxon_data = wilcoxon_data.append(new_row, ignore_index=True)
+
+    # Generate LaTeX tables
+    caption = "Median and interquartile range (IQR) of the results of the {} quality indicator. " + \
+            "Cells with dark and light gray background highlights, respectively, the best and second best indicator values. " +\
+              "The algorithm in the last column is the reference " +\
+              "algorithm, and the symbols $+$, $-$ and $\\approx$ indicate that the differences with the reference " + \
+              "algorithm are significantly better, worse, or there is no difference according to the Wilcoxon rank " + \
+              "sum test (confidence level: 95\%)."
+    for indicator_name in indicators:
+        with open(os.path.join(output_dir, "MedianIQRWilcoxon-{}.tex".format(indicator_name)), "w") as latex:
+            latex.write(
+                __median_wilcoxon_to_latex(
+                    indicator_name,
+                    wilcoxon_data,
+                    caption=caption.format(indicator_name),
+                    label="table:{}".format(indicator_name),
+                )
+            )
+
+def __averages_to_latex(
+    central_tendency: pd.DataFrame,
+    dispersion: pd.DataFrame,
+    caption: str,
+    label: str,
+    minimization=True,
+    alignment: str = "c",
+):
+    """Convert a pandas DataFrame to a LaTeX tabular. Prints labels in bold and does use math mode.
 
     :param caption: LaTeX table caption.
     :param label: LaTeX table label.
     :param minimization: If indicator is minimization, highlight the best values of mean/median; else, the lowest.
     """
     num_columns, num_rows = central_tendency.shape[1], central_tendency.shape[0]
     output = io.StringIO()
 
-    col_format = '{}|{}'.format(alignment, alignment * num_columns)
-    column_labels = ['\\textbf{{{0}}}'.format(label.replace('_', '\\_')) for label in central_tendency.columns]
+    col_format = "{}|{}".format(alignment, alignment * num_columns)
+    column_labels = ["\\textbf{{{0}}}".format(label.replace("_", "\\_")) for label in central_tendency.columns]
 
     # Write header
-    output.write('\\documentclass{article}\n')
+    output.write("\\documentclass{article}\n")
 
-    output.write('\\usepackage[utf8]{inputenc}\n')
-    output.write('\\usepackage{tabularx}\n')
-    output.write('\\usepackage{colortbl}\n')
-    output.write('\\usepackage[table*]{xcolor}\n')
-
-    output.write('\\xdefinecolor{gray95}{gray}{0.65}\n')
-    output.write('\\xdefinecolor{gray25}{gray}{0.8}\n')
-
-    output.write('\\title{Median and IQR}\n')
-    output.write('\\author{}\n')
-
-    output.write('\\begin{document}\n')
-    output.write('\\maketitle\n')
-
-    output.write('\\section{Table}\n')
-
-    output.write('\\begin{table}[!htp]\n')
-    output.write('  \\caption{{{}}}\n'.format(caption))
-    output.write('  \\label{{{}}}\n'.format(label))
-    output.write('  \\centering\n')
-    output.write('  \\begin{scriptsize}\n')
-    output.write('  \\begin{tabular}{%s}\n' % col_format)
-    output.write('      & {} \\\\\\hline\n'.format(' & '.join(column_labels)))
+    output.write("\\usepackage[utf8]{inputenc}\n")
+    output.write("\\usepackage{tabularx}\n")
+    output.write("\\usepackage{colortbl}\n")
+    output.write("\\usepackage[table*]{xcolor}\n")
+
+    output.write("\\xdefinecolor{gray95}{gray}{0.65}\n")
+    output.write("\\xdefinecolor{gray25}{gray}{0.8}\n")
+
+    output.write("\\title{Median and IQR}\n")
+    output.write("\\author{}\n")
+
+    output.write("\\begin{document}\n")
+    output.write("\\maketitle\n")
+
+    output.write("\\section{Table}\n")
+
+    output.write("\\begin{table}[!htp]\n")
+    output.write("  \\caption{{{}}}\n".format(caption))
+    output.write("  \\label{{{}}}\n".format(label))
+    output.write("  \\centering\n")
+    output.write("  \\begin{scriptsize}\n")
+    output.write("  \\begin{tabular}{%s}\n" % col_format)
+    output.write("      & {} \\\\\\hline\n".format(" & ".join(column_labels)))
 
     # Write data lines
     for i in range(num_rows):
-        central_values = [v for v in central_tendency.ix[i]]
-        dispersion_values = [v for v in dispersion.ix[i]]
+        central_values = [v for v in central_tendency.iloc[i]]
+        dispersion_values = [v for v in dispersion.iloc[i]]
 
         # Sort mean/median values (the lower the better if minimization)
         # Note that mean/median values could be the same: in that case, sort by Std/IQR (the lower the better)
         sorted_values = sorted(
             zip(central_values, dispersion_values, [i for i in range(len(central_values))]), key=lambda v: (v[0], -v[1])
         )
 
         if minimization:
             second_best, best = sorted_values[0][2], sorted_values[1][2]
         else:
             second_best, best = sorted_values[-1][2], sorted_values[-2][2]
 
         # Compose cell
-        values = ['{:.2e}_{{{:.2e}}}'.format(central_values[i], dispersion_values[i]) for i in
-                  range(len(central_values))]
+        values = [
+            "{:.2e}_{{{:.2e}}}".format(central_values[i], dispersion_values[i]) for i in range(len(central_values))
+        ]
 
         # Highlight values
-        values[best] = '\\cellcolor{gray25} ' + values[best]
-        values[second_best] = '\\cellcolor{gray95} ' + values[second_best]
+        values[best] = "\\cellcolor{gray25} " + values[best]
+        values[second_best] = "\\cellcolor{gray95} " + values[second_best]
 
-        output.write('      \\textbf{{{0}}} & ${1}$ \\\\\n'.format(
-            central_tendency.index[i], ' $ & $ '.join([str(val) for val in values]))
+        output.write(
+            "      \\textbf{{{0}}} & ${1}$ \\\\\n".format(
+                central_tendency.index[i], " $ & $ ".join([str(val) for val in values])
+            )
         )
 
     # Write footer
-    output.write('  \\end{tabular}\n')
-    output.write('  \\end{scriptsize}\n')
-    output.write('\\end{table}\n')
+    output.write("  \\end{tabular}\n")
+    output.write("  \\end{scriptsize}\n")
+    output.write("\\end{table}\n")
 
-    output.write('\\end{document}')
+    output.write("\\end{document}")
 
     return output.getvalue()
 
 
-def __wilcoxon_to_latex(df: pd.DataFrame, caption: str, label: str, minimization=True, alignment: str = 'c'):
-    """ Convert a pandas DataFrame to a LaTeX tabular. Prints labels in bold and does use math mode.
+def __wilcoxon_to_latex(df: pd.DataFrame, caption: str, label: str, minimization=True, alignment: str = "c"):
+    """Convert a pandas DataFrame to a LaTeX tabular. Prints labels in bold and does use math mode.
 
     :param df: Pandas dataframe.
     :param caption: LaTeX table caption.
     :param label: LaTeX table label.
     :param minimization: If indicator is minimization, highlight the best values of mean/median; else, the lowest.
     """
     num_columns, num_rows = df.shape[1], df.shape[0]
     output = io.StringIO()
 
-    col_format = '{}|{}'.format(alignment, alignment * num_columns)
-    column_labels = ['\\textbf{{{0}}}'.format(label.replace('_', '\\_')) for label in df.columns]
+    col_format = "{}|{}".format(alignment, alignment * num_columns)
+    column_labels = ["\\textbf{{{0}}}".format(label.replace("_", "\\_")) for label in df.columns]
 
     # Write header
-    output.write('\\documentclass{article}\n')
+    output.write("\\documentclass{article}\n")
 
-    output.write('\\usepackage[utf8]{inputenc}\n')
-    output.write('\\usepackage{tabularx}\n')
-    output.write('\\usepackage{amssymb}\n')
-    output.write('\\usepackage{amsmath}\n')
-
-    output.write('\\title{Wilcoxon - Mann-Whitney rank sum test}\n')
-    output.write('\\author{}\n')
-
-    output.write('\\begin{document}\n')
-    output.write('\\maketitle\n')
-
-    output.write('\\section{Table}\n')
-
-    output.write('\\begin{table}[!htp]\n')
-    output.write('  \\caption{{{}}}\n'.format(caption))
-    output.write('  \\label{{{}}}\n'.format(label))
-    output.write('  \\centering\n')
-    output.write('  \\begin{scriptsize}\n')
-    output.write('  \\begin{tabular}{%s}\n' % col_format)
-    output.write('      & {} \\\\\\hline\n'.format(' & '.join(column_labels)))
+    output.write("\\usepackage[utf8]{inputenc}\n")
+    output.write("\\usepackage{tabularx}\n")
+    output.write("\\usepackage{amssymb}\n")
+    output.write("\\usepackage{amsmath}\n")
+
+    output.write("\\title{Wilcoxon - Mann-Whitney rank sum test}\n")
+    output.write("\\author{}\n")
+
+    output.write("\\begin{document}\n")
+    output.write("\\maketitle\n")
+
+    output.write("\\section{Table}\n")
+
+    output.write("\\begin{table}[!htp]\n")
+    output.write("  \\caption{{{}}}\n".format(caption))
+    output.write("  \\label{{{}}}\n".format(label))
+    output.write("  \\centering\n")
+    output.write("  \\begin{scriptsize}\n")
+    output.write("  \\begin{tabular}{%s}\n" % col_format)
+    output.write("      & {} \\\\\\hline\n".format(" & ".join(column_labels)))
 
-    symbolo = '\\triangledown\ '
-    symbolplus = '\\blacktriangle\ '
+    symbolo = "\\triangledown\ "
+    symbolplus = "\\blacktriangle\ "
 
     if not minimization:
         symbolo, symbolplus = symbolplus, symbolo
 
     # Write data lines
     for i in range(num_rows):
-        values = [val.replace('-', '\\text{--}\ ').replace('o', symbolo).replace('+', symbolplus) for val in df.ix[i]]
-        output.write('      \\textbf{{{0}}} & ${1}$ \\\\\n'.format(
-            df.index[i], ' $ & $ '.join([str(val) for val in values]))
+        values = [val.replace("-", "\\text{--}\ ").replace("o", symbolo).replace("+", symbolplus) for val in df.iloc[i]]
+        output.write(
+            "      \\textbf{{{0}}} & ${1}$ \\\\\n".format(df.index[i], " $ & $ ".join([str(val) for val in values]))
         )
 
     # Write footer
-    output.write('  \\end{tabular}\n')
-    output.write('  \\end{scriptsize}\n')
-    output.write('\\end{table}\n')
+    output.write("  \\end{tabular}\n")
+    output.write("  \\end{scriptsize}\n")
+    output.write("\\end{table}\n")
 
-    output.write('\\end{document}')
+    output.write("\\end{document}")
 
     return output.getvalue()
 
+def __median_wilcoxon_to_latex(
+        indicator_name:str,
+        wilcoxon_data:pd.DataFrame,
+        caption:str,
+        label):
+    indicator_data = wilcoxon_data[wilcoxon_data["Indicator"] == indicator_name]
+
+    problems = pd.unique(indicator_data["Problem"])
+    algorithms = pd.unique(indicator_data["Algorithm"])
+
+    num_columns = len(algorithms)
+    columns = algorithms
+
+    alignment= "c"
+    col_format = "{}|{}".format(alignment, alignment * num_columns)
+    column_labels = ["\\textbf{{{0}}}".format(label.replace("_", "\\_")) for label in columns]
+
+    output = io.StringIO()
+
+    output.write("\\documentclass{article}\n")
+
+    output.write("\\usepackage[utf8]{inputenc}\n")
+    output.write("\\usepackage{tabularx}\n")
+    output.write("\\usepackage{colortbl}\n")
+    output.write("\\usepackage[table*]{xcolor}\n")
+
+    output.write("\\xdefinecolor{gray95}{gray}{0.65}\n")
+    output.write("\\xdefinecolor{gray25}{gray}{0.8}\n")
+
+    output.write("\\title{Median and Wilcoxon}\n")
+    output.write("\\author{}\n")
+
+    output.write("\\begin{document}\n")
+    output.write("\\maketitle\n")
+
+    output.write("\\section{Table}\n")
+
+    output.write("\\begin{table}[!htp]\n")
+    output.write("  \\caption{{{}}}\n".format(caption))
+    output.write("  \\label{{{}}}\n".format(label))
+    output.write("  \\centering\n")
+    output.write("  \\begin{tiny}\n")
+    output.write("  \\begin{tabular}{%s}\n" % col_format)
+    output.write("      & {} \\\\\\hline\n".format(" & ".join(column_labels)))
+
+    # Counts the number of times that an algorithm performs better, worse or equal than the reference algorithm
+    counters = {}
+    for algorithm in algorithms:
+        counters[algorithm] = [0, 0, 0] # best, equal, worse
+
+    for problem in problems:
+        values = []
+
+        for algorithm in algorithms:
+            row = indicator_data[(indicator_data["Problem"] == problem) & (indicator_data["Algorithm"] == algorithm)]
+            value = "{:.2e}({:.2e})".format(row["Median"].tolist()[0], row["IQR"].tolist()[0])
+
+            # Include the symbol according to the Wilcoxon rank sum test with the reference algorithm
+            if algorithm != algorithms[-1]:
+                if row["TestResult"].tolist()[0] == "-":
+                    value = "{{{}-}}".format(value)
+                    counters[algorithm][2] = counters[algorithm][2] + 1
+                elif row["TestResult"].tolist()[0] == "+":
+                    value = "{{{}+}}".format(value)
+                    counters[algorithm][0] = counters[algorithm][0] + 1
+                else:
+                    value = "{{{}\\approx}}".format(value)
+                    counters[algorithm][1] = counters[algorithm][1] + 1
+            values.append(value)
+
+        # Find the best and second best values
+        medians = indicator_data[(indicator_data["Problem"] == problem)]["Median"]
+        iqrs = indicator_data[(indicator_data["Problem"] == problem)]["IQR"]
+        pairs = list(zip(medians, iqrs))
+        indexes = sorted(range(len(pairs)), key = lambda x: pairs[x])
+
+        if check_minimization(indicator_name):
+            best = indexes[0]
+            second_best = indexes[1]
+        else:
+            best = indexes[-1]
+            second_best = indexes[-2]
+
+        values[best] = "\\cellcolor{gray95} " + values[best]
+        values[second_best] = "\\cellcolor{gray25} " + values[second_best]
+
+        output.write(
+                  "\\textbf{{{0}}} & ${1}$ \\\\\n".format(problem, " $ & $ ".join([str(val).replace("e-", "e\makebox[0.1cm]{-}").replace("e+", "e\makebox[0.1cm]{+}") for val in values])
+            )
+        )
+
+    # Select all but the last counter
+    counter_summary = []
+    for algorithm in algorithms[:-1]:
+        counter_summary.append(counters[algorithm])
+
+    output.write("  \\hline\n")
+    output.write(
+        "\\textbf{{{0}}} & ${1}$ \\\\\n".format("$+/\\approx/-$", " $ & $ ".join([str(val[0]) + "/" + str(val[1]) + "/" + str(val[2]) for val in counter_summary])))
+
+    # Write footer
+    output.write("  \\end{tabular}\n")
+    output.write("  \\end{tiny}\n")
+    output.write("\\end{table}\n")
+
+    output.write("\\end{document}")
+
+    return output.getvalue()
 
 def check_minimization(indicator) -> bool:
-    if indicator == 'HV':
+    if indicator == "HV":
         return False
     else:
         return True
```

### Comparing `jmetalpy-1.5.5/jmetal/lab/statistical_test/apv_procedures.py` & `jmetalpy-1.6.0/jmetal/lab/statistical_test/apv_procedures.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,35 +17,32 @@
     """
 
     # Initial Checking
     if type(p_values) == pd.DataFrame:
         algorithms = p_values.columns
         p_values = p_values.values
     elif type(p_values) == np.ndarray:
-        algorithms = np.array(
-            ['Alg%d' % alg for alg in range(p_values.shape[1])])
+        algorithms = np.array(["Alg%d" % alg for alg in range(p_values.shape[1])])
 
     if type(control) == str:
         control = int(np.where(algorithms == control)[0])
     if control is None:
-        raise ValueError(
-            'Initialization ERROR. Incorrect value for control.')
+        raise ValueError("Initialization ERROR. Incorrect value for control.")
 
     k = p_values.shape[1]
 
     # sort p-values p(0) <= p(1) <= ... <= p(k-1)
     argsorted_pvals = np.argsort(p_values[0, :])
 
     APVs = np.zeros((k - 1, 1))
     comparison = []
     for i in range(k - 1):
-        comparison.append(algorithms[control] +
-                          ' vs ' + algorithms[argsorted_pvals[i]])
+        comparison.append(algorithms[control] + " vs " + algorithms[argsorted_pvals[i]])
         APVs[i, 0] = np.min([(k - 1) * p_values[0, argsorted_pvals[i]], 1])
-    return pd.DataFrame(data=APVs, index=comparison, columns=['Bonferroni'])
+    return pd.DataFrame(data=APVs, index=comparison, columns=["Bonferroni"])
 
 
 def holland(p_values, control):
     """
     Holland's procedure for the adjusted p-value computation.
 
     Parameters:
@@ -59,40 +56,37 @@
     """
 
     # Initial Checking
     if type(p_values) == pd.DataFrame:
         algorithms = p_values.columns
         p_values = p_values.values
     elif type(p_values) == np.ndarray:
-        algorithms = np.array(
-            ['Alg%d' % alg for alg in range(p_values.shape[1])])
+        algorithms = np.array(["Alg%d" % alg for alg in range(p_values.shape[1])])
 
     if type(control) == str:
         control = int(np.where(algorithms == control)[0])
     if control is None:
-        raise ValueError(
-            'Initialization ERROR. Incorrect value for control.')
+        raise ValueError("Initialization ERROR. Incorrect value for control.")
 
     # --------------------------------------------------------------------------
     # ------------------------------- Procedure --------------------------------
     # --------------------------------------------------------------------------
     k = p_values.shape[1]
 
     # sort p-values p(0) <= p(1) <= ... <= p(k-1)
     argsorted_pvals = np.argsort(p_values[0, :])
 
     APVs = np.zeros((k - 1, 1))
     comparison = []
     for i in range(k - 1):
-        comparison.append(algorithms[control] +
-                          ' vs ' + algorithms[argsorted_pvals[i]])
+        comparison.append(algorithms[control] + " vs " + algorithms[argsorted_pvals[i]])
         aux = k - 1 - np.arange(i + 1)
-        v = np.max(1 - (1 - p_values[0, argsorted_pvals[:(i + 1)]]) ** aux)
+        v = np.max(1 - (1 - p_values[0, argsorted_pvals[: (i + 1)]]) ** aux)
         APVs[i, 0] = np.min([v, 1])
-    return pd.DataFrame(data=APVs, index=comparison, columns=['Holland'])
+    return pd.DataFrame(data=APVs, index=comparison, columns=["Holland"])
 
 
 def finner(p_values, control):
     """
     Finner's procedure for the adjusted p-value computation.
 
     Parameters:
@@ -106,37 +100,34 @@
     """
 
     # Initial Checking
     if type(p_values) == pd.DataFrame:
         algorithms = p_values.columns
         p_values = p_values.values
     elif type(p_values) == np.ndarray:
-        algorithms = np.array(
-            ['Alg%d' % alg for alg in range(p_values.shape[1])])
+        algorithms = np.array(["Alg%d" % alg for alg in range(p_values.shape[1])])
 
     if type(control) == str:
         control = int(np.where(algorithms == control)[0])
     if control is None:
-        raise ValueError(
-            'Initialization ERROR. Incorrect value for control.')
+        raise ValueError("Initialization ERROR. Incorrect value for control.")
 
     k = p_values.shape[1]
 
     # sort p-values p(0) <= p(1) <= ... <= p(k-1)
     argsorted_pvals = np.argsort(p_values[0, :])
 
     APVs = np.zeros((k - 1, 1))
     comparison = []
     for i in range(k - 1):
-        comparison.append(algorithms[control] +
-                          ' vs ' + algorithms[argsorted_pvals[i]])
+        comparison.append(algorithms[control] + " vs " + algorithms[argsorted_pvals[i]])
         aux = float(k - 1) / (np.arange(i + 1) + 1)
-        v = np.max(1 - (1 - p_values[0, argsorted_pvals[:(i + 1)]]) ** aux)
+        v = np.max(1 - (1 - p_values[0, argsorted_pvals[: (i + 1)]]) ** aux)
         APVs[i, 0] = np.min([v, 1])
-    return pd.DataFrame(data=APVs, index=comparison, columns=['Finner'])
+    return pd.DataFrame(data=APVs, index=comparison, columns=["Finner"])
 
 
 def hochberg(p_values, control):
     """
     Hochberg's procedure for the adjusted p-value computation.
 
     Parameters:
@@ -150,37 +141,34 @@
     """
 
     # Initial Checking
     if type(p_values) == pd.DataFrame:
         algorithms = p_values.columns
         p_values = p_values.values
     elif type(p_values) == np.ndarray:
-        algorithms = np.array(
-            ['Alg%d' % alg for alg in range(p_values.shape[1])])
+        algorithms = np.array(["Alg%d" % alg for alg in range(p_values.shape[1])])
 
     if type(control) == str:
         control = int(np.where(algorithms == control)[0])
     if control is None:
-        raise ValueError(
-            'Initialization ERROR. Incorrect value for control.')
+        raise ValueError("Initialization ERROR. Incorrect value for control.")
 
     k = p_values.shape[1]
 
     # sort p-values p(0) <= p(1) <= ... <= p(k-1)
     argsorted_pvals = np.argsort(p_values[0, :])
 
     APVs = np.zeros((k - 1, 1))
     comparison = []
     for i in range(k - 1):
-        comparison.append(algorithms[control] +
-                          ' vs ' + algorithms[argsorted_pvals[i]])
+        comparison.append(algorithms[control] + " vs " + algorithms[argsorted_pvals[i]])
         aux = np.arange(k, i, -1).astype(np.uint8)
         v = np.max(p_values[0, argsorted_pvals[aux - 1]] * (k - aux))
         APVs[i, 0] = np.min([v, 1])
-    return pd.DataFrame(data=APVs, index=comparison, columns=['Hochberg'])
+    return pd.DataFrame(data=APVs, index=comparison, columns=["Hochberg"])
 
 
 def li(p_values, control):
     """
     Li's procedure for the adjusted p-value computation.
 
     Parameters:
@@ -196,36 +184,38 @@
     """
 
     # Initial Checking
     if type(p_values) == pd.DataFrame:
         algorithms = p_values.columns
         p_values = p_values.values
     elif type(p_values) == np.ndarray:
-        algorithms = np.array(
-            ['Alg%d' % alg for alg in range(p_values.shape[1])])
+        algorithms = np.array(["Alg%d" % alg for alg in range(p_values.shape[1])])
 
     if type(control) == str:
         control = int(np.where(algorithms == control)[0])
     if control is None:
-        raise ValueError(
-            'Initialization ERROR. Incorrect value for control.')
+        raise ValueError("Initialization ERROR. Incorrect value for control.")
 
     k = p_values.shape[1]
 
     # sort p-values p(0) <= p(1) <= ... <= p(k-1)
     argsorted_pvals = np.argsort(p_values[0, :])
 
     APVs = np.zeros((k - 1, 1))
     comparison = []
     for i in range(k - 1):
-        comparison.append(algorithms[control] +
-                          ' vs ' + algorithms[argsorted_pvals[i]])
-        APVs[i, 0] = np.min([p_values[0, argsorted_pvals[-2]], p_values[0, argsorted_pvals[i]] / (
-                p_values[0, argsorted_pvals[i]] + 1 - p_values[0, argsorted_pvals[-2]])])
-    return pd.DataFrame(data=APVs, index=comparison, columns=['Li'])
+        comparison.append(algorithms[control] + " vs " + algorithms[argsorted_pvals[i]])
+        APVs[i, 0] = np.min(
+            [
+                p_values[0, argsorted_pvals[-2]],
+                p_values[0, argsorted_pvals[i]]
+                / (p_values[0, argsorted_pvals[i]] + 1 - p_values[0, argsorted_pvals[-2]]),
+            ]
+        )
+    return pd.DataFrame(data=APVs, index=comparison, columns=["Li"])
 
 
 def holm(p_values, control=None):
     """
     Holm's procedure for the adjusted p-value computation.
 
     Parameters:
@@ -241,33 +231,31 @@
     """
 
     # Initial Checking
     if type(p_values) == pd.DataFrame:
         algorithms = p_values.columns
         p_values = p_values.values
     elif type(p_values) == np.ndarray:
-        algorithms = np.array(
-            ['Alg%d' % alg for alg in range(p_values.shape[1])])
+        algorithms = np.array(["Alg%d" % alg for alg in range(p_values.shape[1])])
 
     if type(control) == str:
         control = int(np.where(algorithms == control)[0])
 
     if type(control) == int:
         k = p_values.shape[1]
 
         # sort p-values p(0) <= p(1) <= ... <= p(k-1)
         argsorted_pvals = np.argsort(p_values[0, :])
 
         APVs = np.zeros((k - 1, 1))
         comparison = []
         for i in range(k - 1):
             aux = k - 1 - np.arange(i + 1)
-            comparison.append(
-                algorithms[control] + ' vs ' + algorithms[argsorted_pvals[i]])
-            v = np.max(aux * p_values[0, argsorted_pvals[:(i + 1)]])
+            comparison.append(algorithms[control] + " vs " + algorithms[argsorted_pvals[i]])
+            v = np.max(aux * p_values[0, argsorted_pvals[: (i + 1)]])
             APVs[i, 0] = np.min([v, 1])
 
     elif control is None:
         k = p_values.shape[1]
         m = int((k * (k - 1)) / 2.0)
 
         # sort p-values p(0) <= p(1) <= ... <= p(m-1)
@@ -277,18 +265,18 @@
 
         APVs = np.zeros((m, 1))
         aux = pairs_pvals[pairs_sorted] * (m - np.arange(m))
         comparison = []
         for i in range(m):
             row = pairs_index[0][pairs_sorted[i]]
             col = pairs_index[1][pairs_sorted[i]]
-            comparison.append(algorithms[row] + ' vs ' + algorithms[col])
-            v = np.max(aux[:i + 1])
+            comparison.append(algorithms[row] + " vs " + algorithms[col])
+            v = np.max(aux[: i + 1])
             APVs[i, 0] = np.min([v, 1])
-    return pd.DataFrame(data=APVs, index=comparison, columns=['Holm'])
+    return pd.DataFrame(data=APVs, index=comparison, columns=["Holm"])
 
 
 def shaffer(p_values):
     """
     Shaffer's procedure for adjusted p_value ccmputation.
 
     Parameters:
@@ -316,32 +304,28 @@
         """
 
         from scipy.special import binom as binomial
 
         TrueHset = [0]
         if k > 1:
             for j in np.arange(k, 0, -1, dtype=int):
-                TrueHset = list(set(TrueHset) | set(
-                    [binomial(j, 2) + x for x in S(k - j)]))
+                TrueHset = list(set(TrueHset) | set([binomial(j, 2) + x for x in S(k - j)]))
         return TrueHset
 
     # Initial Checking
     if type(p_values) == pd.DataFrame:
         algorithms = p_values.columns
         p_values = p_values.values
     elif type(p_values) == np.ndarray:
-        algorithms = np.array(
-            ['Alg%d' % alg for alg in range(p_values.shape[1])])
+        algorithms = np.array(["Alg%d" % alg for alg in range(p_values.shape[1])])
 
     if p_values.ndim != 2:
-        raise ValueError(
-            'Initialization ERROR. Incorrect number of array dimensions.')
+        raise ValueError("Initialization ERROR. Incorrect number of array dimensions.")
     elif p_values.shape[0] != p_values.shape[1]:
-        raise ValueError(
-            'Initialization ERROR. Incorrect number of array dimensions.')
+        raise ValueError("Initialization ERROR. Incorrect number of array dimensions.")
 
     # define parameters
     k = p_values.shape[0]
     m = int(k * (k - 1) / 2.0)
     s = np.array(S(k)[1:])
 
     # sort p-values p(0) <= p(1) <= ... <= p(m-1)
@@ -352,23 +336,23 @@
     # compute ti: max number of hypotheses that can be true given that any
     # (i-1) hypotheses are false.
     t = np.sort(-np.repeat(s[:-1], (s[1:] - s[:-1]).astype(np.uint8)))
     t = np.insert(-t, 0, s[-1])
 
     # Adjust p-values
     APVs = np.zeros((m, 1))
-    aux = (pairs_pvals[pairs_sorted] * t)
+    aux = pairs_pvals[pairs_sorted] * t
     comparison = []
     for i in range(m):
         row = pairs_index[0][pairs_sorted[i]]
         col = pairs_index[1][pairs_sorted[i]]
-        comparison.append(algorithms[row] + ' vs ' + algorithms[col])
-        v = np.max(aux[:i + 1])
+        comparison.append(algorithms[row] + " vs " + algorithms[col])
+        v = np.max(aux[: i + 1])
         APVs[i, 0] = np.min([v, 1])
-    return pd.DataFrame(data=APVs, index=comparison, columns=['Shaffer'])
+    return pd.DataFrame(data=APVs, index=comparison, columns=["Shaffer"])
 
 
 def nemenyi(p_values):
     """
     Nemenyi's procedure for adjusted p_value computation.
 
     Parameters:
@@ -381,23 +365,20 @@
     """
 
     # Initial Checking
     if type(p_values) == pd.DataFrame:
         algorithms = p_values.columns
         p_values = p_values.values
     elif type(p_values) == np.ndarray:
-        algorithms = np.array(
-            ['Alg%d' % alg for alg in range(p_values.shape[1])])
+        algorithms = np.array(["Alg%d" % alg for alg in range(p_values.shape[1])])
 
     if p_values.ndim != 2:
-        raise ValueError(
-            'Initialization ERROR. Incorrect number of array dimensions.')
+        raise ValueError("Initialization ERROR. Incorrect number of array dimensions.")
     elif p_values.shape[0] != p_values.shape[1]:
-        raise ValueError(
-            'Initialization ERROR. Incorrect number of array dimensions.')
+        raise ValueError("Initialization ERROR. Incorrect number of array dimensions.")
 
     # define parameters
     k = p_values.shape[0]
     m = int(k * (k - 1) / 2.0)
 
     # sort p-values p(0) <= p(1) <= ... <= p(m-1)
     pairs_index = np.triu_indices(k, 1)
@@ -406,10 +387,10 @@
 
     # Adjust p-values
     APVs = np.zeros((m, 1))
     comparison = []
     for i in range(m):
         row = pairs_index[0][pairs_sorted[i]]
         col = pairs_index[1][pairs_sorted[i]]
-        comparison.append(algorithms[row] + ' vs ' + algorithms[col])
+        comparison.append(algorithms[row] + " vs " + algorithms[col])
         APVs[i, 0] = np.min([pairs_pvals[pairs_sorted[i]] * m, 1])
-    return pd.DataFrame(data=APVs, index=comparison, columns=['Nemenyi'])
+    return pd.DataFrame(data=APVs, index=comparison, columns=["Nemenyi"])
```

### Comparing `jmetalpy-1.5.5/jmetal/lab/statistical_test/bayesian.py` & `jmetalpy-1.6.0/jmetal/lab/statistical_test/bayesian.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import numpy as np
 import pandas as pd
 
 
-def bayesian_sign_test(data, rope_limits=[-0.01, 0.01], prior_strength=0.5, prior_place='rope', sample_size=50000,
-                       return_sample=False):
-    """ Bayesian version of the sign test.
+def bayesian_sign_test(
+    data, rope_limits=[-0.01, 0.01], prior_strength=0.5, prior_place="rope", sample_size=50000, return_sample=False
+):
+    """Bayesian version of the sign test.
 
     :param data: An (n x 2) array or DataFrame contaning the results. In data, each column represents an algorithm and, and each row a problem.
     :param rope_limits: array_like. Default [-0.01, 0.01]. Limits of the practical equivalence.
     :param prior_strength: positive float. Default 0.5. Value of the prior strengt
     :param prior_place: string {left, rope, right}. Default 'left'. Place of the pseudo-observation z_0.
     :param sample_size: integer. Default 10000. Total number of random_search samples generated
     :param return_sample: boolean. Default False. If true, also return the samples drawn from the Dirichlet process.
@@ -23,24 +24,21 @@
     if type(data) == pd.DataFrame:
         data = data.values
 
     if data.shape[1] == 2:
         sample1, sample2 = data[:, 0], data[:, 1]
         n = data.shape[0]
     else:
-        raise ValueError(
-            'Initialization ERROR. Incorrect number of dimensions for axis 1')
+        raise ValueError("Initialization ERROR. Incorrect number of dimensions for axis 1")
 
     if prior_strength <= 0:
-        raise ValueError(
-            'Initialization ERROR. prior_strength mustb be a positive float')
+        raise ValueError("Initialization ERROR. prior_strength mustb be a positive float")
 
-    if prior_place not in ['left', 'rope', 'right']:
-        raise ValueError(
-            'Initialization ERROR. Incorrect value fro prior_place')
+    if prior_place not in ["left", "rope", "right"]:
+        raise ValueError("Initialization ERROR. Incorrect value fro prior_place")
 
     # Compute the differences
     Z = sample1 - sample2
 
     # Compute the number of pairs diff > right_limit
     Nright = sum(Z > rope_limits[1])
     # Compute the number of pairs diff < right_lelft
@@ -49,15 +47,15 @@
     Nequiv = n - Nright - Nleft
 
     # compute the the probabilities that the mean difference of accuracy is in
     # the interval (−Inf, left), [left, right], or (ringth, Inf).
 
     # Parameters of the Dirichlet distribution
     alpha = np.array([Nleft, Nequiv, Nright], dtype=float) + 1e-6
-    alpha[['left', 'rope', 'right'].index(prior_place)] += prior_strength
+    alpha[["left", "rope", "right"].index(prior_place)] += prior_strength
     # Simulate dirichlet process
     Dprocess = np.random.dirichlet(alpha, sample_size)
 
     # Compute posterior probabilities
     winner_id = np.argmax(Dprocess, axis=1)
     win_left = sum(winner_id == 0)
     win_rifht = sum(winner_id == 2)
@@ -65,18 +63,18 @@
 
     if return_sample is True:
         return np.array([win_left, win_rope, win_rifht]) / float(sample_size), Dprocess
     else:
         return np.array([win_left, win_rope, win_rifht]) / float(sample_size)
 
 
-def bayesian_signed_rank_test(data, rope_limits=[-0.01, 0.01], prior_strength=1.0, prior_place='rope',
-                              sample_size=10000,
-                              return_sample=False):
-    """ Bayesian version of the signed rank test.
+def bayesian_signed_rank_test(
+    data, rope_limits=[-0.01, 0.01], prior_strength=1.0, prior_place="rope", sample_size=10000, return_sample=False
+):
+    """Bayesian version of the signed rank test.
 
     :param data: An (n x 2) array or DataFrame contaning the results. In data, each column represents an algorithm and, and each row a problem.
     :param rope_limits: array_like. Default [-0.01, 0.01]. Limits of the practical equivalence.
     :param prior_strength: positive float. Default 0.5. Value of the prior strengt
     :param prior_place: string {left, rope, right}. Default 'left'. Place of the pseudo-observation z_0.
     :param sample_size: integer. Default 10000. Total number of random_search samples generated
     :param return_sample: boolean. Default False. If true, also return the samples drawn from the Dirichlet process.
@@ -94,29 +92,25 @@
     if type(data) == pd.DataFrame:
         data = data.values
 
     if data.shape[1] == 2:
         sample1, sample2 = data[:, 0], data[:, 1]
         n = data.shape[0]
     else:
-        raise ValueError(
-            'Initialization ERROR. Incorrect number of dimensions for axis 1')
+        raise ValueError("Initialization ERROR. Incorrect number of dimensions for axis 1")
 
     if prior_strength <= 0:
-        raise ValueError(
-            'Initialization ERROR. prior_strength must be a positive float')
+        raise ValueError("Initialization ERROR. prior_strength must be a positive float")
 
-    if prior_place not in ['left', 'rope', 'right']:
-        raise ValueError(
-            'Initialization ERROR. Incorrect value for prior_place')
+    if prior_place not in ["left", "rope", "right"]:
+        raise ValueError("Initialization ERROR. Incorrect value for prior_place")
 
     # Compute the differences
     Z = sample1 - sample2
-    Z0 = [-float('Inf'), 0.0, float('Inf')][['left',
-                                             'rope', 'right'].index(prior_place)]
+    Z0 = [-float("Inf"), 0.0, float("Inf")][["left", "rope", "right"].index(prior_place)]
     Z = np.concatenate(([Z0], Z), axis=None)
 
     # compute the the probabilities that the mean difference of accuracy is in
     # the interval (−Inf, left), [left, right], or (ringth, Inf).
 
     Dprocess = np.zeros((sample_size, 3))
     for mc in range(sample_size):
```

### Comparing `jmetalpy-1.5.5/jmetal/lab/statistical_test/critical_distance.py` & `jmetalpy-1.6.0/jmetal/lab/statistical_test/critical_distance.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from matplotlib import pyplot as plt
 from statsmodels.stats.libqsturng import qsturng
 
 from jmetal.lab.statistical_test.functions import ranks
 
 
 def NemenyiCD(alpha: float, num_alg, num_dataset):
-    """ Computes Nemenyi's critical difference:
+    """Computes Nemenyi's critical difference:
     * CD = q_alpha * sqrt(num_alg*(num_alg + 1)/(6*num_prob))
     where q_alpha is the critical value, of the Studentized range statistic divided by sqrt(2).
     :param alpha: {0.1, 0.999}. Significance level.
     :param num_alg: number of tested algorithms.
     :param num_dataset: Number of problems/datasets where the algorithms have been tested.
     """
 
@@ -20,32 +20,37 @@
 
     # compute the critical difference
     cd = q_alpha * np.sqrt(num_alg * (num_alg + 1) / (6.0 * num_dataset))
 
     return cd
 
 
-def CDplot(results, alpha: float = 0.05, higher_is_better: bool=False, alg_names: list = None, output_filename: str = 'cdplot.eps'):
-    """ CDgraph plots the critical difference graph show in Janez Demsar's 2006 work:
+def CDplot(
+    results,
+    alpha: float = 0.05,
+    higher_is_better: bool = False,
+    alg_names: list = None,
+    output_filename: str = "cdplot.eps",
+):
+    """CDgraph plots the critical difference graph show in Janez Demsar's 2006 work:
     * Statistical Comparisons of Classifiers over Multiple Data Sets.
     :param results: A 2-D array containing results from each algorithm. Each row of 'results' represents an algorithm, and each column a dataset.
     :param alpha: {0.1, 0.999}. Significance level for the critical difference.
     :param alg_names: Names of the tested algorithms.
     """
 
     def _join_alg(avranks, num_alg, cd):
         """
         join_alg returns the set of non significant methods
         """
 
         # get all pairs
         sets = (-1) * np.ones((num_alg, 2))
         for i in range(num_alg):
-            elements = np.where(np.logical_and(
-                avranks - avranks[i] > 0, avranks - avranks[i] < cd))[0]
+            elements = np.where(np.logical_and(avranks - avranks[i] > 0, avranks - avranks[i] < cd))[0]
             if elements.size > 0:
                 sets[i, :] = [avranks[i], avranks[elements[-1]]]
         sets = np.delete(sets, np.where(sets[:, 0] < 0)[0], axis=0)
 
         # group pairs
         group = sets[0, :]
         for i in range(1, sets.shape[0]):
@@ -55,22 +60,20 @@
         return group
 
     # Initial Checking
     if type(results) == pd.DataFrame:
         alg_names = results.index
         results = results.values
     elif type(results) == np.ndarray and alg_names is None:
-        alg_names = np.array(
-            ['Alg%d' % alg for alg in range(results.shape[1])])
+        alg_names = np.array(["Alg%d" % alg for alg in range(results.shape[1])])
 
     if results.ndim == 2:
         num_alg, num_dataset = results.shape
     else:
-        raise ValueError(
-            'Initialization ERROR: In CDplot(...) results must be 2-D array')
+        raise ValueError("Initialization ERROR: In CDplot(...) results must be 2-D array")
 
     # Get the critical difference
     cd = NemenyiCD(alpha, num_alg, num_dataset)
 
     # Compute ranks. (ranks[i][j] rank of the i-th algorithm on the j-th problem.)
 
     rranks = ranks(results.T, descending=higher_is_better)
@@ -86,15 +89,15 @@
     rightalg = avranks[spoint:]
     rows = np.ceil(num_alg / 2.0).astype(np.uint8)
 
     # Figure settings.
     highest = np.ceil(np.max(avranks)).astype(np.uint8)  # highest shown rank
     lowest = np.floor(np.min(avranks)).astype(np.uint8)  # lowest shown rank
     width = 6  # default figure width (in inches)
-    height = (0.575 * (rows + 1))  # figure height
+    height = 0.575 * (rows + 1)  # figure height
 
     """
                         FIGURE
       (1,0)
         +-----+---------------------------+-------+
         |     |                           |       |
         |     |                           |       |
@@ -114,95 +117,116 @@
 
     stop, sbottom, sleft, sright = 0.65, 0.1, 0.15, 0.85
 
     # main horizontal axis length
     lline = sright - sleft
 
     # Initialize figure
-    fig = plt.figure(figsize=(width, height), facecolor='white')
+    fig = plt.figure(figsize=(width, height), facecolor="white")
     ax = fig.add_axes([0, 0, 1, 1])
     ax.set_xlim(0, 1)
     ax.set_ylim(0, 1)
     ax.set_axis_off()
 
     # Main horizontal axis
-    ax.hlines(stop, sleft, sright, color='black', linewidth=0.7)
+    ax.hlines(stop, sleft, sright, color="black", linewidth=0.7)
     for xi in range(highest - lowest + 1):
         # Plot mayor ticks
-        ax.vlines(x=sleft + (lline * xi) / (highest - lowest),
-                  ymin=stop, ymax=stop + 0.05, color='black', linewidth=0.7)
+        ax.vlines(
+            x=sleft + (lline * xi) / (highest - lowest), ymin=stop, ymax=stop + 0.05, color="black", linewidth=0.7
+        )
         # Mayor ticks labels
-        ax.text(x=sleft + (lline * xi) / (highest - lowest),
-                y=stop + 0.06,
-                s=str(lowest + xi), ha='center', va='bottom')
+        ax.text(
+            x=sleft + (lline * xi) / (highest - lowest), y=stop + 0.06, s=str(lowest + xi), ha="center", va="bottom"
+        )
         # Minor ticks
         if xi < highest - lowest:
-            ax.vlines(x=sleft + (lline * (xi + 0.5)) / (highest - lowest),
-                      ymin=stop, ymax=stop + 0.025, color='black', linewidth=0.7)
+            ax.vlines(
+                x=sleft + (lline * (xi + 0.5)) / (highest - lowest),
+                ymin=stop,
+                ymax=stop + 0.025,
+                color="black",
+                linewidth=0.7,
+            )
 
     # Plot lines/names for left models
     vspace = 0.5 * (stop - sbottom) / (spoint + 1)
     for i in range(spoint):
-        ax.vlines(x=sleft + (lline * (leftalg[i] - lowest)) / (highest - lowest),
-                  ymin=sbottom + (spoint - 1 - i) * vspace, ymax=stop, color='black', linewidth=0.7)
-        ax.hlines(y=sbottom + (spoint - 1 - i) * vspace, xmin=sleft,
-                  xmax=sleft +
-                       (lline * (leftalg[i] - lowest)) / (highest - lowest),
-                  color='black', linewidth=0.7)
-        ax.text(x=sleft - 0.01, y=sbottom + (spoint - 1 - i) * vspace,
-                s=alg_names[indices][i], ha='right', va='center')
+        ax.vlines(
+            x=sleft + (lline * (leftalg[i] - lowest)) / (highest - lowest),
+            ymin=sbottom + (spoint - 1 - i) * vspace,
+            ymax=stop,
+            color="black",
+            linewidth=0.7,
+        )
+        ax.hlines(
+            y=sbottom + (spoint - 1 - i) * vspace,
+            xmin=sleft,
+            xmax=sleft + (lline * (leftalg[i] - lowest)) / (highest - lowest),
+            color="black",
+            linewidth=0.7,
+        )
+        ax.text(x=sleft - 0.01, y=sbottom + (spoint - 1 - i) * vspace, s=alg_names[indices][i], ha="right", va="center")
 
     # Plot lines/names for right models
     vspace = 0.5 * (stop - sbottom) / (num_alg - spoint + 1)
     for i in range(num_alg - spoint):
-        ax.vlines(x=sleft + (lline * (rightalg[i] - lowest)) / (highest - lowest),
-                  ymin=sbottom + i * vspace, ymax=stop, color='black', linewidth=0.7)
-        ax.hlines(y=sbottom + i * vspace,
-                  xmin=sleft +
-                       (lline * (rightalg[i] - lowest)) / (highest - lowest),
-                  xmax=sright, color='black', linewidth=0.7)
-        ax.text(x=sright + 0.01, y=sbottom + i * vspace,
-                s=alg_names[indices][spoint + i], ha='left', va='center')
+        ax.vlines(
+            x=sleft + (lline * (rightalg[i] - lowest)) / (highest - lowest),
+            ymin=sbottom + i * vspace,
+            ymax=stop,
+            color="black",
+            linewidth=0.7,
+        )
+        ax.hlines(
+            y=sbottom + i * vspace,
+            xmin=sleft + (lline * (rightalg[i] - lowest)) / (highest - lowest),
+            xmax=sright,
+            color="black",
+            linewidth=0.7,
+        )
+        ax.text(x=sright + 0.01, y=sbottom + i * vspace, s=alg_names[indices][spoint + i], ha="left", va="center")
 
     # Plot critical difference rule
     if sleft + (cd * lline) / (highest - lowest) <= sright:
-        ax.hlines(y=stop + 0.2, xmin=sleft, xmax=sleft +
-                                                 (cd * lline) / (highest - lowest), linewidth=1.5)
-        ax.text(x=sleft + 0.5 * (cd * lline) /
-                  (highest - lowest), y=stop + 0.21, s='CD=%.3f' % cd, ha='center', va='bottom')
+        ax.hlines(y=stop + 0.2, xmin=sleft, xmax=sleft + (cd * lline) / (highest - lowest), linewidth=1.5)
+        ax.text(
+            x=sleft + 0.5 * (cd * lline) / (highest - lowest), y=stop + 0.21, s="CD=%.3f" % cd, ha="center", va="bottom"
+        )
     else:
-        ax.text(x=(sleft + sright) / 2, y=stop + 0.2, s='CD=%.3f' %
-                                                        cd, ha='center', va='bottom')
+        ax.text(x=(sleft + sright) / 2, y=stop + 0.2, s="CD=%.3f" % cd, ha="center", va="bottom")
 
     # Get pair of non-significant methods
     nonsig = _join_alg(avranks, num_alg, cd)
     if nonsig.ndim == 2:
         if nonsig.shape[0] == 2:
             left_lines = np.reshape(nonsig[0, :], (1, 2))
             right_lines = np.reshape(nonsig[1, :], (1, 2))
         else:
-            left_lines = nonsig[:np.round(
-                nonsig.shape[0] / 2.0).astype(np.uint8), :]
-            right_lines = nonsig[np.round(
-                nonsig.shape[0] / 2.0).astype(np.uint8):, :]
+            left_lines = nonsig[: np.round(nonsig.shape[0] / 2.0).astype(np.uint8), :]
+            right_lines = nonsig[np.round(nonsig.shape[0] / 2.0).astype(np.uint8) :, :]
     else:
         left_lines = np.reshape(nonsig, (1, nonsig.shape[0]))
 
     # plot from the left
     vspace = 0.5 * (stop - sbottom) / (left_lines.shape[0] + 1)
     for i in range(left_lines.shape[0]):
-        ax.hlines(y=stop - (i + 1) * vspace,
-                  xmin=sleft + lline * (left_lines[i, 0] -
-                                        lowest - 0.025) / (highest - lowest),
-                  xmax=sleft + lline * (left_lines[i, 1] - lowest + 0.025) / (highest - lowest), linewidth=2)
+        ax.hlines(
+            y=stop - (i + 1) * vspace,
+            xmin=sleft + lline * (left_lines[i, 0] - lowest - 0.025) / (highest - lowest),
+            xmax=sleft + lline * (left_lines[i, 1] - lowest + 0.025) / (highest - lowest),
+            linewidth=2,
+        )
 
     # plot from the rigth
     if nonsig.ndim == 2:
         vspace = 0.5 * (stop - sbottom) / (left_lines.shape[0])
         for i in range(right_lines.shape[0]):
-            ax.hlines(y=stop - (i + 1) * vspace,
-                      xmin=sleft + lline * (right_lines[i, 0] -
-                                            lowest - 0.025) / (highest - lowest),
-                      xmax=sleft + lline * (right_lines[i, 1] - lowest + 0.025) / (highest - lowest), linewidth=2)
+            ax.hlines(
+                y=stop - (i + 1) * vspace,
+                xmin=sleft + lline * (right_lines[i, 0] - lowest - 0.025) / (highest - lowest),
+                xmax=sleft + lline * (right_lines[i, 1] - lowest + 0.025) / (highest - lowest),
+                linewidth=2,
+            )
 
-    plt.savefig(output_filename, bbox_inches='tight')
+    plt.savefig(output_filename, bbox_inches="tight")
     plt.show()
```

### Comparing `jmetalpy-1.5.5/jmetal/lab/statistical_test/functions.py` & `jmetalpy-1.6.0/jmetal/lab/statistical_test/functions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,47 @@
-from scipy.stats import chi2, f, binom, norm
+from scipy.stats import binom, chi2, f, norm
 
 from jmetal.lab.statistical_test.apv_procedures import *
 
 
 def ranks(data: np.array, descending=False):
-    """ Computes the rank of the elements in data.
+    """Computes the rank of the elements in data.
 
     :param data: 2-D matrix
     :param descending: boolean (default False). If true, rank is sorted in descending order.
     :return: ranks, where ranks[i][j] == rank of the i-th row w.r.t the j-th column.
     """
     s = 0 if (descending is False) else 1
 
     # Compute ranks. (ranks[i][j] == rank of the i-th treatment on the j-th sample.)
     if data.ndim == 2:
         ranks = np.ones(data.shape)
         for i in range(data.shape[0]):
             values, indices, rep = np.unique(
-                (-1) ** s * np.sort((-1) ** s * data[i, :]), return_index=True, return_counts=True, )
+                (-1) ** s * np.sort((-1) ** s * data[i, :]),
+                return_index=True,
+                return_counts=True,
+            )
             for j in range(data.shape[1]):
-                ranks[i, j] += indices[values == data[i, j]] + \
-                               0.5 * (rep[values == data[i, j]] - 1)
+                ranks[i, j] += indices[values == data[i, j]] + 0.5 * (rep[values == data[i, j]] - 1)
         return ranks
     elif data.ndim == 1:
         ranks = np.ones((data.size,))
         values, indices, rep = np.unique(
-            (-1) ** s * np.sort((-1) ** s * data), return_index=True, return_counts=True, )
+            (-1) ** s * np.sort((-1) ** s * data),
+            return_index=True,
+            return_counts=True,
+        )
         for i in range(data.size):
-            ranks[i] += indices[values == data[i]] + \
-                        0.5 * (rep[values == data[i]] - 1)
+            ranks[i] += indices[values == data[i]] + 0.5 * (rep[values == data[i]] - 1)
         return ranks
 
 
 def sign_test(data):
-    """ Given the results drawn from two algorithms/methods X and Y, the sign test analyses if
+    """Given the results drawn from two algorithms/methods X and Y, the sign test analyses if
     there is a difference between X and Y.
 
     .. note:: Null Hypothesis: Pr(X<Y)= 0.5
 
     :param data: An (n x 2) array or DataFrame contaning the results. In data, each column represents an algorithm and, and each row a problem.
     :return p_value: The associated p-value from the binomial distribution.
     :return bstat: Number of successes.
@@ -46,16 +50,15 @@
     if type(data) == pd.DataFrame:
         data = data.values
 
     if data.shape[1] == 2:
         X, Y = data[:, 0], data[:, 1]
         n_perf = data.shape[0]
     else:
-        raise ValueError(
-            'Initialization ERROR. Incorrect number of dimensions for axis 1')
+        raise ValueError("Initialization ERROR. Incorrect number of dimensions for axis 1")
 
     # Compute the differences
     Z = X - Y
     # Compute the number of pairs Z<0
     Wminus = sum(Z < 0)
     # If H_0 is true ---> W follows Binomial(n,0.5)
     p_value_minus = 1 - binom.cdf(k=Wminus, p=0.5, n=n_perf)
@@ -63,20 +66,21 @@
     # Compute the number of pairs Z>0
     Wplus = sum(Z > 0)
     # If H_0 is true ---> W follows Binomial(n,0.5)
     p_value_plus = 1 - binom.cdf(k=Wplus, p=0.5, n=n_perf)
 
     p_value = 2 * min([p_value_minus, p_value_plus])
 
-    return pd.DataFrame(data=np.array([Wminus, Wplus, p_value]), index=['Num X<Y', 'Num X>Y', 'p-value'],
-                        columns=['Results'])
+    return pd.DataFrame(
+        data=np.array([Wminus, Wplus, p_value]), index=["Num X<Y", "Num X>Y", "p-value"], columns=["Results"]
+    )
 
 
 def friedman_test(data):
-    """ Friedman ranking test.
+    """Friedman ranking test.
 
     ..note:: Null Hypothesis: In a set of k (>=2) treaments (or tested algorithms), all the treatments are equivalent, so their average ranks should be equal.
 
     :param data: An (n x 2) array or DataFrame contaning the results. In data, each column represents an algorithm and, and each row a problem.
     :return p_value: The associated p-value.
     :return friedman_stat: Friedman's chi-square.
     """
@@ -84,39 +88,37 @@
     # Initial Checking
     if type(data) == pd.DataFrame:
         data = data.values
 
     if data.ndim == 2:
         n_samples, k = data.shape
     else:
-        raise ValueError(
-            'Initialization ERROR. Incorrect number of array dimensions')
+        raise ValueError("Initialization ERROR. Incorrect number of array dimensions")
     if k < 2:
-        raise ValueError(
-            'Initialization Error. Incorrect number of dimensions for axis 1.')
+        raise ValueError("Initialization Error. Incorrect number of dimensions for axis 1.")
 
     # Compute ranks.
     datarank = ranks(data)
 
     # Compute for each algorithm the ranking average.
     avranks = np.mean(datarank, axis=0)
 
     # Get Friedman statistics
-    friedman_stat = (12.0 * n_samples) / (k * (k + 1.0)) * \
-                    (np.sum(avranks ** 2) - (k * (k + 1) ** 2) / 4.0)
+    friedman_stat = (12.0 * n_samples) / (k * (k + 1.0)) * (np.sum(avranks**2) - (k * (k + 1) ** 2) / 4.0)
 
     # Compute p-value
-    p_value = (1.0 - chi2.cdf(friedman_stat, df=(k - 1)))
+    p_value = 1.0 - chi2.cdf(friedman_stat, df=(k - 1))
 
-    return pd.DataFrame(data=np.array([friedman_stat, p_value]), index=['Friedman-statistic', 'p-value'],
-                        columns=['Results'])
+    return pd.DataFrame(
+        data=np.array([friedman_stat, p_value]), index=["Friedman-statistic", "p-value"], columns=["Results"]
+    )
 
 
 def friedman_aligned_rank_test(data):
-    """ Method of aligned ranks for the Friedman test.
+    """Method of aligned ranks for the Friedman test.
 
     ..note:: Null Hypothesis: In a set of k (>=2) treaments (or tested algorithms), all the treatments are equivalent, so their average ranks should be equal.
 
     :param data: An (n x 2) array or DataFrame contaning the results. In data, each column represents an algorithm and, and each row a problem.
     :return p_value: The associated p-value.
     :return aligned_rank_stat: Friedman's aligned rank chi-square statistic.
     """
@@ -124,47 +126,46 @@
     # Initial Checking
     if type(data) == pd.DataFrame:
         data = data.values
 
     if data.ndim == 2:
         n_samples, k = data.shape
     else:
-        raise ValueError(
-            'Initialization ERROR. Incorrect number of array dimensions')
+        raise ValueError("Initialization ERROR. Incorrect number of array dimensions")
     if k < 2:
-        raise ValueError(
-            'Initialization Error. Incorrect number of dimensions for axis 1.')
+        raise ValueError("Initialization Error. Incorrect number of dimensions for axis 1.")
 
     # Compute the average value achieved by all algorithms in each problem
     control = np.mean(data, axis=1)
     # Compute the difference between control an data
     diff = [data[:, j] - control for j in range(data.shape[1])]
     # rank diff
     alignedRanks = ranks(np.ravel(diff))
-    alignedRanks = np.reshape(alignedRanks, newshape=(n_samples, k), order='F')
+    alignedRanks = np.reshape(alignedRanks, newshape=(n_samples, k), order="F")
 
     # Compute statistic
     Rhat_i = np.sum(alignedRanks, axis=1)
     Rhat_j = np.sum(alignedRanks, axis=0)
-    si, sj = np.sum(Rhat_i ** 2), np.sum(Rhat_j ** 2)
+    si, sj = np.sum(Rhat_i**2), np.sum(Rhat_j**2)
 
-    A = sj - (k * n_samples ** 2 / 4.0) * (k * n_samples + 1) ** 2
-    B1 = (k * n_samples * (k * n_samples + 1) * (2 * k * n_samples + 1) / 6.0)
+    A = sj - (k * n_samples**2 / 4.0) * (k * n_samples + 1) ** 2
+    B1 = k * n_samples * (k * n_samples + 1) * (2 * k * n_samples + 1) / 6.0
     B2 = si / float(k)
 
     alignedRanks_stat = ((k - 1) * A) / (B1 - B2)
 
     p_value = 1 - chi2.cdf(alignedRanks_stat, df=k - 1)
 
-    return pd.DataFrame(data=np.array([alignedRanks_stat, p_value]), index=['Aligned Rank stat', 'p-value'],
-                        columns=['Results'])
+    return pd.DataFrame(
+        data=np.array([alignedRanks_stat, p_value]), index=["Aligned Rank stat", "p-value"], columns=["Results"]
+    )
 
 
 def quade_test(data):
-    """ Quade test.
+    """Quade test.
 
     ..note:: Null Hypothesis: In a set of k (>=2) treaments (or tested algorithms), all the treatments are equivalent, so their average ranks should be equal.
 
     :param data: An (n x 2) array or DataFrame contaning the results. In data, each column represents an algorithm and, and each row a problem.
     :return p_value: The associated p-value from the F-distribution.
     :return fq: Computed F-value.
     """
@@ -172,19 +173,17 @@
     # Initial Checking
     if type(data) == pd.DataFrame:
         data = data.values
 
     if data.ndim == 2:
         n_samples, k = data.shape
     else:
-        raise ValueError(
-            'Initialization ERROR. Incorrect number of array dimensions')
+        raise ValueError("Initialization ERROR. Incorrect number of array dimensions")
     if k < 2:
-        raise ValueError(
-            'Initialization Error. Incorrect number of dimensions for axis 1.')
+        raise ValueError("Initialization Error. Incorrect number of dimensions for axis 1.")
 
     # Compute ranks.
     datarank = ranks(data)
     # Compute the range of each problem
     problemRange = np.max(data, axis=1) - np.min(data, axis=1)
     # Compute problem rank
     problemRank = ranks(problemRange)
@@ -193,29 +192,29 @@
     # the significance of the problem when it appears.
     S_stat = np.zeros((n_samples, k))
     for i in range(n_samples):
         S_stat[i, :] = problemRank[i] * (datarank[i, :] - 0.5 * (k + 1))
     Salg = np.sum(S_stat, axis=0)
 
     # Compute Fq (Quade Test statistic) and associated p_value
-    A = np.sum(S_stat ** 2)
-    B = np.sum(Salg ** 2) / float(n_samples)
+    A = np.sum(S_stat**2)
+    B = np.sum(Salg**2) / float(n_samples)
 
     if A == B:
         Fq = np.Inf
         p_value = (1 / (np.math.factorial(k))) ** (n_samples - 1)
     else:
         Fq = (n_samples - 1.0) * B / (A - B)
         p_value = 1 - f.cdf(Fq, k - 1, (k - 1) * (n_samples - 1))
 
-    return pd.DataFrame(data=np.array([Fq, p_value]), index=['Quade Test statistic', 'p-value'], columns=['Results'])
+    return pd.DataFrame(data=np.array([Fq, p_value]), index=["Quade Test statistic", "p-value"], columns=["Results"])
 
 
 def friedman_ph_test(data, control=None, apv_procedure=None):
-    """ Friedman post-hoc test.
+    """Friedman post-hoc test.
 
     :param data: An (n x 2) array or DataFrame contaning the results. In data, each column represents an algorithm and, and each row a problem.
     :param control: optional int or string. Default None. Index or Name of the control algorithm. If control = None all FriedmanPosHocTest considers all possible comparisons among algorithms.
     :param apv_procedure: optional string. Default None.
         Name of the procedure for computing adjusted p-values. If apv_procedure
         is None, adjusted p-value are not computed, else the values are computed
         according to the specified procedure:
@@ -229,44 +228,49 @@
     """
 
     # Initial Checking
     if type(data) == pd.DataFrame:
         algorithms = data.columns
         data = data.values
     elif type(data) == np.ndarray:
-        algorithms = np.array(['Alg%d' % alg for alg in range(data.shape[1])])
+        algorithms = np.array(["Alg%d" % alg for alg in range(data.shape[1])])
 
     if control is None:
         index = algorithms
     elif type(control) == int:
         index = [algorithms[control]]
     else:
         index = [control]
 
     if data.ndim == 2:
         n_samples, k = data.shape
     else:
-        raise ValueError(
-            'Initialization ERROR. Incorrect number of array dimensions.')
+        raise ValueError("Initialization ERROR. Incorrect number of array dimensions.")
     if k < 2:
-        raise ValueError(
-            'Initialization Error. Incorrect number of dimensions for axis 1.')
+        raise ValueError("Initialization Error. Incorrect number of dimensions for axis 1.")
 
     if control is not None:
         if type(control) == int and control >= data.shape[1]:
-            raise ValueError('Initialization ERROR. control is out of bounds')
+            raise ValueError("Initialization ERROR. control is out of bounds")
         if type(control) == str and control not in algorithms:
-            raise ValueError(
-                'Initialization ERROR. %s is not a column name of data' % control)
+            raise ValueError("Initialization ERROR. %s is not a column name of data" % control)
 
     if apv_procedure is not None:
-        if apv_procedure not in ['Bonferroni', 'Holm', 'Hochberg', 'Hommel', 'Holland', 'Finner', 'Li', 'Shaffer',
-                                 'Nemenyi']:
-            raise ValueError(
-                'Initialization ERROR. Incorrect value for APVprocedure.')
+        if apv_procedure not in [
+            "Bonferroni",
+            "Holm",
+            "Hochberg",
+            "Hommel",
+            "Holland",
+            "Finner",
+            "Li",
+            "Shaffer",
+            "Nemenyi",
+        ]:
+            raise ValueError("Initialization ERROR. Incorrect value for APVprocedure.")
 
     # Compute ranks.
     datarank = ranks(data)
     # Compute for each algorithm the ranking average.
     avranks = np.mean(datarank, axis=0)
 
     # Compute z-values
@@ -290,36 +294,36 @@
 
     pvalues_df = pd.DataFrame(data=p_value, index=index, columns=algorithms)
     zvalues_df = pd.DataFrame(data=z, index=index, columns=algorithms)
 
     if apv_procedure is None:
         return zvalues_df, pvalues_df
     else:
-        if apv_procedure == 'Bonferroni':
+        if apv_procedure == "Bonferroni":
             ap_vs_df = bonferroni_dunn(pvalues_df, control=control)
-        elif apv_procedure == 'Holm':
+        elif apv_procedure == "Holm":
             ap_vs_df = holm(pvalues_df, control=control)
-        elif apv_procedure == 'Hochberg':
+        elif apv_procedure == "Hochberg":
             ap_vs_df = hochberg(pvalues_df, control=control)
-        elif apv_procedure == 'Holland':
+        elif apv_procedure == "Holland":
             ap_vs_df = holland(pvalues_df, control=control)
-        elif apv_procedure == 'Finner':
+        elif apv_procedure == "Finner":
             ap_vs_df = finner(pvalues_df, control=control)
-        elif apv_procedure == 'Li':
+        elif apv_procedure == "Li":
             ap_vs_df = li(pvalues_df, control=control)
-        elif apv_procedure == 'Shaffer':
+        elif apv_procedure == "Shaffer":
             ap_vs_df = shaffer(pvalues_df)
-        elif apv_procedure == 'Nemenyi':
+        elif apv_procedure == "Nemenyi":
             ap_vs_df = nemenyi(pvalues_df)
 
         return zvalues_df, pvalues_df, ap_vs_df
 
 
 def friedman_aligned_ph_test(data, control=None, apv_procedure=None):
-    """ Friedman Aligned Ranks post-hoc test.
+    """Friedman Aligned Ranks post-hoc test.
 
     :param data: An (n x 2) array or DataFrame contaning the results. In data, each column represents an algorithm and, and each row a problem.
     :param control: optional int or string. Default None. Index or Name of the control algorithm. If control = None all FriedmanPosHocTest considers all possible comparisons among algorithms.
     :param apv_procedure: optional string. Default None.
         Name of the procedure for computing adjusted p-values. If apv_procedure
         is None, adjusted p-value are not computed, else the values are computed
         according to the specified procedure:
@@ -333,38 +337,35 @@
     """
 
     # Initial Checking
     if type(data) == pd.DataFrame:
         algorithms = data.columns
         data = data.values
     elif type(data) == np.ndarray:
-        algorithms = np.array(['Alg%d' % alg for alg in range(data.shape[1])])
+        algorithms = np.array(["Alg%d" % alg for alg in range(data.shape[1])])
 
     if control is None:
         index = algorithms
     elif type(control) == int:
         index = [algorithms[control]]
     else:
         index = [control]
 
     if data.ndim == 2:
         n_samples, k = data.shape
     else:
-        raise ValueError(
-            'Initialization ERROR. Incorrect number of array dimensions.')
+        raise ValueError("Initialization ERROR. Incorrect number of array dimensions.")
     if k < 2:
-        raise ValueError(
-            'Initialization Error. Incorrect number of dimensions for axis 1.')
+        raise ValueError("Initialization Error. Incorrect number of dimensions for axis 1.")
 
     if control is not None:
         if type(control) == int and control >= data.shape[1]:
-            raise ValueError('Initialization ERROR. control is out of bounds')
+            raise ValueError("Initialization ERROR. control is out of bounds")
         if type(control) == str and control not in algorithms:
-            raise ValueError(
-                'Initialization ERROR. %s is not a column name of data' % control)
+            raise ValueError("Initialization ERROR. %s is not a column name of data" % control)
 
     # Compute the average value achieved by all algorithms in each problem
     problemmean = np.mean(data, axis=1)
     # Compute the difference between control an data
     diff = np.zeros((n_samples, k))
     for j in range(k):
         diff[:, j] = data[:, j] - problemmean
@@ -395,36 +396,36 @@
 
     pvalues_df = pd.DataFrame(data=p_value, index=index, columns=algorithms)
     zvalues_df = pd.DataFrame(data=z, index=index, columns=algorithms)
 
     if apv_procedure is None:
         return zvalues_df, pvalues_df
     else:
-        if apv_procedure == 'Bonferroni':
+        if apv_procedure == "Bonferroni":
             ap_vs_df = bonferroni_dunn(pvalues_df, control=control)
-        elif apv_procedure == 'Holm':
+        elif apv_procedure == "Holm":
             ap_vs_df = holm(pvalues_df, control=control)
-        elif apv_procedure == 'Hochberg':
+        elif apv_procedure == "Hochberg":
             ap_vs_df = hochberg(pvalues_df, control=control)
-        elif apv_procedure == 'Holland':
+        elif apv_procedure == "Holland":
             ap_vs_df = holland(pvalues_df, control=control)
-        elif apv_procedure == 'Finner':
+        elif apv_procedure == "Finner":
             ap_vs_df = finner(pvalues_df, control=control)
-        elif apv_procedure == 'Li':
+        elif apv_procedure == "Li":
             ap_vs_df = li(pvalues_df, control=control)
-        elif apv_procedure == 'Shaffer':
+        elif apv_procedure == "Shaffer":
             ap_vs_df = shaffer(pvalues_df)
-        elif apv_procedure == 'Nemenyi':
+        elif apv_procedure == "Nemenyi":
             ap_vs_df = nemenyi(pvalues_df)
 
         return zvalues_df, pvalues_df, ap_vs_df
 
 
 def quade_ph_test(data, control=None, apv_procedure=None):
-    """ Quade post-hoc test.
+    """Quade post-hoc test.
 
     :param data: An (n x 2) array or DataFrame contaning the results. In data, each column represents an algorithm and, and each row a problem.
     :param control: optional int or string. Default None. Index or Name of the control algorithm. If control = None all FriedmanPosHocTest considers all possible comparisons among algorithms.
     :param apv_procedure: optional string. Default None.
         Name of the procedure for computing adjusted p-values. If apv_procedure
         is None, adjusted p-value are not computed, else the values are computed
         according to the specified procedure:
@@ -438,54 +439,50 @@
     """
 
     # Initial Checking
     if type(data) == pd.DataFrame:
         algorithms = data.columns
         data = data.values
     elif type(data) == np.ndarray:
-        algorithms = np.array(['Alg%d' % alg for alg in range(data.shape[1])])
+        algorithms = np.array(["Alg%d" % alg for alg in range(data.shape[1])])
 
     if control is None:
         index = algorithms
     elif type(control) == int:
         index = [algorithms[control]]
     else:
         index = [control]
 
     if data.ndim == 2:
         n_samples, k = data.shape
     else:
-        raise ValueError(
-            'Initialization ERROR. Incorrect number of array dimensions.')
+        raise ValueError("Initialization ERROR. Incorrect number of array dimensions.")
     if k < 2:
-        raise ValueError(
-            'Initialization Error. Incorrect number of dimensions for axis 1.')
+        raise ValueError("Initialization Error. Incorrect number of dimensions for axis 1.")
 
     if control is not None:
         if type(control) == int and control >= data.shape[1]:
-            raise ValueError('Initialization ERROR. control is out of bounds')
+            raise ValueError("Initialization ERROR. control is out of bounds")
         if type(control) == str and control not in algorithms:
-            raise ValueError(
-                'Initialization ERROR. %s is not a column name of data' % control)
+            raise ValueError("Initialization ERROR. %s is not a column name of data" % control)
 
     # Compute ranks.
     datarank = ranks(data)
     # Compute the range of each problem
     problemRange = np.max(data, axis=1) - np.min(data, axis=1)
     # Compute problem rank
     problemRank = ranks(problemRange)
 
     # Compute average rakings
     W = np.zeros((n_samples, k))
     for i in range(n_samples):
         W[i, :] = problemRank[i] * datarank[i, :]
     avranks = 2 * np.sum(W, axis=0) / (n_samples * (n_samples + 1))
     # Compute test statistics
-    aux = 1.0 / np.sqrt(k * (k + 1) * (2 * n_samples + 1) * (k - 1) /
-                        (18.0 * n_samples * (n_samples + 1)))
+    aux = 1.0 / np.sqrt(k * (k + 1) * (2 * n_samples + 1) * (k - 1) / (18.0 * n_samples * (n_samples + 1)))
     if control is None:
         z = np.zeros((k, k))
         for i in range(k):
             for j in range(i + 1, k):
                 z[i, j] = abs(avranks[i] - avranks[j]) * aux
         z += z.T
     else:
@@ -500,25 +497,25 @@
 
     pvalues_df = pd.DataFrame(data=p_value, index=index, columns=algorithms)
     zvalues_df = pd.DataFrame(data=z, index=index, columns=algorithms)
 
     if apv_procedure is None:
         return zvalues_df, pvalues_df
     else:
-        if apv_procedure == 'Bonferroni':
+        if apv_procedure == "Bonferroni":
             ap_vs_df = bonferroni_dunn(pvalues_df, control=control)
-        elif apv_procedure == 'Holm':
+        elif apv_procedure == "Holm":
             ap_vs_df = holm(pvalues_df, control=control)
-        elif apv_procedure == 'Hochberg':
+        elif apv_procedure == "Hochberg":
             ap_vs_df = hochberg(pvalues_df, control=control)
-        elif apv_procedure == 'Holland':
+        elif apv_procedure == "Holland":
             ap_vs_df = holland(pvalues_df, control=control)
-        elif apv_procedure == 'Finner':
+        elif apv_procedure == "Finner":
             ap_vs_df = finner(pvalues_df, control=control)
-        elif apv_procedure == 'Li':
+        elif apv_procedure == "Li":
             ap_vs_df = li(pvalues_df, control=control)
-        elif apv_procedure == 'Shaffer':
+        elif apv_procedure == "Shaffer":
             ap_vs_df = shaffer(pvalues_df)
-        elif apv_procedure == 'Nemenyi':
+        elif apv_procedure == "Nemenyi":
             ap_vs_df = nemenyi(pvalues_df)
 
         return zvalues_df, pvalues_df, ap_vs_df
```

### Comparing `jmetalpy-1.5.5/jmetal/lab/visualization/chord_plot.py` & `jmetalpy-1.6.0/jmetal/lab/visualization/chord_plot.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,85 +10,122 @@
 from jmetal.core.solution import FloatSolution
 
 
 def polar_to_cartesian(r, theta):
     return np.array([r * np.cos(theta), r * np.sin(theta)])
 
 
-def draw_sector(start_angle=0, end_angle=60, radius=1.0, width=0.2, lw=2, ls='-', ax=None, fc=(1, 0, 0), ec=(0, 0, 0),
-                z_order=1):
+def draw_sector(
+    start_angle=0, end_angle=60, radius=1.0, width=0.2, lw=2, ls="-", ax=None, fc=(1, 0, 0), ec=(0, 0, 0), z_order=1
+):
     if start_angle > end_angle:
         start_angle, end_angle = end_angle, start_angle
-    start_angle *= np.pi / 180.
-    end_angle *= np.pi / 180.
+    start_angle *= np.pi / 180.0
+    end_angle *= np.pi / 180.0
 
     # https://stackoverflow.com/questions/1734745/how-to-create-circle-with-b%C3%A9zier-curves
-    opt = 4. / 3. * np.tan((end_angle - start_angle) / 4.) * radius
+    opt = 4.0 / 3.0 * np.tan((end_angle - start_angle) / 4.0) * radius
     inner = radius * (1 - width)
 
-    vertsPath = [polar_to_cartesian(radius, start_angle),
-                 polar_to_cartesian(radius, start_angle) + polar_to_cartesian(opt, start_angle + 0.5 * np.pi),
-                 polar_to_cartesian(radius, end_angle) + polar_to_cartesian(opt, end_angle - 0.5 * np.pi),
-                 polar_to_cartesian(radius, end_angle),
-                 polar_to_cartesian(inner, end_angle),
-                 polar_to_cartesian(inner, end_angle) + polar_to_cartesian(opt * (1 - width), end_angle - 0.5 * np.pi),
-                 polar_to_cartesian(inner, start_angle) + polar_to_cartesian(opt * (1 - width),
-                                                                             start_angle + 0.5 * np.pi),
-                 polar_to_cartesian(inner, start_angle),
-                 polar_to_cartesian(radius, start_angle)]
-
-    codesPaths = [Path.MOVETO, Path.CURVE4, Path.CURVE4, Path.CURVE4, Path.LINETO, Path.CURVE4, Path.CURVE4,
-                  Path.CURVE4, Path.CLOSEPOLY]
+    vertsPath = [
+        polar_to_cartesian(radius, start_angle),
+        polar_to_cartesian(radius, start_angle) + polar_to_cartesian(opt, start_angle + 0.5 * np.pi),
+        polar_to_cartesian(radius, end_angle) + polar_to_cartesian(opt, end_angle - 0.5 * np.pi),
+        polar_to_cartesian(radius, end_angle),
+        polar_to_cartesian(inner, end_angle),
+        polar_to_cartesian(inner, end_angle) + polar_to_cartesian(opt * (1 - width), end_angle - 0.5 * np.pi),
+        polar_to_cartesian(inner, start_angle) + polar_to_cartesian(opt * (1 - width), start_angle + 0.5 * np.pi),
+        polar_to_cartesian(inner, start_angle),
+        polar_to_cartesian(radius, start_angle),
+    ]
+
+    codesPaths = [
+        Path.MOVETO,
+        Path.CURVE4,
+        Path.CURVE4,
+        Path.CURVE4,
+        Path.LINETO,
+        Path.CURVE4,
+        Path.CURVE4,
+        Path.CURVE4,
+        Path.CLOSEPOLY,
+    ]
 
     if ax is None:
         return vertsPath, codesPaths
     else:
         path = Path(vertsPath, codesPaths)
         patch = patches.PathPatch(path, facecolor=fc, edgecolor=ec, lw=lw, linestyle=ls, zorder=z_order)
         ax.add_patch(patch)
-        return (patch)
+        return patch
 
 
-def draw_chord(start_angle1=0, end_angle1=60, start_angle2=180, end_angle2=240, radius=1.0, chord_width=0.7, ax=None,
-               color=(1, 0, 0), z_order=1):
+def draw_chord(
+    start_angle1=0,
+    end_angle1=60,
+    start_angle2=180,
+    end_angle2=240,
+    radius=1.0,
+    chord_width=0.7,
+    ax=None,
+    color=(1, 0, 0),
+    z_order=1,
+):
     if start_angle1 > end_angle1:
         start_angle1, end_angle1 = end_angle1, start_angle1
     if start_angle2 > end_angle2:
         start_angle2, end_angle2 = end_angle2, start_angle2
-    start_angle1 *= np.pi / 180.
-    end_angle1 *= np.pi / 180.
-    start_angle2 *= np.pi / 180.
-    end_angle2 *= np.pi / 180.
+    start_angle1 *= np.pi / 180.0
+    end_angle1 *= np.pi / 180.0
+    start_angle2 *= np.pi / 180.0
+    end_angle2 *= np.pi / 180.0
 
-    optAngle1 = 4. / 3. * np.tan((end_angle1 - start_angle1) / 4.) * radius
-    optAngle2 = 4. / 3. * np.tan((end_angle2 - start_angle2) / 4.) * radius
+    optAngle1 = 4.0 / 3.0 * np.tan((end_angle1 - start_angle1) / 4.0) * radius
+    optAngle2 = 4.0 / 3.0 * np.tan((end_angle2 - start_angle2) / 4.0) * radius
     rchord = radius * (1 - chord_width)
 
-    vertsPath = [polar_to_cartesian(radius, start_angle1),
-                 polar_to_cartesian(radius, start_angle1) + polar_to_cartesian(optAngle1, start_angle1 + 0.5 * np.pi),
-                 polar_to_cartesian(radius, end_angle1) + polar_to_cartesian(optAngle1, end_angle1 - 0.5 * np.pi),
-                 polar_to_cartesian(radius, end_angle1),
-                 polar_to_cartesian(rchord, end_angle1), polar_to_cartesian(rchord, start_angle2),
-                 polar_to_cartesian(radius, start_angle2),
-                 polar_to_cartesian(radius, start_angle2) + polar_to_cartesian(optAngle2, start_angle2 + 0.5 * np.pi),
-                 polar_to_cartesian(radius, end_angle2) + polar_to_cartesian(optAngle2, end_angle2 - 0.5 * np.pi),
-                 polar_to_cartesian(radius, end_angle2),
-                 polar_to_cartesian(rchord, end_angle2), polar_to_cartesian(rchord, start_angle1),
-                 polar_to_cartesian(radius, start_angle1)]
-
-    codesPath = [Path.MOVETO, Path.CURVE4, Path.CURVE4, Path.CURVE4, Path.CURVE4, Path.CURVE4, Path.CURVE4,
-                 Path.CURVE4, Path.CURVE4, Path.CURVE4, Path.CURVE4, Path.CURVE4, Path.CURVE4]
+    vertsPath = [
+        polar_to_cartesian(radius, start_angle1),
+        polar_to_cartesian(radius, start_angle1) + polar_to_cartesian(optAngle1, start_angle1 + 0.5 * np.pi),
+        polar_to_cartesian(radius, end_angle1) + polar_to_cartesian(optAngle1, end_angle1 - 0.5 * np.pi),
+        polar_to_cartesian(radius, end_angle1),
+        polar_to_cartesian(rchord, end_angle1),
+        polar_to_cartesian(rchord, start_angle2),
+        polar_to_cartesian(radius, start_angle2),
+        polar_to_cartesian(radius, start_angle2) + polar_to_cartesian(optAngle2, start_angle2 + 0.5 * np.pi),
+        polar_to_cartesian(radius, end_angle2) + polar_to_cartesian(optAngle2, end_angle2 - 0.5 * np.pi),
+        polar_to_cartesian(radius, end_angle2),
+        polar_to_cartesian(rchord, end_angle2),
+        polar_to_cartesian(rchord, start_angle1),
+        polar_to_cartesian(radius, start_angle1),
+    ]
+
+    codesPath = [
+        Path.MOVETO,
+        Path.CURVE4,
+        Path.CURVE4,
+        Path.CURVE4,
+        Path.CURVE4,
+        Path.CURVE4,
+        Path.CURVE4,
+        Path.CURVE4,
+        Path.CURVE4,
+        Path.CURVE4,
+        Path.CURVE4,
+        Path.CURVE4,
+        Path.CURVE4,
+    ]
 
     if ax == None:
         return vertsPath, codesPath
     else:
         path = Path(vertsPath, codesPath)
         patch = patches.PathPatch(path, facecolor=color + (0.5,), edgecolor=color + (0.4,), lw=2, alpha=0.5)
         ax.add_patch(patch)
-        return (patch)
+        return patch
 
 
 def hover_over_bin(event, handle_tickers, handle_plots, colors, fig):
     is_found = False
 
     for iobj in range(len(handle_tickers)):
         for ibin in range(len(handle_tickers[iobj])):
@@ -105,31 +142,37 @@
             else:
                 plt.setp(handle_tickers[iobj][ibin], facecolor=(1, 1, 1))
                 for h in handle_plots[iobj][ibin]:
                     h.set_visible(False)
                 fig.canvas.draw_idle()
 
 
-def chord_diagram(solutions: List[FloatSolution], nbins='auto', ax=None, obj_labels=None,
-                  prop_labels=dict(fontsize=13, ha='center', va='center'), pad=6):
+def chord_diagram(
+    solutions: List[FloatSolution],
+    nbins="auto",
+    ax=None,
+    obj_labels=None,
+    prop_labels=dict(fontsize=13, ha="center", va="center"),
+    pad=6,
+):
     points_matrix = np.array([s.objectives for s in solutions])
     (NPOINTS, NOBJ) = np.shape(points_matrix)
 
     HSV_tuples = [(x * 1.0 / NOBJ, 0.5, 0.5) for x in range(NOBJ)]
     colors = list(map(lambda x: colorsys.hsv_to_rgb(*x), HSV_tuples))
 
     if ax is None:
         fig = plt.figure(figsize=(6, 6))
-        ax = plt.axes([0, 0, 1, 1], aspect='equal')
+        ax = plt.axes([0, 0, 1, 1], aspect="equal")
 
     ax.set_xlim(-2.3, 2.3)
     ax.set_ylim(-2.3, 2.3)
-    ax.axis('off')
+    ax.axis("off")
 
-    y = np.array([1. / NOBJ] * NOBJ) * (360 - pad * NOBJ)
+    y = np.array([1.0 / NOBJ] * NOBJ) * (360 - pad * NOBJ)
     sector_angles = []
     labels_pos_and_ros = []
 
     start_angle = 0
     for i in range(NOBJ):
         end_angle = start_angle + y[i]
         sector_angles.append((start_angle, end_angle))
@@ -141,17 +184,21 @@
         angleText = start_angle - 2.5
         if -30 <= angleText <= 210:
             angleText -= 90
         else:
             angleText -= 270
 
         labels_pos_and_ros.append(
-            tuple(polar_to_cartesian(1.0, 0.5 * (start_angle + end_angle) * np.pi / 180.)) + (angle_diff,) +
-            tuple(polar_to_cartesian(0.725, (start_angle - 2.5) * np.pi / 180.)) + (angleText,) +
-            tuple(polar_to_cartesian(0.85, (start_angle - 2.5) * np.pi / 180.)) + (angleText,))
+            tuple(polar_to_cartesian(1.0, 0.5 * (start_angle + end_angle) * np.pi / 180.0))
+            + (angle_diff,)
+            + tuple(polar_to_cartesian(0.725, (start_angle - 2.5) * np.pi / 180.0))
+            + (angleText,)
+            + tuple(polar_to_cartesian(0.85, (start_angle - 2.5) * np.pi / 180.0))
+            + (angleText,)
+        )
         start_angle = end_angle + pad
 
     arc_points = []
     for point in points_matrix:
         arc_points.append([])
         idim = 0
 
@@ -160,91 +207,169 @@
             arc_points[-1].append((anglePoint, anglePoint))
             idim = idim + 1
 
     max_hist_values = []
     handle_tickers = []
     handle_plots = []
 
-    for iobj in tqdm(range(NOBJ), ascii=True, desc='Chord diagram'):
-        draw_sector(start_angle=sector_angles[iobj][0], end_angle=sector_angles[iobj][1], radius=0.925, width=0.225,
-                    ax=ax,
-                    fc=(1, 1, 1, 0.0), ec=(0, 0, 0), lw=2, z_order=10)
-        draw_sector(start_angle=sector_angles[iobj][0], end_angle=sector_angles[iobj][1], radius=0.925, width=0.05,
-                    ax=ax,
-                    fc=colors[iobj], ec=(0, 0, 0), lw=2, z_order=10)
-        draw_sector(start_angle=sector_angles[iobj][0], end_angle=sector_angles[iobj][1], radius=0.7 + 0.15, width=0.0,
-                    ax=ax, fc=colors[iobj], ec=colors[iobj], lw=2, ls=':', z_order=5)
+    for iobj in tqdm(range(NOBJ), ascii=True, desc="Chord diagram"):
+        draw_sector(
+            start_angle=sector_angles[iobj][0],
+            end_angle=sector_angles[iobj][1],
+            radius=0.925,
+            width=0.225,
+            ax=ax,
+            fc=(1, 1, 1, 0.0),
+            ec=(0, 0, 0),
+            lw=2,
+            z_order=10,
+        )
+        draw_sector(
+            start_angle=sector_angles[iobj][0],
+            end_angle=sector_angles[iobj][1],
+            radius=0.925,
+            width=0.05,
+            ax=ax,
+            fc=colors[iobj],
+            ec=(0, 0, 0),
+            lw=2,
+            z_order=10,
+        )
+        draw_sector(
+            start_angle=sector_angles[iobj][0],
+            end_angle=sector_angles[iobj][1],
+            radius=0.7 + 0.15,
+            width=0.0,
+            ax=ax,
+            fc=colors[iobj],
+            ec=colors[iobj],
+            lw=2,
+            ls=":",
+            z_order=5,
+        )
 
         histValues, binsDim = np.histogram(points_matrix[:, iobj], bins=nbins)
         relativeHeightBinPre = 0.025
         max_hist_values.append(max(histValues))
         handle_tickers.append([])
         handle_plots.append([])
 
         for indexBin in range(len(histValues)):
-            startAngleBin = sector_angles[iobj][0] + (sector_angles[iobj][1] - sector_angles[iobj][0]) * binsDim[
-                indexBin]
-            endAngleBin = sector_angles[iobj][0] + (sector_angles[iobj][1] - sector_angles[iobj][0]) * binsDim[
-                indexBin + 1]
+            startAngleBin = (
+                sector_angles[iobj][0] + (sector_angles[iobj][1] - sector_angles[iobj][0]) * binsDim[indexBin]
+            )
+            endAngleBin = (
+                sector_angles[iobj][0] + (sector_angles[iobj][1] - sector_angles[iobj][0]) * binsDim[indexBin + 1]
+            )
             relativeHeightBin = 0.15 * histValues[indexBin] / max(histValues)
             handle_tickers[-1].append(
-                draw_sector(start_angle=startAngleBin, end_angle=endAngleBin, radius=0.69, width=0.08, ax=ax, lw=1,
-                            fc=(1, 1, 1), ec=(0, 0, 0)))
+                draw_sector(
+                    start_angle=startAngleBin,
+                    end_angle=endAngleBin,
+                    radius=0.69,
+                    width=0.08,
+                    ax=ax,
+                    lw=1,
+                    fc=(1, 1, 1),
+                    ec=(0, 0, 0),
+                )
+            )
             handle_plots[-1].append([])
 
             if histValues[indexBin] > 0:
-                draw_sector(start_angle=startAngleBin, end_angle=endAngleBin, radius=0.7 + relativeHeightBin, width=0,
-                            ax=ax, lw=1, fc=colors[iobj], ec=colors[iobj])
-                plotPoint1 = polar_to_cartesian(0.7 + relativeHeightBinPre, startAngleBin * np.pi / 180.)
-                plotPoint2 = polar_to_cartesian(0.7 + relativeHeightBin, startAngleBin * np.pi / 180.)
+                draw_sector(
+                    start_angle=startAngleBin,
+                    end_angle=endAngleBin,
+                    radius=0.7 + relativeHeightBin,
+                    width=0,
+                    ax=ax,
+                    lw=1,
+                    fc=colors[iobj],
+                    ec=colors[iobj],
+                )
+                plotPoint1 = polar_to_cartesian(0.7 + relativeHeightBinPre, startAngleBin * np.pi / 180.0)
+                plotPoint2 = polar_to_cartesian(0.7 + relativeHeightBin, startAngleBin * np.pi / 180.0)
                 plt.plot([plotPoint1[0], plotPoint2[0]], [plotPoint1[1], plotPoint2[1]], c=colors[iobj], lw=1)
                 relativeHeightBinPre = relativeHeightBin
             else:
-                plotPoint1 = polar_to_cartesian(0.7 + relativeHeightBinPre, startAngleBin * np.pi / 180.)
-                plotPoint2 = polar_to_cartesian(0.725 + relativeHeightBin, startAngleBin * np.pi / 180.)
+                plotPoint1 = polar_to_cartesian(0.7 + relativeHeightBinPre, startAngleBin * np.pi / 180.0)
+                plotPoint2 = polar_to_cartesian(0.725 + relativeHeightBin, startAngleBin * np.pi / 180.0)
                 plt.plot([plotPoint1[0], plotPoint2[0]], [plotPoint1[1], plotPoint2[1]], c=colors[iobj], lw=1)
                 relativeHeightBinPre = 0.025
             if indexBin == len(histValues) - 1:
-                plotPoint1 = polar_to_cartesian(0.7 + relativeHeightBin, endAngleBin * np.pi / 180.)
-                plotPoint2 = polar_to_cartesian(0.725, endAngleBin * np.pi / 180.)
+                plotPoint1 = polar_to_cartesian(0.7 + relativeHeightBin, endAngleBin * np.pi / 180.0)
+                plotPoint2 = polar_to_cartesian(0.725, endAngleBin * np.pi / 180.0)
                 plt.plot([plotPoint1[0], plotPoint2[0]], [plotPoint1[1], plotPoint2[1]], c=colors[iobj], lw=1)
 
             for ipoint in range(len(points_matrix)):
-                plotPoint1 = polar_to_cartesian(0.6, arc_points[ipoint][iobj][0] * np.pi / 180.)
-                plotPoint2 = polar_to_cartesian(0.6, arc_points[ipoint][iobj][0] * np.pi / 180.)
-                plt.plot([plotPoint1[0], plotPoint2[0]], [plotPoint1[1], plotPoint2[1]], marker='o', markersize=3,
-                         c=colors[iobj], lw=2)
+                plotPoint1 = polar_to_cartesian(0.6, arc_points[ipoint][iobj][0] * np.pi / 180.0)
+                plotPoint2 = polar_to_cartesian(0.6, arc_points[ipoint][iobj][0] * np.pi / 180.0)
+                plt.plot(
+                    [plotPoint1[0], plotPoint2[0]],
+                    [plotPoint1[1], plotPoint2[1]],
+                    marker="o",
+                    markersize=3,
+                    c=colors[iobj],
+                    lw=2,
+                )
 
-                if binsDim[indexBin] < points_matrix[ipoint, iobj] <= binsDim[
-                    indexBin + 1]:
+                if binsDim[indexBin] < points_matrix[ipoint, iobj] <= binsDim[indexBin + 1]:
                     for jdim in range(NOBJ):
                         if jdim >= 1:
                             handle_plots[iobj][indexBin].append(
-                                draw_chord(arc_points[ipoint][jdim - 1][0], arc_points[ipoint][jdim - 1][1],
-                                           arc_points[ipoint][jdim][0], arc_points[ipoint][jdim][1], radius=0.55,
-                                           color=colors[iobj], chord_width=1, ax=ax))
+                                draw_chord(
+                                    arc_points[ipoint][jdim - 1][0],
+                                    arc_points[ipoint][jdim - 1][1],
+                                    arc_points[ipoint][jdim][0],
+                                    arc_points[ipoint][jdim][1],
+                                    radius=0.55,
+                                    color=colors[iobj],
+                                    chord_width=1,
+                                    ax=ax,
+                                )
+                            )
                             handle_plots[iobj][indexBin][-1].set_visible(False)
                     handle_plots[iobj][indexBin].append(
-                        draw_chord(arc_points[ipoint][-1][0], arc_points[ipoint][-1][1], arc_points[ipoint][0][0],
-                                   arc_points[ipoint][0][1], radius=0.55, color=colors[iobj], chord_width=1, ax=ax))
+                        draw_chord(
+                            arc_points[ipoint][-1][0],
+                            arc_points[ipoint][-1][1],
+                            arc_points[ipoint][0][0],
+                            arc_points[ipoint][0][1],
+                            radius=0.55,
+                            color=colors[iobj],
+                            chord_width=1,
+                            ax=ax,
+                        )
+                    )
                     handle_plots[iobj][indexBin][-1].set_visible(False)
 
     if obj_labels is None:
-        obj_labels = ['$f_{' + str(i) + '}(\mathbf{x})$' for i in range(NOBJ)]
+        obj_labels = ["$f_{" + str(i) + "}(\mathbf{x})$" for i in range(NOBJ)]
 
-    prop_legend_bins = dict(fontsize=9, ha='center', va='center')
+    prop_legend_bins = dict(fontsize=9, ha="center", va="center")
 
     for i in range(NOBJ):
-        p0, p1 = polar_to_cartesian(0.975, sector_angles[i][0] * np.pi / 180.)
-        ax.text(p0, p1, '0', **prop_legend_bins)
-        p0, p1 = polar_to_cartesian(0.975, sector_angles[i][1] * np.pi / 180.)
-        ax.text(p0, p1, '1', **prop_legend_bins)
-        ax.text(labels_pos_and_ros[i][0], labels_pos_and_ros[i][1], obj_labels[i], rotation=labels_pos_and_ros[i][2],
-                **prop_labels)
-        ax.text(labels_pos_and_ros[i][3], labels_pos_and_ros[i][4], '0', **prop_legend_bins, color=colors[i])
-        ax.text(labels_pos_and_ros[i][6], labels_pos_and_ros[i][7], str(max_hist_values[i]), **prop_legend_bins,
-                color=colors[i])
+        p0, p1 = polar_to_cartesian(0.975, sector_angles[i][0] * np.pi / 180.0)
+        ax.text(p0, p1, "0", **prop_legend_bins)
+        p0, p1 = polar_to_cartesian(0.975, sector_angles[i][1] * np.pi / 180.0)
+        ax.text(p0, p1, "1", **prop_legend_bins)
+        ax.text(
+            labels_pos_and_ros[i][0],
+            labels_pos_and_ros[i][1],
+            obj_labels[i],
+            rotation=labels_pos_and_ros[i][2],
+            **prop_labels
+        )
+        ax.text(labels_pos_and_ros[i][3], labels_pos_and_ros[i][4], "0", **prop_legend_bins, color=colors[i])
+        ax.text(
+            labels_pos_and_ros[i][6],
+            labels_pos_and_ros[i][7],
+            str(max_hist_values[i]),
+            **prop_legend_bins,
+            color=colors[i]
+        )
 
     plt.axis([-1.2, 1.2, -1.2, 1.2])
-    fig.canvas.mpl_connect("motion_notify_event",
-                           lambda event: hover_over_bin(event, handle_tickers, handle_plots, colors, fig))
+    fig.canvas.mpl_connect(
+        "motion_notify_event", lambda event: hover_over_bin(event, handle_tickers, handle_plots, colors, fig)
+    )
     plt.show()
```

### Comparing `jmetalpy-1.5.5/jmetal/lab/visualization/interactive.py` & `jmetalpy-1.6.0/jmetal/lab/visualization/interactive.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,102 +1,112 @@
 import logging
-from typing import TypeVar, List
+from typing import List, TypeVar
 
 import pandas as pd
 from plotly import graph_objs as go
 from plotly import io as pio
 from plotly import offline
 
 from jmetal.lab.visualization.plotting import Plot
 
-LOGGER = logging.getLogger('jmetal')
+logger = logging.getLogger(__name__)
 
-S = TypeVar('S')
+S = TypeVar("S")
 
 
 class InteractivePlot(Plot):
-
-    def __init__(self,
-                 title: str = 'Pareto front approximation',
-                 reference_front: List[S] = None,
-                 reference_point: list = None,
-                 axis_labels: list = None):
+    def __init__(
+        self,
+        title: str = "Pareto front approximation",
+        reference_front: List[S] = None,
+        reference_point: list = None,
+        axis_labels: list = None,
+    ):
         super(InteractivePlot, self).__init__(title, reference_front, reference_point, axis_labels)
         self.figure = None
         self.layout = None
         self.data = []
 
-    def plot(self, front, label=None, normalize: bool = False, filename: str = None, format: str = 'HTML'):
-        """ Plot a front of solutions (2D, 3D or parallel coordinates).
+    def plot(self, front, label=None, normalize: bool = False, filename: str = None, format: str = "HTML"):
+        """Plot a front of solutions (2D, 3D or parallel coordinates).
 
         :param front: List of solutions.
         :param label: Front name.
         :param normalize: Normalize the input front between 0 and 1 (for problems with more than 3 objectives).
         :param filename: Output filename.
         """
         if not isinstance(label, list):
             label = [label]
 
         self.layout = go.Layout(
             margin=dict(l=80, r=80, b=80, t=150),
             height=800,
-            title='{}<br>{}'.format(self.plot_title, label[0]),
+            title="{}<br>{}".format(self.plot_title, label[0]),
             scene=dict(
                 xaxis=dict(title=self.axis_labels[0:1][0] if self.axis_labels[0:1] else None),
                 yaxis=dict(title=self.axis_labels[1:2][0] if self.axis_labels[1:2] else None),
-                zaxis=dict(title=self.axis_labels[2:3][0] if self.axis_labels[2:3] else None)
+                zaxis=dict(title=self.axis_labels[2:3][0] if self.axis_labels[2:3] else None),
             ),
-            hovermode='closest'
+            hovermode="closest",
         )
 
         # If any reference front, plot
         if self.reference_front:
             points, _ = self.get_points(self.reference_front)
-            trace = self.__generate_trace(points=points, legend='Reference front', normalize=normalize,
-                                          color='black', size=2)
+            trace = self.__generate_trace(
+                points=points, legend="Reference front", normalize=normalize, color="black", size=2
+            )
             self.data.append(trace)
 
         # If any reference point, plot
         if self.reference_point:
             points = pd.DataFrame(self.reference_point)
-            trace = self.__generate_trace(points=points, legend='Reference point', color='red', size=8)
+            trace = self.__generate_trace(points=points, legend="Reference point", color="red", size=8)
             self.data.append(trace)
 
         # Get points and metadata
         points, _ = self.get_points(front)
         metadata = list(solution.__str__() for solution in front)
 
-        trace = self.__generate_trace(points=points, metadata=metadata, legend='Front approximation',
-                                      normalize=normalize)
+        trace = self.__generate_trace(
+            points=points, metadata=metadata, legend="Front approximation", normalize=normalize
+        )
         self.data.append(trace)
         self.figure = go.Figure(data=self.data, layout=self.layout)
 
         # Plot the figure
         if filename:
-            if format == 'HTML':
+            if format == "HTML":
                 self.export_to_html(filename)
+                logger.info("Figure {_filename} exported to HTML file")
             else:
-                pio.write_image(self.figure, filename + '.' + format)
+                _filename = filename + "." + format
+
+                pio.write_image(self.figure, _filename)
+                logger.info("Figure {_filename} saved to file")
 
     def export_to_html(self, filename: str) -> str:
-        """ Export the graph to an interactive HTML (solutions can be selected to show some metadata).
+        """Export the graph to an interactive HTML (solutions can be selected to show some metadata).
 
         :param filename: Output file name.
-        :return: Script as string. """
-        html_string = '''
+        :return: Script as string."""
+        html_string = (
+            """
         <!DOCTYPE html>
         <html>
             <head>
                 <meta charset="utf-8"/>
                 <script src="https://cdn.plot.ly/plotly-latest.min.js"></script>
                 <script src="https://unpkg.com/sweetalert2@7.7.0/dist/sweetalert2.all.js"></script>
                 <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.1/css/bootstrap.min.css">
             </head>
             <body>
-                ''' + self.export_to_div(filename=None, include_plotlyjs=False) + '''
+                """
+            + self.export_to_div(filename=None, include_plotlyjs=False)
+            + """
                 <script>                
                     var myPlot = document.querySelectorAll('div')[0];
                     myPlot.on('plotly_click', function(data){
                         var pts = '';
 
                         for(var i=0; i < data.points.length; i++){
                             pts = '(x, y) = ('+data.points[i].x +', '+ data.points[i].y.toPrecision(4)+')';
@@ -114,91 +124,77 @@
                     });
 
                     window.onresize = function() {
                        Plotly.Plots.resize(myPlot);
                     };
                 </script>
             </body>
-        </html>'''
+        </html>"""
+        )
 
-        with open(filename + '.html', 'w') as outf:
+        with open(filename + ".html", "w") as outf:
             outf.write(html_string)
 
         return html_string
 
     def export_to_div(self, filename=None, include_plotlyjs: bool = False) -> str:
-        """ Export as a `div` for embedding the graph in an HTML file.
+        """Export as a `div` for embedding the graph in an HTML file.
 
         :param filename: Output file name (if desired, default to None).
         :param include_plotlyjs: If True, include plot.ly JS script (default to False).
         :return: Script as string.
         """
-        script = offline.plot(self.figure, output_type='div', include_plotlyjs=include_plotlyjs, show_link=False)
+        script = offline.plot(self.figure, output_type="div", include_plotlyjs=include_plotlyjs, show_link=False)
 
         if filename:
-            with open(filename + '.html', 'w') as outf:
+            with open(filename + ".html", "w") as outf:
                 outf.write(script)
 
         return script
 
-    def __generate_trace(self, points: pd.DataFrame, legend: str, metadata: list = None, normalize: bool = False,
-                         **kwargs):
+    def __generate_trace(
+        self, points: pd.DataFrame, legend: str, metadata: list = None, normalize: bool = False, **kwargs
+    ):
         dimension = points.shape[1]
 
         # tweak points size for 3D plots
         marker_size = 8
         if dimension == 3:
             marker_size = 4
 
         # if indicated, perform normalization
         if normalize:
             points = (points - points.min()) / (points.max() - points.min())
 
         marker = dict(
-            color='#236FA4',
-            size=marker_size,
-            symbol='circle',
-            line=dict(
-                color='#236FA4',
-                width=1
-            ),
-            opacity=0.8
+            color="#236FA4", size=marker_size, symbol="circle", line=dict(color="#236FA4", width=1), opacity=0.8
         )
         marker.update(**kwargs)
 
         if dimension == 2:
             trace = go.Scattergl(
-                x=points[0],
-                y=points[1],
-                mode='markers',
-                marker=marker,
-                name=legend,
-                customdata=metadata
+                x=points[0], y=points[1], mode="markers", marker=marker, name=legend, customdata=metadata
             )
         elif dimension == 3:
             trace = go.Scatter3d(
-                x=points[0],
-                y=points[1],
-                z=points[2],
-                mode='markers',
-                marker=marker,
-                name=legend,
-                customdata=metadata
+                x=points[0], y=points[1], z=points[2], mode="markers", marker=marker, name=legend, customdata=metadata
             )
         else:
             dimensions = list()
             for column in points:
                 dimensions.append(
-                    dict(range=[0, 1],
-                         label=self.axis_labels[column:column + 1][0] if self.axis_labels[column:column + 1] else None,
-                         values=points[column])
+                    dict(
+                        range=[0, 1],
+                        label=self.axis_labels[column : column + 1][0]
+                        if self.axis_labels[column : column + 1]
+                        else None,
+                        values=points[column],
+                    )
                 )
 
             trace = go.Parcoords(
-                line=dict(
-                    color='#236FA4'
-                ),
+                line=dict(color="#236FA4"),
                 dimensions=dimensions,
                 name=legend,
             )
 
         return trace
```

### Comparing `jmetalpy-1.5.5/jmetal/lab/visualization/plotting.py` & `jmetalpy-1.6.0/jmetal/lab/visualization/plotting.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 import logging
-from typing import TypeVar, List, Tuple
+from typing import List, Tuple, TypeVar
 
 import numpy as np
 import pandas as pd
 from matplotlib import pyplot as plt
 from pandas import plotting
 
-LOGGER = logging.getLogger('jmetal')
+logger = logging.getLogger(__name__)
 
-S = TypeVar('S')
+S = TypeVar("S")
 
 
 class Plot:
-
-    def __init__(self,
-                 title: str = 'Pareto front approximation',
-                 reference_front: List[S] = None,
-                 reference_point: list = None,
-                 axis_labels: list = None):
+    def __init__(
+        self,
+        title: str = "Pareto front approximation",
+        reference_front: List[S] = None,
+        reference_point: list = None,
+        axis_labels: list = None,
+    ):
         """
         :param title: Title of the graph.
         :param axis_labels: List of axis labels.
         :param reference_point: Reference point (e.g., [0.4, 1.2]).
         :param reference_front: Reference Pareto front (if any) as solutions.
         """
         self.plot_title = title
@@ -32,54 +33,54 @@
 
         self.reference_point = reference_point
         self.reference_front = reference_front
         self.dimension = None
 
     @staticmethod
     def get_points(solutions: List[S]) -> Tuple[pd.DataFrame, int]:
-        """ Get points for each solution of the front.
+        """Get points for each solution of the front.
 
         :param solutions: List of solutions.
         :return: Pandas dataframe with one column for each objective and one row for each solution.
         """
         if solutions is None:
-            raise Exception('Front is none!')
+            raise Exception("Front is none!")
 
         points = pd.DataFrame(list(solution.objectives for solution in solutions))
         return points, points.shape[1]
 
-    def plot(self, front, label='', normalize: bool = False, filename: str = None, format: str = 'eps'):
-        """ Plot any arbitrary number of fronts in 2D, 3D or p-coords.
+    def plot(self, front, label="", normalize: bool = False, filename: str = None, format: str = "eps"):
+        """Plot any arbitrary number of fronts in 2D, 3D or p-coords.
 
         :param front: Pareto front or a list of them.
         :param label: Pareto front title or a list of them.
         :param normalize: If True, normalize data (for p-coords).
         :param filename: Output filename.
         :param format: Output file format.
         """
         if not isinstance(front[0], list):
             front = [front]
 
         if not isinstance(label, list):
             label = [label]
 
         if len(front) != len(label):
-            raise Exception('Number of fronts and labels must be the same')
+            raise Exception("Number of fronts and labels must be the same")
 
         dimension = front[0][0].number_of_objectives
 
         if dimension == 2:
             self.two_dim(front, label, filename, format)
         elif dimension == 3:
             self.three_dim(front, label, filename, format)
         else:
             self.pcoords(front, normalize, filename, format)
 
-    def two_dim(self, fronts: List[list], labels: List[str] = None, filename: str = None, format: str = 'eps'):
-        """ Plot any arbitrary number of fronts in 2D.
+    def two_dim(self, fronts: List[list], labels: List[str] = None, filename: str = None, format: str = "eps"):
+        """Plot any arbitrary number of fronts in 2D.
 
         :param fronts: List of fronts (containing solutions).
         :param labels: List of fronts title (if any).
         :param filename: Output filename.
         """
         n = int(np.ceil(np.sqrt(len(fronts))))
         fig = plt.figure()
@@ -89,82 +90,92 @@
         if self.reference_front:
             reference, _ = self.get_points(self.reference_front)
 
         for i, _ in enumerate(fronts):
             points, _ = self.get_points(fronts[i])
 
             ax = fig.add_subplot(n, n, i + 1)
-            points.plot(kind='scatter', x=0, y=1, ax=ax, s=10, color='#236FA4', alpha=1.0)
+            points.plot(kind="scatter", x=0, y=1, ax=ax, s=10, color="#236FA4", alpha=1.0)
 
             if labels:
                 ax.set_title(labels[i])
 
             if self.reference_front:
-                reference.plot(x=0, y=1, ax=ax, color='k', legend=False)
+                reference.plot(x=0, y=1, ax=ax, color="k", legend=False)
 
             if self.reference_point:
                 for point in self.reference_point:
-                    plt.plot([point[0]], [point[1]], marker='o', markersize=5, color='r')
-                    plt.axvline(x=point[0], color='r', linestyle=':')
-                    plt.axhline(y=point[1], color='r', linestyle=':')
+                    plt.plot([point[0]], [point[1]], marker="o", markersize=5, color="r")
+                    plt.axvline(x=point[0], color="r", linestyle=":")
+                    plt.axhline(y=point[1], color="r", linestyle=":")
 
             if self.axis_labels:
                 plt.xlabel(self.axis_labels[0])
                 plt.ylabel(self.axis_labels[1])
 
         if filename:
-            plt.savefig(filename + '.' + format, format=format, dpi=200)
+            _filename = filename + "." + format
+
+            plt.savefig(_filename, format=format, dpi=1000)
+            logger.info("Figure {_filename} saved to file")
         else:
             plt.show()
 
         plt.close(fig=fig)
 
-    def three_dim(self, fronts: List[list], labels: List[str] = None, filename: str = None, format: str = 'eps'):
-        """ Plot any arbitrary number of fronts in 3D.
+    def three_dim(self, fronts: List[list], labels: List[str] = None, filename: str = None, format: str = "eps"):
+        """Plot any arbitrary number of fronts in 3D.
 
         :param fronts: List of fronts (containing solutions).
         :param labels: List of fronts title (if any).
         :param filename: Output filename.
         """
         n = int(np.ceil(np.sqrt(len(fronts))))
         fig = plt.figure()
         fig.suptitle(self.plot_title, fontsize=16)
 
         for i, _ in enumerate(fronts):
-            ax = fig.add_subplot(n, n, i + 1, projection='3d')
-            ax.scatter([s.objectives[0] for s in fronts[i]],
-                       [s.objectives[1] for s in fronts[i]],
-                       [s.objectives[2] for s in fronts[i]])
+            ax = fig.add_subplot(n, n, i + 1, projection="3d")
+            ax.scatter(
+                [s.objectives[0] for s in fronts[i]],
+                [s.objectives[1] for s in fronts[i]],
+                [s.objectives[2] for s in fronts[i]],
+            )
 
             if labels:
                 ax.set_title(labels[i])
 
             if self.reference_front:
-                ax.scatter([s.objectives[0] for s in self.reference_front],
-                           [s.objectives[1] for s in self.reference_front],
-                           [s.objectives[2] for s in self.reference_front])
+                ax.scatter(
+                    [s.objectives[0] for s in self.reference_front],
+                    [s.objectives[1] for s in self.reference_front],
+                    [s.objectives[2] for s in self.reference_front],
+                )
 
             if self.reference_point:
                 # todo
                 pass
 
             ax.relim()
             ax.autoscale_view(True, True, True)
             ax.view_init(elev=30.0, azim=15.0)
             ax.locator_params(nbins=4)
 
         if filename:
-            plt.savefig(filename + '.' + format, format=format, dpi=1000)
+            _filename = filename + "." + format
+
+            plt.savefig(_filename, format=format, dpi=1000)
+            logger.info("Figure {_filename} saved to file")
         else:
             plt.show()
 
         plt.close(fig=fig)
 
-    def pcoords(self, fronts: List[list], normalize: bool = False, filename: str = None, format: str = 'eps'):
-        """ Plot any arbitrary number of fronts in parallel coordinates.
+    def pcoords(self, fronts: List[list], normalize: bool = False, filename: str = None, format: str = "eps"):
+        """Plot any arbitrary number of fronts in parallel coordinates.
 
         :param fronts: List of fronts (containing solutions).
         :param filename: Output filename.
         """
         n = int(np.ceil(np.sqrt(len(fronts))))
         fig = plt.figure()
         fig.suptitle(self.plot_title, fontsize=16)
@@ -174,21 +185,21 @@
 
             if normalize:
                 points = (points - points.min()) / (points.max() - points.min())
 
             ax = fig.add_subplot(n, n, i + 1)
 
             min_, max_ = points.values.min(), points.values.max()
-            points['scale'] = np.linspace(0, 1, len(points)) * (max_ - min_) + min_
-            pd.plotting.parallel_coordinates(points, 'scale', ax=ax)
+            points["scale"] = np.linspace(0, 1, len(points)) * (max_ - min_) + min_
+            pd.plotting.parallel_coordinates(points, "scale", ax=ax)
 
             ax.get_legend().remove()
 
             if self.axis_labels:
                 ax.set_xticklabels(self.axis_labels)
 
         if filename:
-            plt.savefig(filename + '.' + format, format=format, dpi=1000)
+            plt.savefig(filename + "." + format, format=format, dpi=1000)
         else:
             plt.show()
 
         plt.close(fig=fig)
```

### Comparing `jmetalpy-1.5.5/jmetal/lab/visualization/posterior.py` & `jmetalpy-1.6.0/jmetal/lab/visualization/posterior.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,23 @@
+import logging
+
 import numpy as np
 import pandas as pd
 from matplotlib import pyplot as plt
 
+logger = logging.getLogger(__name__)
+
 
-def plot_posterior(sample, higher_is_better: bool = False, min_points_per_hexbin: int = 2, alg_names: list = None,
-                   filename: str = 'posterior.eps'):
+def plot_posterior(
+    sample,
+    higher_is_better: bool = False,
+    min_points_per_hexbin: int = 2,
+    alg_names: list = None,
+    filename: str = "posterior.eps",
+):
     """
     Plots the sample from posterior distribution of a Bayesian statistical test.
     Parameters:
     -----------
     data: An (n x 3) array or DataFrame contaning the probabilities.
     alg_names: array of strings. Default np.array(['Alg1', 'Alg2'])
         Names of the algorithms under evaluation
@@ -20,95 +29,73 @@
     # Initial Checking
     if type(sample) == pd.DataFrame:
         sample = sample.values
 
     if sample.ndim == 2:
         nrow, ncol = sample.shape
         if ncol != 3:
-            raise ValueError(
-                'Initialization ERROR. Incorrect number of dimensions in axis 1.')
+            raise ValueError("Initialization ERROR. Incorrect number of dimensions in axis 1.")
     else:
-        raise ValueError(
-            'Initialization ERROR. Incorrect number of dimensions for sample')
+        raise ValueError("Initialization ERROR. Incorrect number of dimensions for sample")
 
     def transform(p):
         lambda1, lambda2, lambda3 = p.T
-        x = (0.1 * lambda1 + 0.5 * lambda2 + 0.9 * lambda3)
+        x = 0.1 * lambda1 + 0.5 * lambda2 + 0.9 * lambda3
         y = (0.2 * lambda1 + 1.4 * lambda2 + 0.2 * lambda3) / np.sqrt(3)
         return np.vstack((x, y)).T
 
     # Initialize figure
-    fig = plt.figure(figsize=(5, 5), facecolor='white')
+    fig = plt.figure(figsize=(5, 5), facecolor="white")
     ax = fig.add_axes([0, 0, 1, 1])
     ax.set_xlim(0, 1)
     ax.set_ylim(0, 1)
     ax.set_axis_off()
 
     # plot text
 
     if not higher_is_better:
         if not alg_names:
-            ax.text(x=0.5, y=1.4 / np.sqrt(3) + 0.005,
-                    s='P(rope)', ha='center', va='bottom')
-            ax.text(x=0.15, y=0.175 / np.sqrt(3) - 0.005,
-                    s='P(alg1<alg2)', ha='right', va='top')
-            ax.text(x=0.85, y=0.175 / np.sqrt(3) - 0.005,
-                    s='P(alg1>alg2)', ha='left', va='top')
+            ax.text(x=0.5, y=1.4 / np.sqrt(3) + 0.005, s="P(rope)", ha="center", va="bottom")
+            ax.text(x=0.15, y=0.175 / np.sqrt(3) - 0.005, s="P(alg1<alg2)", ha="right", va="top")
+            ax.text(x=0.85, y=0.175 / np.sqrt(3) - 0.005, s="P(alg1>alg2)", ha="left", va="top")
         else:
-            ax.text(x=0.5, y=1.4 / np.sqrt(3) + 0.005,
-                    s='P(rope)', ha='center', va='bottom')
-            ax.text(x=0.15, y=0.175 / np.sqrt(3) - 0.005,
-                    s='P(' + alg_names[0] + ')', ha='right', va='top')
-            ax.text(x=0.85, y=0.175 / np.sqrt(3) - 0.005,
-                    s='P(' + alg_names[1] + ')', ha='left', va='top')
+            ax.text(x=0.5, y=1.4 / np.sqrt(3) + 0.005, s="P(rope)", ha="center", va="bottom")
+            ax.text(x=0.15, y=0.175 / np.sqrt(3) - 0.005, s="P(" + alg_names[0] + ")", ha="right", va="top")
+            ax.text(x=0.85, y=0.175 / np.sqrt(3) - 0.005, s="P(" + alg_names[1] + ")", ha="left", va="top")
     else:
         if not alg_names:
-            ax.text(x=0.5, y=1.4 / np.sqrt(3) + 0.005,
-                    s='P(rope)', ha='center', va='bottom')
-            ax.text(x=0.15, y=0.175 / np.sqrt(3) - 0.005,
-                    s='P(alg2<alg1)', ha='right', va='top')
-            ax.text(x=0.85, y=0.175 / np.sqrt(3) - 0.005,
-                    s='P(alg2>alg1)', ha='left', va='top')
+            ax.text(x=0.5, y=1.4 / np.sqrt(3) + 0.005, s="P(rope)", ha="center", va="bottom")
+            ax.text(x=0.15, y=0.175 / np.sqrt(3) - 0.005, s="P(alg2<alg1)", ha="right", va="top")
+            ax.text(x=0.85, y=0.175 / np.sqrt(3) - 0.005, s="P(alg2>alg1)", ha="left", va="top")
         else:
-            ax.text(x=0.5, y=1.4 / np.sqrt(3) + 0.005,
-                    s='P(rope)', ha='center', va='bottom')
-            ax.text(x=0.15, y=0.175 / np.sqrt(3) - 0.005,
-                    s='P(' + alg_names[1] + ')', ha='right', va='top')
-            ax.text(x=0.85, y=0.175 / np.sqrt(3) - 0.005,
-                    s='P(' + alg_names[0] + ')', ha='left', va='top')
+            ax.text(x=0.5, y=1.4 / np.sqrt(3) + 0.005, s="P(rope)", ha="center", va="bottom")
+            ax.text(x=0.15, y=0.175 / np.sqrt(3) - 0.005, s="P(" + alg_names[1] + ")", ha="right", va="top")
+            ax.text(x=0.85, y=0.175 / np.sqrt(3) - 0.005, s="P(" + alg_names[0] + ")", ha="left", va="top")
 
     # Conversion between barycentric and Cartesian coordinates
     sample2d = np.zeros((sample.shape[0], 2))
     for p in range(sample.shape[0]):
         sample2d[p, :] = transform(sample[p, :])
 
     # Plot projected points
     ax.hexbin(sample2d[:, 0], sample2d[:, 1], mincnt=min_points_per_hexbin, cmap=plt.cm.plasma)
 
     # Plot triangle
 
-    ax.plot([0.095, 0.505], [0.2 / np.sqrt(3), 1.4 / np.sqrt(3)],
-            linewidth=3.0, color='white')
-    ax.plot([0.505, 0.905], [1.4 / np.sqrt(3), 0.2 / np.sqrt(3)],
-            linewidth=3.0, color='white')
-    ax.plot([0.09, 0.905], [0.2 / np.sqrt(3), 0.2 / np.sqrt(3)],
-            linewidth=3.0, color='white')
-
-    ax.plot([0.1, 0.5], [0.2 / np.sqrt(3), 1.4 / np.sqrt(3)],
-            linewidth=3.0, color='gray')
-    ax.plot([0.5, 0.9], [1.4 / np.sqrt(3), 0.2 / np.sqrt(3)],
-            linewidth=3.0, color='gray')
-    ax.plot([0.1, 0.9], [0.2 / np.sqrt(3), 0.2 / np.sqrt(3)],
-            linewidth=3.0, color='gray')
+    ax.plot([0.095, 0.505], [0.2 / np.sqrt(3), 1.4 / np.sqrt(3)], linewidth=3.0, color="white")
+    ax.plot([0.505, 0.905], [1.4 / np.sqrt(3), 0.2 / np.sqrt(3)], linewidth=3.0, color="white")
+    ax.plot([0.09, 0.905], [0.2 / np.sqrt(3), 0.2 / np.sqrt(3)], linewidth=3.0, color="white")
+
+    ax.plot([0.1, 0.5], [0.2 / np.sqrt(3), 1.4 / np.sqrt(3)], linewidth=3.0, color="gray")
+    ax.plot([0.5, 0.9], [1.4 / np.sqrt(3), 0.2 / np.sqrt(3)], linewidth=3.0, color="gray")
+    ax.plot([0.1, 0.9], [0.2 / np.sqrt(3), 0.2 / np.sqrt(3)], linewidth=3.0, color="gray")
 
     # plot division lines
-    ax.plot([0.5, 0.5], [0.2 / np.sqrt(3), 0.6 / np.sqrt(3)],
-            linewidth=3.0, color='gray')
-    ax.plot([0.3, 0.5], [0.8 / np.sqrt(3), 0.6 / np.sqrt(3)],
-            linewidth=3.0, color='gray')
-    ax.plot([0.5, 0.7], [0.6 / np.sqrt(3), 0.8 / np.sqrt(3)],
-            linewidth=3.0, color='gray')
+    ax.plot([0.5, 0.5], [0.2 / np.sqrt(3), 0.6 / np.sqrt(3)], linewidth=3.0, color="gray")
+    ax.plot([0.3, 0.5], [0.8 / np.sqrt(3), 0.6 / np.sqrt(3)], linewidth=3.0, color="gray")
+    ax.plot([0.5, 0.7], [0.6 / np.sqrt(3), 0.8 / np.sqrt(3)], linewidth=3.0, color="gray")
 
     if filename:
-        plt.savefig(filename, bbox_inches='tight')
+        plt.savefig(filename, bbox_inches="tight")
+        logger.info("Figure {filename} saved to file")
 
     plt.show()
```

### Comparing `jmetalpy-1.5.5/jmetal/lab/visualization/streaming.py` & `jmetalpy-1.6.0/jmetal/lab/visualization/streaming.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 import logging
-from typing import TypeVar, List
+from typing import List, TypeVar
 
 import matplotlib
 from matplotlib import pyplot as plt
 from mpl_toolkits.mplot3d import Axes3D
 
 from jmetal.lab.visualization.plotting import Plot
 
-LOGGER = logging.getLogger('jmetal')
+logger = logging.getLogger(__name__)
 
-S = TypeVar('S')
+S = TypeVar("S")
 
 """
 .. module:: streaming
    :platform: Unix, Windows
    :synopsis: Classes for plotting solutions in real-time.
 
 .. moduleauthor:: Antonio Benítez-Hidalgo <antonio.b@uma.es>
 """
 
 
 class StreamingPlot:
-
-    def __init__(self,
-                 plot_title: str = 'Pareto front approximation',
-                 reference_front: List[S] = None,
-                 reference_point: list = None,
-                 axis_labels: list = None):
+    def __init__(
+        self,
+        plot_title: str = "Pareto front approximation",
+        reference_front: List[S] = None,
+        reference_point: list = None,
+        axis_labels: list = None,
+    ):
         """
         :param plot_title: Title of the graph.
         :param axis_labels: List of axis labels.
         :param reference_point: Reference point (e.g., [0.4, 1.2]).
         :param reference_front: Reference Pareto front (if any) as solutions.
         """
         self.plot_title = plot_title
@@ -40,14 +41,15 @@
             reference_point = [reference_point]
 
         self.reference_point = reference_point
         self.reference_front = reference_front
         self.dimension = None
 
         import warnings
+
         warnings.filterwarnings("ignore", ".*GUI is implemented.*")
 
         self.fig, self.ax = plt.subplots()
         self.sc = None
         self.axis = None
 
     def plot(self, front):
@@ -56,32 +58,38 @@
 
         # Create an empty figure
         self.create_layout(dimension)
 
         # If any reference point, plot
         if self.reference_point:
             for point in self.reference_point:
-                self.scp, = self.ax.plot(*[[p] for p in point], c='r', ls='None', marker='*', markersize=3)
+                (self.scp,) = self.ax.plot(*[[p] for p in point], c="r", ls="None", marker="*", markersize=3)
 
         # If any reference front, plot
         if self.reference_front:
             rpoints, _ = Plot.get_points(self.reference_front)
-            self.scf, = self.ax.plot(*[rpoints[column].tolist() for column in rpoints.columns.values],
-                                     c='k', ls='None', marker='*', markersize=1)
+            (self.scf,) = self.ax.plot(
+                *[rpoints[column].tolist() for column in rpoints.columns.values],
+                c="k",
+                ls="None",
+                marker="*",
+                markersize=1
+            )
 
         # Plot data
-        self.sc, = self.ax.plot(*[points[column].tolist() for column in points.columns.values],
-                                ls='None', marker='o', markersize=4)
+        (self.sc,) = self.ax.plot(
+            *[points[column].tolist() for column in points.columns.values], ls="None", marker="o", markersize=4
+        )
 
         # Show plot
         plt.show(block=False)
 
     def update(self, front: List[S], reference_point: list = None) -> None:
         if self.sc is None:
-            raise Exception('Figure is none')
+            raise Exception("Figure is none")
 
         points, dimension = Plot.get_points(front)
 
         # Replace with new points
         self.sc.set_data(points[0], points[1])
 
         if dimension == 3:
@@ -100,38 +108,40 @@
             self.fig.canvas.flush_events()
         except KeyboardInterrupt:
             pass
 
         pause(0.01)
 
     def create_layout(self, dimension: int) -> None:
+        logger.info("Creating figure layout")
+
         self.fig.canvas.set_window_title(self.plot_title)
         self.fig.suptitle(self.plot_title, fontsize=16)
 
         if dimension == 2:
             # Stylize axis
-            self.ax.spines['top'].set_visible(False)
-            self.ax.spines['right'].set_visible(False)
+            self.ax.spines["top"].set_visible(False)
+            self.ax.spines["right"].set_visible(False)
             self.ax.get_xaxis().tick_bottom()
             self.ax.get_yaxis().tick_left()
         elif dimension == 3:
             self.ax = Axes3D(self.fig)
-            self.ax.autoscale(enable=True, axis='both')
+            self.ax.autoscale(enable=True, axis="both")
         else:
-            raise Exception('Dimension must be either 2 or 3')
+            raise Exception("Dimension must be either 2 or 3")
 
         self.ax.set_autoscale_on(True)
         self.ax.autoscale_view(True, True, True)
 
         # Style options
-        self.ax.grid(color='#f0f0f5', linestyle='-', linewidth=0.5, alpha=0.5)
+        self.ax.grid(color="#f0f0f5", linestyle="-", linewidth=0.5, alpha=0.5)
 
 
 def pause(interval: float):
-    backend = plt.rcParams['backend']
+    backend = plt.rcParams["backend"]
 
     if backend in matplotlib.rcsetup.interactive_bk:
         figManager = matplotlib._pylab_helpers.Gcf.get_active()
         if figManager is not None:
             canvas = figManager.canvas
             if canvas.figure.stale:
                 canvas.draw()
```

### Comparing `jmetalpy-1.5.5/jmetal/operator/crossover.py` & `jmetalpy-1.6.0/jmetal/operator/crossover.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 import copy
 import random
 from typing import List
 
 from jmetal.core.operator import Crossover
-from jmetal.core.solution import Solution, FloatSolution, BinarySolution, PermutationSolution, IntegerSolution, \
-    CompositeSolution
+from jmetal.core.solution import (
+    BinarySolution,
+    CompositeSolution,
+    FloatSolution,
+    IntegerSolution,
+    PermutationSolution,
+    Solution,
+)
 from jmetal.util.ckecking import Check
 
 """
 .. module:: crossover
    :platform: Unix, Windows
    :synopsis: Module implementing crossover operators.
 
@@ -18,37 +24,37 @@
 
 class NullCrossover(Crossover[Solution, Solution]):
     def __init__(self):
         super(NullCrossover, self).__init__(probability=0.0)
 
     def execute(self, parents: List[Solution]) -> List[Solution]:
         if len(parents) != 2:
-            raise Exception('The number of parents is not two: {}'.format(len(parents)))
+            raise Exception("The number of parents is not two: {}".format(len(parents)))
 
         return parents
 
     def get_number_of_parents(self) -> int:
         return 2
 
     def get_number_of_children(self) -> int:
         return 2
 
     def get_name(self):
-        return 'Null crossover'
+        return "Null crossover"
 
 
 class PMXCrossover(Crossover[PermutationSolution, PermutationSolution]):
     def __init__(self, probability: float):
         super(PMXCrossover, self).__init__(probability=probability)
 
     def execute(self, parents: List[PermutationSolution]) -> List[PermutationSolution]:
         if len(parents) != 2:
-            raise Exception('The number of parents is not two: {}'.format(len(parents)))
+            raise Exception("The number of parents is not two: {}".format(len(parents)))
 
-        offspring = [copy.deepcopy(parents[0]), copy.deepcopy(parents[1])]
+        offspring = copy.deepcopy(parents)
         permutation_length = offspring[0].number_of_variables
 
         rand = random.random()
         if rand <= self.probability:
             cross_points = sorted([random.randint(0, permutation_length) for _ in range(2)])
 
             def _repeated(element, collection):
@@ -87,73 +93,72 @@
     def get_number_of_parents(self) -> int:
         return 2
 
     def get_number_of_children(self) -> int:
         return 2
 
     def get_name(self):
-        return 'Partially Matched crossover'
+        return "Partially Matched crossover"
 
 
 class CXCrossover(Crossover[PermutationSolution, PermutationSolution]):
     def __init__(self, probability: float):
         super(CXCrossover, self).__init__(probability=probability)
 
     def execute(self, parents: List[PermutationSolution]) -> List[PermutationSolution]:
         if len(parents) != 2:
-            raise Exception('The number of parents is not two: {}'.format(len(parents)))
+            raise Exception("The number of parents is not two: {}".format(len(parents)))
 
-        offspring = [copy.deepcopy(parents[1]), copy.deepcopy(parents[0])]
+        offspring = copy.deepcopy(parents[::-1])
         rand = random.random()
 
         if rand <= self.probability:
-            for i in range(parents[0].number_of_variables):
-                idx = random.randint(0, len(parents[0].variables[i]) - 1)
-                curr_idx = idx
-                cycle = []
-
-                while True:
-                    cycle.append(curr_idx)
-                    curr_idx = parents[0].variables[i].index(parents[1].variables[i][curr_idx])
-
-                    if curr_idx == idx:
-                        break
-
-                for j in range(len(parents[0].variables[i])):
-                    if j in cycle:
-                        offspring[0].variables[i][j] = parents[0].variables[i][j]
-                        offspring[1].variables[i][j] = parents[0].variables[i][j]
+            idx = random.randint(0, len(parents[0].variables) - 1)
+            curr_idx = idx
+            cycle = []
+
+            while True:
+                cycle.append(curr_idx)
+                curr_idx = parents[0].variables.index(parents[1].variables[curr_idx])
+
+                if curr_idx == idx:
+                    break
+
+            for j in range(len(parents[0].variables)):
+                if j in cycle:
+                    offspring[0].variables[j] = parents[0].variables[j]
+                    offspring[1].variables[j] = parents[1].variables[j]
 
         return offspring
 
     def get_number_of_parents(self) -> int:
         return 2
 
     def get_number_of_children(self) -> int:
         return 2
 
     def get_name(self):
-        return 'Cycle crossover'
+        return "Cycle crossover"
 
 
 class SBXCrossover(Crossover[FloatSolution, FloatSolution]):
     __EPS = 1.0e-14
 
     def __init__(self, probability: float, distribution_index: float = 20.0):
         super(SBXCrossover, self).__init__(probability=probability)
         self.distribution_index = distribution_index
         if distribution_index < 0:
             raise Exception("The distribution index is negative: " + str(distribution_index))
 
     def execute(self, parents: List[FloatSolution]) -> List[FloatSolution]:
         Check.that(issubclass(type(parents[0]), FloatSolution), "Solution type invalid: " + str(type(parents[0])))
         Check.that(issubclass(type(parents[1]), FloatSolution), "Solution type invalid")
-        Check.that(len(parents) == 2, 'The number of parents is not two: {}'.format(len(parents)))
+        Check.that(len(parents) == 2, "The number of parents is not two: {}".format(len(parents)))
 
-        offspring = [copy.deepcopy(parents[0]), copy.deepcopy(parents[1])]
+        offspring = copy.deepcopy(parents)
         rand = random.random()
 
         if rand <= self.probability:
             for i in range(parents[0].number_of_variables):
                 value_x1, value_x2 = parents[0].variables[i], parents[1].variables[i]
 
                 if random.random() <= 0.5:
@@ -211,30 +216,30 @@
     def get_number_of_parents(self) -> int:
         return 2
 
     def get_number_of_children(self) -> int:
         return 2
 
     def get_name(self) -> str:
-        return 'SBX crossover'
+        return "SBX crossover"
 
 
 class IntegerSBXCrossover(Crossover[IntegerSolution, IntegerSolution]):
     __EPS = 1.0e-14
 
     def __init__(self, probability: float, distribution_index: float = 20.0):
         super(IntegerSBXCrossover, self).__init__(probability=probability)
         self.distribution_index = distribution_index
 
     def execute(self, parents: List[IntegerSolution]) -> List[IntegerSolution]:
         Check.that(issubclass(type(parents[0]), IntegerSolution), "Solution type invalid")
         Check.that(issubclass(type(parents[1]), IntegerSolution), "Solution type invalid")
-        Check.that(len(parents) == 2, 'The number of parents is not two: {}'.format(len(parents)))
+        Check.that(len(parents) == 2, "The number of parents is not two: {}".format(len(parents)))
 
-        offspring = [copy.deepcopy(parents[0]), copy.deepcopy(parents[1])]
+        offspring = copy.deepcopy(parents)
         rand = random.random()
 
         if rand <= self.probability:
             for i in range(parents[0].number_of_variables):
                 value_x1, value_x2 = parents[0].variables[i], parents[1].variables[i]
 
                 if random.random() <= 0.5:
@@ -292,28 +297,27 @@
     def get_number_of_parents(self) -> int:
         return 2
 
     def get_number_of_children(self) -> int:
         return 2
 
     def get_name(self) -> str:
-        return 'Integer SBX crossover'
+        return "Integer SBX crossover"
 
 
 class SPXCrossover(Crossover[BinarySolution, BinarySolution]):
-
     def __init__(self, probability: float):
         super(SPXCrossover, self).__init__(probability=probability)
 
     def execute(self, parents: List[BinarySolution]) -> List[BinarySolution]:
         Check.that(type(parents[0]) is BinarySolution, "Solution type invalid")
         Check.that(type(parents[1]) is BinarySolution, "Solution type invalid")
-        Check.that(len(parents) == 2, 'The number of parents is not two: {}'.format(len(parents)))
+        Check.that(len(parents) == 2, "The number of parents is not two: {}".format(len(parents)))
 
-        offspring = [copy.deepcopy(parents[0]), copy.deepcopy(parents[1])]
+        offspring = copy.deepcopy(parents)
         rand = random.random()
 
         if rand <= self.probability:
             # 1. Get the total number of bits
             total_number_of_bits = parents[0].get_total_number_of_bits()
 
             # 2. Calculate the point to make the crossover
@@ -352,37 +356,36 @@
     def get_number_of_parents(self) -> int:
         return 2
 
     def get_number_of_children(self) -> int:
         return 2
 
     def get_name(self) -> str:
-        return 'Single point crossover'
+        return "Single point crossover"
 
 
 class DifferentialEvolutionCrossover(Crossover[FloatSolution, FloatSolution]):
-    """ This operator receives two parameters: the current individual and an array of three parent individuals. The
+    """This operator receives two parameters: the current individual and an array of three parent individuals. The
     best and rand variants depends on the third parent, according whether it represents the current of the "best"
     individual or a random_search one. The implementation of both variants are the same, due to that the parent selection is
     external to the crossover operator.
     """
 
     def __init__(self, CR: float, F: float, K: float = 0.5):
         super(DifferentialEvolutionCrossover, self).__init__(probability=1.0)
         self.CR = CR
         self.F = F
         self.K = K
 
         self.current_individual: FloatSolution = None
 
     def execute(self, parents: List[FloatSolution]) -> List[FloatSolution]:
-        """ Execute the differential evolution crossover ('best/1/bin' variant in jMetal).
-        """
+        """Execute the differential evolution crossover ('best/1/bin' variant in jMetal)."""
         if len(parents) != self.get_number_of_parents():
-            raise Exception('The number of parents is not {}: {}'.format(self.get_number_of_parents(), len(parents)))
+            raise Exception("The number of parents is not {}: {}".format(self.get_number_of_parents(), len(parents)))
 
         child = copy.deepcopy(self.current_individual)
 
         number_of_variables = parents[0].number_of_variables
         rand = random.randint(0, number_of_variables - 1)
 
         for i in range(number_of_variables):
@@ -403,21 +406,21 @@
     def get_number_of_parents(self) -> int:
         return 3
 
     def get_number_of_children(self) -> int:
         return 1
 
     def get_name(self) -> str:
-        return 'Differential Evolution crossover'
+        return "Differential Evolution crossover"
 
 
 class CompositeCrossover(Crossover[CompositeSolution, CompositeSolution]):
     __EPS = 1.0e-14
 
-    def __init__(self, crossover_operator_list:[Crossover]):
+    def __init__(self, crossover_operator_list: [Crossover]):
         super(CompositeCrossover, self).__init__(probability=1.0)
 
         Check.is_not_none(crossover_operator_list)
         Check.collection_is_not_empty(crossover_operator_list)
 
         self.crossover_operators_list = []
         for operator in crossover_operator_list:
@@ -444,8 +447,8 @@
     def get_number_of_parents(self) -> int:
         return 2
 
     def get_number_of_children(self) -> int:
         return 2
 
     def get_name(self) -> str:
-        return 'Composite crossover'
+        return "Composite crossover"
```

### Comparing `jmetalpy-1.5.5/jmetal/operator/mutation.py` & `jmetalpy-1.6.0/jmetal/operator/mutation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 import random
 
 from jmetal.core.operator import Mutation
-from jmetal.core.solution import BinarySolution, Solution, FloatSolution, IntegerSolution, PermutationSolution, \
-    CompositeSolution
+from jmetal.core.solution import (
+    BinarySolution,
+    CompositeSolution,
+    FloatSolution,
+    IntegerSolution,
+    PermutationSolution,
+    Solution,
+)
 from jmetal.util.ckecking import Check
 
 """
 .. module:: mutation
    :platform: Unix, Windows
    :synopsis: Module implementing mutation operators.
 
 .. moduleauthor:: Antonio J. Nebro <antonio@lcc.uma.es>, Antonio Benítez-Hidalgo <antonio.b@uma.es>
 """
 
 
 class NullMutation(Mutation[Solution]):
-
     def __init__(self):
         super(NullMutation, self).__init__(probability=0)
 
     def execute(self, solution: Solution) -> Solution:
         return solution
 
     def get_name(self):
-        return 'Null mutation'
+        return "Null mutation"
 
 
 class BitFlipMutation(Mutation[BinarySolution]):
-
     def __init__(self, probability: float):
         super(BitFlipMutation, self).__init__(probability=probability)
 
     def execute(self, solution: BinarySolution) -> BinarySolution:
         Check.that(type(solution) is BinarySolution, "Solution type invalid")
 
         for i in range(solution.number_of_variables):
@@ -39,19 +43,18 @@
                 rand = random.random()
                 if rand <= self.probability:
                     solution.variables[i][j] = True if solution.variables[i][j] is False else False
 
         return solution
 
     def get_name(self):
-        return 'BitFlip mutation'
+        return "BitFlip mutation"
 
 
 class PolynomialMutation(Mutation[FloatSolution]):
-
     def __init__(self, probability: float, distribution_index: float = 0.20):
         super(PolynomialMutation, self).__init__(probability=probability)
         self.distribution_index = distribution_index
 
     def execute(self, solution: FloatSolution) -> FloatSolution:
         Check.that(issubclass(type(solution), FloatSolution), "Solution type invalid")
         for i in range(solution.number_of_variables):
@@ -84,19 +87,18 @@
                         y = solution.upper_bound[i]
 
                 solution.variables[i] = y
 
         return solution
 
     def get_name(self):
-        return 'Polynomial mutation'
+        return "Polynomial mutation"
 
 
 class IntegerPolynomialMutation(Mutation[IntegerSolution]):
-
     def __init__(self, probability: float, distribution_index: float = 0.20):
         super(IntegerPolynomialMutation, self).__init__(probability=probability)
         self.distribution_index = distribution_index
 
     def execute(self, solution: IntegerSolution) -> IntegerSolution:
         Check.that(issubclass(type(solution), IntegerSolution), "Solution type invalid")
 
@@ -111,54 +113,53 @@
                     delta1 = (y - yl) / (yu - yl)
                     delta2 = (yu - y) / (yu - yl)
                     mut_pow = 1.0 / (self.distribution_index + 1.0)
                     rnd = random.random()
                     if rnd <= 0.5:
                         xy = 1.0 - delta1
                         val = 2.0 * rnd + (1.0 - 2.0 * rnd) * (xy ** (self.distribution_index + 1.0))
-                        deltaq = val ** mut_pow - 1.0
+                        deltaq = val**mut_pow - 1.0
                     else:
                         xy = 1.0 - delta2
                         val = 2.0 * (1.0 - rnd) + 2.0 * (rnd - 0.5) * (xy ** (self.distribution_index + 1.0))
-                        deltaq = 1.0 - val ** mut_pow
+                        deltaq = 1.0 - val**mut_pow
 
                     y += deltaq * (yu - yl)
                     if y < solution.lower_bound[i]:
                         y = solution.lower_bound[i]
                     if y > solution.upper_bound[i]:
                         y = solution.upper_bound[i]
 
                 solution.variables[i] = int(round(y))
         return solution
 
     def get_name(self):
-        return 'Polynomial mutation (Integer)'
+        return "Polynomial mutation (Integer)"
 
 
 class SimpleRandomMutation(Mutation[FloatSolution]):
-
     def __init__(self, probability: float):
         super(SimpleRandomMutation, self).__init__(probability=probability)
 
     def execute(self, solution: FloatSolution) -> FloatSolution:
         Check.that(type(solution) is FloatSolution, "Solution type invalid")
 
         for i in range(solution.number_of_variables):
             rand = random.random()
             if rand <= self.probability:
-                solution.variables[i] = solution.lower_bound[i] + \
-                                        (solution.upper_bound[i] - solution.lower_bound[i]) * random.random()
+                solution.variables[i] = (
+                    solution.lower_bound[i] + (solution.upper_bound[i] - solution.lower_bound[i]) * random.random()
+                )
         return solution
 
     def get_name(self):
-        return 'Simple random_search mutation'
+        return "Simple random_search mutation"
 
 
 class UniformMutation(Mutation[FloatSolution]):
-
     def __init__(self, probability: float, perturbation: float = 0.5):
         super(UniformMutation, self).__init__(probability=probability)
         self.perturbation = perturbation
 
     def execute(self, solution: FloatSolution) -> FloatSolution:
         Check.that(type(solution) is FloatSolution, "Solution type invalid")
 
@@ -175,19 +176,18 @@
                     tmp = solution.upper_bound[i]
 
                 solution.variables[i] = tmp
 
         return solution
 
     def get_name(self):
-        return 'Uniform mutation'
+        return "Uniform mutation"
 
 
 class NonUniformMutation(Mutation[FloatSolution]):
-
     def __init__(self, probability: float, perturbation: float = 0.5, max_iterations: int = 0.5):
         super(NonUniformMutation, self).__init__(probability=probability)
         self.perturbation = perturbation
         self.max_iterations = max_iterations
         self.current_iteration = 0
 
     def execute(self, solution: FloatSolution) -> FloatSolution:
@@ -213,42 +213,47 @@
 
         return solution
 
     def set_current_iteration(self, current_iteration: int):
         self.current_iteration = current_iteration
 
     def __delta(self, y: float, b_mutation_parameter: float):
-        return (y * (1.0 - pow(random.random(),
-                               pow((1.0 - 1.0 * self.current_iteration / self.max_iterations), b_mutation_parameter))))
+        return y * (
+            1.0
+            - pow(
+                random.random(), pow((1.0 - 1.0 * self.current_iteration / self.max_iterations), b_mutation_parameter)
+            )
+        )
 
     def get_name(self):
-        return 'Uniform mutation'
+        return "Uniform mutation"
 
 
 class PermutationSwapMutation(Mutation[PermutationSolution]):
-
     def execute(self, solution: PermutationSolution) -> PermutationSolution:
         Check.that(type(solution) is PermutationSolution, "Solution type invalid")
 
         rand = random.random()
 
         if rand <= self.probability:
-            pos_one, pos_two = random.sample(range(solution.number_of_variables - 1), 2)
-            solution.variables[pos_one], solution.variables[pos_two] = \
-                solution.variables[pos_two], solution.variables[pos_one]
+            pos_one, pos_two = random.sample(range(solution.number_of_variables), 2)
+            solution.variables[pos_one], solution.variables[pos_two] = (
+                solution.variables[pos_two],
+                solution.variables[pos_one],
+            )
 
         return solution
 
     def get_name(self):
-        return 'Permutation Swap mutation'
+        return "Permutation Swap mutation"
 
 
 class CompositeMutation(Mutation[Solution]):
-    def __init__(self, mutation_operator_list:[Mutation]):
-        super(CompositeMutation,self).__init__(probability=1.0)
+    def __init__(self, mutation_operator_list: [Mutation]):
+        super(CompositeMutation, self).__init__(probability=1.0)
 
         Check.is_not_none(mutation_operator_list)
         Check.collection_is_not_empty(mutation_operator_list)
 
         self.mutation_operators_list = []
         for operator in mutation_operator_list:
             Check.that(issubclass(operator.__class__, Mutation), "Object is not a subclass of Mutation")
@@ -264,31 +269,29 @@
         return CompositeSolution(mutated_solution_components)
 
     def get_name(self) -> str:
         return "Composite mutation operator"
 
 
 class ScrambleMutation(Mutation[PermutationSolution]):
-
     def execute(self, solution: PermutationSolution) -> PermutationSolution:
-        for i in range(solution.number_of_variables):
-            rand = random.random()
+        rand = random.random()
 
-            if rand <= self.probability:
-                point1 = random.randint(0, len(solution.variables[i]))
-                point2 = random.randint(0, len(solution.variables[i]) - 1)
+        if rand <= self.probability:
+            point1 = random.randint(0, len(solution.variables))
+            point2 = random.randint(0, len(solution.variables) - 1)
 
-                if point2 >= point1:
-                    point2 += 1
-                else:
-                    point1, point2 = point2, point1
+            if point2 >= point1:
+                point2 += 1
+            else:
+                point1, point2 = point2, point1
 
-                if point2 - point1 >= 20:
-                    point2 = point1 + 20
+            if point2 - point1 >= 20:
+                point2 = point1 + 20
 
-                values = solution.variables[i][point1:point2]
-                solution.variables[i][point1:point2] = random.sample(values, len(values))
+            values = solution.variables[point1:point2]
+            solution.variables[point1:point2] = random.sample(values, len(values))
 
         return solution
 
     def get_name(self):
-        return 'Scramble'
+        return "Scramble"
```

### Comparing `jmetalpy-1.5.5/jmetal/operator/selection.py` & `jmetalpy-1.6.0/jmetal/operator/selection.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,68 +1,67 @@
 import random
 from typing import List, TypeVar
 
 import numpy as np
 
 from jmetal.core.operator import Selection
+from jmetal.core.solution import Solution
 from jmetal.util.comparator import Comparator, DominanceComparator
 from jmetal.util.density_estimator import CrowdingDistance
 from jmetal.util.ranking import FastNonDominatedRanking
 
-S = TypeVar('S')
+S = TypeVar("S", bound=Solution)
 
 """
 .. module:: selection
    :platform: Unix, Windows
    :synopsis: Module implementing selection operators.
 
 .. moduleauthor:: Antonio J. Nebro <antonio@lcc.uma.es>, Antonio Benítez-Hidalgo <antonio.b@uma.es>
 """
 
 
 class RouletteWheelSelection(Selection[List[S], S]):
-    """Performs roulette wheel selection.
-    """
+    """Performs roulette wheel selection."""
 
     def __init__(self):
         super(RouletteWheelSelection).__init__()
 
     def execute(self, front: List[S]) -> S:
         if front is None:
-            raise Exception('The front is null')
+            raise Exception("The front is null")
         elif len(front) == 0:
-            raise Exception('The front is empty')
+            raise Exception("The front is empty")
 
         maximum = sum([solution.objectives[0] for solution in front])
         rand = random.uniform(0.0, maximum)
         value = 0.0
 
         for solution in front:
             value += solution.objectives[0]
 
             if value > rand:
                 return solution
 
         return None
 
     def get_name(self) -> str:
-        return 'Roulette wheel selection'
+        return "Roulette wheel selection"
 
 
 class BinaryTournamentSelection(Selection[List[S], S]):
-
     def __init__(self, comparator: Comparator = DominanceComparator()):
         super(BinaryTournamentSelection, self).__init__()
         self.comparator = comparator
 
     def execute(self, front: List[S]) -> S:
         if front is None:
-            raise Exception('The front is null')
+            raise Exception("The front is null")
         elif len(front) == 0:
-            raise Exception('The front is empty')
+            raise Exception("The front is empty")
 
         if len(front) == 1:
             result = front[0]
         else:
             # Sampling without replacement
             i, j = random.sample(range(0, len(front)), 2)
             solution1 = front[i]
@@ -76,77 +75,74 @@
                 result = solution2
             else:
                 result = [solution1, solution2][random.random() < 0.5]
 
         return result
 
     def get_name(self) -> str:
-        return 'Binary tournament selection'
+        return "Binary tournament selection"
 
 
 class BestSolutionSelection(Selection[List[S], S]):
-
     def __init__(self):
         super(BestSolutionSelection, self).__init__()
 
     def execute(self, front: List[S]) -> S:
         if front is None:
-            raise Exception('The front is null')
+            raise Exception("The front is null")
         elif len(front) == 0:
-            raise Exception('The front is empty')
+            raise Exception("The front is empty")
 
         result = front[0]
 
         for solution in front[1:]:
             if DominanceComparator().compare(solution, result) < 0:
                 result = solution
 
         return result
 
     def get_name(self) -> str:
-        return 'Best solution selection'
+        return "Best solution selection"
 
 
 class NaryRandomSolutionSelection(Selection[List[S], S]):
-
     def __init__(self, number_of_solutions_to_be_returned: int = 1):
         super(NaryRandomSolutionSelection, self).__init__()
         if number_of_solutions_to_be_returned < 0:
-            raise Exception('The number of solutions to be returned must be positive integer')
+            raise Exception("The number of solutions to be returned must be positive integer")
 
         self.number_of_solutions_to_be_returned = number_of_solutions_to_be_returned
 
     def execute(self, front: List[S]) -> S:
         if front is None:
-            raise Exception('The front is null')
+            raise Exception("The front is null")
         if len(front) == 0:
-            raise Exception('The front is empty')
+            raise Exception("The front is empty")
         if len(front) < self.number_of_solutions_to_be_returned:
-            raise Exception('The front contains less elements than required')
+            raise Exception("The front contains less elements than required")
 
         # random_search sampling without replacement
         return random.sample(front, self.number_of_solutions_to_be_returned)
 
     def get_name(self) -> str:
-        return 'Nary random_search solution selection'
+        return "Nary random_search solution selection"
 
 
 class DifferentialEvolutionSelection(Selection[List[S], List[S]]):
-
     def __init__(self):
         super(DifferentialEvolutionSelection, self).__init__()
         self.index_to_exclude = None
 
     def execute(self, front: List[S]) -> List[S]:
         if front is None:
-            raise Exception('The front is null')
+            raise Exception("The front is null")
         elif len(front) == 0:
-            raise Exception('The front is empty')
+            raise Exception("The front is empty")
         elif len(front) < 4:
-            raise Exception('The front has less than four solutions: ' + str(len(front)))
+            raise Exception("The front has less than four solutions: " + str(len(front)))
 
         selected_indexes = random.sample(range(len(front)), 3)
         while self.index_to_exclude in selected_indexes:
             selected_indexes = random.sample(range(len(front)), 3)
 
         return [front[i] for i in selected_indexes]
 
@@ -154,42 +150,40 @@
         self.index_to_exclude = index
 
     def get_name(self) -> str:
         return "Differential evolution selection"
 
 
 class RandomSolutionSelection(Selection[List[S], S]):
-
     def __init__(self):
         super(RandomSolutionSelection, self).__init__()
 
     def execute(self, front: List[S]) -> S:
         if front is None:
-            raise Exception('The front is null')
+            raise Exception("The front is null")
         elif len(front) == 0:
-            raise Exception('The front is empty')
+            raise Exception("The front is empty")
 
         return random.choice(front)
 
     def get_name(self) -> str:
-        return 'Random solution selection'
+        return "Random solution selection"
 
 
 class RankingAndCrowdingDistanceSelection(Selection[List[S], List[S]]):
-
     def __init__(self, max_population_size: int, dominance_comparator: Comparator = DominanceComparator()):
         super(RankingAndCrowdingDistanceSelection, self).__init__()
         self.max_population_size = max_population_size
         self.dominance_comparator = dominance_comparator
 
     def execute(self, front: List[S]) -> List[S]:
         if front is None:
-            raise Exception('The front is null')
+            raise Exception("The front is null")
         elif len(front) == 0:
-            raise Exception('The front is empty')
+            raise Exception("The front is empty")
 
         ranking = FastNonDominatedRanking(self.dominance_comparator)
         crowding_distance = CrowdingDistance()
         ranking.compute_ranking(front)
 
         ranking_index = 0
         new_solution_list = []
@@ -197,29 +191,28 @@
         while len(new_solution_list) < self.max_population_size:
             if len(ranking.get_subfront(ranking_index)) < (self.max_population_size - len(new_solution_list)):
                 new_solution_list = new_solution_list + ranking.get_subfront(ranking_index)
                 ranking_index += 1
             else:
                 subfront = ranking.get_subfront(ranking_index)
                 crowding_distance.compute_density_estimator(subfront)
-                sorted_subfront = sorted(subfront, key=lambda x: x.attributes['crowding_distance'], reverse=True)
+                sorted_subfront = sorted(subfront, key=lambda x: x.attributes["crowding_distance"], reverse=True)
                 for i in range((self.max_population_size - len(new_solution_list))):
                     new_solution_list.append(sorted_subfront[i])
 
         return new_solution_list
 
     def get_name(self) -> str:
-        return 'Ranking and crowding distance selection'
+        return "Ranking and crowding distance selection"
 
 
 class RankingAndFitnessSelection(Selection[List[S], List[S]]):
-
-    def __init__(self,
-                 max_population_size: int, reference_point: S,
-                 dominance_comparator: Comparator = DominanceComparator()):
+    def __init__(
+        self, max_population_size: int, reference_point: S, dominance_comparator: Comparator = DominanceComparator()
+    ):
         super(RankingAndFitnessSelection, self).__init__()
         self.max_population_size = max_population_size
         self.dominance_comparator = dominance_comparator
         self.reference_point = reference_point
 
     def hypesub(self, l, A, actDim, bounds, pvec, alpha, k):
         h = [0 for _ in range(l)]
@@ -238,16 +231,18 @@
                 if i > k:
                     break
                 if all(alpha) >= 0:
                     for p in pvec[0:i]:
                         h[p] = h[p] + extrusion * alpha[i - 1]
             else:
                 if extrusion > 0:
-                    h = [h[j] + extrusion * self.hypesub(l, S[0:i], actDim - 1, bounds, pvec[0:i], alpha, k)[j] for j in
-                         range(l)]
+                    h = [
+                        h[j] + extrusion * self.hypesub(l, S[0:i], actDim - 1, bounds, pvec[0:i], alpha, k)[j]
+                        for j in range(l)
+                    ]
 
         return h
 
     def compute_hypervol_fitness_values(self, population: List[S], reference_point: S, k: int):
         points = [ind.objectives for ind in population]
         bounds = reference_point.objectives
         population_size = len(points)
@@ -261,23 +256,23 @@
 
         for i in range(1, k + 1):
             alpha.append(np.prod([float(k - j) / (population_size - j) for j in range(1, i)]) / i)
 
         f = self.hypesub(population_size, points, actDim, bounds, pvec, alpha, k)
 
         for i in range(len(population)):
-            population[i].attributes['fitness'] = f[i]
+            population[i].attributes["fitness"] = f[i]
 
         return population
 
     def execute(self, front: List[S]) -> List[S]:
         if front is None:
-            raise Exception('The front is null')
+            raise Exception("The front is null")
         elif len(front) == 0:
-            raise Exception('The front is empty')
+            raise Exception("The front is empty")
 
         ranking = FastNonDominatedRanking(self.dominance_comparator)
         ranking.compute_ranking(front)
 
         ranking_index = 0
         new_solution_list = []
 
@@ -287,37 +282,36 @@
                 new_solution_list = new_solution_list + subfront
                 ranking_index += 1
             else:
                 subfront = ranking.get_subfront(ranking_index)
                 parameter_K = len(subfront) - (self.max_population_size - len(new_solution_list))
                 while parameter_K > 0:
                     subfront = self.compute_hypervol_fitness_values(subfront, self.reference_point, parameter_K)
-                    subfront = sorted(subfront, key=lambda x: x.attributes['fitness'], reverse=True)
+                    subfront = sorted(subfront, key=lambda x: x.attributes["fitness"], reverse=True)
                     subfront = subfront[:-1]
                     parameter_K = parameter_K - 1
                 new_solution_list = new_solution_list + subfront
         return new_solution_list
 
     def get_name(self) -> str:
-        return 'Ranking and fitness selection'
+        return "Ranking and fitness selection"
 
 
 class BinaryTournament2Selection(Selection[List[S], S]):
-
     def __init__(self, comparator_list: List[Comparator]):
         super(BinaryTournament2Selection, self).__init__()
         self.comparator_list = comparator_list
 
     def execute(self, front: List[S]) -> S:
         if front is None:
-            raise Exception('The front is null')
+            raise Exception("The front is null")
         elif len(front) == 0:
-            raise Exception('The front is empty')
+            raise Exception("The front is empty")
         elif not self.comparator_list:
-            raise Exception('The comparators\' list is empty')
+            raise Exception("The comparators' list is empty")
 
         winner = None
 
         if len(front) == 1:
             winner = front[0]
         else:
             for comparator in self.comparator_list:
@@ -346,8 +340,8 @@
             result = solution2
         else:
             result = None
 
         return result
 
     def get_name(self) -> str:
-        return 'Binary tournament selection (experimental)'
+        return "Binary tournament selection (experimental)"
```

### Comparing `jmetalpy-1.5.5/jmetal/operator/test/test_crossover.py` & `jmetalpy-1.6.0/jmetal/operator/test/test_crossover.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,36 @@
 import unittest
 from typing import List
 from unittest import mock
 
 from jmetal.core.operator import Crossover
-from jmetal.core.solution import BinarySolution, PermutationSolution, FloatSolution, CompositeSolution, IntegerSolution
-from jmetal.operator.crossover import NullCrossover, SPXCrossover, CXCrossover, PMXCrossover, SBXCrossover, \
-    CompositeCrossover, IntegerSBXCrossover
-from jmetal.util.ckecking import NoneParameterException, EmptyCollectionException, InvalidConditionException
+from jmetal.core.solution import (
+    BinarySolution,
+    CompositeSolution,
+    FloatSolution,
+    IntegerSolution,
+    PermutationSolution,
+)
+from jmetal.operator.crossover import (
+    CompositeCrossover,
+    CXCrossover,
+    IntegerSBXCrossover,
+    NullCrossover,
+    PMXCrossover,
+    SBXCrossover,
+    SPXCrossover,
+)
+from jmetal.util.ckecking import (
+    EmptyCollectionException,
+    InvalidConditionException,
+    NoneParameterException,
+)
 
 
 class NullCrossoverTestCases(unittest.TestCase):
-
     def test_should_constructor_create_a_non_null_object(self):
         solution = NullCrossover()
         self.assertIsNotNone(solution)
 
     def test_should_constructor_create_a_valid_operator(self):
         operator = NullCrossover()
         self.assertEqual(0, operator.probability)
@@ -28,15 +44,14 @@
 
         offspring = operator.execute([solution1, solution2])
         self.assertEqual([True, False, False, True, True, False], offspring[0].variables[0])
         self.assertEqual([False, True, False, False, True, False], offspring[1].variables[0])
 
 
 class SinglePointTestCases(unittest.TestCase):
-
     def test_should_constructor_raises_an_exception_is_probability_is_negative(self) -> None:
         with self.assertRaises(Exception):
             SPXCrossover(-1)
 
     def test_should_constructor_raises_an_exception_is_probability_is_higher_than_one(self) -> None:
         with self.assertRaises(Exception):
             SPXCrossover(1.01)
@@ -64,54 +79,54 @@
         solution2 = BinarySolution(number_of_variables=1, number_of_objectives=1)
         solution2.variables[0] = [False, True, False, False, True, False]
 
         offspring = operator.execute([solution1, solution2])
         self.assertEqual([True, False, False, True, True, False], offspring[0].variables[0])
         self.assertEqual([False, True, False, False, True, False], offspring[1].variables[0])
 
-    @mock.patch('random.randrange')
+    @mock.patch("random.randrange")
     def test_should_the_operator_work_if_the_first_bit_is_selected(self, random_call):
         operator = SPXCrossover(1.0)
         solution1 = BinarySolution(number_of_variables=1, number_of_objectives=1)
         solution1.variables[0] = [True, False, False, True, True, False]
         solution2 = BinarySolution(number_of_variables=1, number_of_objectives=1)
         solution2.variables[0] = [False, True, False, False, True, False]
 
         random_call.return_value = 0
         offspring = operator.execute([solution1, solution2])
         self.assertEqual([False, True, False, False, True, False], offspring[0].variables[0])
         self.assertEqual([True, False, False, True, True, False], offspring[1].variables[0])
 
-    @mock.patch('random.randrange')
+    @mock.patch("random.randrange")
     def test_should_the_operator_work_if_the_last_bit_is_selected(self, random_call):
         operator = SPXCrossover(1.0)
         solution1 = BinarySolution(number_of_variables=1, number_of_objectives=1)
         solution1.variables[0] = [True, False, False, True, True, False]
         solution2 = BinarySolution(number_of_variables=1, number_of_objectives=1)
         solution2.variables[0] = [False, True, False, False, True, True]
 
         random_call.return_value = 5
         offspring = operator.execute([solution1, solution2])
         self.assertEqual([True, False, False, True, True, True], offspring[0].variables[0])
         self.assertEqual([False, True, False, False, True, False], offspring[1].variables[0])
 
-    @mock.patch('random.randrange')
+    @mock.patch("random.randrange")
     def test_should_the_operator_work_if_the_third_bit_is_selected(self, random_call):
         operator = SPXCrossover(1.0)
         solution1 = BinarySolution(number_of_variables=1, number_of_objectives=1)
         solution1.variables[0] = [True, False, False, True, True, False]
         solution2 = BinarySolution(number_of_variables=1, number_of_objectives=1)
         solution2.variables[0] = [False, True, False, False, True, True]
 
         random_call.return_value = 3
         offspring = operator.execute([solution1, solution2])
         self.assertEqual([True, False, False, False, True, True], offspring[0].variables[0])
         self.assertEqual([False, True, False, True, True, False], offspring[1].variables[0])
 
-    @mock.patch('random.randrange')
+    @mock.patch("random.randrange")
     def test_should_the_operator_work_with_a_solution_with_three_binary_variables(self, random_call):
         operator = SPXCrossover(1.0)
         solution1 = BinarySolution(number_of_variables=3, number_of_objectives=1)
         solution1.variables[0] = [True, False, False, True, True, False]
         solution1.variables[1] = [True, False, False, True, False, False]
         solution1.variables[2] = [True, False, True, True, True, True]
         solution2 = BinarySolution(number_of_variables=3, number_of_objectives=1)
@@ -126,15 +141,14 @@
         self.assertEqual([True, True, True, False, False, True], offspring[0].variables[2])
         self.assertEqual([False, True, False, False, True, True], offspring[1].variables[0])
         self.assertEqual([True, True, False, True, False, False], offspring[1].variables[1])
         self.assertEqual([True, False, True, True, True, True], offspring[1].variables[2])
 
 
 class PMXTestCases(unittest.TestCase):
-
     def test_should_constructor_raises_an_exception_is_probability_is_negative(self) -> None:
         with self.assertRaises(Exception):
             PMXCrossover(-1)
 
     def test_should_constructor_raises_an_exception_is_probability_is_higher_than_one(self) -> None:
         with self.assertRaises(Exception):
             PMXCrossover(1.01)
@@ -161,15 +175,15 @@
 
         self.assertEqual([1, 2], offspring[0].variables[0])
         self.assertEqual([2, 6], offspring[0].variables[1])
 
         self.assertEqual([2, 3], offspring[1].variables[0])
         self.assertEqual([5, 3], offspring[1].variables[1])
 
-    @mock.patch('random.randint')
+    @mock.patch("random.randint")
     def test_should_the_operator_work_with_permutation_at_the_middle(self, random_call):
         operator = PMXCrossover(1.0)
 
         solution1 = PermutationSolution(number_of_variables=10, number_of_objectives=1)
         solution1.variables = [i for i in range(10)]
 
         solution2 = PermutationSolution(number_of_variables=10, number_of_objectives=1)
@@ -177,15 +191,15 @@
 
         random_call.side_effect = (2, 4)
         offspring = operator.execute([solution1, solution2])
 
         self.assertEqual([0, 1, 12, 13, 4, 5, 6, 7, 8, 9], offspring[0].variables)
         self.assertEqual([10, 11, 2, 3, 14, 15, 16, 17, 18, 19], offspring[1].variables)
 
-    @mock.patch('random.randint')
+    @mock.patch("random.randint")
     def test_should_the_operator_work_with_permutation_at_the_beginning(self, random_call):
         operator = PMXCrossover(1.0)
 
         solution1 = PermutationSolution(number_of_variables=10, number_of_objectives=1)
         solution1.variables = [i for i in range(10)]
 
         solution2 = PermutationSolution(number_of_variables=10, number_of_objectives=1)
@@ -195,15 +209,14 @@
         offspring = operator.execute([solution1, solution2])
 
         self.assertEqual([10, 11, 12, 13, 14, 5, 6, 7, 8, 9], offspring[0].variables)
         self.assertEqual([0, 1, 2, 3, 4, 15, 16, 17, 18, 19], offspring[1].variables)
 
 
 class CXTestCases(unittest.TestCase):
-
     def test_should_constructor_raises_an_exception_is_probability_is_negative(self) -> None:
         with self.assertRaises(Exception):
             CXCrossover(-1)
 
     def test_should_constructor_raises_an_exception_is_probability_is_higher_than_one(self) -> None:
         with self.assertRaises(Exception):
             CXCrossover(1.01)
@@ -220,33 +233,29 @@
         with self.assertRaises(Exception):
             CXCrossover(2)
 
     def test_should_constructor_raise_an_exception_if_the_probability_is_lower_than_zero(self):
         with self.assertRaises(Exception):
             CXCrossover(-12)
 
-    @mock.patch('random.randint')
-    def test_should_the_operator_work_with_two_solutions_with_two_variables(self, random_call):
+    @mock.patch("random.randint")
+    def test_should_the_operator_work_with_two_solutions_with_same_number_of_variables(self, random_call):
         operator = CXCrossover(1.0)
-        solution1 = PermutationSolution(number_of_variables=2, number_of_objectives=1)
-        solution1.variables[0] = [1, 2, 3, 4, 7]
-        solution1.variables[1] = [2, 6, 4, 5, 3]
+        solution1 = PermutationSolution(number_of_variables=5, number_of_objectives=1)
+        solution1.variables = [1, 2, 3, 4, 7]
 
-        solution2 = PermutationSolution(number_of_variables=2, number_of_objectives=1)
-        solution2.variables[0] = [2, 3, 4, 1, 9]
-        solution2.variables[1] = [5, 3, 2, 4, 6]
+        solution2 = PermutationSolution(number_of_variables=5, number_of_objectives=1)
+        solution2.variables = [2, 3, 4, 1, 9]
 
         random_call.return_value = 0
         offspring = operator.execute([solution1, solution2])
 
-        self.assertEqual([1, 2, 3, 4, 9], offspring[0].variables[0])
-        self.assertEqual([2, 3, 4, 5, 6], offspring[0].variables[1])
+        self.assertEqual([1, 2, 3, 4, 9], offspring[0].variables)
 
-        self.assertEqual([1, 2, 3, 4, 7], offspring[1].variables[0])
-        self.assertEqual([2, 6, 4, 5, 3], offspring[1].variables[1])
+        self.assertEqual([2, 3, 4, 1, 7], offspring[1].variables)
 
 
 class SBXCrossoverTestCases(unittest.TestCase):
     def test_should_constructor_assign_the_correct_probability_value(self):
         crossover_probability = 0.1
         crossover: SBXCrossover = SBXCrossover(crossover_probability, 2.0)
 
@@ -293,33 +302,38 @@
 
         self.assertEqual(2, len(offspring))
         self.assertEqual(solution1.variables, offspring[0].variables)
         self.assertEqual(solution2.variables, offspring[1].variables)
 
     def test_should_execute_work_with_a_solution_subclass_of_float_solution(self):
         class NewFloatSolution(FloatSolution):
-            def __init__(self, lower_bound: List[float], upper_bound: List[float], number_of_objectives: int,
-                         number_of_constraints: int = 0):
-                super(NewFloatSolution, self).__init__(lower_bound, upper_bound, number_of_objectives,
-                                                       number_of_constraints)
+            def __init__(
+                self,
+                lower_bound: List[float],
+                upper_bound: List[float],
+                number_of_objectives: int,
+                number_of_constraints: int = 0,
+            ):
+                super(NewFloatSolution, self).__init__(
+                    lower_bound, upper_bound, number_of_objectives, number_of_constraints
+                )
 
         solution1 = NewFloatSolution([1, 2], [2, 4], 2, 2)
         solution2 = NewFloatSolution([1, 2], [2, 4], 2, 2)
 
         solution1.variables = [1.5, 2.7]
         solution2.variables = [1.7, 3.6]
 
         crossover: SBXCrossover = SBXCrossover(0.0, 20.0)
         offspring = crossover.execute([solution1, solution2])
 
         self.assertEqual(2, len(offspring))
         self.assertEqual(solution1.variables, offspring[0].variables)
         self.assertEqual(solution2.variables, offspring[1].variables)
 
-
     def test_should_execute_produce_valid_solutions_when_crossing_two_single_variable_solutions(self):
         pass
 
 
 class CompositeCrossoverTestCases(unittest.TestCase):
     def test_should_constructor_raise_an_exception_if_the_parameter_list_is_None(self):
         with self.assertRaises(NoneParameterException):
@@ -397,9 +411,9 @@
         composite_solution1 = CompositeSolution([float_solution1, float_solution2])
         composite_solution2 = CompositeSolution([float_solution1, float_solution2])
 
         with self.assertRaises(InvalidConditionException):
             operator.execute([composite_solution1, composite_solution2])
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `jmetalpy-1.5.5/jmetal/operator/test/test_mutation.py` & `jmetalpy-1.6.0/jmetal/operator/test/test_mutation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,33 @@
 import unittest
 from typing import List
 
 from jmetal.core.operator import Mutation
-from jmetal.core.solution import BinarySolution, FloatSolution, IntegerSolution, CompositeSolution
-from jmetal.operator.mutation import BitFlipMutation, UniformMutation, SimpleRandomMutation, PolynomialMutation, \
-    IntegerPolynomialMutation, CompositeMutation
-from jmetal.util.ckecking import NoneParameterException, EmptyCollectionException, InvalidConditionException
+from jmetal.core.solution import (
+    BinarySolution,
+    CompositeSolution,
+    FloatSolution,
+    IntegerSolution,
+)
+from jmetal.operator.mutation import (
+    BitFlipMutation,
+    CompositeMutation,
+    IntegerPolynomialMutation,
+    PolynomialMutation,
+    SimpleRandomMutation,
+    UniformMutation,
+)
+from jmetal.util.ckecking import (
+    EmptyCollectionException,
+    InvalidConditionException,
+    NoneParameterException,
+)
 
 
 class PolynomialMutationTestMethods(unittest.TestCase):
-
     def test_should_constructor_raises_an_exception_is_probability_is_negative(self) -> None:
         with self.assertRaises(Exception):
             PolynomialMutation(-1)
 
     def test_should_constructor_raises_an_exception_is_probability_is_higher_than_one(self) -> None:
         with self.assertRaises(Exception):
             PolynomialMutation(1.01)
@@ -50,30 +64,35 @@
 
         mutated_solution = operator.execute(solution)
 
         self.assertNotEqual([1.0, 2.0, 3.0], mutated_solution.variables)
 
     def test_should_execute_work_with_a_solution_subclass_of_float_solution(self):
         class NewFloatSolution(FloatSolution):
-            def __init__(self, lower_bound: List[float], upper_bound: List[float], number_of_objectives: int,
-                         number_of_constraints: int = 0):
-                super(NewFloatSolution, self).__init__(lower_bound, upper_bound, number_of_objectives,
-                                                       number_of_constraints)
+            def __init__(
+                self,
+                lower_bound: List[float],
+                upper_bound: List[float],
+                number_of_objectives: int,
+                number_of_constraints: int = 0,
+            ):
+                super(NewFloatSolution, self).__init__(
+                    lower_bound, upper_bound, number_of_objectives, number_of_constraints
+                )
 
         operator = PolynomialMutation(1.0)
         solution = NewFloatSolution([-5, -5, -5], [5, 5, 5], 2)
         solution.variables = [1.0, 2.0, 3.0]
 
         mutated_solution = operator.execute(solution)
 
         self.assertNotEqual([1.0, 2.0, 3.0], mutated_solution.variables)
 
 
 class BitFlipTestCases(unittest.TestCase):
-
     def test_should_constructor_raises_an_exception_is_probability_is_negative(self) -> None:
         with self.assertRaises(Exception):
             BitFlipMutation(-1)
 
     def test_should_constructor_raises_an_exception_is_probability_is_higher_than_one(self) -> None:
         with self.assertRaises(Exception):
             BitFlipMutation(1.01)
@@ -110,15 +129,14 @@
 
         mutated_solution = operator.execute(solution)
         self.assertEqual([False, False, True, True, False, True], mutated_solution.variables[0])
         self.assertEqual([True, False, False, True, True, False], mutated_solution.variables[1])
 
 
 class UniformMutationTestCases(unittest.TestCase):
-
     def test_should_constructor_raises_an_exception_is_probability_is_negative(self) -> None:
         with self.assertRaises(Exception):
             UniformMutation(-1)
 
     def test_should_constructor_raises_an_exception_is_probability_is_higher_than_one(self) -> None:
         with self.assertRaises(Exception):
             UniformMutation(1.01)
@@ -166,15 +184,14 @@
         mutated_solution = operator.execute(solution)
         for i in range(solution.number_of_variables):
             self.assertGreaterEqual(mutated_solution.variables[i], solution.lower_bound[i])
             self.assertLessEqual(mutated_solution.variables[i], solution.upper_bound[i])
 
 
 class RandomMutationTestCases(unittest.TestCase):
-
     def test_should_constructor_raises_an_exception_is_probability_is_negative(self) -> None:
         with self.assertRaises(Exception):
             SimpleRandomMutation(-1)
 
     def test_should_constructor_raises_an_exception_is_probability_is_higher_than_one(self) -> None:
         with self.assertRaises(Exception):
             SimpleRandomMutation(1.01)
@@ -219,15 +236,14 @@
         mutated_solution = operator.execute(solution)
         for i in range(solution.number_of_variables):
             self.assertGreaterEqual(mutated_solution.variables[i], solution.lower_bound[i])
             self.assertLessEqual(mutated_solution.variables[i], solution.upper_bound[i])
 
 
 class IntegerPolynomialMutationTestCases(unittest.TestCase):
-
     def test_should_constructor_raises_an_exception_is_probability_is_negative(self) -> None:
         with self.assertRaises(Exception):
             IntegerPolynomialMutation(-1)
 
     def test_should_constructor_raises_an_exception_is_probability_is_higher_than_one(self) -> None:
         with self.assertRaises(Exception):
             IntegerPolynomialMutation(1.01)
@@ -274,15 +290,15 @@
             CompositeMutation(None)
 
     def test_should_constructor_raise_an_exception_if_the_parameter_list_is_Empty(self):
         with self.assertRaises(EmptyCollectionException):
             CompositeMutation([])
 
     def test_should_constructor_create_a_valid_operator_when_adding_a_single_mutation_operator(self):
-        mutation: Mutation =  PolynomialMutation(0.9, 20.0)
+        mutation: Mutation = PolynomialMutation(0.9, 20.0)
 
         operator = CompositeMutation([mutation])
         self.assertIsNotNone(operator)
         self.assertEqual(1, len(operator.mutation_operators_list))
 
     def test_should_constructor_create_a_valid_operator_when_adding_two_mutation_operators(self):
         polynomial_mutation = PolynomialMutation(1.0, 20.0)
@@ -304,9 +320,9 @@
 
         composite_solution = CompositeSolution([float_solution, binary_solution])
 
         with self.assertRaises(InvalidConditionException):
             operator.execute(composite_solution)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `jmetalpy-1.5.5/jmetal/operator/test/test_selection.py` & `jmetalpy-1.6.0/jmetal/operator/test/test_selection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 import unittest
 
-from hamcrest import assert_that, any_of
+from hamcrest import any_of, assert_that
 
 from jmetal.core.solution import Solution
-from jmetal.operator.selection import BinaryTournamentSelection, BestSolutionSelection, RandomSolutionSelection, \
-    NaryRandomSolutionSelection, RankingAndCrowdingDistanceSelection, BinaryTournament2Selection, \
-    DifferentialEvolutionSelection
-from jmetal.util.comparator import SolutionAttributeComparator, EqualSolutionsComparator
+from jmetal.operator.selection import (
+    BestSolutionSelection,
+    BinaryTournament2Selection,
+    BinaryTournamentSelection,
+    DifferentialEvolutionSelection,
+    NaryRandomSolutionSelection,
+    RandomSolutionSelection,
+    RankingAndCrowdingDistanceSelection,
+)
+from jmetal.util.comparator import EqualSolutionsComparator, SolutionAttributeComparator
 
 
 class BinaryTournamentTestCases(unittest.TestCase):
-
     def setUp(self):
         self.selection = BinaryTournamentSelection[Solution]()
 
     def test_should_constructor_create_a_non_null_object(self):
         self.assertIsNotNone(self.selection)
 
     def test_should_execute_raise_an_exception_if_the_list_of_solutions_is_none(self):
@@ -51,15 +56,14 @@
 
         solution_list = [solution1, solution2]
 
         assert_that(solution2, self.selection.execute(solution_list))
 
 
 class BestSolutionSelectionTestCases(unittest.TestCase):
-
     def setUp(self):
         self.selection = BestSolutionSelection[Solution]()
 
     def test_should_constructor_create_a_non_null_object(self):
         self.assertIsNotNone(self.selection)
 
     def test_should_execute_raise_an_exception_if_the_list_of_solutions_is_none(self):
@@ -113,15 +117,14 @@
 
         solution_list = [solution1, solution2, solution3, solution4, solution5]
 
         self.assertEqual(solution2, self.selection.execute(solution_list))
 
 
 class RandomSolutionSelectionTestCases(unittest.TestCase):
-
     def setUp(self):
         self.selection = RandomSolutionSelection[Solution]()
 
     def test_should_constructor_create_a_non_null_object(self):
         self.assertIsNotNone(self.selection)
 
     def test_should_execute_raise_an_exception_if_the_list_of_solutions_is_none(self):
@@ -191,21 +194,21 @@
         selection = DifferentialEvolutionSelection[Solution]()
         solution_list = []
         with self.assertRaises(Exception):
             selection.execute(solution_list)
 
     def test_should_execute_raise_an_exception_if_the_list_of_solutions_is_smaller_than_required(self):
         selection = DifferentialEvolutionSelection[Solution]()
-        solution_list = [Solution(1, 1), Solution(1, 1), Solution(1,1)]
+        solution_list = [Solution(1, 1), Solution(1, 1), Solution(1, 1)]
         with self.assertRaises(Exception):
             selection.execute(solution_list)
 
     def test_should_execute_return_three_solutions_if_the_list_of_solutions_larger_than_three(self):
         selection = DifferentialEvolutionSelection[Solution]()
-        solution_list = [Solution(1, 1), Solution(1, 1), Solution(1,1), Solution(1,1)]
+        solution_list = [Solution(1, 1), Solution(1, 1), Solution(1, 1), Solution(1, 1)]
 
         self.assertEqual(3, len(selection.execute(solution_list)))
 
     def test_should_execute_exclude_the_indicated_solution_if_the_list_of_solutions_has_size_four(self):
         selection = DifferentialEvolutionSelection[Solution]()
         solution1 = Solution(2, 2)
         solution1.variables = [1, 2]
@@ -227,15 +230,14 @@
         selected_solutions = selection.execute(solution_list)
 
         self.assertEqual(3, len(selected_solutions))
         self.assertTrue(solution4 not in selected_solutions)
 
 
 class NaryRandomSolutionSelectionTestCases(unittest.TestCase):
-
     def test_should_constructor_create_a_non_null_object(self):
         selection = NaryRandomSolutionSelection[Solution]()
         self.assertIsNotNone(selection)
 
     def test_should_constructor_create_a_non_null_object_and_check_number_of_elements(self):
         selection = NaryRandomSolutionSelection[Solution](3)
         self.assertEqual(selection.number_of_solutions_to_be_returned, 3)
@@ -293,15 +295,14 @@
 
         solution_list = [solution1, solution2, solution3, solution4, solution5]
 
         self.assertTrue(selection.execute(solution_list)[0] in solution_list)
 
 
 class DominanceRankingTestCases(unittest.TestCase):
-
     def setUp(self):
         self.ranking_and_crowding_selection = RankingAndCrowdingDistanceSelection(5)
 
     def test_should_len_of_nsgaii_execute_be_5(self):
         solution1 = Solution(2, 2)
         solution2 = Solution(2, 2)
         solution3 = Solution(2, 2)
@@ -331,15 +332,14 @@
         self.assertEqual(solution3, list_of_crowding_and_rankings[1])
         self.assertEqual(solution5, list_of_crowding_and_rankings[2])
         self.assertEqual(solution4, list_of_crowding_and_rankings[3])
         self.assertEqual(solution2, list_of_crowding_and_rankings[4])
 
 
 class BinaryTournament2TestCases(unittest.TestCase):
-
     def test_should_constructor_create_a_non_null_object(self):
         selection = BinaryTournament2Selection[Solution]([])
 
         self.assertIsNotNone(selection)
 
     def test_should_execute_raise_an_exception_if_the_list_of_solutions_is_none(self):
         solution_list = None
@@ -381,9 +381,9 @@
         solution_list = [solution1, solution2]
         operator = BinaryTournament2Selection[Solution]([SolutionAttributeComparator("key")])
         selection1 = operator.execute(solution_list)
 
         self.assertTrue(1, selection1.attributes["dominance_ranking"])
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `jmetalpy-1.5.5/jmetal/problem/multiobjective/constrained.py` & `jmetalpy-1.6.0/jmetal/problem/multiobjective/constrained.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,39 @@
-from math import pi, cos, atan
+from math import atan, cos, pi
 
 from jmetal.core.problem import FloatProblem
 from jmetal.core.solution import FloatSolution
 
 """
 .. module:: constrained
    :platform: Unix, Windows
    :synopsis: Constrained test problems for multi-objective optimization
 
 .. moduleauthor:: Antonio J. Nebro <antonio@lcc.uma.es>
 """
 
 
 class Srinivas(FloatProblem):
-    """ Class representing problem Srinivas. """
+    """Class representing problem Srinivas."""
 
     def __init__(self):
         super(Srinivas, self).__init__()
-        self.number_of_variables = 2
-        self.number_of_objectives = 2
-        self.number_of_constraints = 2
+        number_of_variables = 2
 
         self.obj_directions = [self.MINIMIZE, self.MINIMIZE]
-        self.obj_labels = ['f(x)', 'f(y)']
+        self.obj_labels = ["f(x)", "f(y)"]
 
-        self.lower_bound = [-20.0 for _ in range(self.number_of_variables)]
-        self.upper_bound = [20.0 for _ in range(self.number_of_variables)]
+        self.lower_bound = [-20.0 for _ in range(number_of_variables)]
+        self.upper_bound = [20.0 for _ in range(number_of_variables)]
+
+    def number_of_objectives(self) -> int:
+        return len(self.obj_directions)
+
+    def number_of_constraints(self) -> int:
+        return 2
 
     def evaluate(self, solution: FloatSolution) -> FloatSolution:
         x1 = solution.variables[0]
         x2 = solution.variables[1]
 
         solution.objectives[0] = 2.0 + (x1 - 2.0) * (x1 - 2.0) + (x2 - 1.0) * (x2 - 1.0)
         solution.objectives[1] = 9.0 * x1 - (x2 - 1.0) * (x2 - 1.0)
@@ -41,139 +45,138 @@
     def __evaluate_constraints(self, solution: FloatSolution) -> None:
         x1 = solution.variables[0]
         x2 = solution.variables[1]
 
         solution.constraints[0] = 1.0 - (x1 * x1 + x2 * x2) / 225.0
         solution.constraints[1] = (3.0 * x2 - x1) / 10.0 - 1.0
 
-    def get_name(self):
-        return 'Srinivas'
+    def name(self):
+        return "Srinivas"
 
 
 class Tanaka(FloatProblem):
-    """ Class representing problem Tanaka. """
+    """Class representing problem Tanaka."""
 
     def __init__(self):
         super(Tanaka, self).__init__()
-        self.number_of_variables = 2
-        self.number_of_objectives = 2
-        self.number_of_constraints = 2
 
         self.obj_directions = [self.MINIMIZE, self.MINIMIZE]
-        self.obj_labels = ['f(x)', 'f(y)']
+        self.obj_labels = ["f(x)", "f(y)"]
+
+        number_of_variables = 2
+        self.lower_bound = [10e-5 for _ in range(number_of_variables)]
+        self.upper_bound = [pi for _ in range(number_of_variables)]
 
-        self.lower_bound = [10e-5 for _ in range(self.number_of_variables)]
-        self.upper_bound = [pi for _ in range(self.number_of_variables)]
+    def number_of_objectives(self) -> int:
+        return len(self.obj_directions)
 
+    def number_of_constraints(self) -> int:
+        return 2
 
     def evaluate(self, solution: FloatSolution) -> FloatSolution:
         solution.objectives[0] = solution.variables[0]
         solution.objectives[1] = solution.variables[1]
 
         self.__evaluate_constraints(solution)
 
         return solution
 
     def __evaluate_constraints(self, solution: FloatSolution) -> None:
-        constraints = [0.0 for _ in range(self.number_of_constraints)]
+        constraints = [0.0 for _ in range(self.number_of_constraints())]
 
         x1 = solution.variables[0]
         x2 = solution.variables[1]
 
-        constraints[0] = (x1 * x1 + x2 * x2 - 1.0 - 0.1 * cos(16.0 * atan(x1 / x2)))
+        constraints[0] = x1 * x1 + x2 * x2 - 1.0 - 0.1 * cos(16.0 * atan(x1 / x2))
         constraints[1] = -2.0 * ((x1 - 0.5) * (x1 - 0.5) + (x2 - 0.5) * (x2 - 0.5) - 0.5)
 
         solution.constraints = constraints
 
-        #set_overall_constraint_violation_degree(solution)
+        # set_overall_constraint_violation_degree(solution)
 
-
-    def get_name(self):
-        return 'Tanaka'
+    def name(self):
+        return "Tanaka"
 
 
 class Osyczka2(FloatProblem):
-    """ Class representing problem Osyczka2. """
+    """Class representing problem Osyczka2."""
 
     def __init__(self):
         super(Osyczka2, self).__init__()
-        self.number_of_variables = 6
-        self.number_of_objectives = 2
-        self.number_of_constraints = 6
 
         self.obj_directions = [self.MINIMIZE, self.MINIMIZE]
-        self.obj_labels = ['f(x)', 'f(y)']
+        self.obj_labels = ["f(x)", "f(y)"]
 
         self.lower_bound = [0.0, 0.0, 1.0, 0.0, 1.0, 0.0]
         self.upper_bound = [10.0, 10.0, 5.0, 6.0, 5.0, 10.0]
 
-        FloatSolution.lower_bound = self.lower_bound
-        FloatSolution.upper_bound = self.upper_bound
+    def number_of_objectives(self) -> int:
+        return len(self.obj_directions)
+
+    def number_of_constraints(self) -> int:
+        return 6
 
     def evaluate(self, solution: FloatSolution) -> FloatSolution:
         x = solution.variables
-        solution.objectives[0] = - (25.0 *
-                                    (x[0] - 2.0) ** 2 +
-                                    (x[1] - 2.0) ** 2 +
-                                    (x[2] - 1.0) ** 2 +
-                                    (x[3] - 4.0) ** 2 +
-                                    (x[4] - 1.0) ** 2)
+        solution.objectives[0] = -(
+            25.0 * (x[0] - 2.0) ** 2 + (x[1] - 2.0) ** 2 + (x[2] - 1.0) ** 2 + (x[3] - 4.0) ** 2 + (x[4] - 1.0) ** 2
+        )
 
         solution.objectives[1] = sum([x[i] ** 2 for i in range(len(x))])
 
         self.__evaluate_constraints(solution)
 
         return solution
 
     def __evaluate_constraints(self, solution: FloatSolution) -> None:
-        constraints = [0.0 for _ in range(self.number_of_constraints)]
+        constraints = [0.0 for _ in range(self.number_of_constraints())]
 
         x = solution.variables
         constraints[0] = (x[0] + x[1]) / 2.0 - 1.0
         constraints[1] = (6.0 - x[0] - x[1]) / 6.0
         constraints[2] = (2.0 - x[1] + x[0]) / 2.0
         constraints[3] = (2.0 - x[0] + 3.0 * x[1]) / 2.0
         constraints[4] = (4.0 - (x[2] - 3.0) * (x[2] - 3.0) - x[3]) / 4.0
         constraints[5] = ((x[4] - 3.0) * (x[4] - 3.0) + x[5] - 4.0) / 4.0
 
         solution.constraints = constraints
 
-    def get_name(self):
-        return 'Osyczka2'
+    def name(self):
+        return "Osyczka2"
 
 
 class Binh2(FloatProblem):
-    """ Class representing problem Binh2. """
+    """Class representing problem Binh2."""
 
     def __init__(self):
         super(Binh2, self).__init__()
-        self.number_of_variables = 2
-        self.number_of_objectives = 2
-        self.number_of_constraints = 2
 
         self.obj_directions = [self.MINIMIZE, self.MINIMIZE]
-        self.obj_labels = ['f(x)', 'f(y)']
+        self.obj_labels = ["f(x)", "f(y)"]
 
         self.lower_bound = [0.0, 0.0]
         self.upper_bound = [5.0, 3.0]
 
-        FloatSolution.lower_bound = self.lower_bound
-        FloatSolution.upper_bound = self.upper_bound
+    def number_of_objectives(self) -> int:
+        return len(self.obj_directions)
+
+    def number_of_constraints(self) -> int:
+        return 2
 
     def evaluate(self, solution: FloatSolution) -> FloatSolution:
         x = solution.variables
         solution.objectives[0] = 4.0 * x[0] * x[0] + 4 * x[1] * x[1]
         solution.objectives[1] = (x[0] - 5.0) * (x[0] - 5.0) + (x[1] - 5.0) * (x[1] - 5.0)
 
         self.__evaluate_constraints(solution)
 
         return solution
 
     def __evaluate_constraints(self, solution: FloatSolution) -> None:
-        constraints = [0.0 for _ in range(self.number_of_constraints)]
+        constraints = [0.0 for _ in range(self.number_of_constraints())]
 
         x = solution.variables
         constraints[0] = -1.0 * (x[0] - 5) * (x[0] - 5) - x[1] * x[1] + 25.0
         constraints[1] = (x[0] - 8) * (x[0] - 8) + (x[1] + 3) * (x[1] + 3) - 7.7
 
-    def get_name(self):
-        return 'Binh2'
+    def name(self):
+        return "Binh2"
```

### Comparing `jmetalpy-1.5.5/jmetal/problem/multiobjective/dtlz.py` & `jmetalpy-1.6.0/jmetal/problem/multiobjective/dtlz.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,110 +1,116 @@
-from math import pi, cos, sin
+from math import cos, pi, sin
 
 from jmetal.core.problem import FloatProblem
 from jmetal.core.solution import FloatSolution
 
 """
 .. module:: DTLZ
    :platform: Unix, Windows
    :synopsis: DTLZ problem family of multi-objective problems.
 
 .. moduleauthor:: Antonio J. Nebro <antonio@lcc.uma.es>
 """
 
 
 class DTLZ1(FloatProblem):
-    """ Problem DTLZ1. Continuous problem having a flat Pareto front
+    """Problem DTLZ1. Continuous problem having a flat Pareto front
 
     .. note:: Unconstrained problem. The default number of variables and objectives are, respectively, 7 and 3.
     """
 
     def __init__(self, number_of_variables: int = 7, number_of_objectives=3):
-        """ :param number_of_variables: number of decision variables of the problem.
-        """
+        """:param number_of_variables: number of decision variables of the problem."""
         super(DTLZ1, self).__init__()
-        self.number_of_variables = number_of_variables
-        self.number_of_objectives = number_of_objectives
-        self.number_of_constraints = 0
 
         self.obj_directions = [self.MINIMIZE] * number_of_objectives
-        self.obj_labels = ['$ f_{} $'.format(i) for i in range(number_of_objectives)]
+        self.obj_labels = ["$ f_{} $".format(i) for i in range(number_of_objectives)]
 
-        self.lower_bound = self.number_of_variables * [0.0]
-        self.upper_bound = self.number_of_variables * [1.0]
+        self.lower_bound = number_of_variables * [0.0]
+        self.upper_bound = number_of_variables * [1.0]
+
+    def number_of_objectives(self) -> int:
+        return len(self.obj_directions)
+
+    def number_of_constraints(self) -> int:
+        return 0
 
     def evaluate(self, solution: FloatSolution) -> FloatSolution:
-        k = self.number_of_variables - self.number_of_objectives + 1
+        k = self.number_of_variables() - self.number_of_objectives() + 1
 
-        g = sum([(x - 0.5) * (x - 0.5) - cos(20.0 * pi * (x - 0.5))
-                 for x in solution.variables[self.number_of_variables - k:]])
+        g = sum(
+            [
+                (x - 0.5) * (x - 0.5) - cos(20.0 * pi * (x - 0.5))
+                for x in solution.variables[self.number_of_variables() - k :]
+            ]
+        )
 
         g = 100 * (k + g)
 
-        solution.objectives = [(1.0 + g) * 0.5] * self.number_of_objectives
+        solution.objectives = [(1.0 + g) * 0.5] * self.number_of_objectives()
 
-        for i in range(self.number_of_objectives):
-            for j in range(self.number_of_objectives - (i + 1)):
+        for i in range(self.number_of_objectives()):
+            for j in range(self.number_of_objectives() - (i + 1)):
                 solution.objectives[i] *= solution.variables[j]
 
             if i != 0:
-                solution.objectives[i] *= 1 - solution.variables[self.number_of_objectives - (i + 1)]
+                solution.objectives[i] *= 1 - solution.variables[self.number_of_objectives() - (i + 1)]
 
         return solution
 
-    def get_name(self):
-        return 'DTLZ1'
+    def name(self):
+        return "DTLZ1"
 
 
 class DTLZ2(DTLZ1):
-    """ Problem DTLZ2. Continuous problem having a convex Pareto front
+    """Problem DTLZ2. Continuous problem having a convex Pareto front
 
     .. note:: Unconstrained problem. The default number of variables and objectives are, respectively, 12 and 3.
     """
 
     def __init__(self, number_of_variables: int = 12, number_of_objectives=3):
-        """:param number_of_variables: number of decision variables of the problem
-        """
+        """:param number_of_variables: number of decision variables of the problem"""
         super(DTLZ2, self).__init__(number_of_variables, number_of_objectives)
 
     def evaluate(self, solution: FloatSolution) -> FloatSolution:
-        k = self.number_of_variables - self.number_of_objectives + 1
+        k = self.number_of_variables() - self.number_of_objectives() + 1
 
-        g = sum([(x - 0.5) * (x - 0.5) for x in solution.variables[self.number_of_variables - k:]])
+        g = sum([(x - 0.5) * (x - 0.5) for x in solution.variables[self.number_of_variables() - k :]])
 
-        solution.objectives = [1.0 + g] * self.number_of_objectives
+        solution.objectives = [1.0 + g] * self.number_of_objectives()
 
-        for i in range(self.number_of_objectives):
-            for j in range(self.number_of_objectives - (i + 1)):
+        for i in range(self.number_of_objectives()):
+            for j in range(self.number_of_objectives() - (i + 1)):
                 solution.objectives[i] *= cos(solution.variables[j] * 0.5 * pi)
 
             if i != 0:
-                solution.objectives[i] *= sin(0.5 * pi * solution.variables[self.number_of_objectives - (i + 1)])
+                solution.objectives[i] *= sin(0.5 * pi * solution.variables[self.number_of_objectives() - (i + 1)])
 
         return solution
 
-    def get_name(self):
-        return 'DTLZ2'
+    def name(self):
+        return "DTLZ2"
 
 
 class DTLZ3(DTLZ1):
-    """ Problem DTLZ3. Continuous problem having a convex Pareto front
+    """Problem DTLZ3. Continuous problem having a convex Pareto front
 
     .. note:: Unconstrained problem. The default number of variables and objectives are, respectively, 12 and 3.
     """
 
     def __init__(self, number_of_variables: int = 12, number_of_objectives=3):
-        """:param number_of_variables: number of decision variables of the problem
-        """
+        """:param number_of_variables: number of decision variables of the problem"""
         super(DTLZ3, self).__init__(number_of_variables, number_of_objectives)
 
     def evaluate(self, solution: FloatSolution) -> FloatSolution:
         k = self.number_of_variables - self.number_of_objectives + 1
 
-        g = sum([(x - 0.5) ** 2 - cos(20.0 * pi * (x - 0.5)) for x in solution.variables[self.number_of_variables - k:]])
+        g = sum(
+            [(x - 0.5) ** 2 - cos(20.0 * pi * (x - 0.5)) for x in solution.variables[self.number_of_variables - k :]]
+        )
         g = 100.0 * (k + g)
 
         f = [1.0 + g for _ in range(self.number_of_objectives)]
 
         for i in range(self.number_of_objectives):
             for j in range(self.number_of_objectives - (i + 1)):
                 f[i] *= cos(solution.variables[j] * 0.5 * pi)
@@ -113,72 +119,70 @@
                 aux = self.number_of_objectives - (i + 1)
                 f[i] *= sin(solution.variables[aux] * 0.5 * pi)
 
         solution.objectives = [f[x] for x in range(self.number_of_objectives)]
 
         return solution
 
-    def get_name(self):
-        return 'DTLZ3'
+    def name(self):
+        return "DTLZ3"
 
 
 class DTLZ4(DTLZ1):
-    """ Problem DTLZ4. Continuous problem having a convex Pareto front
+    """Problem DTLZ4. Continuous problem having a convex Pareto front
 
     .. note:: Unconstrained problem. The default number of variables and objectives are, respectively, 12 and 3.
     """
 
     def __init__(self, number_of_variables: int = 12, number_of_objectives=3):
-        """:param number_of_variables: number of decision variables of the problem
-        """
+        """:param number_of_variables: number of decision variables of the problem"""
         super(DTLZ4, self).__init__(number_of_variables, number_of_objectives)
 
     def evaluate(self, solution: FloatSolution) -> FloatSolution:
         alpha = 100.0
         k = self.number_of_variables - self.number_of_objectives + 1
 
-        g = sum([(x - 0.5) ** 2 for x in solution.variables[self.number_of_variables - k:]])
+        g = sum([(x - 0.5) ** 2 for x in solution.variables[self.number_of_variables - k :]])
         f = [1.0 + g for _ in range(self.number_of_objectives)]
 
         for i in range(self.number_of_objectives):
             for j in range(self.number_of_objectives - (i + 1)):
                 f[i] *= cos(pow(solution.variables[j], alpha) * pi / 2.0)
 
             if i != 0:
                 aux = self.number_of_objectives - (i + 1)
                 f[i] *= sin(pow(solution.variables[aux], alpha) * pi / 2.0)
 
         solution.objectives = [f[x] for x in range(self.number_of_objectives)]
 
         return solution
 
-    def get_name(self):
-        return 'DTLZ4'
+    def name(self):
+        return "DTLZ4"
 
 
 class DTLZ5(DTLZ1):
-    """ Problem DTLZ5. Continuous problem having a convex Pareto front
+    """Problem DTLZ5. Continuous problem having a convex Pareto front
 
     .. note:: Unconstrained problem. The default number of variables and objectives are, respectively, 12 and 3.
     """
 
     def __init__(self, number_of_variables: int = 12, number_of_objectives=3):
-        """:param number_of_variables: number of decision variables of the problem
-        """
+        """:param number_of_variables: number of decision variables of the problem"""
         super(DTLZ5, self).__init__(number_of_variables, number_of_objectives)
 
     def evaluate(self, solution: FloatSolution) -> FloatSolution:
         k = self.number_of_variables - self.number_of_objectives + 1
 
-        g = sum([(x - 0.5) ** 2 for x in solution.variables[self.number_of_variables - k:]])
-        t = pi/(4.0 * (1.0 + g))
+        g = sum([(x - 0.5) ** 2 for x in solution.variables[self.number_of_variables - k :]])
+        t = pi / (4.0 * (1.0 + g))
 
-        theta = [0.0]*(self.number_of_objectives - 1)
-        theta[0] = solution.variables[0]*pi/2.0
-        theta[1:] = [t * (1.0 + 2.0 * g * solution.variables[i]) for i in range(1,self.number_of_objectives-1)]
+        theta = [0.0] * (self.number_of_objectives - 1)
+        theta[0] = solution.variables[0] * pi / 2.0
+        theta[1:] = [t * (1.0 + 2.0 * g * solution.variables[i]) for i in range(1, self.number_of_objectives - 1)]
 
         f = [1.0 + g for _ in range(self.number_of_objectives)]
 
         for i in range(self.number_of_objectives):
             for j in range(self.number_of_objectives - (i + 1)):
                 f[i] *= cos(theta[j])
 
@@ -186,38 +190,37 @@
                 aux = self.number_of_objectives - (i + 1)
                 f[i] *= sin(theta[aux])
 
         solution.objectives = [f[x] for x in range(self.number_of_objectives)]
 
         return solution
 
-    def get_name(self):
-        return 'DTLZ5'
+    def name(self):
+        return "DTLZ5"
 
 
 class DTLZ6(DTLZ1):
-    """ Problem DTLZ6. Continuous problem having a convex Pareto front
+    """Problem DTLZ6. Continuous problem having a convex Pareto front
 
     .. note:: Unconstrained problem. The default number of variables and objectives are, respectively, 12 and 3.
     """
 
     def __init__(self, number_of_variables: int = 12, number_of_objectives=3):
-        """:param number_of_variables: number of decision variables of the problem
-        """
+        """:param number_of_variables: number of decision variables of the problem"""
         super(DTLZ6, self).__init__(number_of_variables, number_of_objectives)
 
     def evaluate(self, solution: FloatSolution) -> FloatSolution:
         k = self.number_of_variables - self.number_of_objectives + 1
 
-        g = sum([pow(x, 0.1) for x in solution.variables[self.number_of_variables - k:]])
-        t = pi/(4.0 * (1.0 + g))
+        g = sum([pow(x, 0.1) for x in solution.variables[self.number_of_variables - k :]])
+        t = pi / (4.0 * (1.0 + g))
 
-        theta = [0.0]*(self.number_of_objectives - 1)
-        theta[0] = solution.variables[0]*pi/2.0
-        theta[1:] = [t * (1.0 + 2.0 * g * solution.variables[i]) for i in range(1,self.number_of_objectives-1)]
+        theta = [0.0] * (self.number_of_objectives - 1)
+        theta[0] = solution.variables[0] * pi / 2.0
+        theta[1:] = [t * (1.0 + 2.0 * g * solution.variables[i]) for i in range(1, self.number_of_objectives - 1)]
 
         f = [1.0 + g for _ in range(self.number_of_objectives)]
 
         for i in range(self.number_of_objectives):
             for j in range(self.number_of_objectives - (i + 1)):
                 f[i] *= cos(theta[j])
 
@@ -225,38 +228,39 @@
                 aux = self.number_of_objectives - (i + 1)
                 f[i] *= sin(theta[aux])
 
         solution.objectives = [f[x] for x in range(self.number_of_objectives)]
 
         return solution
 
-    def get_name(self):
-        return 'DTLZ6'
+    def name(self):
+        return "DTLZ6"
 
 
 class DTLZ7(DTLZ1):
-    """ Problem DTLZ6. Continuous problem having a disconnected Pareto front
+    """Problem DTLZ6. Continuous problem having a disconnected Pareto front
 
     .. note:: Unconstrained problem. The default number of variables and objectives are, respectively, 22 and 3.
     """
 
     def __init__(self, number_of_variables: int = 22, number_of_objectives=3):
-        """:param number_of_variables: number of decision variables of the problem
-        """
+        """:param number_of_variables: number of decision variables of the problem"""
         super(DTLZ7, self).__init__(number_of_variables, number_of_objectives)
 
     def evaluate(self, solution: FloatSolution) -> FloatSolution:
         k = self.number_of_variables - self.number_of_objectives + 1
 
-        g = sum([x for x in solution.variables[self.number_of_variables - k:]])
+        g = sum([x for x in solution.variables[self.number_of_variables - k :]])
         g = 1.0 + (9.0 * g) / k
 
-        h = sum([(x / (1.0 + g)) * (1 + sin(3.0 * pi * x)) for x in solution.variables[:self.number_of_objectives-1]])
+        h = sum(
+            [(x / (1.0 + g)) * (1 + sin(3.0 * pi * x)) for x in solution.variables[: self.number_of_objectives - 1]]
+        )
         h = self.number_of_objectives - h
 
-        solution.objectives[:self.number_of_objectives-1] = solution.variables[:self.number_of_objectives-1]
+        solution.objectives[: self.number_of_objectives - 1] = solution.variables[: self.number_of_objectives - 1]
         solution.objectives[-1] = (1.0 + g) * h
 
         return solution
 
-    def get_name(self):
-        return 'DTLZ7'
+    def name(self):
+        return "DTLZ7"
```

### Comparing `jmetalpy-1.5.5/jmetal/problem/multiobjective/fda.py` & `jmetalpy-1.6.0/jmetal/problem/multiobjective/fda.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from abc import ABC, abstractmethod
-from math import sqrt, pow, sin, pi, floor, cos
+from math import cos, floor, pi, pow, sin, sqrt
 
 import numpy
 
-from jmetal.core.problem import FloatProblem, DynamicProblem
+from jmetal.core.problem import DynamicProblem, FloatProblem
 from jmetal.core.solution import FloatSolution
 
 """
 .. module:: FDA
    :platform: Unix, Windows
    :synopsis: FDA problem family of dynamic multi-objective problems.
 
@@ -36,29 +36,28 @@
 
     @abstractmethod
     def evaluate(self, solution: FloatSolution):
         pass
 
 
 class FDA1(FDA):
-    """ Problem FDA1.
+    """Problem FDA1.
 
     .. note:: Bi-objective dynamic unconstrained problem. The default number of variables is 100.
     """
 
     def __init__(self, number_of_variables: int = 100):
-        """ :param number_of_variables: Number of decision variables of the problem.
-        """
+        """:param number_of_variables: Number of decision variables of the problem."""
         super(FDA1, self).__init__()
         self.number_of_variables = number_of_variables
         self.number_of_objectives = 2
         self.number_of_constraints = 0
 
         self.obj_directions = [self.MINIMIZE, self.MINIMIZE]
-        self.obj_labels = ['f(x)', 'f(y)']
+        self.obj_labels = ["f(x)", "f(y)"]
 
         self.lower_bound = self.number_of_variables * [-1.0]
         self.upper_bound = self.number_of_variables * [1.0]
         self.lower_bound[0] = 0.0
         self.upper_bound[0] = 1.0
 
     def evaluate(self, solution: FloatSolution) -> FloatSolution:
@@ -76,33 +75,32 @@
 
         return g
 
     def __eval_h(self, f: float, g: float) -> float:
         return 1.0 - sqrt(f / g)
 
     def get_name(self):
-        return 'FDA1'
+        return "FDA1"
 
 
 class FDA2(FDA):
-    """ Problem FDA2
+    """Problem FDA2
 
     .. note:: Bi-objective dynamic unconstrained problem. The default number of variables is 31.
     """
 
     def __init__(self, number_of_variables: int = 31):
-        """ :param number_of_variables: Number of decision variables of the problem.
-        """
+        """:param number_of_variables: Number of decision variables of the problem."""
         super(FDA2, self).__init__()
         self.number_of_variables = number_of_variables
         self.number_of_objectives = 2
         self.number_of_constraints = 0
 
         self.obj_directions = [self.MINIMIZE, self.MINIMIZE]
-        self.obj_labels = ['f(x)', 'f(y)']
+        self.obj_labels = ["f(x)", "f(y)"]
 
         self.lower_bound = self.number_of_variables * [-1.0]
         self.upper_bound = self.number_of_variables * [1.0]
         self.lower_bound[0] = 0.0
         self.upper_bound[0] = 1.0
 
     def evaluate(self, solution: FloatSolution) -> FloatSolution:
@@ -121,36 +119,35 @@
         return g
 
     def __eval_h(self, f: float, g: float) -> float:
         ht = 0.2 + 4.8 * pow(self.time, 2.0)
         return 1.0 - pow(f / g, ht)
 
     def get_name(self):
-        return 'FDA2'
+        return "FDA2"
 
 
 class FDA3(FDA):
-    """ Problem FDA3
+    """Problem FDA3
 
     .. note:: Bi-objective dynamic unconstrained problem. The default number of variables is 30.
     """
 
     def __init__(self, number_of_variables: int = 30):
-        """ :param number_of_variables: Number of decision variables of the problem.
-        """
+        """:param number_of_variables: Number of decision variables of the problem."""
         super(FDA3, self).__init__()
         self.number_of_variables = number_of_variables
         self.number_of_objectives = 2
         self.number_of_constraints = 0
         self.limitInfI = 0
         self.limitSupI = 1
         self.limitInfII = 1
 
         self.obj_directions = [self.MINIMIZE, self.MINIMIZE]
-        self.obj_labels = ['f(x)', 'f(y)']
+        self.obj_labels = ["f(x)", "f(y)"]
 
         self.lower_bound = self.number_of_variables * [-1.0]
         self.upper_bound = self.number_of_variables * [1.0]
         self.lower_bound[0] = 0.0
         self.upper_bound[0] = 1.0
 
     def evaluate(self, solution: FloatSolution) -> FloatSolution:
@@ -178,34 +175,34 @@
         return g
 
     def __eval_h(self, f: float, g: float) -> float:
         h = 1.0 - sqrt(f / g)
         return h
 
     def get_name(self):
-        return 'FDA3'
+        return "FDA3"
 
 
 class FDA4(FDA):
-    """ Problem FDA4
+    """Problem FDA4
 
     .. note:: Three-objective dynamic unconstrained problem. The default number of variables is 12.
     """
+
     M = 3
 
     def __init__(self, number_of_variables: int = 12):
-        """ :param number_of_variables: Number of decision variables of the problem.
-        """
+        """:param number_of_variables: Number of decision variables of the problem."""
         super(FDA4, self).__init__()
         self.number_of_variables = number_of_variables
         self.number_of_objectives = 3
         self.number_of_constraints = 0
 
         self.obj_directions = [self.MINIMIZE, self.MINIMIZE]
-        self.obj_labels = ['f(x)', 'f(y)', 'f(z)']
+        self.obj_labels = ["f(x)", "f(y)", "f(z)"]
 
         self.lower_bound = self.number_of_variables * [0.0]
         self.upper_bound = self.number_of_variables * [1.0]
 
     def evaluate(self, solution: FloatSolution) -> FloatSolution:
         g = self.__eval_g(solution, self.M - 1)
 
@@ -219,52 +216,52 @@
         gt = abs(sin(0.5 * pi * self.time))
         g = sum([pow(v - gt, 2) for v in solution.variables[lower_limit:]])
 
         return g
 
     def __eval_f1(self, solution: FloatSolution, g: float) -> float:
         f = 1.0 + g
-        mult = numpy.prod([cos(v * pi / 2.0) for v in solution.variables[:self.M - 1]])
+        mult = numpy.prod([cos(v * pi / 2.0) for v in solution.variables[: self.M - 1]])
 
         return f * mult
 
     def __eval_fk(self, solution: FloatSolution, g: float, k: int) -> float:
         f = 1.0 + g
         aux = sin((solution.variables[self.M - k] * pi) / 2.0)
-        mult = numpy.prod([cos(v * pi / 2.0) for v in solution.variables[:self.M - k]])
+        mult = numpy.prod([cos(v * pi / 2.0) for v in solution.variables[: self.M - k]])
 
         return f * mult * aux
 
     def __eval_fm(self, solution: FloatSolution, g: float) -> float:
         fm = 1.0 + g
         fm *= sin((solution.variables[0] * pi) / 2.0)
 
         return fm
 
     def get_name(self):
-        return 'FDA4'
+        return "FDA4"
 
 
 class FDA5(FDA):
-    """ Problem FDA5
+    """Problem FDA5
 
     .. note:: Three-objective dynamic unconstrained problem. The default number of variables is 12.
     """
+
     M = 3
 
     def __init__(self, number_of_variables: int = 12):
-        """ :param number_of_variables: Number of decision variables of the problem.
-        """
+        """:param number_of_variables: Number of decision variables of the problem."""
         super(FDA5, self).__init__()
         self.number_of_variables = number_of_variables
         self.number_of_objectives = 3
         self.number_of_constraints = 0
 
         self.obj_directions = [self.MINIMIZE, self.MINIMIZE]
-        self.obj_labels = ['f(x)', 'f(y)', 'f(z)']
+        self.obj_labels = ["f(x)", "f(y)", "f(z)"]
 
         self.lower_bound = self.number_of_variables * [0.0]
         self.upper_bound = self.number_of_variables * [1.0]
 
     def evaluate(self, solution: FloatSolution) -> FloatSolution:
         g = self.__eval_g(solution, self.M - 1)
         ft = 1.0 + 100.0 * pow(sin(0.5 * pi * self.time), 4.0)
@@ -279,29 +276,29 @@
         gt = abs(sin(0.5 * pi * self.time))
         g = sum([pow(v - gt, 2) for v in solution.variables[lower_limit:]])
 
         return g
 
     def __eval_f1(self, solution: FloatSolution, g: float, ft: float) -> float:
         f = 1.0 + g
-        mult = numpy.prod([cos(pow(v, ft) * pi / 2.0) for v in solution.variables[:self.M - 1]])
+        mult = numpy.prod([cos(pow(v, ft) * pi / 2.0) for v in solution.variables[: self.M - 1]])
 
         return f * mult
 
     def __eval_fk(self, solution: FloatSolution, g: float, k: int, ft: float) -> float:
         f = 1.0 + g
 
-        mult = numpy.prod([cos(pow(v, ft) * pi / 2.0) for v in solution.variables[:self.M - k]])
+        mult = numpy.prod([cos(pow(v, ft) * pi / 2.0) for v in solution.variables[: self.M - k]])
         yy = pow(solution.variables[self.M - k], ft)
         mult *= sin(yy * pi / 2.0)
 
         return f * mult
 
     def __eval_fm(self, solution: FloatSolution, g: float, ft: float) -> float:
         fm = 1.0 + g
         y_1 = pow(solution.variables[0], ft)
         mult = sin(y_1 * pi / 2.0)
 
         return fm * mult
 
     def get_name(self):
-        return 'FDA5'
+        return "FDA5"
```

### Comparing `jmetalpy-1.5.5/jmetal/problem/multiobjective/lircmop.py` & `jmetalpy-1.6.0/jmetal/problem/multiobjective/lircmop.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,35 @@
-from math import sin, pi, cos, sqrt
+from math import cos, pi, sin, sqrt
+from typing import List
 
 from jmetal.core.problem import FloatProblem
 from jmetal.core.solution import FloatSolution
 
 
 class LIRCMOP1(FloatProblem):
-    """ Class representing problem LIR-CMOP1, defined in:
+    """Class representing problem LIR-CMOP1, defined in:
 
     * An Improved epsilon-constrained Method in MOEA/D for CMOPs with Large Infeasible Regions.
       Fan, Z., Li, W., Cai, X. et al. Soft Comput (2019). https://doi.org/10.1007/s00500-019-03794-x
     """
 
     def __init__(self, number_of_variables: int = 30):
         super(LIRCMOP1, self).__init__()
-        self.number_of_variables = number_of_variables
-        self.number_of_objectives = 2
-        self.number_of_constraints = 2
 
         self.obj_directions = [self.MINIMIZE, self.MINIMIZE]
-        self.obj_labels = ['f(x)', 'f(y)']
+        self.obj_labels = ["f(x)", "f(y)"]
 
-        self.lower_bound = [0.0 for _ in range(self.number_of_variables)]
-        self.upper_bound = [1.0 for _ in range(self.number_of_variables)]
+        self.lower_bound = [0.0 for _ in range(number_of_variables)]
+        self.upper_bound = [1.0 for _ in range(number_of_variables)]
+
+    def number_of_objectives(self) -> int:
+        return len(self.obj_directions)
+
+    def number_of_constraints(self) -> int:
+        return 2
 
     def evaluate(self, solution: FloatSolution) -> FloatSolution:
         x = solution.variables
 
         solution.objectives[0] = x[0] + self.g1(x)
         solution.objectives[1] = 1 - x[0] * x[0] + self.g2(x)
 
@@ -43,34 +47,34 @@
         constraints[0] = (a - self.g1(x)) * (self.g1(x) - b)
         constraints[1] = (a - self.g2(x)) * (self.g2(x) - b)
 
         solution.constraints = constraints
 
         return solution
 
-    def g1(self, x: [float]) -> float:
+    def g1(self, x: List[float]) -> float:
         result = 0
         for i in range(2, self.number_of_variables, 2):
             result += pow(x[i] - sin(0.5 * pi * x[0]), 2.0)
 
         return result
 
-    def g2(self, x: [float]) -> float:
+    def g2(self, x: List[float]) -> float:
         result = 0
         for i in range(1, self.number_of_variables, 2):
             result += pow(x[i] - cos(0.5 * pi * x[0]), 2.0)
 
         return result
 
-    def get_name(self):
-        return 'LIR-CMOP1'
+    def name(self):
+        return "LIR-CMOP1"
 
 
 class LIRCMOP2(LIRCMOP1):
-    """ Class representing problem LIR-CMOP1, defined in:
+    """Class representing problem LIR-CMOP1, defined in:
 
     * An Improved epsilon-constrained Method in MOEA/D for CMOPs with Large Infeasible Regions.
       Fan, Z., Li, W., Cai, X. et al. Soft Comput (2019). https://doi.org/10.1007/s00500-019-03794-x
     """
 
     def __init__(self, number_of_variables: int = 30):
         super(LIRCMOP2, self).__init__(number_of_variables)
@@ -81,28 +85,31 @@
         solution.objectives[0] = x[0] + self.g1(x)
         solution.objectives[1] = 1 - sqrt(x[0]) + self.g2(x)
 
         self.evaluate_constraints(solution)
 
         return solution
 
-    def get_name(self):
-        return 'LIR-CMOP2'
+    def name(self):
+        return "LIR-CMOP2"
 
 
 class LIRCMOP3(LIRCMOP1):
-    """ Class representing problem LIR-CMOP3, defined in:
+    """Class representing problem LIR-CMOP3, defined in:
 
     * An Improved epsilon-constrained Method in MOEA/D for CMOPs with Large Infeasible Regions.
       Fan, Z., Li, W., Cai, X. et al. Soft Comput (2019). https://doi.org/10.1007/s00500-019-03794-x
     """
 
     def __init__(self, number_of_variables: int = 30):
         super(LIRCMOP3, self).__init__(number_of_variables)
 
+    def number_of_constraints(self) -> int:
+        return 3
+
     def evaluate_constraints(self, solution: FloatSolution) -> FloatSolution:
         x = solution.variables
         constraints = [0.0 for _ in range(self.number_of_constraints)]
 
         a = 0.51
         b = 0.5
         c = 20.0
@@ -111,28 +118,31 @@
         constraints[1] = (a - self.g2(x)) * (self.g2(x) - b)
         constraints[2] = sin(c * pi * x[0]) - 0.5
 
         solution.constraints = constraints
 
         return solution
 
-    def get_name(self):
-        return 'LIR-CMOP3'
+    def name(self):
+        return "LIR-CMOP3"
 
 
 class LIRCMOP4(LIRCMOP2):
-    """ Class representing problem LIR-CMOP4, defined in:
+    """Class representing problem LIR-CMOP4, defined in:
 
     * An Improved epsilon-constrained Method in MOEA/D for CMOPs with Large Infeasible Regions.
       Fan, Z., Li, W., Cai, X. et al. Soft Comput (2019). https://doi.org/10.1007/s00500-019-03794-x
     """
 
     def __init__(self, number_of_variables: int = 30):
         super(LIRCMOP4, self).__init__(number_of_variables)
 
+    def number_of_constraints(self) -> int:
+        return 3
+
     def evaluate_constraints(self, solution: FloatSolution) -> FloatSolution:
         x = solution.variables
         constraints = [0.0 for _ in range(self.number_of_constraints)]
 
         a = 0.51
         b = 0.5
         c = 20.0
@@ -141,36 +151,39 @@
         constraints[1] = (a - self.g2(x)) * (self.g2(x) - b)
         constraints[2] = sin(c * pi * x[0]) - 0.5
 
         solution.constraints = constraints
 
         return solution
 
-    def get_name(self):
-        return 'LIR-CMOP4'
+    def name(self):
+        return "LIR-CMOP4"
 
 
 class LIRCMOP5(FloatProblem):
-    """ Class representing problem LIR-CMOP5, defined in:
+    """Class representing problem LIR-CMOP5, defined in:
 
     * An Improved epsilon-constrained Method in MOEA/D for CMOPs with Large Infeasible Regions.
       Fan, Z., Li, W., Cai, X. et al. Soft Comput (2019). https://doi.org/10.1007/s00500-019-03794-x
     """
 
     def __init__(self, number_of_variables: int = 30):
         super(LIRCMOP5, self).__init__()
-        self.number_of_variables = number_of_variables
-        self.number_of_objectives = 2
-        self.number_of_constraints = 2
 
         self.obj_directions = [self.MINIMIZE, self.MINIMIZE]
-        self.obj_labels = ['f(x)', 'f(y)']
+        self.obj_labels = ["f(x)", "f(y)"]
 
-        self.lower_bound = [0.0 for _ in range(self.number_of_variables)]
-        self.upper_bound = [1.0 for _ in range(self.number_of_variables)]
+        self.lower_bound = [0.0 for _ in range(number_of_variables)]
+        self.upper_bound = [1.0 for _ in range(number_of_variables)]
+
+    def number_of_objectives(self) -> int:
+        return len(self.obj_directions)
+
+    def number_of_constraints(self) -> int:
+        return 2
 
     def evaluate(self, solution: FloatSolution) -> FloatSolution:
         x = solution.variables
 
         solution.objectives[0] = x[0] + 10 * self.g1(x) + 0.7057
         solution.objectives[1] = 1 - sqrt(x[0]) + 10 * self.g2(x) + 7057
 
@@ -187,19 +200,19 @@
         b_array = [4.0, 8.0]
         x_offset = [1.6, 2.5]
         y_offset = [1.6, 2.5]
         f1 = solution.objectives[0]
         f2 = solution.objectives[1]
 
         for i in range(len(x_offset)):
-            constraints[i] = pow(
-                ((f1 - x_offset[i]) * cos(theta) - (f2 - y_offset[i]) * sin(theta)) / a_array[i], 2) + \
-                             pow(
-                                 ((f1 - x_offset[i]) * sin(theta) + (f2 - y_offset[i]) * cos(theta)) / b_array[i],
-                                 2) - r
+            constraints[i] = (
+                pow(((f1 - x_offset[i]) * cos(theta) - (f2 - y_offset[i]) * sin(theta)) / a_array[i], 2)
+                + pow(((f1 - x_offset[i]) * sin(theta) + (f2 - y_offset[i]) * cos(theta)) / b_array[i], 2)
+                - r
+            )
 
         solution.constraints = constraints
 
         return solution
 
     def g1(self, x: [float]) -> float:
         result = 0
@@ -211,20 +224,20 @@
     def g2(self, x: [float]) -> float:
         result = 0
         for i in range(1, self.number_of_variables, 2):
             result += pow(x[i] - cos(0.5 * i / len(x) * pi * x[0]), 2.0)
 
         return result
 
-    def get_name(self):
-        return 'LIR-CMOP5'
+    def name(self):
+        return "LIR-CMOP5"
 
 
 class LIRCMOP6(LIRCMOP5):
-    """ Class representing problem LIR-CMOP6, defined in:
+    """Class representing problem LIR-CMOP6, defined in:
 
     * An Improved epsilon-constrained Method in MOEA/D for CMOPs with Large Infeasible Regions.
       Fan, Z., Li, W., Cai, X. et al. Soft Comput (2019). https://doi.org/10.1007/s00500-019-03794-x
     """
 
     def __init__(self, number_of_variables: int = 30):
         super(LIRCMOP6, self).__init__(number_of_variables)
@@ -236,116 +249,116 @@
         solution.objectives[1] = 1 - x[0] * x[0] + 10 * self.g2(x) + 7057
 
         self.evaluate_constraints(solution)
 
         return solution
 
     def evaluate_constraints(self, solution: FloatSolution) -> FloatSolution:
-        constraints = [0.0 for _ in range(self.number_of_constraints)]
+        constraints = [0.0 for _ in range(self.number_of_constraints())]
 
         r = 0.1
         theta = -0.25 * pi
         a_array = [2.0, 2.0]
         b_array = [8.0, 8.0]
         x_offset = [1.8, 2.8]
         y_offset = [1.8, 2.8]
         f1 = solution.objectives[0]
         f2 = solution.objectives[1]
 
         for i in range(len(x_offset)):
-            constraints[i] = pow(
-                ((f1 - x_offset[i]) * cos(theta) - (f2 - y_offset[i]) * sin(theta)) / a_array[i], 2) + \
-                             pow(
-                                 ((f1 - x_offset[i]) * sin(theta) + (f2 - y_offset[i]) * cos(theta)) / b_array[i],
-                                 2) - r
+            constraints[i] = (
+                pow(((f1 - x_offset[i]) * cos(theta) - (f2 - y_offset[i]) * sin(theta)) / a_array[i], 2)
+                + pow(((f1 - x_offset[i]) * sin(theta) + (f2 - y_offset[i]) * cos(theta)) / b_array[i], 2)
+                - r
+            )
 
         solution.constraints = constraints
 
         return solution
 
-    def get_name(self):
-        return 'LIR-CMOP6'
+    def name(self):
+        return "LIR-CMOP6"
 
 
 class LIRCMOP7(LIRCMOP5):
-    """ Class representing problem LIR-CMOP7, defined in:
+    """Class representing problem LIR-CMOP7, defined in:
 
     * An Improved epsilon-constrained Method in MOEA/D for CMOPs with Large Infeasible Regions.
       Fan, Z., Li, W., Cai, X. et al. Soft Comput (2019). https://doi.org/10.1007/s00500-019-03794-x
     """
 
     def __init__(self, number_of_variables: int = 30):
         super(LIRCMOP7, self).__init__(number_of_variables)
 
     def evaluate_constraints(self, solution: FloatSolution) -> FloatSolution:
-        constraints = [0.0 for _ in range(self.number_of_constraints)]
+        constraints = [0.0 for _ in range(self.number_of_constraints())]
 
         r = 0.1
         theta = -0.25 * pi
         a_array = [2.0, 2.5, 2.5]
         b_array = [6.0, 12.0, 10.0]
         x_offset = [1.2, 2.25, 3.5]
         y_offset = [1.2, 2.25, 3.5]
         f1 = solution.objectives[0]
         f2 = solution.objectives[1]
 
         for i in range(len(x_offset)):
-            constraints[i] = pow(
-                ((f1 - x_offset[i]) * cos(theta) - (f2 - y_offset[i]) * sin(theta)) / a_array[i], 2) + \
-                             pow(
-                                 ((f1 - x_offset[i]) * sin(theta) + (f2 - y_offset[i]) * cos(theta)) / b_array[i],
-                                 2) - r
+            constraints[i] = (
+                pow(((f1 - x_offset[i]) * cos(theta) - (f2 - y_offset[i]) * sin(theta)) / a_array[i], 2)
+                + pow(((f1 - x_offset[i]) * sin(theta) + (f2 - y_offset[i]) * cos(theta)) / b_array[i], 2)
+                - r
+            )
 
         solution.constraints = constraints
 
         return solution
 
-    def get_name(self):
-        return 'LIR-CMOP7'
+    def name(self):
+        return "LIR-CMOP7"
 
 
 class LIRCMOP8(LIRCMOP6):
-    """ Class representing problem LIR-CMOP8, defined in:
+    """Class representing problem LIR-CMOP8, defined in:
 
     * An Improved epsilon-constrained Method in MOEA/D for CMOPs with Large Infeasible Regions.
       Fan, Z., Li, W., Cai, X. et al. Soft Comput (2019). https://doi.org/10.1007/s00500-019-03794-x
     """
 
     def __init__(self, number_of_variables: int = 30):
         super(LIRCMOP8, self).__init__(number_of_variables)
 
     def evaluate_constraints(self, solution: FloatSolution) -> FloatSolution:
-        constraints = [0.0 for _ in range(self.number_of_constraints)]
+        constraints = [0.0 for _ in range(self.number_of_constraints())]
 
         r = 0.1
         theta = -0.25 * pi
         a_array = [2.0, 2.5, 2.5]
         b_array = [6.0, 12.0, 10.0]
         x_offset = [1.2, 2.25, 3.5]
         y_offset = [1.2, 2.25, 3.5]
         f1 = solution.objectives[0]
         f2 = solution.objectives[1]
 
         for i in range(len(x_offset)):
-            constraints[i] = pow(
-                ((f1 - x_offset[i]) * cos(theta) - (f2 - y_offset[i]) * sin(theta)) / a_array[i], 2) + \
-                             pow(
-                                 ((f1 - x_offset[i]) * sin(theta) + (f2 - y_offset[i]) * cos(theta)) / b_array[i],
-                                 2) - r
+            constraints[i] = (
+                pow(((f1 - x_offset[i]) * cos(theta) - (f2 - y_offset[i]) * sin(theta)) / a_array[i], 2)
+                + pow(((f1 - x_offset[i]) * sin(theta) + (f2 - y_offset[i]) * cos(theta)) / b_array[i], 2)
+                - r
+            )
 
         solution.constraints = constraints
 
         return solution
 
-    def get_name(self):
-        return 'LIR-CMOP8'
+    def name(self):
+        return "LIR-CMOP8"
 
 
 class LIRCMOP9(LIRCMOP8):
-    """ Class representing problem LIR-CMOP9, defined in:
+    """Class representing problem LIR-CMOP9, defined in:
 
     * An Improved epsilon-constrained Method in MOEA/D for CMOPs with Large Infeasible Regions.
       Fan, Z., Li, W., Cai, X. et al. Soft Comput (2019). https://doi.org/10.1007/s00500-019-03794-x
     """
 
     def __init__(self, number_of_variables: int = 30):
         super(LIRCMOP9, self).__init__(number_of_variables)
@@ -358,42 +371,45 @@
 
         self.evaluate_constraints(solution)
 
         return solution
 
     def evaluate_constraints(self, solution: FloatSolution) -> FloatSolution:
         x = solution.variables
-        constraints = [0.0 for _ in range(self.number_of_constraints)]
+        constraints = [0.0 for _ in range(self.number_of_constraints())]
 
         theta = -0.25 * pi
         n = 4.0
         f0 = solution.objectives[0]
         f1 = solution.objectives[1]
 
-        constraints[0] = f0 * sin(theta) + f1 * cos(theta) - sin(n * pi * (f0 * cos(theta) - f1 * sin(theta))) - 2;
+        constraints[0] = f0 * sin(theta) + f1 * cos(theta) - sin(n * pi * (f0 * cos(theta) - f1 * sin(theta))) - 2
 
         x_offset = 1.40
         y_offset = 1.40
         a = 1.5
         b = 6.0
-        r = 0.1;
+        r = 0.1
 
-        constraints[1] = pow(((f0 - x_offset) * cos(theta) - (f1 - y_offset) * sin(theta)) / a, 2) + pow(
-            ((f0 - x_offset) * sin(theta) + (f1 - y_offset) * cos(theta)) / b, 2) - r
+        constraints[1] = (
+            pow(((f0 - x_offset) * cos(theta) - (f1 - y_offset) * sin(theta)) / a, 2)
+            + pow(((f0 - x_offset) * sin(theta) + (f1 - y_offset) * cos(theta)) / b, 2)
+            - r
+        )
 
         solution.constraints = constraints
 
         return solution
 
-    def get_name(self):
-        return 'LIR-CMOP9'
+    def name(self):
+        return "LIR-CMOP9"
 
 
 class LIRCMOP10(LIRCMOP8):
-    """ Class representing problem LIR-CMOP10, defined in:
+    """Class representing problem LIR-CMOP10, defined in:
 
     * An Improved epsilon-constrained Method in MOEA/D for CMOPs with Large Infeasible Regions.
       Fan, Z., Li, W., Cai, X. et al. Soft Comput (2019). https://doi.org/10.1007/s00500-019-03794-x
     """
 
     def __init__(self, number_of_variables: int = 30):
         super(LIRCMOP10, self).__init__(number_of_variables)
@@ -405,133 +421,144 @@
         solution.objectives[1] = 1.7957 * (1 - sqrt(x[0])) * (10 * self.g2(x) + 1)
 
         self.evaluate_constraints(solution)
 
         return solution
 
     def evaluate_constraints(self, solution: FloatSolution) -> FloatSolution:
-        constraints = [0.0 for _ in range(self.number_of_constraints)]
+        constraints = [0.0 for _ in range(self.number_of_constraints())]
 
         theta = -0.25 * pi
         n = 4.0
         f0 = solution.objectives[0]
         f1 = solution.objectives[1]
 
-        constraints[0] = f0 * sin(theta) + f1 * cos(theta) - sin(n * pi * (f0 * cos(theta) - f1 * sin(theta))) - 1;
+        constraints[0] = f0 * sin(theta) + f1 * cos(theta) - sin(n * pi * (f0 * cos(theta) - f1 * sin(theta))) - 1
 
         x_offset = 1.1
         y_offset = 1.2
         a = 2.0
         b = 4.0
-        r = 0.1;
+        r = 0.1
 
-        constraints[1] = pow(((f0 - x_offset) * cos(theta) - (f1 - y_offset) * sin(theta)) / a, 2) + pow(
-            ((f0 - x_offset) * sin(theta) + (f1 - y_offset) * cos(theta)) / b, 2) - r
+        constraints[1] = (
+            pow(((f0 - x_offset) * cos(theta) - (f1 - y_offset) * sin(theta)) / a, 2)
+            + pow(((f0 - x_offset) * sin(theta) + (f1 - y_offset) * cos(theta)) / b, 2)
+            - r
+        )
 
         solution.constraints = constraints
 
         return solution
 
-    def get_name(self):
-        return 'LIR-CMOP10'
+    def name(self):
+        return "LIR-CMOP10"
 
 
 class LIRCMOP11(LIRCMOP10):
-    """ Class representing problem LIR-CMOP11, defined in:
+    """Class representing problem LIR-CMOP11, defined in:
 
     * An Improved epsilon-constrained Method in MOEA/D for CMOPs with Large Infeasible Regions.
       Fan, Z., Li, W., Cai, X. et al. Soft Comput (2019). https://doi.org/10.1007/s00500-019-03794-x
     """
 
     def __init__(self, number_of_variables: int = 30):
         super(LIRCMOP11, self).__init__(number_of_variables)
 
     def evaluate_constraints(self, solution: FloatSolution) -> FloatSolution:
-        constraints = [0.0 for _ in range(self.number_of_constraints)]
+        constraints = [0.0 for _ in range(self.number_of_constraints())]
 
         theta = -0.25 * pi
         n = 4.0
         f0 = solution.objectives[0]
         f1 = solution.objectives[1]
 
-        constraints[0] = f0 * sin(theta) + f1 * cos(theta) - sin(n * pi * (f0 * cos(theta) - f1 * sin(theta))) - 2.1;
+        constraints[0] = f0 * sin(theta) + f1 * cos(theta) - sin(n * pi * (f0 * cos(theta) - f1 * sin(theta))) - 2.1
 
         x_offset = 1.2
         y_offset = 1.2
         a = 1.5
         b = 5.0
-        r = 0.1;
+        r = 0.1
 
-        constraints[1] = pow(((f0 - x_offset) * cos(theta) - (f1 - y_offset) * sin(theta)) / a, 2) + pow(
-            ((f0 - x_offset) * sin(theta) + (f1 - y_offset) * cos(theta)) / b, 2) - r
+        constraints[1] = (
+            pow(((f0 - x_offset) * cos(theta) - (f1 - y_offset) * sin(theta)) / a, 2)
+            + pow(((f0 - x_offset) * sin(theta) + (f1 - y_offset) * cos(theta)) / b, 2)
+            - r
+        )
 
         solution.constraints = constraints
 
         return solution
 
-    def get_name(self):
-        return 'LIR-CMOP11'
+    def name(self):
+        return "LIR-CMOP11"
 
 
 class LIRCMOP12(LIRCMOP9):
-    """ Class representing problem LIR-CMOP9, defined in:
+    """Class representing problem LIR-CMOP9, defined in:
 
     * An Improved epsilon-constrained Method in MOEA/D for CMOPs with Large Infeasible Regions.
       Fan, Z., Li, W., Cai, X. et al. Soft Comput (2019). https://doi.org/10.1007/s00500-019-03794-x
     """
 
     def __init__(self, number_of_variables: int = 30):
         super(LIRCMOP12, self).__init__(number_of_variables)
 
     def evaluate_constraints(self, solution: FloatSolution) -> FloatSolution:
-        constraints = [0.0 for _ in range(self.number_of_constraints)]
+        constraints = [0.0 for _ in range(self.number_of_constraints())]
 
         theta = -0.25 * pi
         n = 4.0
         f0 = solution.objectives[0]
         f1 = solution.objectives[1]
 
-        constraints[0] = f0 * sin(theta) + f1 * cos(theta) - sin(n * pi * (f0 * cos(theta) - f1 * sin(theta))) - 2.5;
+        constraints[0] = f0 * sin(theta) + f1 * cos(theta) - sin(n * pi * (f0 * cos(theta) - f1 * sin(theta))) - 2.5
 
         x_offset = 1.6
         y_offset = 1.6
         a = 1.5
         b = 6.0
-        r = 0.1;
+        r = 0.1
 
-        constraints[1] = pow(((f0 - x_offset) * cos(theta) - (f1 - y_offset) * sin(theta)) / a, 2) + pow(
-            ((f0 - x_offset) * sin(theta) + (f1 - y_offset) * cos(theta)) / b, 2) - r
+        constraints[1] = (
+            pow(((f0 - x_offset) * cos(theta) - (f1 - y_offset) * sin(theta)) / a, 2)
+            + pow(((f0 - x_offset) * sin(theta) + (f1 - y_offset) * cos(theta)) / b, 2)
+            - r
+        )
 
         solution.constraints = constraints
 
         return solution
 
-    def get_name(self):
-        return 'LIR-CMOP12'
+    def name(self):
+        return "LIR-CMOP12"
 
 
 class LIRCMOP13(FloatProblem):
-    """ Class representing problem LIR-CMOP13, defined in:
+    """Class representing problem LIR-CMOP13, defined in:
 
     * An Improved epsilon-constrained Method in MOEA/D for CMOPs with Large Infeasible Regions.
       Fan, Z., Li, W., Cai, X. et al. Soft Comput (2019). https://doi.org/10.1007/s00500-019-03794-x
     """
 
     def __init__(self, number_of_variables: int = 30):
         super(LIRCMOP13, self).__init__()
-        self.number_of_variables = number_of_variables
-        self.number_of_objectives = 3
-        self.number_of_constraints = 2
 
         self.obj_directions = [self.MINIMIZE, self.MINIMIZE]
-        self.obj_labels = ['f(x)', 'f(y)']
+        self.obj_labels = ["f(x)", "f(y)"]
+
+        self.lower_bound = [0.0 for _ in range(number_of_variables)]
+        self.upper_bound = [1.0 for _ in range(number_of_variables)]
 
-        self.lower_bound = [0.0 for _ in range(self.number_of_variables)]
-        self.upper_bound = [1.0 for _ in range(self.number_of_variables)]
+    def number_of_objectives(self) -> int:
+        return len(self.obj_directions)
 
+    def number_of_constraints(self) -> int:
+        return 2
     def evaluate(self, solution: FloatSolution) -> FloatSolution:
         x = solution.variables
 
         solution.objectives[0] = (1.7057 + self.g1(x)) * cos(0.5 * pi * x[0]) * cos(0.5 * pi + x[1])
         solution.objectives[1] = (1.7057 + self.g1(x)) * cos(0.5 * pi * x[0]) * sin(0.5 * pi + x[1])
         solution.objectives[2] = (1.7057 + self.g1(x)) * sin(0.5 * pi + x[0])
 
@@ -554,37 +581,42 @@
     def g1(self, x: [float]) -> float:
         result = 0
         for i in range(2, self.number_of_variables, 2):
             result += 10 * pow(x[i] - 0.5, 2.0)
 
         return result
 
-    def get_name(self):
-        return 'LIR-CMOP13'
+    def name(self):
+        return "LIR-CMOP13"
 
 
 class LIRCMOP14(LIRCMOP13):
-    """ Class representing problem LIR-CMOP14, defined in:
+    """Class representing problem LIR-CMOP14, defined in:
 
     * An Improved epsilon-constrained Method in MOEA/D for CMOPs with Large Infeasible Regions.
       Fan, Z., Li, W., Cai, X. et al. Soft Comput (2019). https://doi.org/10.1007/s00500-019-03794-x
     """
 
     def __init__(self, number_of_variables: int = 30):
         super(LIRCMOP14, self).__init__(number_of_variables)
-        self.number_of_constraints = 3
+
+    def number_of_objectives(self) -> int:
+        return len(self.obj_directions)
+
+    def number_of_constraints(self) -> int:
+        return 3
 
     def evaluate_constraints(self, solution: FloatSolution) -> FloatSolution:
-        constraints = [0.0 for _ in range(self.number_of_constraints)]
+        constraints = [0.0 for _ in range(self.number_of_constraints())]
 
         f = sum([pow(solution.objectives[i], 2) for i in range(solution.number_of_objectives)])
 
         constraints[0] = (f - 9) * (f - 4)
         constraints[1] = (f - 1.9 * 1.9) * (f - 1.8 * 1.8)
         constraints[2] = (f - 1.75 * 1.75) * (f - 1.6 * 1.6)
 
         solution.constraints = constraints
 
         return solution
 
-    def get_name(self):
-        return 'LIR-CMOP14'
+    def name(self):
+        return "LIR-CMOP14"
```

### Comparing `jmetalpy-1.5.5/jmetal/problem/multiobjective/lz09.py` & `jmetalpy-1.6.0/jmetal/problem/multiobjective/lz09.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,125 +13,121 @@
 """
 
 
 class LZ09(FloatProblem):
 
     __metaclass__ = ABCMeta
 
-    def __init__(self,
-                 number_of_variables: int,
-                 number_of_objectives: int,
-                 number_of_constraints: int,
-                 ptype: int,
-                 dtype: int,
-                 ltype: int):
-        """ LZ09 benchmark family as defined in:
+    def __init__(
+        self,
+        number_of_variables: int,
+        ptype: int,
+        dtype: int,
+        ltype: int,
+    ):
+        """LZ09 benchmark family as defined in:
 
         * H. Li and Q. Zhang. Multiobjective optimization problems with complicated pareto sets, MOEA/D and NSGA-II.
         IEEE Transactions on Evolutionary Computation, 12(2):284-302, April 2009.
         """
         super(LZ09, self).__init__()
-        self.number_of_variables = number_of_variables
-        self.number_of_objectives = number_of_objectives
-        self.number_of_constraints = number_of_constraints
 
-        self.obj_directions = [self.MINIMIZE, self.MINIMIZE, self.MINIMIZE]
-        self.obj_labels = ['f(x)', 'f(y)', 'f(z)']
-
-        self.lower_bound = self.number_of_variables * [0.0]
-        self.upper_bound = self.number_of_variables * [1.0]
+        self.lower_bound = number_of_variables * [0.0]
+        self.upper_bound = number_of_variables * [1.0]
 
         self.ptype = ptype
         self.dtype = dtype
         self.ltype = ltype
 
+    def number_of_constraints(self) -> int:
+        return 0
+
     def evaluate(self, solution: FloatSolution) -> FloatSolution:
         x = solution.variables
         y = self.objective(x)
 
-        for i in range(self.number_of_objectives):
+        for i in range(self.number_of_objectives()):
             solution.objectives[i] = y[i]
 
         return solution
 
     def __ps_func2(self, x: float, t1: float, dim: int, type: int, css: int) -> float:
-        """ Control the PS shapes of 2-D instances.
+        """Control the PS shapes of 2-D instances.
 
         :param type: The type of the curve.
         :param css: The class of the index.
         """
         beta = 0.0
         dim += 1
 
         if type == 21:
             xy = 2 * (x - 0.5)
-            beta = xy - math.pow(t1, 0.5 * (self.number_of_variables + 3 * dim - 8) / (self.number_of_variables - 2))
+            beta = xy - math.pow(t1, 0.5 * (self.number_of_variables() + 3 * dim - 8) / (self.number_of_variables() - 2))
         if type == 22:
-            theta = 6 * math.pi * t1 + dim * math.pi / self.number_of_variables
+            theta = 6 * math.pi * t1 + dim * math.pi / self.number_of_variables()
             xy = 2 * (x - 0.5)
             beta = xy - math.sin(theta)
         if type == 23:
-            theta = 6 * math.pi * t1 + dim * math.pi / self.number_of_variables
+            theta = 6 * math.pi * t1 + dim * math.pi / self.number_of_variables()
             ra = 0.8 * t1
             xy = 2 * (x - 0.5)
             if css == 1:
                 beta = xy - ra * math.cos(theta)
             else:
                 beta = xy - ra * math.sin(theta)
         if type == 24:
-            theta = 6 * math.pi * t1 + dim * math.pi / self.number_of_variables
+            theta = 6 * math.pi * t1 + dim * math.pi / self.number_of_variables()
             xy = 2 * (x - 0.5)
             ra = 0.8 * t1
             if css == 1:
                 beta = xy - ra * math.cos(theta / 3)
             else:
                 beta = xy - ra * math.sin(theta)
         if type == 25:
             rho = 0.8
             phi = math.pi * t1
-            theta = 6 * math.pi * t1 + dim * math.pi / self.number_of_variables
+            theta = 6 * math.pi * t1 + dim * math.pi / self.number_of_variables()
             xy = 2 * (x - 0.5)
             if css == 1:
                 beta = xy - rho * math.sin(phi) * math.sin(theta)
             elif css == 2:
                 beta = xy - rho * math.sin(phi) * math.cos(theta)
             else:
                 beta = xy - rho * math.cos(phi)
         if type == 26:
-            theta = 6 * math.pi * t1 + dim * math.pi / self.number_of_variables
+            theta = 6 * math.pi * t1 + dim * math.pi / self.number_of_variables()
             ra = 0.3 * t1 * (t1 * math.cos(4 * theta) + 2)
             xy = 2 * (x - 0.5)
             if css == 1:
                 beta = xy - ra * math.cos(theta)
             else:
                 beta = xy - ra * math.sin(theta)
 
         return beta
 
     def __ps_func3(self, x: float, t1: float, t2: float, dim: int, type: int):
-        """ Control the PS shapes of 3-D instances.
+        """Control the PS shapes of 3-D instances.
         :param type: The type of curve.
         """
         beta = 0.0
         dim += 1
 
         if type == 31:
-            xy = 4 * (x - .5)
-            rate = 1.0 * dim / self.number_of_variables
+            xy = 4 * (x - 0.5)
+            rate = 1.0 * dim / self.number_of_variables()
             beta = xy - 4 * (t1 * t1 * rate + t2 * (1.0 - rate)) + 2
         if type == 32:
-            theta = 2 * math.pi * t1 + dim * math.pi / self.number_of_variables
-            xy = 4 * (x - .5)
+            theta = 2 * math.pi * t1 + dim * math.pi / self.number_of_variables()
+            xy = 4 * (x - 0.5)
             beta = xy - 2 * t2 * math.sin(theta)
 
         return beta
 
     def __alpha_func(self, x: list, dim: int, type: int) -> list:
-        """ Control the PF shape.
-        """
+        """Control the PF shape."""
         alpha = [0.0] * dim
 
         if dim == 2:
             if type == 21:
                 alpha[0] = x[0]
                 alpha[1] = 1 - math.sqrt(x[0])
             if type == 22:
@@ -160,16 +156,15 @@
                 alpha[0] = x[0] - x[1]
                 alpha[1] = x[0] * (1 - x[1])
                 alpha[2] = 1 - x[0]
 
         return alpha
 
     def __beta_func(self, x: list, type: int) -> float:
-        """ Control the distance.
-        """
+        """Control the distance."""
         beta = 0.0
         dim = len(x)
 
         if dim == 0:
             beta = 0.0
         if type == 1:
             for i in range(dim):
@@ -179,15 +174,15 @@
             for i in range(dim):
                 beta += math.sqrt(i + 1) * x[i] * x[i]
             beta = 2.0 * beta / dim
         if type == 3:
             sum, xx = 0, 0
             for i in range(dim):
                 xx = 2 * x[i]
-                sum += (xx * xx - math.cos(4 * math.pi * xx) + 1)
+                sum += xx * xx - math.cos(4 * math.pi * xx) + 1
             beta = 2.0 * sum / dim
         if type == 4:
             sum, prod, xx = 0, 1, 0
             for i in range(dim):
                 xx = 2 * x[i]
                 sum += xx * xx
                 prod *= math.cos(10 * math.pi * xx / math.sqrt(i + 1))
@@ -196,19 +191,19 @@
         return beta
 
     def objective(self, x_variables: list) -> list:
         aa = []
         bb = []
         cc = []
 
-        y_objectives = [0.0] * self.number_of_objectives
+        y_objectives = [0.0] * self.number_of_objectives()
 
-        if self.number_of_objectives == 2:
+        if self.number_of_objectives() == 2:
             if self.ltype in [21, 22, 23, 24, 26]:
-                for n in range(1, self.number_of_variables):
+                for n in range(1, self.number_of_variables()):
                     if n % 2 == 0:
                         a = self.__ps_func2(x_variables[n], x_variables[0], n, self.ltype, 1)
                         aa.append(a)
                     else:
                         b = self.__ps_func2(x_variables[n], x_variables[0], n, self.ltype, 2)
                         bb.append(b)
 
@@ -216,15 +211,15 @@
                 h = self.__beta_func(bb, self.dtype)
 
                 alpha = self.__alpha_func(x_variables, 2, self.ptype)
 
                 y_objectives[0] = alpha[0] + h
                 y_objectives[1] = alpha[1] + g
             if self.ltype == 25:
-                for n in range(1, self.number_of_variables):
+                for n in range(1, self.number_of_variables()):
                     if n % 3 == 0:
                         a = self.__ps_func2(x_variables[n], x_variables[0], n, self.ltype, 1)
                         aa.append(a)
                     elif n % 3 == 1:
                         b = self.__ps_func2(x_variables[n], x_variables[n], n, self.ltype, 2)
                         bb.append(b)
                     else:
@@ -238,18 +233,18 @@
                 h = self.__beta_func(bb, self.dtype)
 
                 alpha = self.__alpha_func(x_variables, 2, self.ptype)
 
                 y_objectives[0] = alpha[0] + h
                 y_objectives[1] = alpha[1] + g
 
-        if self.number_of_objectives == 3:
+        if self.number_of_objectives() == 3:
             if self.ltype == 31 or self.ltype == 32:
 
-                for n in range(2, self.number_of_variables):
+                for n in range(2, self.number_of_variables()):
                     a = self.__ps_func3(x_variables[n], x_variables[0], x_variables[1], n, self.ltype)
 
                     if n % 3 == 0:
                         aa.append(a)
                     elif n % 3 == 1:
                         bb.append(a)
                     else:
@@ -264,98 +259,146 @@
                 y_objectives[0] = alpha[0] + h
                 y_objectives[1] = alpha[1] + g
                 y_objectives[2] = alpha[2] + e
 
         return y_objectives
 
     def get_name(self):
-        return 'LZ09'
+        return "LZ09"
 
 
 class LZ09_F1(LZ09):
+    def __init__(self, number_of_variables=10):
+        super(LZ09_F1, self).__init__(
+            number_of_variables, dtype=1, ltype=21, ptype=21
+        )
+        self.obj_directions = [self.MINIMIZE, self.MINIMIZE]
+        self.obj_labels = ["f(x)", "f(y)"]
 
-    def __init__(self):
-        super(LZ09_F1, self).__init__(number_of_variables=10, number_of_objectives=2, number_of_constraints=0,
-                                      dtype=1, ltype=21, ptype=21)
+    def number_of_objectives(self) -> int:
+        return len(self.obj_directions)
 
-    def get_name(self):
-        return 'LZ09_F1'
+    def name(self):
+        return "LZ09_F1"
 
 
 class LZ09_F2(LZ09):
+    def __init__(self, number_of_variables=30):
+        super(LZ09_F2, self).__init__(
+            number_of_variables, dtype=1, ltype=22, ptype=21
+        )
 
-    def __init__(self):
-        super(LZ09_F2, self).__init__(number_of_variables=30, number_of_objectives=2, number_of_constraints=0,
-                                      dtype=1, ltype=22, ptype=21)
+        self.obj_directions = [self.MINIMIZE, self.MINIMIZE]
+        self.obj_labels = ["f(x)", "f(y)"]
 
-    def get_name(self):
-        return 'LZ09_F2'
+    def number_of_objectives(self) -> int:
+        return len(self.obj_directions)
+
+    def name(self):
+        return "LZ09_F2"
 
 
 class LZ09_F3(LZ09):
+    def __init__(self, number_of_variables=30):
+        super(LZ09_F3, self).__init__(
+            number_of_variables, dtype=1, ltype=23, ptype=21
+        )
+        self.obj_directions = [self.MINIMIZE, self.MINIMIZE]
+        self.obj_labels = ["f(x)", "f(y)"]
 
-    def __init__(self):
-        super(LZ09_F3, self).__init__(number_of_variables=30, number_of_objectives=2, number_of_constraints=0,
-                                      dtype=1, ltype=23, ptype=21)
+    def number_of_objectives(self) -> int:
+        return len(self.obj_directions)
 
-    def get_name(self):
-        return 'LZ09_F3'
+    def name(self):
+        return "LZ09_F3"
 
 
 class LZ09_F4(LZ09):
+    def __init__(self, number_of_variables=30):
+        super(LZ09_F4, self).__init__(
+            number_of_variables, dtype=1, ltype=24, ptype=21
+        )
+        self.obj_directions = [self.MINIMIZE, self.MINIMIZE]
+        self.obj_labels = ["f(x)", "f(y)"]
 
-    def __init__(self):
-        super(LZ09_F4, self).__init__(number_of_variables=30, number_of_objectives=2, number_of_constraints=0,
-                                      dtype=1, ltype=24, ptype=21)
+    def number_of_objectives(self) -> int:
+        return len(self.obj_directions)
 
-    def get_name(self):
-        return 'LZ09_F4'
+    def name(self):
+        return "LZ09_F4"
 
 
 class LZ09_F5(LZ09):
+    def __init__(self, number_of_variables=30):
+        super(LZ09_F5, self).__init__(
+            number_of_variables, dtype=1, ltype=26, ptype=21
+        )
+        self.obj_directions = [self.MINIMIZE, self.MINIMIZE]
+        self.obj_labels = ["f(x)", "f(y)"]
 
-    def __init__(self):
-        super(LZ09_F5, self).__init__(number_of_variables=30, number_of_objectives=2, number_of_constraints=0,
-                                      dtype=1, ltype=26, ptype=21)
+    def number_of_objectives(self) -> int:
+        return len(self.obj_directions)
 
-    def get_name(self):
-        return 'LZ09_F5'
+    def name(self):
+        return "LZ09_F5"
 
 
 class LZ09_F6(LZ09):
+    def __init__(self, number_of_variables=10):
+        super(LZ09_F6, self).__init__(
+            number_of_variables, dtype=1, ltype=32, ptype=31
+        )
+        self.obj_directions = [self.MINIMIZE, self.MINIMIZE, self.MINIMIZE]
+        self.obj_labels = ["f(x)", "f(y)", "f(z)"]
 
-    def __init__(self):
-        super(LZ09_F6, self).__init__(number_of_variables=10, number_of_objectives=3, number_of_constraints=0,
-                                      dtype=1, ltype=32, ptype=31)
+    def number_of_objectives(self) -> int:
+        return len(self.obj_directions)
 
-    def get_name(self):
-        return 'LZ09_F6'
+    def name(self):
+        return "LZ09_F6"
 
 
 class LZ09_F7(LZ09):
+    def __init__(self, number_of_variables=10):
+        super(LZ09_F7, self).__init__(
+            number_of_variables, dtype=3, ltype=21, ptype=21
+        )
 
-    def __init__(self):
-        super(LZ09_F7, self).__init__(number_of_variables=10, number_of_objectives=2, number_of_constraints=0,
-                                      dtype=3, ltype=21, ptype=21)
+        self.obj_directions = [self.MINIMIZE, self.MINIMIZE]
+        self.obj_labels = ["f(x)", "f(y)"]
 
-    def get_name(self):
-        return 'LZ09_F7'
+    def number_of_objectives(self) -> int:
+        return len(self.obj_directions)
+
+    def name(self):
+        return "LZ09_F7"
 
 
 class LZ09_F8(LZ09):
+    def __init__(self, number_of_variables=10):
+        super(LZ09_F8, self).__init__(
+            number_of_variables, dtype=4, ltype=21, ptype=21
+        )
+        self.obj_directions = [self.MINIMIZE, self.MINIMIZE]
+        self.obj_labels = ["f(x)", "f(y)"]
 
-    def __init__(self):
-        super(LZ09_F8, self).__init__(number_of_variables=10, number_of_objectives=2, number_of_constraints=0,
-                                      dtype=4, ltype=21, ptype=21)
+    def number_of_objectives(self) -> int:
+        return len(self.obj_directions)
 
-    def get_name(self):
-        return 'LZ09_F8'
+    def name(self):
+        return "LZ09_F8"
 
 
 class LZ09_F9(LZ09):
+    def __init__(self, number_of_variables=30):
+        super(LZ09_F9, self).__init__(
+            number_of_variables, dtype=1, ltype=22, ptype=22
+        )
 
-    def __init__(self):
-        super(LZ09_F9, self).__init__(number_of_variables=30, number_of_objectives=2, number_of_constraints=0,
-                                      dtype=1, ltype=22, ptype=22)
+        self.obj_directions = [self.MINIMIZE, self.MINIMIZE]
+        self.obj_labels = ["f(x)", "f(y)"]
 
-    def get_name(self):
-        return 'LZ09_F9'
+    def number_of_objectives(self) -> int:
+        return len(self.obj_directions)
+
+    def name(self):
+        return "LZ09_F9"
```

### Comparing `jmetalpy-1.5.5/jmetal/problem/multiobjective/test/test_constrained.py` & `jmetalpy-1.6.0/jmetal/problem/multiobjective/test/test_constrained.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,68 +1,66 @@
 import unittest
 from math import pi
 
 from jmetal.problem.multiobjective.constrained import Srinivas, Tanaka
 
 
 class SrinivasTestCases(unittest.TestCase):
-
     def test_should_constructor_create_a_non_null_object(self) -> None:
         problem = Srinivas()
         self.assertIsNotNone(problem)
 
     def test_should_constructor_create_a_valid_problem_with_default_settings(self) -> None:
         problem = Srinivas()
-        self.assertEqual(2, problem.number_of_variables)
-        self.assertEqual(2, problem.number_of_objectives)
-        self.assertEqual(2, problem.number_of_constraints)
+        self.assertEqual(2, problem.number_of_variables())
+        self.assertEqual(2, problem.number_of_objectives())
+        self.assertEqual(2, problem.number_of_constraints())
         self.assertEqual([-20.0, -20.0], problem.lower_bound)
         self.assertEqual([20.0, 20.0], problem.upper_bound)
 
     def test_should_create_solution_create_a_valid_float_solution(self) -> None:
         problem = Srinivas()
         solution = problem.create_solution()
         self.assertEqual(2, solution.number_of_variables)
         self.assertEqual(2, len(solution.variables))
         self.assertEqual(2, solution.number_of_objectives)
         self.assertEqual(2, len(solution.objectives))
-        self.assertEqual(2, problem.number_of_constraints)
+        self.assertEqual(2, problem.number_of_constraints())
         self.assertTrue(all(variable >= -20.0 for variable in solution.variables))
         self.assertTrue(all(variable <= 20.0 for variable in solution.variables))
 
     def test_should_get_name_return_the_right_name(self):
         problem = Srinivas()
-        self.assertEqual("Srinivas", problem.get_name())
+        self.assertEqual("Srinivas", problem.name())
 
 
 class TanakaTestCases(unittest.TestCase):
-
     def test_should_constructor_create_a_non_null_object(self) -> None:
         problem = Tanaka()
         self.assertIsNotNone(problem)
 
     def test_should_constructor_create_a_valid_problem_with_default_settings(self) -> None:
         problem = Tanaka()
-        self.assertEqual(2, problem.number_of_variables)
-        self.assertEqual(2, problem.number_of_objectives)
-        self.assertEqual(2, problem.number_of_constraints)
+        self.assertEqual(2, problem.number_of_variables())
+        self.assertEqual(2, problem.number_of_objectives())
+        self.assertEqual(2, problem.number_of_constraints())
         self.assertEqual([10e-5, 10e-5], problem.lower_bound)
         self.assertEqual([pi, pi], problem.upper_bound)
 
     def test_should_create_solution_create_a_valid_float_solution(self) -> None:
         problem = Tanaka()
         solution = problem.create_solution()
         self.assertEqual(2, solution.number_of_variables)
         self.assertEqual(2, len(solution.variables))
         self.assertEqual(2, solution.number_of_objectives)
         self.assertEqual(2, len(solution.objectives))
-        self.assertEqual(2, problem.number_of_constraints)
+        self.assertEqual(2, problem.number_of_constraints())
         self.assertTrue(all(variable >= 10e-5 for variable in solution.variables))
         self.assertTrue(all(variable <= pi for variable in solution.variables))
 
     def test_should_get_name_return_the_right_name(self):
         problem = Tanaka()
-        self.assertEqual("Tanaka", problem.get_name())
+        self.assertEqual("Tanaka", problem.name())
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `jmetalpy-1.5.5/jmetal/problem/multiobjective/test/test_unconstrained.py` & `jmetalpy-1.6.0/jmetal/problem/multiobjective/test/test_unconstrained.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,77 +1,80 @@
 import unittest
 
-from jmetal.problem.multiobjective.unconstrained import Kursawe, Fonseca, Schaffer, Viennet2
+from jmetal.problem.multiobjective.unconstrained import (
+    Fonseca,
+    Kursawe,
+    Schaffer,
+    Viennet2,
+)
 
 
 class KursaweTestCases(unittest.TestCase):
-
     def test_should_constructor_create_a_non_null_object(self) -> None:
         problem = Kursawe(3)
         self.assertIsNotNone(problem)
 
     def test_should_constructor_create_a_valid_problem_with_default_settings(self) -> None:
         problem = Kursawe()
-        self.assertEqual(3, problem.number_of_variables)
-        self.assertEqual(2, problem.number_of_objectives)
-        self.assertEqual(0, problem.number_of_constraints)
+        self.assertEqual(3, problem.number_of_variables())
+        self.assertEqual(2, problem.number_of_objectives())
+        self.assertEqual(0, problem.number_of_constraints())
         self.assertEqual([-5.0, -5.0, -5.0], problem.lower_bound)
         self.assertEqual([5.0, 5.0, 5.0], problem.upper_bound)
 
     def test_should_constructor_create_a_valid_problem_with_5_variables(self) -> None:
         problem = Kursawe(5)
-        self.assertEqual(5, problem.number_of_variables)
-        self.assertEqual(2, problem.number_of_objectives)
-        self.assertEqual(0, problem.number_of_constraints)
+        self.assertEqual(5, problem.number_of_variables())
+        self.assertEqual(2, problem.number_of_objectives())
+        self.assertEqual(0, problem.number_of_constraints())
 
         self.assertEqual([-5.0, -5.0, -5.0, -5.0, -5.0], problem.lower_bound)
         self.assertEqual([5.0, 5.0, 5.0, 5.0, 5.0], problem.upper_bound)
 
     def test_should_create_solution_create_a_valid_float_solution(self) -> None:
         problem = Kursawe(3)
         solution = problem.create_solution()
         self.assertEqual(3, solution.number_of_variables)
         self.assertEqual(3, len(solution.variables))
         self.assertEqual(2, solution.number_of_objectives)
         self.assertEqual(2, len(solution.objectives))
-        self.assertEqual(0, problem.number_of_constraints)
+        self.assertEqual(0, problem.number_of_constraints())
         self.assertEqual([-5.0, -5.0, -5.0], problem.lower_bound)
         self.assertEqual([5.0, 5.0, 5.0], problem.upper_bound)
         self.assertTrue(all(variable >= -5.0 for variable in solution.variables))
         self.assertTrue(all(variable <= 5.0 for variable in solution.variables))
 
     def test_should_get_name_return_the_right_name(self):
         problem = Kursawe()
-        self.assertEqual("Kursawe", problem.get_name())
+        self.assertEqual("Kursawe", problem.name())
 
 
 class FonsecaTestCases(unittest.TestCase):
-
     def test_should_constructor_create_a_non_null_object(self):
         problem = Fonseca()
         self.assertIsNotNone(problem)
 
     def test_should_constructor_create_a_valid_problem_with_default_settings(self):
         problem = Fonseca()
-        self.assertEqual(3, problem.number_of_variables)
-        self.assertEqual(2, problem.number_of_objectives)
-        self.assertEqual(0, problem.number_of_constraints)
+        self.assertEqual(3, problem.number_of_variables())
+        self.assertEqual(2, problem.number_of_objectives())
+        self.assertEqual(0, problem.number_of_constraints())
 
         self.assertEqual(3 * [-4], problem.lower_bound)
         self.assertEqual(3 * [4], problem.upper_bound)
 
     def test_should_create_solution_create_a_valid_float_solution(self):
         problem = Fonseca()
         solution = problem.create_solution()
 
         self.assertEqual(3, solution.number_of_variables)
         self.assertEqual(3, len(solution.variables))
         self.assertEqual(2, solution.number_of_objectives)
         self.assertEqual(2, len(solution.objectives))
-        self.assertEqual(0, problem.number_of_constraints)
+        self.assertEqual(0, problem.number_of_constraints())
 
         self.assertEqual(3 * [-4], problem.lower_bound)
         self.assertEqual(3 * [4], problem.upper_bound)
 
         self.assertTrue(solution.variables[0] >= -4)
         self.assertTrue(solution.variables[0] <= 4)
 
@@ -86,47 +89,46 @@
         problem.evaluate(solution1)
 
         self.assertAlmostEqual(solution1.objectives[0], 0.991563628, 4)
         self.assertAlmostEqual(solution1.objectives[1], 0.999663388, 4)
 
     def test_should_get_name_return_the_right_name(self):
         problem = Fonseca()
-        self.assertEqual("Fonseca", problem.get_name())
+        self.assertEqual("Fonseca", problem.name())
 
 
 class SchafferTestCases(unittest.TestCase):
-
     def test_should_constructor_create_a_non_null_object(self):
         problem = Schaffer()
         self.assertIsNotNone(problem)
 
     def test_should_constructor_create_a_valid_problem_with_default_settings(self):
         problem = Schaffer()
-        self.assertEqual(1, problem.number_of_variables)
-        self.assertEqual(2, problem.number_of_objectives)
-        self.assertEqual(0, problem.number_of_constraints)
+        self.assertEqual(1, problem.number_of_variables())
+        self.assertEqual(2, problem.number_of_objectives())
+        self.assertEqual(0, problem.number_of_constraints())
 
-        self.assertEqual([-100000], problem.lower_bound)
-        self.assertEqual([100000], problem.upper_bound)
+        self.assertEqual([-1000], problem.lower_bound)
+        self.assertEqual([1000], problem.upper_bound)
 
     def test_should_create_solution_create_a_valid_float_solution(self):
         problem = Schaffer()
         solution = problem.create_solution()
 
         self.assertEqual(1, solution.number_of_variables)
         self.assertEqual(1, len(solution.variables))
         self.assertEqual(2, solution.number_of_objectives)
         self.assertEqual(2, len(solution.objectives))
-        self.assertEqual(0, problem.number_of_constraints)
+        self.assertEqual(0, problem.number_of_constraints())
 
-        self.assertEqual([-100000], problem.lower_bound)
-        self.assertEqual([100000], problem.upper_bound)
+        self.assertEqual([-1000], problem.lower_bound)
+        self.assertEqual([1000], problem.upper_bound)
 
-        self.assertTrue(solution.variables[0] >= -100000)
-        self.assertTrue(solution.variables[0] <= 100000)
+        self.assertTrue(solution.variables[0] >= -1000)
+        self.assertTrue(solution.variables[0] <= 1000)
 
     def test_should_create_solution_return_right_evaluation_values(self):
         problem = Schaffer()
 
         solution1 = problem.create_solution()
         solution2 = problem.create_solution()
         solution1.variables[0] = 3
@@ -139,41 +141,40 @@
         self.assertAlmostEqual(solution1.objectives[1], 1)
 
         self.assertAlmostEqual(solution2.objectives[0], 6.76)
         self.assertAlmostEqual(solution2.objectives[1], 21.16)
 
     def test_should_get_name_return_the_right_name(self):
         problem = Schaffer()
-        self.assertEqual("Schaffer", problem.get_name())
+        self.assertEqual("Schaffer", problem.name())
 
 
 class Viennet2TestCases(unittest.TestCase):
-
     def test_should_constructor_create_a_non_null_object(self):
         problem = Viennet2()
         self.assertIsNotNone(problem)
 
     def test_should_constructor_create_a_valid_problem_with_default_settings(self):
         problem = Viennet2()
-        self.assertEqual(2, problem.number_of_variables)
-        self.assertEqual(3, problem.number_of_objectives)
-        self.assertEqual(0, problem.number_of_constraints)
+        self.assertEqual(2, problem.number_of_variables())
+        self.assertEqual(3, problem.number_of_objectives())
+        self.assertEqual(0, problem.number_of_constraints())
 
         self.assertEqual([-4, -4], problem.lower_bound)
         self.assertEqual([4, 4], problem.upper_bound)
 
     def test_should_create_solution_create_a_valid_float_solution(self):
         problem = Viennet2()
         solution = problem.create_solution()
 
         self.assertEqual(2, solution.number_of_variables)
         self.assertEqual(2, len(solution.variables))
         self.assertEqual(3, solution.number_of_objectives)
         self.assertEqual(3, len(solution.objectives))
-        self.assertEqual(0, problem.number_of_constraints)
+        self.assertEqual(0, problem.number_of_constraints())
 
         self.assertEqual([-4, -4], problem.lower_bound)
         self.assertEqual([4, 4], problem.upper_bound)
 
         self.assertTrue(solution.variables[0] >= -4)
         self.assertTrue(solution.variables[0] <= 4)
 
@@ -187,12 +188,12 @@
 
         self.assertAlmostEqual(solution2.objectives[0], 14.0607692307)
         self.assertAlmostEqual(solution2.objectives[1], -11.8818055555)
         self.assertAlmostEqual(solution2.objectives[2], -11.1532369747)
 
     def test_should_get_name_return_the_right_name(self):
         problem = Viennet2()
-        self.assertEqual("Viennet2", problem.get_name())
+        self.assertEqual("Viennet2", problem.name())
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `jmetalpy-1.5.5/jmetal/problem/multiobjective/test/test_zdt.py` & `jmetalpy-1.6.0/jmetal/problem/multiobjective/test/test_zdt.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,220 +1,216 @@
 import unittest
 
 from jmetal.problem.multiobjective.zdt import ZDT1, ZDT2, ZDT3, ZDT4, ZDT6
 
 
 class ZDT1TestCases(unittest.TestCase):
-
     def test_should_constructor_create_a_non_null_object(self) -> None:
         problem = ZDT1()
         self.assertIsNotNone(problem)
 
     def test_should_constructor_create_a_valid_problem_with_default_settings(self) -> None:
         problem = ZDT1()
-        self.assertEqual(30, problem.number_of_variables)
-        self.assertEqual(2, problem.number_of_objectives)
-        self.assertEqual(0, problem.number_of_constraints)
+        self.assertEqual(30, problem.number_of_variables())
+        self.assertEqual(2, problem.number_of_objectives())
+        self.assertEqual(0, problem.number_of_constraints())
         self.assertEqual(30 * [0.0], problem.lower_bound)
         self.assertEqual(30 * [1.0], problem.upper_bound)
 
     def test_should_constructor_create_a_valid_problem_with_5_variables(self) -> None:
         problem = ZDT1(5)
-        self.assertEqual(5, problem.number_of_variables)
-        self.assertEqual(2, problem.number_of_objectives)
-        self.assertEqual(0, problem.number_of_constraints)
+        self.assertEqual(5, problem.number_of_variables())
+        self.assertEqual(2, problem.number_of_objectives())
+        self.assertEqual(0, problem.number_of_constraints())
 
-        self.assertEqual(5*[0.0], problem.lower_bound)
-        self.assertEqual(5*[1.0], problem.upper_bound)
+        self.assertEqual(5 * [0.0], problem.lower_bound)
+        self.assertEqual(5 * [1.0], problem.upper_bound)
 
     def test_should_create_solution_create_a_valid_float_solution(self) -> None:
         problem = ZDT1()
         solution = problem.create_solution()
+
         self.assertEqual(30, solution.number_of_variables)
         self.assertEqual(30, len(solution.variables))
         self.assertEqual(2, solution.number_of_objectives)
         self.assertEqual(2, len(solution.objectives))
-        self.assertEqual(0, problem.number_of_constraints)
+        self.assertEqual(0, problem.number_of_constraints())
         self.assertEqual(30 * [0.0], problem.lower_bound)
         self.assertEqual(30 * [1.0], problem.upper_bound)
         self.assertTrue(all(value >= 0.0 for value in solution.variables))
         self.assertTrue(all(value <= 1.0 for value in solution.variables))
 
     def test_should_get_name_return_the_right_name(self):
         problem = ZDT1()
-        self.assertEqual("ZDT1", problem.get_name())
+        self.assertEqual("ZDT1", problem.name())
 
 
 class ZDT2TestCases(unittest.TestCase):
-
     def test_should_constructor_create_a_non_null_object(self) -> None:
         problem = ZDT2()
         self.assertIsNotNone(problem)
 
     def test_should_constructor_create_a_valid_problem_with_default_settings(self) -> None:
         problem = ZDT2()
-        self.assertEqual(30, problem.number_of_variables)
-        self.assertEqual(2, problem.number_of_objectives)
-        self.assertEqual(0, problem.number_of_constraints)
+        self.assertEqual(30, problem.number_of_variables())
+        self.assertEqual(2, problem.number_of_objectives())
+        self.assertEqual(0, problem.number_of_constraints())
         self.assertEqual(30 * [0.0], problem.lower_bound)
         self.assertEqual(30 * [1.0], problem.upper_bound)
 
     def test_should_constructor_create_a_valid_problem_with_7_variables(self) -> None:
         problem = ZDT2(7)
-        self.assertEqual(7, problem.number_of_variables)
-        self.assertEqual(2, problem.number_of_objectives)
-        self.assertEqual(0, problem.number_of_constraints)
+        self.assertEqual(7, problem.number_of_variables())
+        self.assertEqual(2, problem.number_of_objectives())
+        self.assertEqual(0, problem.number_of_constraints())
 
-        self.assertEqual(7*[0.0], problem.lower_bound)
-        self.assertEqual(7*[1.0], problem.upper_bound)
+        self.assertEqual(7 * [0.0], problem.lower_bound)
+        self.assertEqual(7 * [1.0], problem.upper_bound)
 
     def test_should_create_solution_create_a_valid_float_solution(self) -> None:
         problem = ZDT2()
         solution = problem.create_solution()
         self.assertEqual(30, solution.number_of_variables)
         self.assertEqual(30, len(solution.variables))
         self.assertEqual(2, solution.number_of_objectives)
         self.assertEqual(2, len(solution.objectives))
-        self.assertEqual(0, problem.number_of_constraints)
+        self.assertEqual(0, problem.number_of_constraints())
         self.assertEqual(30 * [0.0], problem.lower_bound)
         self.assertEqual(30 * [1.0], problem.upper_bound)
         self.assertTrue(all(value >= 0.0 for value in solution.variables))
         self.assertTrue(all(value <= 1.0 for value in solution.variables))
 
     def test_should_get_name_return_the_right_name(self):
         problem = ZDT2()
-        self.assertEqual("ZDT2", problem.get_name())
+        self.assertEqual("ZDT2", problem.name())
 
 
 class ZDT3TestCases(unittest.TestCase):
-
     def test_should_constructor_create_a_non_null_object(self) -> None:
         problem = ZDT3()
         self.assertIsNotNone(problem)
 
     def test_should_constructor_create_a_valid_problem_with_default_settings(self) -> None:
         problem = ZDT3()
-        self.assertEqual(30, problem.number_of_variables)
-        self.assertEqual(2, problem.number_of_objectives)
-        self.assertEqual(0, problem.number_of_constraints)
+        self.assertEqual(30, problem.number_of_variables())
+        self.assertEqual(2, problem.number_of_objectives())
+        self.assertEqual(0, problem.number_of_constraints())
         self.assertEqual(30 * [0.0], problem.lower_bound)
         self.assertEqual(30 * [1.0], problem.upper_bound)
 
     def test_should_constructor_create_a_valid_problem_with_7_variables(self) -> None:
         problem = ZDT3(7)
-        self.assertEqual(7, problem.number_of_variables)
-        self.assertEqual(2, problem.number_of_objectives)
-        self.assertEqual(0, problem.number_of_constraints)
+        self.assertEqual(7, problem.number_of_variables())
+        self.assertEqual(2, problem.number_of_objectives())
+        self.assertEqual(0, problem.number_of_constraints())
 
-        self.assertEqual(7*[0.0], problem.lower_bound)
-        self.assertEqual(7*[1.0], problem.upper_bound)
+        self.assertEqual(7 * [0.0], problem.lower_bound)
+        self.assertEqual(7 * [1.0], problem.upper_bound)
 
     def test_should_create_solution_create_a_valid_float_solution(self) -> None:
         problem = ZDT3()
         solution = problem.create_solution()
         self.assertEqual(30, solution.number_of_variables)
         self.assertEqual(30, len(solution.variables))
         self.assertEqual(2, solution.number_of_objectives)
         self.assertEqual(2, len(solution.objectives))
-        self.assertEqual(0, problem.number_of_constraints)
+        self.assertEqual(0, problem.number_of_constraints())
         self.assertEqual(30 * [0.0], problem.lower_bound)
         self.assertEqual(30 * [1.0], problem.upper_bound)
         self.assertTrue(all(value >= 0.0 for value in solution.variables))
         self.assertTrue(all(value <= 1.0 for value in solution.variables))
 
     def test_should_get_name_return_the_right_name(self):
         problem = ZDT3()
-        self.assertEqual("ZDT3", problem.get_name())
+        self.assertEqual("ZDT3", problem.name())
 
 
 class ZDT4TestCases(unittest.TestCase):
-
     def test_should_constructor_create_a_non_null_object(self) -> None:
         problem = ZDT4()
         self.assertIsNotNone(problem)
 
     def test_should_constructor_create_a_valid_problem_with_default_settings(self) -> None:
         problem = ZDT4()
-        self.assertEqual(10, problem.number_of_variables)
-        self.assertEqual(2, problem.number_of_objectives)
-        self.assertEqual(0, problem.number_of_constraints)
+        self.assertEqual(10, problem.number_of_variables())
+        self.assertEqual(2, problem.number_of_objectives())
+        self.assertEqual(0, problem.number_of_constraints())
         self.assertEqual(0.0, problem.lower_bound[0])
         self.assertEqual(1.0, problem.upper_bound[0])
         self.assertEqual(9 * [-5.0], problem.lower_bound[1:10])
         self.assertEqual(9 * [5.0], problem.upper_bound[1:10])
 
     def test_should_constructor_create_a_valid_problem_with_7_variables(self) -> None:
         problem = ZDT4(7)
-        self.assertEqual(7, problem.number_of_variables)
-        self.assertEqual(2, problem.number_of_objectives)
-        self.assertEqual(0, problem.number_of_constraints)
+        self.assertEqual(7, problem.number_of_variables())
+        self.assertEqual(2, problem.number_of_objectives())
+        self.assertEqual(0, problem.number_of_constraints())
 
         self.assertEqual(0.0, problem.lower_bound[0])
         self.assertEqual(1.0, problem.upper_bound[0])
         self.assertEqual(6 * [-5.0], problem.lower_bound[1:7])
         self.assertEqual(6 * [5.0], problem.upper_bound[1:7])
 
     def test_should_create_solution_create_a_valid_float_solution(self) -> None:
         problem = ZDT4()
         solution = problem.create_solution()
         self.assertEqual(10, solution.number_of_variables)
         self.assertEqual(10, len(solution.variables))
         self.assertEqual(2, solution.number_of_objectives)
         self.assertEqual(2, len(solution.objectives))
-        self.assertEqual(0, problem.number_of_constraints)
+        self.assertEqual(0, problem.number_of_constraints())
         self.assertEqual(0.0, problem.lower_bound[0])
         self.assertEqual(1.0, problem.upper_bound[0])
         self.assertEqual(9 * [-5.0], problem.lower_bound[1:10])
         self.assertEqual(9 * [5.0], problem.upper_bound[1:10])
         self.assertTrue(solution.variables[0] >= -5.0)
         self.assertTrue(solution.variables[0] <= 5.0)
         self.assertTrue(all(value >= -5.0 for value in solution.variables[1:10]))
         self.assertTrue(all(value <= 5.0 for value in solution.variables[1:10]))
 
     def test_should_get_name_return_the_right_name(self):
         problem = ZDT4()
-        self.assertEqual("ZDT4", problem.get_name())
+        self.assertEqual("ZDT4", problem.name())
 
 
 class ZDT6TestCases(unittest.TestCase):
-
     def test_should_constructor_create_a_non_null_object(self) -> None:
         problem = ZDT6()
         self.assertIsNotNone(problem)
 
     def test_should_constructor_create_a_valid_problem_with_default_settings(self) -> None:
         problem = ZDT6()
-        self.assertEqual(10, problem.number_of_variables)
-        self.assertEqual(2, problem.number_of_objectives)
-        self.assertEqual(0, problem.number_of_constraints)
+        self.assertEqual(10, problem.number_of_variables())
+        self.assertEqual(2, problem.number_of_objectives())
+        self.assertEqual(0, problem.number_of_constraints())
         self.assertEqual(10 * [0.0], problem.lower_bound)
         self.assertEqual(10 * [1.0], problem.upper_bound)
 
     def test_should_constructor_create_a_valid_problem_with_7_variables(self) -> None:
         problem = ZDT3(7)
-        self.assertEqual(7, problem.number_of_variables)
-        self.assertEqual(2, problem.number_of_objectives)
-        self.assertEqual(0, problem.number_of_constraints)
+        self.assertEqual(7, problem.number_of_variables())
+        self.assertEqual(2, problem.number_of_objectives())
+        self.assertEqual(0, problem.number_of_constraints())
 
-        self.assertEqual(7*[0.0], problem.lower_bound)
-        self.assertEqual(7*[1.0], problem.upper_bound)
+        self.assertEqual(7 * [0.0], problem.lower_bound)
+        self.assertEqual(7 * [1.0], problem.upper_bound)
 
     def test_should_create_solution_create_a_valid_float_solution(self) -> None:
         problem = ZDT6()
         solution = problem.create_solution()
         self.assertEqual(10, solution.number_of_variables)
         self.assertEqual(10, len(solution.variables))
         self.assertEqual(2, solution.number_of_objectives)
         self.assertEqual(2, len(solution.objectives))
-        self.assertEqual(0, problem.number_of_constraints)
+        self.assertEqual(0, problem.number_of_constraints())
         self.assertEqual(10 * [0.0], problem.lower_bound)
         self.assertEqual(10 * [1.0], problem.upper_bound)
         self.assertTrue(all(value >= 0.0 for value in solution.variables))
         self.assertTrue(all(value <= 1.0 for value in solution.variables))
 
     def test_should_get_name_return_the_right_name(self):
         problem = ZDT6()
-        self.assertEqual("ZDT6", problem.get_name())
+        self.assertEqual("ZDT6", problem.name())
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `jmetalpy-1.5.5/jmetal/problem/multiobjective/uf.py` & `jmetalpy-1.6.0/jmetal/problem/multiobjective/uf.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,56 +9,59 @@
    :synopsis: Problems of the CEC2009 multi-objective competition
 
 .. moduleauthor:: Antonio J. Nebro <antonio@lcc.uma.es>
 """
 
 
 class UF1(FloatProblem):
-    """ Problem UF1.
+    """Problem UF1.
 
     .. note:: Unconstrained problem. The default number of variables is 30.
     """
 
     def __init__(self, number_of_variables: int = 30):
-        """ :param number_of_variables: number of decision variables of the problem.
-        """
+        """:param number_of_variables: number of decision variables of the problem."""
         super(UF1, self).__init__()
         self.number_of_variables = number_of_variables
         self.number_of_objectives = 2
         self.number_of_constraints = 0
 
         self.obj_directions = [self.MINIMIZE] * self.number_of_objectives
-        self.obj_labels = ['$ f_{} $'.format(i) for i in range(self.number_of_objectives)]
+        self.obj_labels = ["$ f_{} $".format(i) for i in range(self.number_of_objectives)]
 
         self.lower_bound = self.number_of_variables * [-1.0]
         self.upper_bound = self.number_of_variables * [1.0]
         self.lower_bound[0] = 0.0
         self.upper_bound[0] = 1.0
 
+    def number_of_objectives(self) -> int:
+        return len(self.obj_directions)
+
+    def number_of_constraints(self) -> int:
+        return 0
+
     def evaluate(self, solution: FloatSolution) -> FloatSolution:
         sum1 = 0
         sum2 = 0
         count1 = 0
         count2 = 0
 
         x = solution.variables
 
         for i in range(2, self.number_of_variables):
-            y = x[i-1] - sin(6.0 * pi * x[0] + i * pi/solution.number_of_variables)
-            y = y*y
+            y = x[i - 1] - sin(6.0 * pi * x[0] + i * pi / solution.number_of_variables)
+            y = y * y
 
-            if i % 2 is 0:
+            if i % 2 == 0:
                 sum2 += y
-                count2 +=1
+                count2 += 1
             else:
-                sum1 +=y
+                sum1 += y
                 count1 += 1
 
-        solution.objectives[0] = x[0] + 2.0 * sum1 /(1.0 * count1)
+        solution.objectives[0] = x[0] + 2.0 * sum1 / (1.0 * count1)
         solution.objectives[1] = 1.0 - sqrt(x[0]) + 2.0 * sum2 / (1.0 * count2)
 
-
         return solution
 
     def get_name(self):
-        return 'UF1'
-
+        return "UF1"
```

### Comparing `jmetalpy-1.5.5/jmetal/problem/multiobjective/unconstrained.py` & `jmetalpy-1.6.0/jmetal/problem/multiobjective/unconstrained.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,131 +1,137 @@
 import random
-from math import sqrt, exp, pow, sin
+from math import exp, pow, sin, sqrt
 
-from jmetal.core.problem import FloatProblem, BinaryProblem, Problem
-from jmetal.core.solution import FloatSolution, BinarySolution, CompositeSolution, IntegerSolution
+from jmetal.core.problem import BinaryProblem, FloatProblem, Problem
+from jmetal.core.solution import (
+    BinarySolution,
+    CompositeSolution,
+    FloatSolution,
+    IntegerSolution,
+)
 
 """
 .. module:: constrained
    :platform: Unix, Windows
    :synopsis: Unconstrained test problems for multi-objective optimization
 
 .. moduleauthor:: Antonio J. Nebro <antonio@lcc.uma.es>
 """
 
 
 class Kursawe(FloatProblem):
-    """ Class representing problem Kursawe. """
+    """Class representing problem Kursawe."""
 
     def __init__(self, number_of_variables: int = 3):
         super(Kursawe, self).__init__()
-        self.number_of_objectives = 2
-        self.number_of_variables = number_of_variables
-        self.number_of_constraints = 0
 
         self.obj_directions = [self.MINIMIZE, self.MINIMIZE]
-        self.obj_labels = ['f(x)', 'f(y)']
+        self.obj_labels = ["f(x)", "f(y)"]
 
         self.lower_bound = [-5.0 for _ in range(number_of_variables)]
         self.upper_bound = [5.0 for _ in range(number_of_variables)]
 
-        FloatSolution.lower_bound = self.lower_bound
-        FloatSolution.upper_bound = self.upper_bound
+    def number_of_objectives(self) -> int:
+        return len(self.obj_directions)
+
+    def number_of_constraints(self) -> int:
+        return 0
 
     def evaluate(self, solution: FloatSolution) -> FloatSolution:
-        fx = [0.0 for _ in range(self.number_of_objectives)]
-        for i in range(self.number_of_variables - 1):
+        fx = [0.0 for _ in range(self.number_of_objectives())]
+        for i in range(self.number_of_variables() - 1):
             xi = solution.variables[i] * solution.variables[i]
             xj = solution.variables[i + 1] * solution.variables[i + 1]
             aux = -0.2 * sqrt(xi + xj)
             fx[0] += -10 * exp(aux)
+
+        for i in range(self.number_of_variables()):
             fx[1] += pow(abs(solution.variables[i]), 0.8) + 5.0 * sin(pow(solution.variables[i], 3.0))
 
         solution.objectives[0] = fx[0]
         solution.objectives[1] = fx[1]
 
         return solution
 
-    def get_name(self):
-        return 'Kursawe'
+    def name(self):
+        return "Kursawe"
 
 
 class Fonseca(FloatProblem):
-
     def __init__(self):
         super(Fonseca, self).__init__()
-        self.number_of_variables = 3
-        self.number_of_objectives = 2
-        self.number_of_constraints = 0
-
         self.obj_directions = [self.MINIMIZE, self.MINIMIZE]
-        self.obj_labels = ['f(x)', 'f(y)']
+        self.obj_labels = ["f(x)", "f(y)"]
+
+        number_of_variables = 3
 
-        self.lower_bound = self.number_of_variables * [-4]
-        self.upper_bound = self.number_of_variables * [4]
+        self.lower_bound = number_of_variables * [-4]
+        self.upper_bound = number_of_variables * [4]
 
-        FloatSolution.lower_bound = self.lower_bound
-        FloatSolution.upper_bound = self.upper_bound
+    def number_of_objectives(self) -> int:
+        return len(self.obj_directions)
+
+    def number_of_constraints(self) -> int:
+        return 0
 
     def evaluate(self, solution: FloatSolution) -> FloatSolution:
-        n = self.number_of_variables
-        solution.objectives[0] = 1 - exp(-sum([(x - 1.0 / n ** 0.5) ** 2 for x in solution.variables]))
-        solution.objectives[1] = 1 - exp(-sum([(x + 1.0 / n ** 0.5) ** 2 for x in solution.variables]))
+        n = self.number_of_variables()
+        solution.objectives[0] = 1 - exp(-sum([(x - 1.0 / n**0.5) ** 2 for x in solution.variables]))
+        solution.objectives[1] = 1 - exp(-sum([(x + 1.0 / n**0.5) ** 2 for x in solution.variables]))
 
         return solution
 
-    def get_name(self):
-        return 'Fonseca'
+    def name(self):
+        return "Fonseca"
 
 
 class Schaffer(FloatProblem):
-
     def __init__(self):
         super(Schaffer, self).__init__()
-        self.number_of_variables = 1
-        self.number_of_objectives = 2
-        self.number_of_constraints = 0
 
         self.obj_directions = [self.MINIMIZE, self.MINIMIZE]
-        self.obj_labels = ['f(x)', 'f(y)']
+        self.obj_labels = ["f(x)", "f(y)"]
 
-        self.lower_bound = [-100000]
-        self.upper_bound = [100000]
+        self.lower_bound = [-1000]
+        self.upper_bound = [1000]
 
-        FloatSolution.lower_bound = self.lower_bound
-        FloatSolution.upper_bound = self.upper_bound
+    def number_of_objectives(self) -> int:
+        return len(self.obj_directions)
+
+    def number_of_constraints(self) -> int:
+        return 0
 
     def evaluate(self, solution: FloatSolution) -> FloatSolution:
         value = solution.variables[0]
 
-        solution.objectives[0] = value ** 2
+        solution.objectives[0] = value**2
         solution.objectives[1] = (value - 2) ** 2
 
         return solution
 
-    def get_name(self):
-        return 'Schaffer'
+    def name(self):
+        return "Schaffer"
 
 
 class Viennet2(FloatProblem):
-
     def __init__(self):
         super(Viennet2, self).__init__()
-        self.number_of_variables = 2
-        self.number_of_objectives = 3
-        self.number_of_constraints = 0
 
         self.obj_directions = [self.MINIMIZE, self.MINIMIZE, self.MINIMIZE]
-        self.obj_labels = ['f(x)', 'f(y)', 'f(z)']
+        self.obj_labels = ["f(x)", "f(y)", "f(z)"]
 
-        self.lower_bound = self.number_of_variables * [-4]
-        self.upper_bound = self.number_of_variables * [4]
+        number_of_variables = 2
+        self.lower_bound = number_of_variables * [-4]
+        self.upper_bound = number_of_variables * [4]
 
-        FloatSolution.lower_bound = self.lower_bound
-        FloatSolution.upper_bound = self.upper_bound
+    def number_of_objectives(self) -> int:
+        return len(self.obj_directions)
+
+    def number_of_constraints(self) -> int:
+        return 0
 
     def evaluate(self, solution: FloatSolution) -> FloatSolution:
         x0 = solution.variables[0]
         x1 = solution.variables[1]
 
         f1 = (x0 - 2) * (x0 - 2) / 2.0 + (x1 + 1) * (x1 + 1) / 13.0 + 3.0
         f2 = (x0 + x1 - 3.0) * (x0 + x1 - 3.0) / 36.0 + (-x0 + x1 + 2.0) * (-x0 + x1 + 2.0) / 8.0 - 17.0
@@ -133,36 +139,35 @@
 
         solution.objectives[0] = f1
         solution.objectives[1] = f2
         solution.objectives[2] = f3
 
         return solution
 
-    def get_name(self):
-        return 'Viennet2'
+    def name(self):
+        return "Viennet2"
 
 
 class SubsetSum(BinaryProblem):
-
     def __init__(self, C: int, W: list):
-        """ The goal is to find a subset S of W whose elements sum is closest to (without exceeding) C.
+        """The goal is to find a subset S of W whose elements sum is closest to (without exceeding) C.
 
         :param C: Large integer.
         :param W: Set of non-negative integers."""
         super(SubsetSum, self).__init__()
         self.C = C
         self.W = W
 
         self.number_of_bits = len(self.W)
         self.number_of_objectives = 2
         self.number_of_variables = 1
         self.number_of_constraints = 0
 
         self.obj_directions = [self.MAXIMIZE, self.MINIMIZE]
-        self.obj_labels = ['Sum', 'No. of Objects']
+        self.obj_labels = ["Sum", "No. of Objects"]
 
     def evaluate(self, solution: BinarySolution) -> BinarySolution:
         total_sum = 0.0
         number_of_objects = 0
 
         for index, bits in enumerate(solution.variables[0]):
             if bits:
@@ -177,36 +182,45 @@
 
         solution.objectives[0] = -1.0 * total_sum
         solution.objectives[1] = number_of_objects
 
         return solution
 
     def create_solution(self) -> BinarySolution:
-        new_solution = BinarySolution(number_of_variables=self.number_of_variables,
-                                      number_of_objectives=self.number_of_objectives)
-        new_solution.variables[0] = \
-            [True if random.randint(0, 1) == 0 else False for _ in range(self.number_of_bits)]
+        new_solution = BinarySolution(
+            number_of_variables=self.number_of_variables, number_of_objectives=self.number_of_objectives
+        )
+        new_solution.variables[0] = [True if random.randint(0, 1) == 0 else False for _ in range(self.number_of_bits)]
 
         return new_solution
 
-    def get_name(self) -> str:
-        return 'Subset Sum'
+    def name(self) -> str:
+        return "Subset Sum"
 
 
 class OneZeroMax(BinaryProblem):
+    """ The implementation of the OneZeroMax problems defines a single binary variable. This variable
+    will contain the bit string representing the solutions.
 
+    """
     def __init__(self, number_of_bits: int = 256):
         super(OneZeroMax, self).__init__()
         self.number_of_bits = number_of_bits
-        self.number_of_objectives = 2
-        self.number_of_variables = 1
-        self.number_of_constraints = 0
 
         self.obj_directions = [self.MINIMIZE]
-        self.obj_labels = ['Ones']
+        self.obj_labels = ["Ones"]
+
+    def number_of_variables(self) -> int:
+        return 1
+
+    def number_of_objectives(self) -> int:
+        return 2
+
+    def number_of_constraints(self) -> int:
+        return 0
 
     def evaluate(self, solution: BinarySolution) -> BinarySolution:
         counter_of_ones = 0
         counter_of_zeroes = 0
         for bits in solution.variables[0]:
             if bits:
                 counter_of_ones += 1
@@ -215,69 +229,76 @@
 
         solution.objectives[0] = -1.0 * counter_of_ones
         solution.objectives[1] = -1.0 * counter_of_zeroes
 
         return solution
 
     def create_solution(self) -> BinarySolution:
-        new_solution = BinarySolution(number_of_variables=self.number_of_variables,
-                                      number_of_objectives=self.number_of_objectives)
-        new_solution.variables[0] = \
-            [True if random.randint(0, 1) == 0 else False for _ in range(self.number_of_bits)]
+        new_solution = BinarySolution(
+            number_of_variables=self.number_of_variables(), number_of_objectives=self.number_of_objectives()
+        )
+        new_solution.variables[0] = [True if random.randint(0, 1) == 0 else False for _ in range(self.number_of_bits)]
         return new_solution
 
-    def get_name(self) -> str:
-        return 'OneZeroMax'
+    def name(self) -> str:
+        return "OneZeroMax"
 
 
 class MixedIntegerFloatProblem(Problem):
-    def __init__(self, number_of_integer_variables=10, number_of_float_variables=10, n=100, m=-100, lower_bound=-1000,
-                 upper_bound=1000):
+    def __init__(
+        self,
+        number_of_integer_variables=10,
+        number_of_float_variables=10,
+        n=100,
+        m=-100,
+        lower_bound=-1000,
+        upper_bound=1000,
+    ):
         super(MixedIntegerFloatProblem, self).__init__()
         self.number_of_objectives = 2
         self.number_of_variables = 2
         self.number_of_constraints = 0
 
         self.n = n
         self.m = m
 
         self.float_lower_bound = [lower_bound for _ in range(number_of_float_variables)]
         self.float_upper_bound = [upper_bound for _ in range(number_of_float_variables)]
         self.int_lower_bound = [lower_bound for _ in range(number_of_integer_variables)]
         self.int_upper_bound = [upper_bound for _ in range(number_of_integer_variables)]
 
         self.obj_directions = [self.MINIMIZE]
-        self.obj_labels = ['Ones']
+        self.obj_labels = ["Ones"]
 
     def evaluate(self, solution: CompositeSolution) -> CompositeSolution:
         distance_to_n = sum([abs(self.n - value) for value in solution.variables[0].variables])
         distance_to_m = sum([abs(self.m - value) for value in solution.variables[0].variables])
 
         distance_to_n += sum([abs(self.n - value) for value in solution.variables[1].variables])
         distance_to_m += sum([abs(self.m - value) for value in solution.variables[1].variables])
 
         solution.objectives[0] = distance_to_n
         solution.objectives[1] = distance_to_m
 
         return solution
 
     def create_solution(self) -> CompositeSolution:
-        integer_solution = IntegerSolution(self.int_lower_bound, self.int_upper_bound, self.number_of_objectives,
-                                           self.number_of_constraints)
+        integer_solution = IntegerSolution(
+            self.int_lower_bound, self.int_upper_bound, self.number_of_objectives, self.number_of_constraints
+        )
         float_solution = FloatSolution(
-            self.float_lower_bound,
-            self.float_upper_bound,
-            self.number_of_objectives, self.number_of_constraints)
-
-        float_solution.variables = \
-            [random.uniform(self.float_lower_bound[i] * 1.0, self.float_upper_bound[i] * .01) for i in
-             range(len(self.int_lower_bound))]
-
-        integer_solution.variables = \
-            [random.uniform(self.float_lower_bound[i], self.float_upper_bound[i]) for i in
-             range(len(self.float_lower_bound))]
+            self.float_lower_bound, self.float_upper_bound, self.number_of_objectives, self.number_of_constraints
+        )
+
+        float_solution.variables = [
+            random.uniform(self.float_lower_bound[i] * 1.0, self.float_upper_bound[i] * 1.0)
+            for i in range(len(self.float_lower_bound))
+        ]
+        integer_solution.variables = [
+            random.uniform(self.int_lower_bound[i], self.int_upper_bound[i])
+            for i in range(len(self.int_lower_bound))
+        ]
 
         return CompositeSolution([integer_solution, float_solution])
 
-    def get_name(self) -> str:
+    def name(self) -> str:
         return "Mixed Integer Float Problem"
-
```

### Comparing `jmetalpy-1.5.5/jmetal/problem/multiobjective/zdt.py` & `jmetalpy-1.6.0/jmetal/problem/multiobjective/zdt.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,43 @@
-from math import sqrt, pow, sin, pi, cos
+from math import cos, pi, pow, sin, sqrt, exp
 
 from jmetal.core.problem import FloatProblem
 from jmetal.core.solution import FloatSolution
 
 """
 .. module:: ZDT
    :platform: Unix, Windows
    :synopsis: ZDT problem family of multi-objective problems.
 
 .. moduleauthor:: Antonio J. Nebro <antonio@lcc.uma.es>
 """
 
 
 class ZDT1(FloatProblem):
-    """ Problem ZDT1.
+    """Problem ZDT1.
 
     .. note:: Bi-objective unconstrained problem. The default number of variables is 30.
     .. note:: Continuous problem having a convex Pareto front
     """
 
-    def __init__(self, number_of_variables: int=30):
-        """ :param number_of_variables: Number of decision variables of the problem.
-        """
+    def __init__(self, number_of_variables: int = 30):
+        """:param number_of_variables: Number of decision variables of the problem."""
         super(ZDT1, self).__init__()
-        self.number_of_variables = number_of_variables
-        self.number_of_objectives = 2
-        self.number_of_constraints = 0
 
         self.obj_directions = [self.MINIMIZE, self.MINIMIZE]
-        self.obj_labels = ['x', 'y']
+        self.obj_labels = ["x", "y"]
 
-        self.lower_bound = self.number_of_variables * [0.0]
-        self.upper_bound = self.number_of_variables * [1.0]
+        self.lower_bound = number_of_variables * [0.0]
+        self.upper_bound = number_of_variables * [1.0]
+
+    def number_of_objectives(self) -> int:
+        return len(self.obj_directions)
+
+    def number_of_constraints(self) -> int:
+        return 0
 
     def evaluate(self, solution: FloatSolution) -> FloatSolution:
         g = self.eval_g(solution)
         h = self.eval_h(solution.variables[0], g)
 
         solution.objectives[0] = solution.variables[0]
         solution.objectives[1] = h * g
@@ -48,74 +50,75 @@
         constant = 9.0 / (solution.number_of_variables - 1)
 
         return constant * g + 1.0
 
     def eval_h(self, f: float, g: float) -> float:
         return 1.0 - sqrt(f / g)
 
-    def get_name(self):
-        return 'ZDT1'
+    def name(self):
+        return "ZDT1"
 
 
 class ZDT1Modified(ZDT1):
-    """ Problem ZDT1Modified.
+    """Problem ZDT1Modified.
 
     .. note:: Version including a loop for increasing the computing time of the evaluation functions.
     """
-    def __init__(self, number_of_variables = 30):
+
+    def __init__(self, number_of_variables=30):
         super(ZDT1Modified, self).__init__(number_of_variables)
 
-    def evaluate(self, solution:FloatSolution) -> FloatSolution:
+    def evaluate(self, solution: FloatSolution) -> FloatSolution:
         s: float = 0.0
         for i in range(1000):
             for j in range(10000):
                 s += i * 0.235 / 1.234 + 1.23525 * j
         return super().evaluate(solution)
 
 
 class ZDT2(ZDT1):
-    """ Problem ZDT2.
+    """Problem ZDT2.
 
     .. note:: Bi-objective unconstrained problem. The default number of variables is 30.
     .. note:: Continuous problem having a non-convex Pareto front
     """
 
     def eval_h(self, f: float, g: float) -> float:
         return 1.0 - pow(f / g, 2.0)
 
-    def get_name(self):
-        return 'ZDT2'
+    def name(self):
+        return "ZDT2"
 
 
 class ZDT3(ZDT1):
-    """ Problem ZDT3.
+    """Problem ZDT3.
 
     .. note:: Bi-objective unconstrained problem. The default number of variables is 30.
     .. note:: Continuous problem having a partitioned Pareto front
     """
+
     def eval_h(self, f: float, g: float) -> float:
         return 1.0 - sqrt(f / g) - (f / g) * sin(10.0 * f * pi)
 
-    def get_name(self):
-        return 'ZDT3'
+    def name(self):
+        return "ZDT3"
 
 
 class ZDT4(ZDT1):
-    """ Problem ZDT4.
+    """Problem ZDT4.
 
     .. note:: Bi-objective unconstrained problem. The default number of variables is 10.
     .. note:: Continuous multi-modal problem having a convex Pareto front
     """
 
-    def __init__(self, number_of_variables: int=10):
-        """ :param number_of_variables: Number of decision variables of the problem.
-        """
-        super(ZDT4, self).__init__(number_of_variables=number_of_variables)
-        self.lower_bound = self.number_of_variables * [-5.0]
-        self.upper_bound = self.number_of_variables * [5.0]
+    def __init__(self, number_of_variables: int = 10):
+        """:param number_of_variables: Number of decision variables of the problem."""
+        super(ZDT4, self).__init__()
+        self.lower_bound = number_of_variables * [-5.0]
+        self.upper_bound = number_of_variables * [5.0]
         self.lower_bound[0] = 0.0
         self.upper_bound[0] = 1.0
 
     def eval_g(self, solution: FloatSolution):
         g = 0.0
 
         for i in range(1, solution.number_of_variables):
@@ -124,37 +127,47 @@
         g += 1.0 + 10.0 * (solution.number_of_variables - 1)
 
         return g
 
     def eval_h(self, f: float, g: float) -> float:
         return 1.0 - sqrt(f / g)
 
-    def get_name(self):
-        return 'ZDT4'
+    def name(self):
+        return "ZDT4"
 
 
 class ZDT6(ZDT1):
-    """ Problem ZDT6.
+    """Problem ZDT6.
 
     .. note:: Bi-objective unconstrained problem. The default number of variables is 10.
     .. note:: Continuous problem having a non-convex Pareto front
     """
 
-    def __init__(self, number_of_variables: int=10):
-        """ :param number_of_variables: Number of decision variables of the problem.
-        """
+    def __init__(self, number_of_variables: int = 10):
+        """:param number_of_variables: Number of decision variables of the problem."""
         super(ZDT6, self).__init__(number_of_variables=number_of_variables)
 
+    def evaluate(self, solution: FloatSolution) -> FloatSolution:
+        solution.objectives[0] = (
+            1.0 - exp(-4.0 * solution.variables[0]) * (sin(6.0 * pi * solution.variables[0])) ** 6.0
+        )
+
+        g = self.eval_g(solution)
+        h = self.eval_h(solution.objectives[0], g)
+        solution.objectives[1] = h * g
+
+        return solution
+
     def eval_g(self, solution: FloatSolution):
         g = sum(solution.variables) - solution.variables[0]
         g = g / (solution.number_of_variables - 1)
         g = pow(g, 0.25)
         g = 9.0 * g
         g = 1.0 + g
 
         return g
 
     def eval_h(self, f: float, g: float) -> float:
         return 1.0 - pow(f / g, 2.0)
 
-    def get_name(self):
-        return 'ZDT6'
+    def name(self):
+        return "ZDT6"
```

### Comparing `jmetalpy-1.5.5/jmetal/problem/singleobjective/knapsack.py` & `jmetalpy-1.6.0/jmetal/problem/singleobjective/knapsack.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,32 +11,45 @@
    :synopsis: Single Objective Knapsack problem
 
 .. moduleauthor:: Alejandro Marrero <alu0100825008@ull.edu.es>
 """
 
 
 class Knapsack(BinaryProblem):
-    """ Class representing Knapsack Problem. """
+    """Class representing Knapsack Problem."""
 
-    def __init__(self, number_of_items: int = 50, capacity: float = 1000, weights: list = None,
-                 profits: list = None, from_file: bool = False, filename: str = None):
+    def __init__(
+        self,
+        number_of_items: int = 50,
+        capacity: float = 1000,
+        weights: list = None,
+        profits: list = None,
+        from_file: bool = False,
+        filename: str = None,
+    ):
         super(Knapsack, self).__init__()
 
         if from_file:
             self.__read_from_file(filename)
         else:
             self.capacity = capacity
             self.weights = weights
             self.profits = profits
             self.number_of_bits = number_of_items
 
-        self.number_of_variables = 1
         self.obj_directions = [self.MAXIMIZE]
-        self.number_of_objectives = 1
-        self.number_of_constraints = 1
+
+    def number_of_variables(self) -> int:
+        return 1
+
+    def number_of_objectives(self) -> int:
+        return 1
+
+    def number_of_constraints(self) -> int:
+        return 1
 
     def __read_from_file(self, filename: str):
         """
         This function reads a Knapsack Problem instance from a file.
         It expects the following format:
 
             num_of_items (dimension)
@@ -44,15 +57,15 @@
             num_of_items-tuples of weight-profit
 
         :param filename: File which describes the instance.
         :type filename: str.
         """
 
         if filename is None:
-            raise FileNotFoundError('Filename can not be None')
+            raise FileNotFoundError("Filename can not be None")
 
         with open(filename) as file:
             lines = file.readlines()
             data = [line.split() for line in lines if len(line.split()) >= 1]
 
             self.number_of_bits = int(data[0][0])
             self.capacity = float(data[1][0])
@@ -74,18 +87,17 @@
         if total_weigths > self.capacity:
             total_profits = 0.0
 
         solution.objectives[0] = -1.0 * total_profits
         return solution
 
     def create_solution(self) -> BinarySolution:
-        new_solution = BinarySolution(number_of_variables=self.number_of_variables,
-                                      number_of_objectives=self.number_of_objectives)
+        new_solution = BinarySolution(
+            number_of_variables=self.number_of_variables(), number_of_objectives=self.number_of_objectives()
+        )
 
-        new_solution.variables[0] = \
-            [True if random.randint(0, 1) == 0 else False for _ in range(
-                self.number_of_bits)]
+        new_solution.variables[0] = [True if random.randint(0, 1) == 0 else False for _ in range(self.number_of_bits)]
 
         return new_solution
 
-    def get_name(self):
-        return 'Knapsack'
+    def name(self):
+        return "Knapsack"
```

### Comparing `jmetalpy-1.5.5/jmetal/problem/singleobjective/test/test_knapsack.py` & `jmetalpy-1.6.0/jmetal/problem/singleobjective/test/test_knapsack.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,55 +1,56 @@
 import unittest
 from unittest import mock
 
 from jmetal.problem.singleobjective.knapsack import Knapsack
 
 
 class KnapsackTestCases(unittest.TestCase):
-
     def test_should_constructor_create_a_non_null_object(self) -> None:
         problem = Knapsack()
         self.assertIsNotNone(problem)
 
     def test_should_constructor_create_a_valid_problem_with_default_settings(self) -> None:
         problem = Knapsack()
-        self.assertEqual(1, problem.number_of_variables)
-        self.assertEqual(1, problem.number_of_objectives)
-        self.assertEqual(1, problem.number_of_constraints)
+        self.assertEqual(1, problem.number_of_variables())
+        self.assertEqual(1, problem.number_of_objectives())
+        self.assertEqual(1, problem.number_of_constraints())
         self.assertEqual(50, problem.number_of_bits)
         self.assertEqual(1000, problem.capacity)
         self.assertIsNone(problem.profits)
         self.assertIsNone(problem.weights)
 
     def test_should_constructor_create_a_valid_problem_with_500_bits(self) -> None:
         problem = Knapsack(500)
-        self.assertEqual(1, problem.number_of_variables)
-        self.assertEqual(1, problem.number_of_objectives)
-        self.assertEqual(1, problem.number_of_constraints)
+        self.assertEqual(1, problem.number_of_variables())
+        self.assertEqual(1, problem.number_of_objectives())
+        self.assertEqual(1, problem.number_of_constraints())
         self.assertEqual(500, problem.number_of_bits)
         self.assertEqual(1000, problem.capacity)
         self.assertIsNone(problem.profits)
         self.assertIsNone(problem.weights)
 
     def test_should_create_solution_a_valid_binary_solution(self) -> None:
         problem = Knapsack(256)
         solution = problem.create_solution()
         self.assertEqual(256, len(solution.variables[0]))
 
     def test_should_create_solution_from_file(self) -> None:
-        filename = 'resources/Knapsack_instances/KnapsackInstance_50_0_0.kp'
+        filename = "resources/Knapsack_instances/KnapsackInstance_50_0_0.kp"
 
-        data = "50\n13629\n 865 445\n395 324\n777 626\n912 656\n431 935\n42 210 \n266 990\n989 566\n524 489\n" \
-               "498 454\n415 887\n941 534\n803 267\n850 64 \n311 825\n992 941\n489 562\n367 938\n598 15 \n914 96 \n" \
-               "930 737\n224 861\n517 409\n143 728\n289 845\n144 804\n774 685\n98 641 \n634 2  \n819 627\n257 506\n" \
-               "932 848\n546 889\n723 342\n830 250\n617 748\n924 334\n151 721\n318 892\n102 65 \n748 196\n76 940 \n" \
-               "921 582\n871 228\n701 245\n339 823\n484 991\n574 146\n104 823\n363 557"
-        with mock.patch('jmetal.problem.singleobjective.knapsack.open', new=mock.mock_open(read_data=data)):
+        data = (
+            "50\n13629\n 865 445\n395 324\n777 626\n912 656\n431 935\n42 210 \n266 990\n989 566\n524 489\n"
+            "498 454\n415 887\n941 534\n803 267\n850 64 \n311 825\n992 941\n489 562\n367 938\n598 15 \n914 96 \n"
+            "930 737\n224 861\n517 409\n143 728\n289 845\n144 804\n774 685\n98 641 \n634 2  \n819 627\n257 506\n"
+            "932 848\n546 889\n723 342\n830 250\n617 748\n924 334\n151 721\n318 892\n102 65 \n748 196\n76 940 \n"
+            "921 582\n871 228\n701 245\n339 823\n484 991\n574 146\n104 823\n363 557"
+        )
+        with mock.patch("jmetal.problem.singleobjective.knapsack.open", new=mock.mock_open(read_data=data)):
             problem = Knapsack(from_file=True, filename=filename)
-            self.assertEqual(1, problem.number_of_variables)
-            self.assertEqual(1, problem.number_of_objectives)
-            self.assertEqual(1, problem.number_of_constraints)
+            self.assertEqual(1, problem.number_of_variables())
+            self.assertEqual(1, problem.number_of_objectives())
+            self.assertEqual(1, problem.number_of_constraints())
             self.assertEqual(50, problem.number_of_bits)
 
     def test_should_get_name_return_the_right_name(self):
         problem = Knapsack()
-        self.assertEqual('Knapsack', problem.get_name())
+        self.assertEqual("Knapsack", problem.name())
```

### Comparing `jmetalpy-1.5.5/jmetal/problem/singleobjective/test/test_unconstrained.py` & `jmetalpy-1.6.0/jmetal/problem/singleobjective/test/test_unconstrained.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 import unittest
 
 from jmetal.problem.singleobjective.unconstrained import OneMax, Sphere
 
 
 class OneMaxTestCases(unittest.TestCase):
-
     def test_should_constructor_create_a_non_null_object(self) -> None:
         problem = OneMax()
         self.assertIsNotNone(problem)
 
     def test_should_constructor_create_a_valid_problem_with_default_settings(self) -> None:
         problem = OneMax()
-        self.assertEqual(1, problem.number_of_variables)
-        self.assertEqual(1, problem.number_of_objectives)
-        self.assertEqual(0, problem.number_of_constraints)
+        self.assertEqual(1, problem.number_of_variables())
+        self.assertEqual(1, problem.number_of_objectives())
+        self.assertEqual(0, problem.number_of_constraints())
         self.assertEqual(256, problem.number_of_bits)
 
     def test_should_constructor_create_a_valid_problem_with_512_bits(self) -> None:
         problem = OneMax(512)
-        self.assertEqual(1, problem.number_of_variables)
-        self.assertEqual(1, problem.number_of_objectives)
-        self.assertEqual(0, problem.number_of_constraints)
+        self.assertEqual(1, problem.number_of_variables())
+        self.assertEqual(1, problem.number_of_objectives())
+        self.assertEqual(0, problem.number_of_constraints())
         self.assertEqual(512, problem.number_of_bits)
 
     def test_should_create_solution_a_valid_binary_solution(self) -> None:
         problem = OneMax(256)
         solution = problem.create_solution()
         self.assertEqual(256, len(solution.variables[0]))
 
@@ -33,50 +32,49 @@
         solution = problem.create_solution()
         solution.variables[0] = [False for _ in range(problem.number_of_bits)]
         problem.evaluate(solution)
         self.assertEqual(0.0, solution.objectives[0])
 
     def test_should_get_name_return_the_right_name(self):
         problem = OneMax()
-        self.assertEqual("OneMax", problem.get_name())
+        self.assertEqual("OneMax", problem.name())
 
 
 class SphereTestCases(unittest.TestCase):
-
     def test_should_constructor_create_a_non_null_object(self):
         problem = Sphere(3)
         self.assertIsNotNone(problem)
 
     def test_should_constructor_create_a_valid_problem_with_default_settings(self):
         problem = Sphere()
-        self.assertEqual(10, problem.number_of_variables)
-        self.assertEqual(1, problem.number_of_objectives)
-        self.assertEqual(0, problem.number_of_constraints)
+        self.assertEqual(10, problem.number_of_variables())
+        self.assertEqual(1, problem.number_of_objectives())
+        self.assertEqual(0, problem.number_of_constraints())
 
         self.assertEqual([-5.12 for _ in range(10)], problem.lower_bound)
         self.assertEqual([5.12 for _ in range(10)], problem.upper_bound)
 
     def test_should_constructor_create_a_valid_problem_with_5_variables(self):
         problem = Sphere(5)
-        self.assertEqual(5, problem.number_of_variables)
-        self.assertEqual(1, problem.number_of_objectives)
-        self.assertEqual(0, problem.number_of_constraints)
+        self.assertEqual(5, problem.number_of_variables())
+        self.assertEqual(1, problem.number_of_objectives())
+        self.assertEqual(0, problem.number_of_constraints())
 
         self.assertEqual([-5.12, -5.12, -5.12, -5.12, -5.12], problem.lower_bound)
         self.assertEqual([5.12, 5.12, 5.12, 5.12, 5.12], problem.upper_bound)
 
     def test_should_create_solution_create_a_valid_float_solution(self):
         problem = Sphere(3)
         solution = problem.create_solution()
 
         self.assertEqual(3, solution.number_of_variables)
         self.assertEqual(3, len(solution.variables))
         self.assertEqual(1, solution.number_of_objectives)
         self.assertEqual(1, len(solution.objectives))
-        self.assertEqual(0, problem.number_of_constraints)
+        self.assertEqual(0, problem.number_of_constraints())
 
         self.assertEqual([-5.12, -5.12, -5.12], problem.lower_bound)
         self.assertEqual([5.12, 5.12, 5.12], problem.upper_bound)
 
         self.assertTrue(solution.variables[0] >= -5.12)
         self.assertTrue(solution.variables[0] <= 5.12)
 
@@ -85,22 +83,22 @@
         solution = problem.create_solution()
         problem.evaluate(solution)
 
         self.assertEqual(3, solution.number_of_variables)
         self.assertEqual(3, len(solution.variables))
         self.assertEqual(1, solution.number_of_objectives)
         self.assertEqual(1, len(solution.objectives))
-        self.assertEqual(0, problem.number_of_constraints)
+        self.assertEqual(0, problem.number_of_constraints())
 
         self.assertEqual([-5.12, -5.12, -5.12], problem.lower_bound)
         self.assertEqual([5.12, 5.12, 5.12], problem.upper_bound)
 
         self.assertTrue(solution.variables[0] >= -5.12)
         self.assertTrue(solution.variables[0] <= 5.12)
 
     def test_should_get_name_return_the_right_name(self):
         problem = Sphere()
-        self.assertEqual("Sphere", problem.get_name())
+        self.assertEqual("Sphere", problem.name())
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `jmetalpy-1.5.5/jmetal/problem/singleobjective/tsp.py` & `jmetalpy-1.6.0/jmetal/problem/singleobjective/tsp.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,55 +11,58 @@
    :synopsis: Single Objective Traveling Salesman problem
 
 .. moduleauthor:: Antonio Benítez-Hidalgo <antonio.b@uma.es>
 """
 
 
 class TSP(PermutationProblem):
-    """ Class representing TSP Problem. """
+    """Class representing TSP Problem."""
 
     def __init__(self, instance: str = None):
         super(TSP, self).__init__()
 
-        distance_matrix, number_of_cities = self.__read_from_file(instance)
+        self.distance_matrix, self.number_of_cities = self.__read_from_file(instance)
+        self.obj_directions = [self.MINIMIZE]
 
-        self.distance_matrix = distance_matrix
+    def number_of_variables(self) -> int:
+        return self.number_of_cities
 
-        self.obj_directions = [self.MINIMIZE]
-        self.number_of_variables = number_of_cities
-        self.number_of_objectives = 1
-        self.number_of_constraints = 0
+    def number_of_objectives(self) -> int:
+        return 1
+
+    def number_of_constraints(self) -> int:
+        return 0
 
     def __read_from_file(self, filename: str):
         """
         This function reads a TSP Problem instance from a file.
 
         :param filename: File which describes the instance.
         :type filename: str.
         """
 
         if filename is None:
-            raise FileNotFoundError('Filename can not be None')
+            raise FileNotFoundError("Filename can not be None")
 
         with open(filename) as file:
             lines = file.readlines()
             data = [line.lstrip() for line in lines if line != ""]
 
-            dimension = re.compile(r'[^\d]+')
+            dimension = re.compile(r"[^\d]+")
 
             for item in data:
-                if item.startswith('DIMENSION'):
-                    dimension = int(dimension.sub('', item))
+                if item.startswith("DIMENSION"):
+                    dimension = int(dimension.sub("", item))
                     break
 
             c = [-1.0] * (2 * dimension)
 
             for item in data:
                 if item[0].isdigit():
-                    j, city_a, city_b = [int(x.strip()) for x in item.split(' ')]
+                    j, city_a, city_b = [int(x.strip()) for x in item.split(" ")]
                     c[2 * (j - 1)] = city_a
                     c[2 * (j - 1) + 1] = city_b
 
             matrix = [[-1] * dimension for _ in range(dimension)]
 
             for k in range(dimension):
                 matrix[k][k] = 0
@@ -71,33 +74,30 @@
                     matrix[j][k] = dist
 
             return matrix, dimension
 
     def evaluate(self, solution: PermutationSolution) -> PermutationSolution:
         fitness = 0
 
-        for i in range(self.number_of_variables - 1):
+        for i in range(self.number_of_variables() - 1):
             x = solution.variables[i]
             y = solution.variables[i + 1]
 
             fitness += self.distance_matrix[x][y]
 
         first_city, last_city = solution.variables[0], solution.variables[-1]
         fitness += self.distance_matrix[first_city][last_city]
 
         solution.objectives[0] = fitness
 
         return solution
 
     def create_solution(self) -> PermutationSolution:
-        new_solution = PermutationSolution(number_of_variables=self.number_of_variables,
-                                           number_of_objectives=self.number_of_objectives)
-        new_solution.variables = random.sample(range(self.number_of_variables), k=self.number_of_variables)
+        new_solution = PermutationSolution(
+            number_of_variables=self.number_of_variables(), number_of_objectives=self.number_of_objectives()
+        )
+        new_solution.variables = random.sample(range(self.number_of_variables()), k=self.number_of_variables())
 
         return new_solution
 
-    @property
-    def number_of_cities(self):
-        return self.number_of_variables
-
-    def get_name(self):
-        return 'Symmetric TSP'
+    def name(self):
+        return "Symmetric TSP"
```

### Comparing `jmetalpy-1.5.5/jmetal/problem/singleobjective/unconstrained.py` & `jmetalpy-1.6.0/jmetal/problem/singleobjective/unconstrained.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,126 +10,142 @@
    :synopsis: Unconstrained test problems for single-objective optimization
 
 .. moduleauthor:: Antonio J. Nebro <antonio@lcc.uma.es>, Antonio Benítez-Hidalgo <antonio.b@uma.es>
 """
 
 
 class OneMax(BinaryProblem):
+    """ The implementation of the OneMax problems defines a single binary variable. This variable
+    will contain the bit string representing the solutions.
 
+    """
     def __init__(self, number_of_bits: int = 256):
         super(OneMax, self).__init__()
         self.number_of_bits = number_of_bits
-        self.number_of_objectives = 1
-        self.number_of_variables = 1
-        self.number_of_constraints = 0
 
         self.obj_directions = [self.MINIMIZE]
-        self.obj_labels = ['Ones']
+        self.obj_labels = ["Ones"]
+
+    def number_of_variables(self) -> int:
+        return 1
+
+    def number_of_objectives(self) -> int:
+        return 1
+
+    def number_of_constraints(self) -> int:
+        return 0
 
     def evaluate(self, solution: BinarySolution) -> BinarySolution:
         counter_of_ones = 0
         for bits in solution.variables[0]:
             if bits:
                 counter_of_ones += 1
 
         solution.objectives[0] = -1.0 * counter_of_ones
 
         return solution
 
     def create_solution(self) -> BinarySolution:
         new_solution = BinarySolution(number_of_variables=1, number_of_objectives=1)
-        new_solution.variables[0] = \
-            [True if random.randint(0, 1) == 0 else False for _ in range(self.number_of_bits)]
+        new_solution.variables[0] = [True if random.randint(0, 1) == 0 else False for _ in range(self.number_of_bits)]
         return new_solution
 
-    def get_name(self) -> str:
-        return 'OneMax'
+    def name(self) -> str:
+        return "OneMax"
 
 
 class Sphere(FloatProblem):
-
     def __init__(self, number_of_variables: int = 10):
         super(Sphere, self).__init__()
-        self.number_of_objectives = 1
-        self.number_of_variables = number_of_variables
-        self.number_of_constraints = 0
 
         self.obj_directions = [self.MINIMIZE]
-        self.obj_labels = ['f(x)']
+        self.obj_labels = ["f(x)"]
 
         self.lower_bound = [-5.12 for _ in range(number_of_variables)]
         self.upper_bound = [5.12 for _ in range(number_of_variables)]
 
         FloatSolution.lower_bound = self.lower_bound
         FloatSolution.upper_bound = self.upper_bound
 
+    def number_of_objectives(self) -> int:
+        return 1
+
+    def number_of_constraints(self) -> int:
+        return 0
+
     def evaluate(self, solution: FloatSolution) -> FloatSolution:
         total = 0.0
         for x in solution.variables:
             total += x * x
 
         solution.objectives[0] = total
 
         return solution
 
-    def get_name(self) -> str:
-        return 'Sphere'
+    def name(self) -> str:
+        return "Sphere"
 
 
 class Rastrigin(FloatProblem):
-
     def __init__(self, number_of_variables: int = 10):
         super(Rastrigin, self).__init__()
-        self.number_of_objectives = 1
-        self.number_of_variables = number_of_variables
-        self.number_of_constraints = 0
 
         self.obj_directions = [self.MINIMIZE]
-        self.obj_labels = ['f(x)']
+        self.obj_labels = ["f(x)"]
 
         self.lower_bound = [-5.12 for _ in range(number_of_variables)]
         self.upper_bound = [5.12 for _ in range(number_of_variables)]
 
         FloatSolution.lower_bound = self.lower_bound
         FloatSolution.upper_bound = self.upper_bound
 
+    def number_of_objectives(self) -> int:
+        return 1
+
+    def number_of_constraints(self) -> int:
+        return 0
+
     def evaluate(self, solution: FloatSolution) -> FloatSolution:
         a = 10.0
         result = a * solution.number_of_variables
         x = solution.variables
 
         for i in range(solution.number_of_variables):
             result += x[i] * x[i] - a * math.cos(2 * math.pi * x[i])
 
         solution.objectives[0] = result
 
         return solution
 
-    def get_name(self) -> str:
-        return 'Rastrigin'
+    def name(self) -> str:
+        return "Rastrigin"
 
 
 class SubsetSum(BinaryProblem):
-
     def __init__(self, C: int, W: list):
-        """ The goal is to find a subset S of W whose elements sum is closest to (without exceeding) C.
+        """The goal is to find a subset S of W whose elements sum is closest to (without exceeding) C.
 
         :param C: Large integer.
         :param W: Set of non-negative integers."""
         super(SubsetSum, self).__init__()
         self.C = C
         self.W = W
 
         self.number_of_bits = len(self.W)
-        self.number_of_objectives = 1
-        self.number_of_variables = 1
-        self.number_of_constraints = 0
 
         self.obj_directions = [self.MAXIMIZE]
-        self.obj_labels = ['Sum']
+        self.obj_labels = ["Sum"]
+
+    def number_of_variables(self) -> int:
+        return 1
+    def number_of_objectives(self) -> int:
+        return 1
+
+    def number_of_constraints(self) -> int:
+        return 0
 
     def evaluate(self, solution: BinarySolution) -> BinarySolution:
         total_sum = 0.0
 
         for index, bits in enumerate(solution.variables[0]):
             if bits:
                 total_sum += self.W[index]
@@ -141,16 +157,16 @@
                 total_sum = 0.0
 
         solution.objectives[0] = -1.0 * total_sum
 
         return solution
 
     def create_solution(self) -> BinarySolution:
-        new_solution = BinarySolution(number_of_variables=self.number_of_variables,
-                                      number_of_objectives=self.number_of_objectives)
-        new_solution.variables[0] = \
-            [True if random.randint(0, 1) == 0 else False for _ in range(self.number_of_bits)]
+        new_solution = BinarySolution(
+            number_of_variables=self.number_of_variables(), number_of_objectives=self.number_of_objectives()
+        )
+        new_solution.variables[0] = [True if random.randint(0, 1) == 0 else False for _ in range(self.number_of_bits)]
 
         return new_solution
 
-    def get_name(self) -> str:
-        return 'Subset Sum'
+    def  name(self) -> str:
+        return "Subset Sum"
```

### Comparing `jmetalpy-1.5.5/jmetal/util/aggregative_function.py` & `jmetalpy-1.6.0/jmetal/util/aggregative_function.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,71 @@
 from abc import ABC, abstractmethod
+from math import sqrt
 
 from jmetal.util.point import IdealPoint
 
 """
 .. module:: aggregative_function
    :platform: Unix, Windows
    :synopsis: Implementation of aggregative (scalarizing) functions.
 
 .. moduleauthor:: Antonio J. Nebro <antonio@lcc.uma.es>, Antonio Benítez-Hidalgo <antonio.b@uma.es>
 """
 
 
 class AggregativeFunction(ABC):
-
     @abstractmethod
     def compute(self, vector: [], weight_vector: []) -> float:
         pass
 
     @abstractmethod
     def update(self, vector: []) -> None:
         pass
 
 
 class WeightedSum(AggregativeFunction):
-
     def compute(self, vector: [], weight_vector: []) -> float:
         return sum(map(lambda x, y: x * y, vector, weight_vector))
 
     def update(self, vector: []) -> None:
         pass
 
 
-class Tschebycheff(AggregativeFunction):
+class PenaltyBoundaryIntersection(AggregativeFunction):
+    def __init__(self, dimension: int, theta: float = 5.0):
+        self.ideal_point = IdealPoint(dimension)
+        self.theta = theta
+
+    def compute(self, vector: [], weight_vector: []) -> float:
+        d1 = d2 = nl = 0.0
+
+        for i in range(len(vector)):
+            d1 += (vector[i] - self.ideal_point.point[i]) * weight_vector[i];
+            nl += pow(weight_vector[i], 2.0)
 
+        nl = sqrt(nl)
+        d1 = abs(d1) / nl
+
+        for i in range(len(vector)):
+            d2 += pow((vector[i] - self.ideal_point.point[i]) -
+                           d1 * (weight_vector[i] / nl), 2.0)
+        d2 = sqrt(d2)
+
+        return d1 + self.theta * d2
+
+    def update(self, vector: []) -> None:
+        self.ideal_point.update(vector)
+
+
+class Tschebycheff(AggregativeFunction):
     def __init__(self, dimension: int):
         self.ideal_point = IdealPoint(dimension)
 
     def compute(self, vector: [], weight_vector: []) -> float:
-        max_fun = -1.0e+30
+        max_fun = -1.0e30
 
         for i in range(len(vector)):
             diff = abs(vector[i] - self.ideal_point.point[i])
 
             if weight_vector[i] == 0:
                 feval = 0.0001 * diff
             else:
```

### Comparing `jmetalpy-1.5.5/jmetal/util/archive.py` & `jmetalpy-1.6.0/jmetal/util/archive.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 import copy
 import random
 from abc import ABC, abstractmethod
 from threading import Lock
-from typing import TypeVar, Generic, List
+from typing import Generic, List, TypeVar
 
-from jmetal.util.comparator import Comparator, DominanceComparator, SolutionAttributeComparator
-from jmetal.util.density_estimator import DensityEstimator, CrowdingDistance
+from jmetal.util.comparator import (
+    Comparator,
+    DominanceComparator,
+    SolutionAttributeComparator, )
+from jmetal.util.density_estimator import CrowdingDistance, DensityEstimator
 
-S = TypeVar('S')
+S = TypeVar("S")
 
 """
 .. module:: archive
    :platform: Unix, Windows
    :synopsis: Archive implementation.
 
 .. moduleauthor:: Antonio J. Nebro <antonio@lcc.uma.es>
 """
 
 
 class Archive(Generic[S], ABC):
-
     def __init__(self):
         self.solution_list: List[S] = []
 
     @abstractmethod
     def add(self, solution: S) -> bool:
         pass
 
@@ -34,24 +36,21 @@
         return len(self.solution_list)
 
     def get_name(self) -> str:
         return self.__class__.__name__
 
 
 class BoundedArchive(Archive[S]):
-
-    def __init__(self,
-                 maximum_size: int,
-                 comparator: Comparator[S] = None,
-                 density_estimator: DensityEstimator = None):
+    def __init__(self, maximum_size: int, comparator: Comparator[S] = None, density_estimator: DensityEstimator = None,
+                 dominance_comparator: Comparator[S] = DominanceComparator()):
         super(BoundedArchive, self).__init__()
         self.maximum_size = maximum_size
         self.comparator = comparator
         self.density_estimator = density_estimator
-        self.non_dominated_solution_archive = NonDominatedSolutionsArchive()
+        self.non_dominated_solution_archive = NonDominatedSolutionsArchive(dominance_comparator=dominance_comparator)
         self.solution_list = self.non_dominated_solution_archive.solution_list
 
     def compute_density_estimator(self):
         self.density_estimator.compute_density_estimator(self.solution_list)
 
     def add(self, solution: S) -> bool:
         success = self.non_dominated_solution_archive.add(solution)
@@ -63,30 +62,29 @@
                 self.solution_list.pop(index_to_remove)
 
         return success
 
     def __find_worst_solution(self, solution_list: List[S]) -> S:
         if solution_list is None:
             raise Exception("The solution list is None")
-        elif len(solution_list) is 0:
+        elif len(solution_list) == 0:
             raise Exception("The solution list is empty")
 
         worst_solution = solution_list[0]
         index_to_remove = 0
 
         for solution_index, solution in enumerate(solution_list[1:]):
             if self.comparator.compare(worst_solution, solution) < 0:
                 worst_solution = solution
                 index_to_remove = solution_index + 1
 
         return worst_solution, index_to_remove
 
 
 class NonDominatedSolutionsArchive(Archive[S]):
-
     def __init__(self, dominance_comparator: Comparator = DominanceComparator()):
         super(NonDominatedSolutionsArchive, self).__init__()
         self.comparator = dominance_comparator
 
     def add(self, solution: S) -> bool:
         is_dominated = False
         is_contained = False
@@ -115,30 +113,31 @@
             self.solution_list.append(solution)
             return True
 
         return False
 
 
 class CrowdingDistanceArchive(BoundedArchive[S]):
-
-    def __init__(self,
-                 maximum_size: int):
+    def __init__(self, maximum_size: int, dominance_comparator=DominanceComparator()):
         super(CrowdingDistanceArchive, self).__init__(
             maximum_size=maximum_size,
             comparator=SolutionAttributeComparator("crowding_distance", lowest_is_best=False),
-            density_estimator=CrowdingDistance())
+            dominance_comparator=dominance_comparator,
+            density_estimator=CrowdingDistance(),
+        )
 
 
 class ArchiveWithReferencePoint(BoundedArchive[S]):
-
-    def __init__(self,
-                 maximum_size: int,
-                 reference_point: List[float],
-                 comparator: Comparator[S],
-                 density_estimator: DensityEstimator):
+    def __init__(
+            self,
+            maximum_size: int,
+            reference_point: List[float],
+            comparator: Comparator[S],
+            density_estimator: DensityEstimator,
+    ):
         super(ArchiveWithReferencePoint, self).__init__(maximum_size, comparator, density_estimator)
         self.__reference_point = reference_point
         self.__comparator = comparator
         self.__density_estimator = density_estimator
         self.lock = Lock()
 
     def add(self, solution: S) -> bool:
@@ -168,17 +167,17 @@
                 self.compute_density_estimator()
 
         return result
 
     def filter(self):
         # In case of having at least a solution which is non-dominated with the reference point, filter it
         if len(self.solution_list) > 1:
-            self.solution_list[:] = \
-                [sol for sol in self.solution_list
-                 if self.__dominance_test(sol.objectives, self.__reference_point) != 0]
+            self.solution_list[:] = [
+                sol for sol in self.solution_list if self.__dominance_test(sol.objectives, self.__reference_point) != 0
+            ]
 
     def update_reference_point(self, new_reference_point) -> None:
         with self.lock:
             self.__reference_point = new_reference_point
 
             first_solution = copy.deepcopy(self.solution_list[0])
             self.filter()
@@ -208,16 +207,14 @@
         else:
             result = 0
 
         return result
 
 
 class CrowdingDistanceArchiveWithReferencePoint(ArchiveWithReferencePoint[S]):
-
-    def __init__(self,
-                 maximum_size: int,
-                 reference_point: List[float]):
+    def __init__(self, maximum_size: int, reference_point: List[float]):
         super(CrowdingDistanceArchiveWithReferencePoint, self).__init__(
             maximum_size=maximum_size,
             reference_point=reference_point,
             comparator=SolutionAttributeComparator("crowding_distance", lowest_is_best=False),
-            density_estimator=CrowdingDistance())
+            density_estimator=CrowdingDistance(),
+        )
```

### Comparing `jmetalpy-1.5.5/jmetal/util/ckecking.py` & `jmetalpy-1.6.0/jmetal/util/ckecking.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,22 +17,29 @@
 #    def __init__(self, message):
 #        super(InvalidConditionException, self).__init__(message)
 
 
 class InvalidProbabilityValueException(RuntimeError):
     def __init__(self, value: float):
         super(InvalidProbabilityValueException, self).__init__(
-            "The parameter " + str(value) + " is not a valid probability value")
+            "The parameter " + str(value) + " is not a valid probability value"
+        )
 
 
 class ValueOutOfRangeException(RuntimeError):
     def __init__(self, value: float, lowest_value: float, highest_value: float):
         super(ValueOutOfRangeException, self).__init__(
-            "The parameter " + str(value) + " is not in the range (" + str(lowest_value) + ", " + str(
-                highest_value) + ")")
+            "The parameter "
+            + str(value)
+            + " is not in the range ("
+            + str(lowest_value)
+            + ", "
+            + str(highest_value)
+            + ")"
+        )
 
 
 class Check:
     @staticmethod
     def is_not_none(obj):
         if obj is None:
             raise NoneParameterException()
```

### Comparing `jmetalpy-1.5.5/jmetal/util/constraint_handling.py` & `jmetalpy-1.6.0/jmetal/util/constraint_handling.py`

 * *Files identical despite different names*

### Comparing `jmetalpy-1.5.5/jmetal/util/density_estimator.py` & `jmetalpy-1.6.0/jmetal/util/density_estimator.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,32 @@
-import logging
 from abc import ABC, abstractmethod
 from functools import cmp_to_key
-from typing import TypeVar, List
+from typing import List, TypeVar
 
 import numpy
 from scipy.spatial.distance import euclidean
 
-from jmetal.util.comparator import SolutionAttributeComparator, Comparator
+from jmetal.logger import get_logger
+from jmetal.util.comparator import Comparator, SolutionAttributeComparator
 
-LOGGER = logging.getLogger('jmetal')
+logger = get_logger(__name__)
 
-S = TypeVar('S')
+S = TypeVar("S")
 
 """
 .. module:: density_estimator
    :platform: Unix, Windows
    :synopsis: Module including the implementation of density estimators.
 
 .. moduleauthor:: Antonio J. Nebro <ajnebro@uma.es>
 """
 
 
 class DensityEstimator(List[S], ABC):
-    """This is the interface of any density estimator algorithm.
-    """
+    """This is the interface of any density estimator algorithm."""
 
     @abstractmethod
     def compute_density_estimator(self, solutions: List[S]) -> float:
         pass
 
     @abstractmethod
     def sort(self, solutions: List[S]) -> List[S]:
@@ -35,75 +34,74 @@
 
     @classmethod
     def get_comparator(cls) -> Comparator:
         pass
 
 
 class CrowdingDistance(DensityEstimator[List[S]]):
-    """This class implements a DensityEstimator based on the crowding distance of algorithm NSGA-II.
-    """
+    """This class implements a DensityEstimator based on the crowding distance of algorithm NSGA-II."""
 
     def compute_density_estimator(self, front: List[S]):
         """This function performs the computation of the crowding density estimation over the solution list.
 
         .. note::
            This method assign the distance in the inner elements of the solution list.
 
         :param front: The list of solutions.
         """
         size = len(front)
 
-        if size is 0:
+        if size == 0:
             return
-        elif size is 1:
-            front[0].attributes['crowding_distance'] = float("inf")
+        elif size == 1:
+            front[0].attributes["crowding_distance"] = float("inf")
             return
-        elif size is 2:
-            front[0].attributes['crowding_distance'] = float("inf")
-            front[1].attributes['crowding_distance'] = float("inf")
+        elif size == 2:
+            front[0].attributes["crowding_distance"] = float("inf")
+            front[1].attributes["crowding_distance"] = float("inf")
             return
 
         for i in range(len(front)):
-            front[i].attributes['crowding_distance'] = 0.0
+            front[i].attributes["crowding_distance"] = 0.0
 
         number_of_objectives = front[0].number_of_objectives
 
         for i in range(number_of_objectives):
             # Sort the population by Obj n
             front = sorted(front, key=lambda x: x.objectives[i])
             objective_minn = front[0].objectives[i]
             objective_maxn = front[len(front) - 1].objectives[i]
 
             # Set de crowding distance
-            front[0].attributes['crowding_distance'] = float('inf')
-            front[size - 1].attributes['crowding_distance'] = float('inf')
+            front[0].attributes["crowding_distance"] = float("inf")
+            front[size - 1].attributes["crowding_distance"] = float("inf")
 
             for j in range(1, size - 1):
                 distance = front[j + 1].objectives[i] - front[j - 1].objectives[i]
 
                 # Check if minimum and maximum are the same (in which case do nothing)
                 if objective_maxn - objective_minn == 0:
-                    pass;  # LOGGER.warning('Minimum and maximum are the same!')
+                    pass
+                    # logger.warning('Minimum and maximum are the same!')
                 else:
                     distance = distance / (objective_maxn - objective_minn)
 
-                distance += front[j].attributes['crowding_distance']
-                front[j].attributes['crowding_distance'] = distance
+                distance += front[j].attributes["crowding_distance"]
+                front[j].attributes["crowding_distance"] = distance
 
     def sort(self, solutions: List[S]) -> List[S]:
         solutions.sort(key=cmp_to_key(self.get_comparator().compare))
 
     @classmethod
     def get_comparator(cls) -> Comparator:
         return SolutionAttributeComparator("crowding_distance", lowest_is_best=False)
 
 
 class KNearestNeighborDensityEstimator(DensityEstimator[List[S]]):
-    """This class implements a density estimator based on the distance to the k-th nearest solution.
-    """
+    """This class implements a density estimator based on the distance to the k-th nearest solution."""
 
     def __init__(self, k: int = 1):
         super().__init__()
         self.k = k
         self.distance_matrix = []
 
     def compute_density_estimator(self, solutions: List[S]):
@@ -115,23 +113,24 @@
         for i in range(solutions_size):
             points.append(solutions[i].objectives)
 
         # Compute distance matrix
         self.distance_matrix = numpy.zeros(shape=(solutions_size, solutions_size))
         for i in range(solutions_size):
             for j in range(solutions_size):
-                self.distance_matrix[i, j] = self.distance_matrix[j, i] = euclidean(solutions[i].objectives,
-                                                                                    solutions[j].objectives)
+                self.distance_matrix[i, j] = self.distance_matrix[j, i] = euclidean(
+                    solutions[i].objectives, solutions[j].objectives
+                )
         # Gets the k-nearest distance of all the solutions
         for i in range(solutions_size):
             distances = []
             for j in range(solutions_size):
                 distances.append(self.distance_matrix[i, j])
             distances.sort()
-            solutions[i].attributes['knn_density'] = distances[self.k]
+            solutions[i].attributes["knn_density"] = distances[self.k]
 
     def sort(self, solutions: List[S]) -> List[S]:
         def compare(solution1, solution2):
             distances1 = solution1.attributes["distances_"]
             distances2 = solution2.attributes["distances_"]
 
             tmp_k = self.k
```

### Comparing `jmetalpy-1.5.5/jmetal/util/distance.py` & `jmetalpy-1.6.0/jmetal/util/distance.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,38 +9,41 @@
    :synopsis: implementation of distances between entities
 
 .. moduleauthor:: Antonio J. Nebro <antonio@lcc.uma.es>
 """
 
 
 class Distance(ABC):
-
     @abstractmethod
     def get_distance(self, element1, element2) -> float:
         pass
 
 
 class EuclideanDistance(Distance):
-
     def get_distance(self, list1: [], list2: []):
         return distance.euclidean(list1, list2)
 
 
 class CosineDistance(Distance):
-
     def __init__(self, reference_point: []):
         self.reference_point = reference_point
 
     def get_distance(self, list1: [], list2: []):
-        total = sum(numpy.multiply([(x - r) for x, r in zip(list1, self.reference_point)],
-                                   [(y - r) for y, r in zip(list2, self.reference_point)]))
-
-        a = distance.cosine([x - y for x, y in zip(list1, self.reference_point)],
-                            [x - y for x, y in zip(list2, self.reference_point)])
-
-        b = total / (self.__sum_of_distances_to_reference_point(list1) *
-                     self.__sum_of_distances_to_reference_point(list2))
+        total = sum(
+            numpy.multiply(
+                [(x - r) for x, r in zip(list1, self.reference_point)],
+                [(y - r) for y, r in zip(list2, self.reference_point)],
+            )
+        )
+
+        a = distance.cosine(
+            [x - y for x, y in zip(list1, self.reference_point)], [x - y for x, y in zip(list2, self.reference_point)]
+        )
+
+        b = total / (
+            self.__sum_of_distances_to_reference_point(list1) * self.__sum_of_distances_to_reference_point(list2)
+        )
 
         return b
 
     def __sum_of_distances_to_reference_point(self, l: []):
         return sum([pow(x - y, 2.0) for x, y in zip(l, self.reference_point)])
```

### Comparing `jmetalpy-1.5.5/jmetal/util/evaluator.py` & `jmetalpy-1.6.0/jmetal/util/evaluator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,49 +1,46 @@
 import functools
 from abc import ABC, abstractmethod
-from multiprocessing.pool import ThreadPool, Pool
-from typing import TypeVar, List, Generic
+from multiprocessing.pool import Pool, ThreadPool
+from typing import Generic, List, TypeVar
 
 try:
     import dask
 except ImportError:
     pass
 
 try:
     from pyspark import SparkConf, SparkContext
 except ImportError:
     pass
 
 from jmetal.core.problem import Problem
 
-S = TypeVar('S')
+S = TypeVar("S")
 
 
 class Evaluator(Generic[S], ABC):
-
     @abstractmethod
     def evaluate(self, solution_list: List[S], problem: Problem) -> List[S]:
         pass
 
     @staticmethod
     def evaluate_solution(solution: S, problem: Problem) -> None:
         problem.evaluate(solution)
 
 
 class SequentialEvaluator(Evaluator[S]):
-
     def evaluate(self, solution_list: List[S], problem: Problem) -> List[S]:
         for solution in solution_list:
             Evaluator.evaluate_solution(solution, problem)
 
         return solution_list
 
 
 class MapEvaluator(Evaluator[S]):
-
     def __init__(self, processes: int = None):
         self.pool = ThreadPool(processes)
 
     def evaluate(self, solution_list: List[S], problem: Problem) -> List[S]:
         self.pool.map(lambda solution: Evaluator.evaluate_solution(solution, problem), solution_list)
 
         return solution_list
@@ -65,26 +62,26 @@
 
         logger = self.spark_context._jvm.org.apache.log4j
         logger.LogManager.getLogger("org").setLevel(logger.Level.WARN)
 
     def evaluate(self, solution_list: List[S], problem: Problem) -> List[S]:
         solutions_to_evaluate = self.spark_context.parallelize(solution_list)
 
-        return solutions_to_evaluate \
-            .map(lambda s: problem.evaluate(s)) \
-            .collect()
+        return solutions_to_evaluate.map(lambda s: problem.evaluate(s)).collect()
 
 
 def evaluate_solution(solution, problem):
     Evaluator[S].evaluate_solution(solution, problem)
     return solution
 
 
 class DaskEvaluator(Evaluator[S]):
-    def __init__(self, scheduler='processes'):
+    def __init__(self, scheduler="processes"):
         self.scheduler = scheduler
 
     def evaluate(self, solution_list: List[S], problem: Problem) -> List[S]:
         with dask.config.set(scheduler=self.scheduler):
-            return list(dask.compute(*[
-                dask.delayed(evaluate_solution)(solution=solution, problem=problem) for solution in solution_list
-            ]))
+            return list(
+                dask.compute(
+                    *[dask.delayed(evaluate_solution)(solution=solution, problem=problem) for solution in solution_list]
+                )
+            )
```

### Comparing `jmetalpy-1.5.5/jmetal/util/generator.py` & `jmetalpy-1.6.0/jmetal/util/generator.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,40 @@
 import copy
 from abc import ABC, abstractmethod
-from typing import TypeVar, Generic, List
+from typing import Generic, List, TypeVar
 
 from jmetal.core.problem import Problem
 from jmetal.core.solution import Solution
 
-R = TypeVar('R')
+R = TypeVar("R")
 
 """
 .. module:: generator
    :platform: Unix, Windows
    :synopsis: Population generators implementation.
 
 .. moduleauthor:: Antonio Benítez-Hidalgo <antonio.b@uma.es>
 """
 
 
 class Generator(Generic[R], ABC):
-
     @abstractmethod
     def new(self, problem: Problem) -> R:
         pass
 
 
 class RandomGenerator(Generator):
-
     def new(self, problem: Problem):
         return problem.create_solution()
 
 
 class InjectorGenerator(Generator):
-
     def __init__(self, solutions: List[Solution]):
         super(InjectorGenerator, self).__init__()
-        self.population = []
-
-        for solution in solutions:
-            self.population.append(copy.deepcopy(solution))
+        self.population = copy.deepcopy(solutions)
 
     def new(self, problem: Problem):
         if len(self.population) > 0:
             # If we have more solutions to inject, return one from the list
             return self.population.pop()
         else:
             # Otherwise generate a new solution
```

### Comparing `jmetalpy-1.5.5/jmetal/util/neighborhood.py` & `jmetalpy-1.6.0/jmetal/util/neighborhood.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from abc import ABC, abstractmethod
 from pathlib import Path
-from typing import TypeVar, Generic, List
+from typing import Generic, List, TypeVar
 
 import numpy
 
 from jmetal.core.solution import Solution
 from jmetal.util.ckecking import Check
 
 """
@@ -12,93 +12,95 @@
    :platform: Unix, Windows
    :synopsis: implementation of neighborhoods in the context of list of solutions. The goal is,
    given the index of an element of the list, to find its neighbour solutions according to a criterion.
 
 .. moduleauthor:: Antonio J. Nebro <antonio@lcc.uma.es>
 """
 
-S = TypeVar('S')
+S = TypeVar("S")
 
 
 class Neighborhood(Generic[S], ABC):
-
     @abstractmethod
     def get_neighbors(self, index: int, solution_list: List[S]) -> List[S]:
         pass
 
 
 class WeightNeighborhood(Neighborhood[Solution], ABC):
-
-    def __init__(self,
-                 number_of_weight_vectors: int,
-                 neighborhood_size: int,
-                 weight_vector_size: int = 2,
-                 weights_path: str = None):
+    def __init__(
+        self,
+        number_of_weight_vectors: int,
+        neighborhood_size: int,
+        weight_vector_size: int = 2,
+        weights_path: str = None,
+    ):
         self.number_of_weight_vectors = number_of_weight_vectors
         self.neighborhood_size = neighborhood_size
         self.weight_vector_size = weight_vector_size
         self.weights_path = weights_path
 
         self.neighborhood = numpy.zeros((number_of_weight_vectors, neighborhood_size), dtype=int)
         self.weight_vectors = numpy.zeros((number_of_weight_vectors, weight_vector_size))
 
 
 class WeightVectorNeighborhood(WeightNeighborhood):
-
-    def __init__(self,
-                 number_of_weight_vectors: int,
-                 neighborhood_size: int,
-                 weight_vector_size: int = 2,
-                 weights_path: str = None):
-        super(WeightVectorNeighborhood, self).__init__(number_of_weight_vectors, neighborhood_size, weight_vector_size,
-                                                       weights_path)
+    def __init__(
+        self,
+        number_of_weight_vectors: int,
+        neighborhood_size: int,
+        weight_vector_size: int = 2,
+        weights_path: str = None,
+    ):
+        super(WeightVectorNeighborhood, self).__init__(
+            number_of_weight_vectors, neighborhood_size, weight_vector_size, weights_path
+        )
         self.__initialize_uniform_weight(weight_vector_size, number_of_weight_vectors)
         self.__initialize_neighborhood()
 
     def __initialize_uniform_weight(self, weight_vector_size: int, number_of_weight_vectors: int) -> None:
-        """ Precomputed weights from
+        """Precomputed weights from
 
         * Zhang, Multiobjective Optimization Problems With Complicated Pareto Sets, MOEA/D and NSGA-II
 
         Downloaded from:
 
         * http://dces.essex.ac.uk/staff/qzhang/MOEAcompetition/CEC09final/code/ZhangMOEADcode/moead030510.rar
         """
         if weight_vector_size == 2:
             for i in range(0, number_of_weight_vectors):
                 v = 1.0 * i / (number_of_weight_vectors - 1)
                 self.weight_vectors[i, 0] = v
                 self.weight_vectors[i, 1] = 1 - v
         else:
-            file_name = 'W{}D_{}.dat'.format(weight_vector_size, number_of_weight_vectors)
-            file_path = self.weights_path + '/' + file_name
+            file_name = "W{}D_{}.dat".format(weight_vector_size, number_of_weight_vectors)
+            file_path = self.weights_path + "/" + file_name
 
             if Path(file_path).is_file():
                 with open(file_path) as file:
                     for index, line in enumerate(file):
                         vector = [float(x) for x in line.split()]
                         self.weight_vectors[index][:] = vector
             else:
-                raise FileNotFoundError('Failed to initialize weights: {} not found'.format(file_path))
+                raise FileNotFoundError("Failed to initialize weights: {} not found".format(file_path))
 
     def __initialize_neighborhood(self) -> None:
         distance = numpy.zeros((len(self.weight_vectors), len(self.weight_vectors)))
 
         for i in range(len(self.weight_vectors)):
             for j in range(len(self.weight_vectors)):
                 distance[i][j] = numpy.linalg.norm(self.weight_vectors[i] - self.weight_vectors[j])
 
             indexes = numpy.argsort(distance[i, :])
-            self.neighborhood[i, :] = indexes[0:self.neighborhood_size]
+            self.neighborhood[i, :] = indexes[0 : self.neighborhood_size]
 
     def get_neighbors(self, index: int, solution_list: List[Solution]) -> List[Solution]:
         neighbors_indexes = self.neighborhood[index]
 
         if any(i > len(solution_list) for i in neighbors_indexes):
-            raise IndexError('Neighbor index out of range')
+            raise IndexError("Neighbor index out of range")
 
         return [solution_list[i] for i in neighbors_indexes]
 
     def get_neighborhood(self):
         return self.neighborhood
 
 
@@ -111,15 +113,15 @@
         self.rows = rows
         self.columns = columns
         self.neighborhood = neighborhood
         self.mesh = None
         self.__create_mesh()
 
     def __create_mesh(self):
-        """ Example:
+        """Example:
         if rows = 5, and columns=3, we need to fill the mesh as follows
         ----------
         |00-01-02|
         |03-04-05|
         |06-07-08|
         |09-10-11|
         |12-13-14|
@@ -190,31 +192,31 @@
         Check.that(len(solution_list) != 0, "The list of solutions is empty")
 
         return self.__find_neighbors(solution_list, index, self.neighborhood)
 
 
 class C9(TwoDimensionalMesh):
     """
-    Class defining an C9 neighborhood of a solution belonging to a list of solutions which is
-    structured as a bi-dimensional mesh. The neighbors are those solutions that are in 1-hop distance
+     Class defining an C9 neighborhood of a solution belonging to a list of solutions which is
+     structured as a bi-dimensional mesh. The neighbors are those solutions that are in 1-hop distance
 
-   Shape:
-           * * *
-           * o *
-           * * *
-
-   Topology:
-            north      = {-1,  0}
-            south      = { 1 , 0}
-            east       = { 0 , 1}
-            west       = { 0 ,-1}
-            north_east = {-1,  1}
-            north_west = {-1, -1}
-            south_east = { 1 , 1}
-            south_west = { 1 ,-1}
+    Shape:
+            * * *
+            * o *
+            * * *
+
+    Topology:
+             north      = {-1,  0}
+             south      = { 1 , 0}
+             east       = { 0 , 1}
+             west       = { 0 ,-1}
+             north_east = {-1,  1}
+             north_west = {-1, -1}
+             south_east = { 1 , 1}
+             south_west = { 1 ,-1}
     """
 
     def __init__(self, rows: int, columns: int):
         super(C9, self).__init__(rows, columns, [[-1, 0], [1, 0], [0, 1], [0, -1], [-1, 1], [-1, -1], [1, 1], [1, -1]])
 
 
 class L5(TwoDimensionalMesh):
```

### Comparing `jmetalpy-1.5.5/jmetal/util/observable.py` & `jmetalpy-1.6.0/jmetal/util/observable.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 import logging
 import threading
 import time
 
 from jmetal.core.observer import Observable, Observer
 
-LOGGER = logging.getLogger('jmetal')
+LOGGER = logging.getLogger("jmetal")
 
 """
 .. module:: observable
    :platform: Unix, Windows
    :synopsis: Implementation of observable entities (using delegation)
 .. moduleauthor:: Antonio J. Nebro <antonio@lcc.uma.es>
 """
 
 
 class DefaultObservable(Observable):
-
     def __init__(self):
         self.observers = []
 
     def register(self, observer: Observer):
         if observer not in self.observers:
             self.observers.append(observer)
```

### Comparing `jmetalpy-1.5.5/jmetal/util/observer.py` & `jmetalpy-1.6.0/jmetal/util/observer.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,220 +1,211 @@
 import logging
 import os
 from pathlib import Path
 from typing import List, TypeVar
 
+import numpy as np
 from tqdm import tqdm
 
 from jmetal.core.observer import Observer
 from jmetal.core.problem import DynamicProblem
 from jmetal.core.quality_indicator import InvertedGenerationalDistance
-from jmetal.lab.visualization import StreamingPlot, Plot
+from jmetal.lab.visualization import Plot, StreamingPlot
 from jmetal.util.solution import print_function_values_to_file
 
-S = TypeVar('S')
+S = TypeVar("S")
 
-LOGGER = logging.getLogger('jmetal')
+LOGGER = logging.getLogger("jmetal")
 
 """
 .. module:: observer
    :platform: Unix, Windows
    :synopsis: Implementation of algorithm's observers.
 
 .. moduleauthor:: Antonio J. Nebro <antonio@lcc.uma.es>
 """
 
 
 class ProgressBarObserver(Observer):
-
     def __init__(self, max: int) -> None:
-        """ Show a smart progress meter with the number of evaluations and computing time.
+        """Show a smart progress meter with the number of evaluations and computing time.
 
         :param max: Number of expected iterations.
         """
         self.progress_bar = None
         self.progress = 0
         self._max = max
 
     def update(self, *args, **kwargs):
         if not self.progress_bar:
-            self.progress_bar = tqdm(total=self._max, ascii=True, desc='Progress')
+            self.progress_bar = tqdm(total=self._max, ascii=True, desc="Progress")
 
-        evaluations = kwargs['EVALUATIONS']
+        evaluations = kwargs["EVALUATIONS"]
 
         self.progress_bar.update(evaluations - self.progress)
         self.progress = evaluations
 
         if self.progress >= self._max:
             self.progress_bar.close()
 
 
 class BasicObserver(Observer):
+    def __init__(self, frequency: int = 1) -> None:
+        """Show the number of evaluations, the best fitness and the computing time.
+        :param frequency: Display frequency."""
 
-    def __init__(self, frequency: float = 1.0) -> None:
-        """ Show the number of evaluations, best fitness and computing time.
-
-        :param frequency: Display frequency. """
         self.display_frequency = frequency
 
     def update(self, *args, **kwargs):
-        computing_time = kwargs['COMPUTING_TIME']
-        evaluations = kwargs['EVALUATIONS']
-        solutions = kwargs['SOLUTIONS']
+        computing_time = kwargs["COMPUTING_TIME"]
+        evaluations = kwargs["EVALUATIONS"]
+        solutions = kwargs["SOLUTIONS"]
 
         if (evaluations % self.display_frequency) == 0 and solutions:
             if type(solutions) == list:
                 fitness = solutions[0].objectives
             else:
                 fitness = solutions.objectives
 
             LOGGER.info(
-                'Evaluations: {} \n Best fitness: {} \n Computing time: {}'.format(
-                    evaluations, fitness, computing_time
-                )
+                "Evaluations: {} \n Best fitness: {} \n Computing time: {}".format(evaluations, fitness, computing_time)
             )
 
 
 class PrintObjectivesObserver(Observer):
+    def __init__(self, frequency: int = 1) -> None:
+        """Show the number of evaluations, best fitness and computing time.
 
-    def __init__(self, frequency: float = 1.0) -> None:
-        """ Show the number of evaluations, best fitness and computing time.
-
-        :param frequency: Display frequency. """
+        :param frequency: Display frequency."""
         self.display_frequency = frequency
 
     def update(self, *args, **kwargs):
-        evaluations = kwargs['EVALUATIONS']
-        solutions = kwargs['SOLUTIONS']
+        evaluations = kwargs["EVALUATIONS"]
+        solutions = kwargs["SOLUTIONS"]
 
         if (evaluations % self.display_frequency) == 0 and solutions:
             if type(solutions) == list:
                 fitness = solutions[0].objectives
             else:
                 fitness = solutions.objectives
 
-            LOGGER.info(
-                'Evaluations: {}. fitness: {}'.format(
-                    evaluations, fitness
-                )
-            )
+            LOGGER.info("Evaluations: {}. fitness: {}".format(evaluations, fitness))
 
 
 class WriteFrontToFileObserver(Observer):
-
     def __init__(self, output_directory: str) -> None:
-        """ Write function values of the front into files.
+        """Write function values of the front into files.
 
-        :param output_directory: Output directory. Each front will be saved on a file `FUN.x`. """
+        :param output_directory: Output directory. Each front will be saved on a file `FUN.x`."""
         self.counter = 0
         self.directory = output_directory
 
         if Path(self.directory).is_dir():
-            LOGGER.warning('Directory {} exists. Removing contents.'.format(self.directory))
+            LOGGER.warning("Directory {} exists. Removing contents.".format(self.directory))
             for file in os.listdir(self.directory):
-                os.remove('{0}/{1}'.format(self.directory, file))
+                os.remove("{0}/{1}".format(self.directory, file))
         else:
-            LOGGER.warning('Directory {} does not exist. Creating it.'.format(self.directory))
+            LOGGER.warning("Directory {} does not exist. Creating it.".format(self.directory))
             Path(self.directory).mkdir(parents=True)
 
     def update(self, *args, **kwargs):
-        problem = kwargs['PROBLEM']
-        solutions = kwargs['SOLUTIONS']
+        problem = kwargs["PROBLEM"]
+        solutions = kwargs["SOLUTIONS"]
 
         if solutions:
             if isinstance(problem, DynamicProblem):
-                termination_criterion_is_met = kwargs.get('TERMINATION_CRITERIA_IS_MET', None)
+                termination_criterion_is_met = kwargs.get("TERMINATION_CRITERIA_IS_MET", None)
 
                 if termination_criterion_is_met:
-                    print_function_values_to_file(solutions, '{}/FUN.{}'.format(self.directory, self.counter))
+                    print_function_values_to_file(solutions, "{}/FUN.{}".format(self.directory, self.counter))
                     self.counter += 1
             else:
-                print_function_values_to_file(solutions, '{}/FUN.{}'.format(self.directory, self.counter))
+                print_function_values_to_file(solutions, "{}/FUN.{}".format(self.directory, self.counter))
                 self.counter += 1
 
 
 class PlotFrontToFileObserver(Observer):
-
     def __init__(self, output_directory: str, step: int = 100, **kwargs) -> None:
-        """ Plot and save Pareto front approximations into files.
+        """Plot and save Pareto front approximations into files.
 
         :param output_directory: Output directory.
         """
         self.directory = output_directory
-        self.plot_front = Plot(title='Pareto front approximation', **kwargs)
+        self.plot_front = Plot(title="Pareto front approximation", **kwargs)
         self.last_front = []
         self.fronts = []
         self.counter = 0
         self.step = step
 
         if Path(self.directory).is_dir():
-            LOGGER.warning('Directory {} exists. Removing contents.'.format(self.directory))
+            LOGGER.warning("Directory {} exists. Removing contents.".format(self.directory))
             for file in os.listdir(self.directory):
-                os.remove('{0}/{1}'.format(self.directory, file))
+                os.remove("{0}/{1}".format(self.directory, file))
         else:
-            LOGGER.warning('Directory {} does not exist. Creating it.'.format(self.directory))
+            LOGGER.warning("Directory {} does not exist. Creating it.".format(self.directory))
             Path(self.directory).mkdir(parents=True)
 
     def update(self, *args, **kwargs):
-        problem = kwargs['PROBLEM']
-        solutions = kwargs['SOLUTIONS']
-        evaluations = kwargs['EVALUATIONS']
+        problem = kwargs["PROBLEM"]
+        solutions = kwargs["SOLUTIONS"]
+        evaluations = kwargs["EVALUATIONS"]
 
         if solutions:
             if (evaluations % self.step) == 0:
                 if isinstance(problem, DynamicProblem):
-                    termination_criterion_is_met = kwargs.get('TERMINATION_CRITERIA_IS_MET', None)
+                    termination_criterion_is_met = kwargs.get("TERMINATION_CRITERIA_IS_MET", None)
 
                     if termination_criterion_is_met:
                         if self.counter > 0:
-                            igd = InvertedGenerationalDistance(self.last_front)
-                            igd_value = igd.compute(solutions)
+                            igd = InvertedGenerationalDistance(np.array([s.objectives for s in self.last_front]))
+                            igd_value = igd.compute(np.array([s.objectives for s in solutions]))
                         else:
                             igd_value = 1
 
                         if igd_value > 0.005:
                             self.fronts += solutions
-                            self.plot_front.plot([self.fronts],
-                                                 label=problem.get_name(),
-                                                 filename=f'{self.directory}/front-{evaluations}')
+                            self.plot_front.plot(
+                                [self.fronts],
+                                label=problem.get_name(),
+                                filename=f"{self.directory}/front-{evaluations}",
+                            )
                         self.counter += 1
                         self.last_front = solutions
                 else:
-                    self.plot_front.plot([solutions],
-                                         label=f'{evaluations} evaluations',
-                                         filename=f'{self.directory}/front-{evaluations}')
+                    self.plot_front.plot(
+                        [solutions],
+                        label=f"{evaluations} evaluations",
+                        filename=f"{self.directory}/front-{evaluations}",
+                    )
                     self.counter += 1
 
 
 class VisualizerObserver(Observer):
-
-    def __init__(self,
-                 reference_front: List[S] = None,
-                 reference_point: list = None,
-                 display_frequency: int = 1) -> None:
+    def __init__(
+        self, reference_front: List[S] = None, reference_point: list = None, display_frequency: int = 1
+    ) -> None:
         self.figure = None
         self.display_frequency = display_frequency
 
         self.reference_point = reference_point
         self.reference_front = reference_front
 
     def update(self, *args, **kwargs):
-        evaluations = kwargs['EVALUATIONS']
-        solutions = kwargs['SOLUTIONS']
+        evaluations = kwargs["EVALUATIONS"]
+        solutions = kwargs["SOLUTIONS"]
 
         if solutions:
             if self.figure is None:
-                self.figure = StreamingPlot(reference_point=self.reference_point,
-                                            reference_front=self.reference_front)
+                self.figure = StreamingPlot(reference_point=self.reference_point, reference_front=self.reference_front)
                 self.figure.plot(solutions)
 
             if (evaluations % self.display_frequency) == 0:
                 # check if reference point has changed
-                reference_point = kwargs.get('REFERENCE_POINT', None)
+                reference_point = kwargs.get("REFERENCE_POINT", None)
 
                 if reference_point:
                     self.reference_point = reference_point
                     self.figure.update(solutions, reference_point)
                 else:
                     self.figure.update(solutions)
 
-                self.figure.ax.set_title('Eval: {}'.format(evaluations), fontsize=13)
+                self.figure.ax.set_title("Eval: {}".format(evaluations), fontsize=13)
```

### Comparing `jmetalpy-1.5.5/jmetal/util/point.py` & `jmetalpy-1.6.0/jmetal/util/point.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,21 +6,18 @@
    :synopsis: implementation of points of n-dimensions (e.g, ideal point, nadir point, etc.
 
 .. moduleauthor:: Antonio J. Nebro <antonio@lcc.uma.es>
 """
 
 
 class Point(ABC):
-
     @abstractmethod
     def update(self, vector: []) -> None:
         pass
 
 
 class IdealPoint(Point):
-
     def __init__(self, dimension: int):
         self.point = dimension * [float("inf")]
 
     def update(self, vector: []) -> None:
         self.point = [y if x > y else x for x, y in zip(self.point, vector)]
-
```

### Comparing `jmetalpy-1.5.5/jmetal/util/ranking.py` & `jmetalpy-1.6.0/jmetal/util/ranking.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from abc import ABC, abstractmethod
-from typing import TypeVar, List
+from typing import List, TypeVar
 
-from jmetal.util.comparator import DominanceComparator, Comparator, SolutionAttributeComparator
+from jmetal.util.comparator import (
+    Comparator,
+    DominanceComparator,
+    SolutionAttributeComparator,
+)
 
-S = TypeVar('S')
+S = TypeVar("S")
 
 
 class Ranking(List[S], ABC):
-
     def __init__(self, comparator: Comparator = DominanceComparator()):
         super(Ranking, self).__init__()
         self.number_of_comparisons = 0
         self.ranked_sublists = []
         self.comparator = comparator
 
     @abstractmethod
@@ -19,33 +22,33 @@
         pass
 
     def get_nondominated(self):
         return self.ranked_sublists[0]
 
     def get_subfront(self, rank: int):
         if rank >= len(self.ranked_sublists):
-            raise Exception('Invalid rank: {0}. Max rank: {1}'.format(rank, len(self.ranked_sublists) - 1))
+            raise Exception("Invalid rank: {0}. Max rank: {1}".format(rank, len(self.ranked_sublists) - 1))
         return self.ranked_sublists[rank]
 
     def get_number_of_subfronts(self):
         return len(self.ranked_sublists)
 
     @classmethod
     def get_comparator(cls) -> Comparator:
         pass
 
 
 class FastNonDominatedRanking(Ranking[List[S]]):
-    """ Class implementing the non-dominated ranking of NSGA-II proposed by Deb et al., see [Deb2002]_ """
+    """Class implementing the non-dominated ranking of NSGA-II proposed by Deb et al., see [Deb2002]_"""
 
     def __init__(self, comparator: Comparator = DominanceComparator()):
         super(FastNonDominatedRanking, self).__init__(comparator)
 
     def compute_ranking(self, solutions: List[S], k: int = None):
-        """ Compute ranking of solutions.
+        """Compute ranking of solutions.
 
         :param solutions: Solution list.
         :param k: Number of individuals.
         """
         # number of solutions dominating solution ith
         dominating_ith = [0 for _ in range(len(solutions))]
 
@@ -59,58 +62,58 @@
             for q in range(p + 1, len(solutions)):
                 dominance_test_result = self.comparator.compare(solutions[p], solutions[q])
                 self.number_of_comparisons += 1
 
                 if dominance_test_result == -1:
                     ith_dominated[p].append(q)
                     dominating_ith[q] += 1
-                elif dominance_test_result is 1:
+                elif dominance_test_result == 1:
                     ith_dominated[q].append(p)
                     dominating_ith[p] += 1
 
         for i in range(len(solutions)):
-            if dominating_ith[i] is 0:
+            if dominating_ith[i] == 0:
                 front[0].append(i)
-                solutions[i].attributes['dominance_ranking'] = 0
+                solutions[i].attributes["dominance_ranking"] = 0
 
         i = 0
         while len(front[i]) != 0:
             i += 1
             for p in front[i - 1]:
                 if p <= len(ith_dominated):
                     for q in ith_dominated[p]:
                         dominating_ith[q] -= 1
-                        if dominating_ith[q] is 0:
+                        if dominating_ith[q] == 0:
                             front[i].append(q)
-                            solutions[q].attributes['dominance_ranking'] = i
+                            solutions[q].attributes["dominance_ranking"] = i
 
         self.ranked_sublists = [[]] * i
         for j in range(i):
             q = [0] * len(front[j])
             for m in range(len(front[j])):
                 q[m] = solutions[front[j][m]]
             self.ranked_sublists[j] = q
 
         if k:
             count = 0
             for i, front in enumerate(self.ranked_sublists):
                 count += len(front)
                 if count >= k:
-                    self.ranked_sublists = self.ranked_sublists[:i + 1]
+                    self.ranked_sublists = self.ranked_sublists[: i + 1]
                     break
 
         return self.ranked_sublists
 
     @classmethod
     def get_comparator(cls) -> Comparator:
-        return SolutionAttributeComparator('dominance_ranking')
+        return SolutionAttributeComparator("dominance_ranking")
 
 
 class StrengthRanking(Ranking[List[S]]):
-    """ Class implementing a ranking scheme based on the strength ranking used in SPEA2. """
+    """Class implementing a ranking scheme based on the strength ranking used in SPEA2."""
 
     def __init__(self, comparator: Comparator = DominanceComparator()):
         super(StrengthRanking, self).__init__(comparator)
 
     def compute_ranking(self, solutions: List[S], k: int = None):
         """
         Compute ranking of solutions.
@@ -132,31 +135,31 @@
         for i in range(len(solutions)):
             for j in range(len(solutions)):
                 if self.comparator.compare(solutions[i], solutions[j]) == 1:
                     raw_fitness[i] += strength[j]
 
         max_fitness_value: int = 0
         for i in range(len(solutions)):
-            solutions[i].attributes['strength_ranking'] = raw_fitness[i]
+            solutions[i].attributes["strength_ranking"] = raw_fitness[i]
             if raw_fitness[i] > max_fitness_value:
                 max_fitness_value = raw_fitness[i]
 
         # Initialize the ranked sublists. In the worst case will be max_fitness_value + 1 different sublists
         self.ranked_sublists = [[] for _ in range(max_fitness_value + 1)]
 
         # Assign each solution to its corresponding front
         for solution in solutions:
-            self.ranked_sublists[int(solution.attributes['strength_ranking'])].append(solution)
+            self.ranked_sublists[int(solution.attributes["strength_ranking"])].append(solution)
 
         # Remove empty fronts
         counter = 0
         while counter < len(self.ranked_sublists):
             if len(self.ranked_sublists[counter]) == 0:
                 del self.ranked_sublists[counter]
             else:
                 counter += 1
 
         return self.ranked_sublists
 
     @classmethod
     def get_comparator(cls) -> Comparator:
-        return SolutionAttributeComparator('strength_ranking')
+        return SolutionAttributeComparator("strength_ranking")
```

### Comparing `jmetalpy-1.5.5/jmetal/util/replacement.py` & `jmetalpy-1.6.0/jmetal/util/replacement.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from enum import Enum
-from typing import TypeVar, List
+from typing import List, TypeVar
 
 from jmetal.util.density_estimator import DensityEstimator
 from jmetal.util.ranking import Ranking
 
-S = TypeVar('S')
+S = TypeVar("S")
 
 
 class RemovalPolicyType(Enum):
     SEQUENTIAL = 1
     ONE_SHOT = 2
 
 
-class RankingAndDensityEstimatorReplacement():
-
-    def __init__(self, ranking: Ranking, density_estimator: DensityEstimator,
-                 removal_policy=RemovalPolicyType.ONE_SHOT):
+class RankingAndDensityEstimatorReplacement:
+    def __init__(
+        self, ranking: Ranking, density_estimator: DensityEstimator, removal_policy=RemovalPolicyType.ONE_SHOT
+    ):
         self.ranking = ranking
         self.density_estimator = density_estimator
         self.removal_policy = removal_policy
 
     def replace(self, solution_list: List[S], offspring_list: List[S]) -> List[S]:
         join_population = solution_list + offspring_list
 
@@ -35,16 +35,17 @@
         current_ranked_solutions = self.ranking.get_subfront(ranking_id)
         self.density_estimator.compute_density_estimator(current_ranked_solutions)
 
         result_list: List[S] = []
 
         if len(current_ranked_solutions) < size_of_the_result_list:
             result_list.extend(self.ranking.get_subfront(ranking_id))
-            result_list.extend(self.sequential_truncation(ranking_id + 1, size_of_the_result_list - len(
-                current_ranked_solutions)))
+            result_list.extend(
+                self.sequential_truncation(ranking_id + 1, size_of_the_result_list - len(current_ranked_solutions))
+            )
         else:
             for solution in current_ranked_solutions:
                 result_list.append(solution)
 
             while len(result_list) > size_of_the_result_list:
                 self.density_estimator.sort(result_list)
 
@@ -57,16 +58,17 @@
         current_ranked_solutions = self.ranking.get_subfront(ranking_id)
         self.density_estimator.compute_density_estimator(current_ranked_solutions)
 
         result_list: List[S] = []
 
         if len(current_ranked_solutions) < size_of_the_result_list:
             result_list.extend(self.ranking.get_subfront(ranking_id))
-            result_list.extend(self.one_shot_truncation(ranking_id + 1, size_of_the_result_list - len(
-                current_ranked_solutions)))
+            result_list.extend(
+                self.one_shot_truncation(ranking_id + 1, size_of_the_result_list - len(current_ranked_solutions))
+            )
         else:
             self.density_estimator.sort(current_ranked_solutions)
             i = 0
             while len(result_list) < size_of_the_result_list:
                 result_list.append(current_ranked_solutions[i])
                 i += 1
```

### Comparing `jmetalpy-1.5.5/jmetal/util/solution.py` & `jmetalpy-1.6.0/jmetal/util/solution.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import logging
 import os
 from pathlib import Path
 from typing import List
 
 from jmetal.core.solution import FloatSolution, Solution
-from jmetal.util.archive import NonDominatedSolutionsArchive, Archive
+from jmetal.util.archive import Archive, NonDominatedSolutionsArchive
 
-LOGGER = logging.getLogger('jmetal')
+logger = logging.getLogger(__name__)
 
 
 """
 .. module:: solutions
    :platform: Unix, Windows
    :synopsis: Utils to print solutions.
 
@@ -24,15 +24,15 @@
     for solution in solutions:
         archive.add(solution)
 
     return archive.solution_list
 
 
 def read_solutions(filename: str) -> List[FloatSolution]:
-    """ Reads a reference front from a file.
+    """Reads a reference front from a file.
 
     :param filename: File path where the front is located.
     """
     front = []
 
     if Path(filename).is_file():
         with open(filename) as file:
@@ -40,31 +40,31 @@
                 vector = [float(x) for x in line.split()]
 
                 solution = FloatSolution([], [], len(vector))
                 solution.objectives = vector
 
                 front.append(solution)
     else:
-        LOGGER.warning('Reference front file was not found at {}'.format(filename))
+        logger.warning("Reference front file was not found at {}".format(filename))
 
     return front
 
 
 def print_variables_to_file(solutions, filename: str):
-    LOGGER.info('Output file (variables): ' + filename)
+    logger.info("Output file (variables): " + filename)
 
     try:
         os.makedirs(os.path.dirname(filename), exist_ok=True)
     except FileNotFoundError:
         pass
 
     if type(solutions) is not list:
         solutions = [solutions]
 
-    with open(filename, 'w') as of:
+    with open(filename, "w") as of:
         for solution in solutions:
             for variables in solution.variables:
                 of.write(str(variables) + " ")
             of.write("\n")
 
 
 def print_variables_to_screen(solutions):
@@ -72,32 +72,32 @@
         solutions = [solutions]
 
     for solution in solutions:
         print(solution.variables[0])
 
 
 def print_function_values_to_file(solutions, filename: str):
-    LOGGER.info('Output file (function values): ' + filename)
+    logger.info("Output file (function values): " + filename)
 
     try:
         os.makedirs(os.path.dirname(filename), exist_ok=True)
     except FileNotFoundError:
         pass
 
     if type(solutions) is not list:
         solutions = [solutions]
 
-    with open(filename, 'w') as of:
+    with open(filename, "w") as of:
         for solution in solutions:
             for function_value in solution.objectives:
-                of.write(str(function_value) + ' ')
-            of.write('\n')
+                of.write(str(function_value) + " ")
+            of.write("\n")
 
 
 def print_function_values_to_screen(solutions):
     if type(solutions) is not list:
         solutions = [solutions]
 
     for solution in solutions:
-        print(str(solutions.index(solution)) + ": ", sep='  ', end='', flush=True)
-        print(solution.objectives, sep='  ', end='', flush=True)
+        print(str(solutions.index(solution)) + ": ", sep="  ", end="", flush=True)
+        print(solution.objectives, sep="  ", end="", flush=True)
         print()
```

### Comparing `jmetalpy-1.5.5/jmetal/util/termination_criterion.py` & `jmetalpy-1.6.0/jmetal/util/termination_criterion.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,62 +10,58 @@
    :synopsis: Implementation of stopping conditions.
 
 .. moduleauthor:: Antonio Benítez-Hidalgo <antonio.b@uma.es>
 """
 
 
 class TerminationCriterion(Observer, ABC):
-
     @abstractmethod
     def update(self, *args, **kwargs):
         pass
 
     @property
     @abstractmethod
     def is_met(self):
         pass
 
 
 class StoppingByEvaluations(TerminationCriterion):
-
     def __init__(self, max_evaluations: int):
         super(StoppingByEvaluations, self).__init__()
         self.max_evaluations = max_evaluations
         self.evaluations = 0
 
     def update(self, *args, **kwargs):
-        self.evaluations = kwargs['EVALUATIONS']
+        self.evaluations = kwargs["EVALUATIONS"]
 
     @property
     def is_met(self):
         return self.evaluations >= self.max_evaluations
 
 
 class StoppingByTime(TerminationCriterion):
-
     def __init__(self, max_seconds: int):
         super(StoppingByTime, self).__init__()
         self.max_seconds = max_seconds
         self.seconds = 0.0
 
     def update(self, *args, **kwargs):
-        self.seconds = kwargs['COMPUTING_TIME']
+        self.seconds = kwargs["COMPUTING_TIME"]
 
     @property
     def is_met(self):
         return self.seconds >= self.max_seconds
 
 
 def key_has_been_pressed(stopping_by_keyboard):
-    input('PRESS ANY KEY + ENTER: ')
+    input("PRESS ANY KEY + ENTER: ")
     stopping_by_keyboard.key_pressed = True
 
 
 class StoppingByKeyboard(TerminationCriterion):
-
     def __init__(self):
         super(StoppingByKeyboard, self).__init__()
         self.key_pressed = False
         thread = threading.Thread(target=key_has_been_pressed, args=(self,))
         thread.start()
 
     def update(self, *args, **kwargs):
@@ -73,24 +69,23 @@
 
     @property
     def is_met(self):
         return self.key_pressed
 
 
 class StoppingByQualityIndicator(TerminationCriterion):
-
     def __init__(self, quality_indicator: QualityIndicator, expected_value: float, degree: float):
         super(StoppingByQualityIndicator, self).__init__()
         self.quality_indicator = quality_indicator
         self.expected_value = expected_value
         self.degree = degree
         self.value = 0.0
 
     def update(self, *args, **kwargs):
-        solutions = kwargs['SOLUTIONS']
+        solutions = kwargs["SOLUTIONS"]
 
         if solutions:
             self.value = self.quality_indicator.compute(solutions)
 
     @property
     def is_met(self):
         if self.quality_indicator.is_minimization:
```

### Comparing `jmetalpy-1.5.5/jmetal/util/test/test_aggregativefunction.py` & `jmetalpy-1.6.0/jmetal/util/test/test_aggregativefunction.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import unittest
 
 from jmetal.util.aggregative_function import WeightedSum
 
 
 class WeightedSumTestCases(unittest.TestCase):
-
     def test_should_aggregative_sum_work_properly_with_2D_vectors(self) -> None:
         aggregative_function = WeightedSum()
 
         self.assertEqual(1.5, aggregative_function.compute([1.5, 2.9], [1.0, 0.0]))
         self.assertEqual(2.9, aggregative_function.compute([1.5, 2.9], [0.0, 1.0]))
         self.assertEqual(1.5 / 2.0 + 2.9 / 2.0, aggregative_function.compute([1.5, 2.9], [0.5, 0.5]))
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `jmetalpy-1.5.5/jmetal/util/test/test_archive.py` & `jmetalpy-1.6.0/jmetal/util/test/test_archive.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 import unittest
 
 from jmetal.core.solution import Solution
-from jmetal.util.archive import NonDominatedSolutionsArchive, BoundedArchive, CrowdingDistanceArchive, Archive
+from jmetal.util.archive import (
+    Archive,
+    BoundedArchive,
+    CrowdingDistanceArchive,
+    NonDominatedSolutionsArchive,
+)
 
 
 class ArchiveTestCases(unittest.TestCase):
     class DummyArchive(Archive):
-
         def add(self, solution) -> bool:
             pass
 
     def setUp(self):
         self.archive = self.DummyArchive()
 
     def test_should_constructor_create_a_non_null_object(self):
         self.assertIsNotNone(self.archive)
 
     def test_should_constructor_create_an_empty_list(self):
         self.assertEqual(0, len(self.archive.solution_list))
 
 
 class BoundedArchiveTestCases(unittest.TestCase):
-
     def setUp(self):
         self.archive = BoundedArchive(5)
 
     def test_should_constructor_create_a_non_null_object(self):
         self.assertIsNotNone(self.archive)
 
     def test_should_constructor_set_the_max_size(self):
         self.assertEqual(5, self.archive.maximum_size)
 
 
 class NonDominatedSolutionListArchiveTestCases(unittest.TestCase):
-
     def setUp(self):
         self.archive = NonDominatedSolutionsArchive()
 
     def test_should_constructor_create_a_non_null_object(self):
         self.assertIsNotNone(self.archive)
 
     def test_should_adding_one_solution_work_properly(self):
@@ -66,16 +68,15 @@
         solution2 = Solution(1, 2)
         solution2.objectives = [0.0, 1.0]
 
         self.archive.add(solution1)
         self.archive.add(solution2)
 
         self.assertEqual(2, self.archive.size())
-        self.assertTrue(solution1 in self.archive.solution_list and
-                        solution2 in self.archive.solution_list)
+        self.assertTrue(solution1 in self.archive.solution_list and solution2 in self.archive.solution_list)
 
     def test_should_adding_four_solutions_work_properly_if_one_dominates_the_others(self):
         solution1 = Solution(1, 2)
         solution1.objectives = [1.0, 1.0]
 
         solution2 = Solution(1, 2)
         solution2.objectives = [0.0, 2.0]
@@ -106,20 +107,18 @@
 
         self.archive.add(solution1)
         self.archive.add(solution2)
         result = self.archive.add(solution3)
 
         self.assertEqual(2, self.archive.size())
         self.assertFalse(result)
-        self.assertTrue(solution1 in self.archive.solution_list
-                        or solution3 in self.archive.solution_list)
+        self.assertTrue(solution1 in self.archive.solution_list or solution3 in self.archive.solution_list)
 
 
 class CrowdingDistanceArchiveTestCases(unittest.TestCase):
-
     def setUp(self):
         self.archive = CrowdingDistanceArchive[Solution](5)
 
     def test_should_constructor_create_a_non_null_object(self):
         self.assertIsNotNone(self.archive)
 
     def test_should_constructor_set_the_max_size(self):
@@ -132,45 +131,42 @@
         solution = Solution(2, 3)
         self.archive.add(solution)
 
         self.assertEqual(1, self.archive.size())
         self.assertEqual(solution, self.archive.get(0))
 
     def test_should_add_work_properly_case1(self):
-        """ Case 1: add a dominated solution when the archive size is 1 must not include the solution.
-        """
+        """Case 1: add a dominated solution when the archive size is 1 must not include the solution."""
         solution1 = Solution(2, 2)
         solution1.objectives = [1, 2]
         solution2 = Solution(2, 2)
         solution2.objectives = [3, 4]
 
         self.archive.add(solution1)
         self.archive.add(solution2)
 
         self.assertEqual(1, self.archive.size())
         self.assertEqual(solution1, self.archive.get(0))
 
     def test_should_add_work_properly_case2(self):
-        """ Case 2: add a non-dominated solution when the archive size is 1 must include the solution.
-        """
+        """Case 2: add a non-dominated solution when the archive size is 1 must include the solution."""
         solution1 = Solution(2, 2)
         solution1.objectives = [1, 2]
         solution2 = Solution(2, 2)
         solution2.objectives = [0, 4]
 
         self.archive.add(solution1)
         self.archive.add(solution2)
 
         self.assertEqual(2, self.archive.size())
         self.assertTrue(solution1 in self.archive.solution_list)
         self.assertTrue(solution2 in self.archive.solution_list)
 
     def test_should_add_work_properly_case3(self):
-        """ Case 3: add a non-dominated solution when the archive size is 3 must include the solution.
-        """
+        """Case 3: add a non-dominated solution when the archive size is 3 must include the solution."""
         solution1 = Solution(2, 2)
         solution1.objectives = [1.0, 2.0]
         solution2 = Solution(2, 2)
         solution2.objectives = [0.0, 4.0]
         solution3 = Solution(2, 2)
         solution3.objectives = [1.5, 1.5]
         solution4 = Solution(2, 2)
@@ -184,16 +180,15 @@
         self.assertEqual(4, self.archive.size())
         self.assertTrue(solution1 in self.archive.solution_list)
         self.assertTrue(solution2 in self.archive.solution_list)
         self.assertTrue(solution3 in self.archive.solution_list)
         self.assertTrue(solution4 in self.archive.solution_list)
 
     def test_should_add_work_properly_case4(self):
-        """ Case 4: add a dominated solution when the archive size is 3 must not include the solution.
-        """
+        """Case 4: add a dominated solution when the archive size is 3 must not include the solution."""
         solution1 = Solution(2, 2)
         solution1.objectives = [1.0, 2.0]
         solution2 = Solution(2, 2)
         solution2.objectives = [0.0, 4.0]
         solution3 = Solution(2, 2)
         solution3.objectives = [1.5, 1.5]
         solution4 = Solution(2, 2)
@@ -206,16 +201,15 @@
 
         self.assertEqual(3, self.archive.size())
         self.assertTrue(solution1 in self.archive.solution_list)
         self.assertTrue(solution2 in self.archive.solution_list)
         self.assertTrue(solution3 in self.archive.solution_list)
 
     def test_should_add_work_properly_case5(self):
-        """ Case 5: add a dominated solution when the archive is full should not include the solution.
-        """
+        """Case 5: add a dominated solution when the archive is full should not include the solution."""
         solution1 = Solution(2, 2)
         solution1.objectives = [1.0, 2.0]
         solution2 = Solution(2, 2)
         solution2.objectives = [0.0, 4.0]
         solution3 = Solution(2, 2)
         solution3.objectives = [1.5, 1.5]
         solution4 = Solution(2, 2)
@@ -228,15 +222,15 @@
 
         self.assertEqual(3, self.archive.size())
         self.assertTrue(solution1 in self.archive.solution_list)
         self.assertTrue(solution2 in self.archive.solution_list)
         self.assertTrue(solution3 in self.archive.solution_list)
 
     def test_should_add_work_properly_case6(self):
-        """ Case 6: add a non-dominated solution when the archive is full should not include
+        """Case 6: add a non-dominated solution when the archive is full should not include
         the solution if it has the highest distance crowding value.
         """
         archive = CrowdingDistanceArchive(4)
 
         solution1 = Solution(1, 2)
         solution1.variables = [1.0]
         solution1.objectives = [0.0, 3.0]
@@ -260,16 +254,15 @@
         archive.add(solution4)
         archive.add(new_solution)
 
         self.assertEqual(4, archive.size())
         self.assertTrue(new_solution not in archive.solution_list)
 
     def test_should_add_work_properly_case7(self):
-        """ Case 7: add a non-dominated solution when the archive is full should remove all the dominated solutions.
-        """
+        """Case 7: add a non-dominated solution when the archive is full should remove all the dominated solutions."""
         archive = CrowdingDistanceArchive(4)
 
         solution1 = Solution(2, 2)
         solution1.objectives = [0.0, 3.0]
         solution2 = Solution(2, 2)
         solution2.objectives = [1.0, 2.0]
         solution3 = Solution(2, 2)
@@ -286,30 +279,28 @@
         archive.add(solution4)
         archive.add(new_solution)
 
         self.assertEqual(1, archive.size())
         self.assertTrue(new_solution in archive.solution_list)
 
     def test_should_compute_density_estimator_work_properly_case1(self):
-        """ Case 1: The archive contains one solution.
-        """
+        """Case 1: The archive contains one solution."""
         archive = CrowdingDistanceArchive(4)
 
         solution1 = Solution(2, 2)
         solution1.objectives = [0.0, 3.0]
         archive.add(solution1)
 
         archive.compute_density_estimator()
 
         self.assertEqual(1, archive.size())
         self.assertEqual(float("inf"), solution1.attributes["crowding_distance"])
 
     def test_should_compute_density_estimator_work_properly_case2(self):
-        """ Case 2: The archive contains two solutions.
-        """
+        """Case 2: The archive contains two solutions."""
         archive = CrowdingDistanceArchive(4)
 
         solution1 = Solution(2, 2)
         solution1.objectives = [0.0, 3.0]
         solution2 = Solution(2, 2)
         solution2.objectives = [1.0, 2.0]
 
@@ -319,16 +310,15 @@
         archive.compute_density_estimator()
 
         self.assertEqual(2, archive.size())
         self.assertEqual(float("inf"), solution1.attributes["crowding_distance"])
         self.assertEqual(float("inf"), solution2.attributes["crowding_distance"])
 
     def test_should_compute_density_estimator_work_properly_case3(self):
-        """ Case 3: The archive contains two solutions.
-        """
+        """Case 3: The archive contains two solutions."""
         archive = CrowdingDistanceArchive(4)
 
         solution1 = Solution(2, 2)
         solution1.objectives = [0.0, 3.0]
         solution2 = Solution(2, 2)
         solution2.objectives = [1.0, 2.0]
         solution3 = Solution(2, 2)
@@ -342,9 +332,9 @@
 
         self.assertEqual(3, archive.size())
         self.assertEqual(float("inf"), solution1.attributes["crowding_distance"])
         self.assertEqual(float("inf"), solution3.attributes["crowding_distance"])
         self.assertTrue(solution2.attributes["crowding_distance"] < float("inf"))
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `jmetalpy-1.5.5/jmetal/util/test/test_checking.py` & `jmetalpy-1.6.0/jmetal/util/test/test_checking.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 import unittest
 
-from jmetal.util.ckecking import Check, NoneParameterException, InvalidProbabilityValueException, \
-    ValueOutOfRangeException, InvalidConditionException
+from jmetal.util.ckecking import (
+    Check,
+    InvalidConditionException,
+    InvalidProbabilityValueException,
+    NoneParameterException,
+    ValueOutOfRangeException,
+)
 
 
 class CheckingTestCases(unittest.TestCase):
-
     def test_should_is_not_null_raise_an_exception(self) -> None:
         with self.assertRaises(NoneParameterException):
             Check.is_not_none(None)
 
     def test_should_is_valid_probability_raise_an_exception_if_the_value_is_negative(self) -> None:
         with self.assertRaises(InvalidProbabilityValueException):
             Check.probability_is_valid(-1.0)
@@ -27,9 +31,9 @@
             Check.value_is_in_range(7, 3, 5)
 
     def test_should_that_raise_an_exception_if_the_expression_is_false(self) -> None:
         with self.assertRaises(InvalidConditionException):
             Check.that(False, "The expression is false")
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `jmetalpy-1.5.5/jmetal/util/test/test_comparator.py` & `jmetalpy-1.6.0/jmetal/util/test/test_comparator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 import unittest
 
-from mockito import mock, when, verify, never
+from mockito import mock, never, verify, when
 
 from jmetal.core.solution import Solution
-from jmetal.util.comparator import DominanceComparator, SolutionAttributeComparator, \
-    RankingAndCrowdingDistanceComparator, Comparator, OverallConstraintViolationComparator, MultiComparator
+from jmetal.util.comparator import (
+    Comparator,
+    DominanceComparator,
+    MultiComparator,
+    OverallConstraintViolationComparator,
+    RankingAndCrowdingDistanceComparator,
+    SolutionAttributeComparator, DominanceWithConstraintsComparator,
+)
 
 
 class OverallConstraintViolationComparatorTestCases(unittest.TestCase):
     def setUp(self):
         self.comparator: Comparator = OverallConstraintViolationComparator()
 
     def test_should_comparator_return_0_if_the_solutions_have_no_constraints(self):
@@ -41,15 +47,14 @@
         solution1.constraints[0] = -2
         solution2.constraints[0] = -5
 
         self.assertEqual(-1, self.comparator.compare(solution1, solution2))
 
 
 class DominanceComparatorTestCases(unittest.TestCase):
-
     def setUp(self):
         self.comparator = DominanceComparator()
 
     def test_should_dominance_comparator_raise_an_exception_if_the_first_solution_is_null(self):
         solution = None
         solution2 = Solution(2, 2)
         with self.assertRaises(Exception):
@@ -66,112 +71,111 @@
         solution2 = Solution(1, 1)
         solution.objectives = [1.0]
         solution2.objectives = [1.0]
 
         self.assertEqual(0, self.comparator.compare(solution, solution2))
 
     def test_should_dominance_comparator_return_one_if_the_two_solutions_have_one_objective_and_the_second_one_is_lower(
-            self):
+            self,
+    ):
         solution = Solution(1, 1)
         solution2 = Solution(1, 1)
         solution.objectives = [2.0]
         solution2.objectives = [1.0]
 
         self.assertEqual(1, self.comparator.compare(solution, solution2))
 
     def test_should_dominance_comparator_return_minus_one_if_the_two_solutions_have_one_objective_and_the_first_one_is_lower(
-            self):
+            self,
+    ):
         solution = Solution(1, 1)
         solution2 = Solution(1, 1)
         solution.objectives = [1.0]
         solution2.objectives = [2.0]
 
         self.assertEqual(-1, self.comparator.compare(solution, solution2))
 
     def test_should_dominance_comparator_work_properly_case_a(self):
-        """ Case A: solution1 has objectives [-1.0, 5.0, 9.0] and solution2 has [2.0, 6.0, 15.0]
-        """
+        """Case A: solution1 has objectives [-1.0, 5.0, 9.0] and solution2 has [2.0, 6.0, 15.0]"""
         solution = Solution(1, 3)
         solution2 = Solution(1, 3)
         solution.objectives = [-1.0, 5.0, 9.0]
         solution2.objectives = [2.0, 6.0, 15.0]
 
         self.assertEqual(-1, self.comparator.compare(solution, solution2))
 
     def test_should_dominance_comparator_work_properly_case_b(self):
-        """ Case b: solution1 has objectives [-1.0, 5.0, 9.0] and solution2 has [-1.0, 5.0, 10.0]
-        """
+        """Case b: solution1 has objectives [-1.0, 5.0, 9.0] and solution2 has [-1.0, 5.0, 10.0]"""
         solution = Solution(1, 3)
         solution2 = Solution(1, 3)
         solution.objectives = [-1.0, 5.0, 9.0]
         solution2.objectives = [-1.0, 5.0, 10.0]
 
         self.assertEqual(-1, self.comparator.compare(solution, solution2))
 
     def test_should_dominance_comparator_work_properly_case_c(self):
-        """ Case c: solution1 has objectives [-1.0, 5.0, 9.0] and solution2 has [-2.0, 5.0, 9.0]
-        """
+        """Case c: solution1 has objectives [-1.0, 5.0, 9.0] and solution2 has [-2.0, 5.0, 9.0]"""
         solution = Solution(1, 3)
         solution2 = Solution(1, 3)
         solution.objectives = [-1.0, 5.0, 9.0]
         solution2.objectives = [-2.0, 5.0, 9.0]
 
         self.assertEqual(1, self.comparator.compare(solution, solution2))
 
     def test_should_dominance_comparator_work_properly_case_d(self):
-        """ Case d: solution1 has objectives [-1.0, 5.0, 9.0] and solution2 has [-1.0, 5.0, 8.0]
-        """
+        """Case d: solution1 has objectives [-1.0, 5.0, 9.0] and solution2 has [-1.0, 5.0, 8.0]"""
         solution = Solution(1, 3)
         solution2 = Solution(1, 3)
         solution.objectives = [-1.0, 5.0, 9.0]
         solution2.objectives = [-1.0, 5.0, 8.0]
 
         self.assertEqual(1, self.comparator.compare(solution, solution2))
 
     def test_should_dominance_comparator_work_properly_case_3(self):
-        """ Case d: solution1 has objectives [-1.0, 5.0, 9.0] and solution2 has [-2.0, 5.0, 10.0]
-        """
+        """Case d: solution1 has objectives [-1.0, 5.0, 9.0] and solution2 has [-2.0, 5.0, 10.0]"""
         solution = Solution(1, 3)
         solution2 = Solution(1, 3)
         solution.objectives = [-1.0, 5.0, 9.0]
         solution2.objectives = [-2.0, 5.0, 10.0]
 
         self.assertEqual(0, self.comparator.compare(solution, solution2))
 
+
+class DominanceWithConstraintsComparatorTestCases(unittest.TestCase):
+    def setUp(self):
+        self.comparator = DominanceWithConstraintsComparator()
+
     def test_should_dominance_comparator_work_properly_with_constrains_case_1(self):
-        """ Case 1: solution1 has a higher degree of constraint violation than solution 2
-        """
+        """Case 1: solution1 has a higher degree of constraint violation than solution 2"""
         solution1 = Solution(1, 3, 1)
         solution2 = Solution(1, 3, 1)
 
         solution1.constraints[0] = -0.1
         solution2.constraints[0] = -0.3
 
         solution1.objectives = [-1.0, 5.0, 9.0]
         solution2.objectives = [-2.0, 5.0, 10.0]
 
         self.assertEqual(-1, self.comparator.compare(solution1, solution2))
 
     def test_should_dominance_comparator_work_properly_with_constrains_case_2(self):
-        """ Case 2: solution1 has a lower degree of constraint violation than solution 2
-        """
+        """Case 2: solution1 has a lower degree of constraint violation than solution 2"""
         solution1 = Solution(1, 3, 1)
         solution2 = Solution(1, 3, 1)
 
         solution1.constraints[0] = -0.3
         solution2.constraints[0] = -0.1
 
         solution1.objectives = [-1.0, 5.0, 9.0]
         solution2.objectives = [-2.0, 5.0, 10.0]
 
         self.assertEqual(1, self.comparator.compare(solution1, solution2))
 
 
 class SolutionAttributeComparatorTestCases(unittest.TestCase):
-
     def setUp(self):
         self.comparator = SolutionAttributeComparator("attribute")
 
     def test_should_compare_return_zero_if_the_first_solution_has_no_the_attribute(self):
         solution1 = Solution(1, 1)
         solution2 = Solution(1, 1)
         solution2.attributes["attribute"] = 1.0
@@ -196,149 +200,140 @@
         solution2 = Solution(1, 1)
         solution1.attributes["attribute"] = 1.0
         solution2.attributes["attribute"] = 1.0
 
         self.assertEqual(0, self.comparator.compare(solution1, solution2))
 
     def test_should_compare_works_properly_case1(self):
-        """ Case 1: solution1.attribute < solution2.attribute (lowest is best)
-        """
+        """Case 1: solution1.attribute < solution2.attribute (lowest is best)"""
         solution1 = Solution(1, 1)
         solution2 = Solution(1, 1)
         solution1.attributes["attribute"] = 0.0
         solution2.attributes["attribute"] = 1.0
 
         self.assertEqual(-1, self.comparator.compare(solution1, solution2))
 
     def test_should_compare_works_properly_case2(self):
-        """ Case 2: solution1.attribute > solution2.attribute (lowest is best)
-        """
+        """Case 2: solution1.attribute > solution2.attribute (lowest is best)"""
         solution1 = Solution(1, 1)
         solution2 = Solution(1, 1)
         solution1.attributes["attribute"] = 1.0
         solution2.attributes["attribute"] = 0.0
 
         self.assertEqual(1, self.comparator.compare(solution1, solution2))
 
     def test_should_compare_works_properly_case3(self):
-        """ Case 3: solution1.attribute < solution2.attribute (highest is best)
-        """
+        """Case 3: solution1.attribute < solution2.attribute (highest is best)"""
         comparator = SolutionAttributeComparator("attribute", False)
         solution1 = Solution(1, 1)
         solution2 = Solution(1, 1)
         solution1.attributes["attribute"] = 0.0
         solution2.attributes["attribute"] = 1.0
 
         self.assertEqual(1, comparator.compare(solution1, solution2))
 
     def test_should_compare_works_properly_case4(self):
-        """ Case 4: solution1.attribute > solution2.attribute (highest is best)
-        """
+        """Case 4: solution1.attribute > solution2.attribute (highest is best)"""
         solution1 = Solution(1, 1)
         solution2 = Solution(1, 1)
         solution1.attributes["attribute"] = 1.0
         solution2.attributes["attribute"] = 0.0
 
         comparator = SolutionAttributeComparator("attribute", False)
         self.assertEqual(-1, comparator.compare(solution1, solution2))
 
 
 class RankingAndCrowdingComparatorTestCases(unittest.TestCase):
-
     def setUp(self):
         self.comparator = RankingAndCrowdingDistanceComparator()
 
     def test_should_compare_work_properly_case_1(self):
-        """ Case 1: solution1.ranking < solution2.ranking
-        """
+        """Case 1: solution1.ranking < solution2.ranking"""
         solution1 = Solution(1, 1)
         solution2 = Solution(1, 1)
         solution1.attributes["dominance_ranking"] = 1.0
         solution2.attributes["dominance_ranking"] = 2.0
 
         self.assertEqual(-1, self.comparator.compare(solution1, solution2))
 
     def test_should_compare_work_properly_case_2(self):
-        """ Case 2: solution1.ranking > solution2.ranking
-        """
+        """Case 2: solution1.ranking > solution2.ranking"""
         solution1 = Solution(1, 1)
         solution2 = Solution(1, 1)
         solution1.attributes["dominance_ranking"] = 2.0
         solution2.attributes["dominance_ranking"] = 1.0
 
         self.assertEqual(1, self.comparator.compare(solution1, solution2))
 
     def test_should_compare_work_properly_case_3(self):
-        """ Case 3: solution1.ranking == solution2.ranking
-                    solution1.crowding < solution2.crowding
+        """Case 3: solution1.ranking == solution2.ranking
+        solution1.crowding < solution2.crowding
         """
         solution1 = Solution(1, 1)
         solution2 = Solution(1, 1)
         solution1.attributes["dominance_ranking"] = 1.0
         solution2.attributes["dominance_ranking"] = 1.0
         solution1.attributes["crowding_distance"] = 1.0
         solution2.attributes["crowding_distance"] = 2.0
 
         self.assertEqual(1, self.comparator.compare(solution1, solution2))
 
     def test_should_compare_work_properly_case_4(self):
-        """ Case 4: solution1.ranking == solution2.ranking
-                    solution1.crowding > solution2.crowding
+        """Case 4: solution1.ranking == solution2.ranking
+        solution1.crowding > solution2.crowding
         """
         solution1 = Solution(1, 1)
         solution2 = Solution(1, 1)
         solution1.attributes["dominance_ranking"] = 1.0
         solution2.attributes["dominance_ranking"] = 1.0
         solution1.attributes["crowding_distance"] = 2.0
         solution2.attributes["crowding_distance"] = 1.0
 
         self.assertEqual(-1, self.comparator.compare(solution1, solution2))
 
     def test_should_compare_work_properly_case_5(self):
-        """ Case 5: solution1.ranking == solution2.ranking
-                    solution1.crowding == solution2.crowding
+        """Case 5: solution1.ranking == solution2.ranking
+        solution1.crowding == solution2.crowding
         """
         solution1 = Solution(1, 1)
         solution2 = Solution(1, 1)
         solution1.attributes["dominance_ranking"] = 1.0
         solution2.attributes["dominance_ranking"] = 1.0
         solution1.attributes["crowding_distance"] = 2.0
         solution2.attributes["crowding_distance"] = 2.0
 
         self.assertEqual(0, self.comparator.compare(solution1, solution2))
 
 
 class MultiComparatorTestCases(unittest.TestCase):
-
     def test_should_compare_return_zero_if_the_comparator_list_is_empty(self):
         solution1 = Solution(2, 2)
         solution2 = Solution(2, 2)
 
         multi_comparator = MultiComparator([])
         self.assertEqual(0, multi_comparator.compare(solution1, solution2))
 
     def test_should_compare_work_properly_case_1(self):
-        """ Case 1: a comparator returning 0.
-        """
+        """Case 1: a comparator returning 0."""
         solution1 = Solution(2, 2)
         solution2 = Solution(2, 2)
 
         mocked_comparator: Comparator = mock()
         when(mocked_comparator).compare(solution1, solution2).thenReturn(0)
 
         comparator_list = [mocked_comparator]
 
         multi_comparator = MultiComparator(comparator_list)
         self.assertEqual(0, multi_comparator.compare(solution1, solution2))
 
         verify(mocked_comparator, times=1).compare(solution1, solution2)
 
     def test_should_compare_work_properly_case_2(self):
-        """ Case 2: two comparators; the first returns 1 and the second one returns 0.
-            Expected result: 1
+        """Case 2: two comparators; the first returns 1 and the second one returns 0.
+        Expected result: 1
         """
         solution1 = Solution(2, 2)
         solution2 = Solution(2, 2)
 
         mocked_comparator1: Comparator = mock()
         when(mocked_comparator1).compare(solution1, solution2).thenReturn(1)
         mocked_comparator2: Comparator = mock()
@@ -349,16 +344,16 @@
         multi_comparator = MultiComparator(comparator_list)
         self.assertEqual(1, multi_comparator.compare(solution1, solution2))
 
         verify(mocked_comparator1, times=1).compare(solution1, solution2)
         verify(mocked_comparator2, never).compare(solution1, solution2)
 
     def test_should_compare_work_properly_case_3(self):
-        """ Case 2: two comparators; the first returns 0 and the second one returns -1.
-            Expected result: -1
+        """Case 2: two comparators; the first returns 0 and the second one returns -1.
+        Expected result: -1
         """
         solution1 = Solution(2, 2)
         solution2 = Solution(2, 2)
 
         mocked_comparator1: Comparator = mock()
         when(mocked_comparator1).compare(solution1, solution2).thenReturn(0)
         mocked_comparator2: Comparator = mock()
@@ -369,9 +364,9 @@
         multi_comparator = MultiComparator(comparator_list)
         self.assertEqual(-1, multi_comparator.compare(solution1, solution2))
 
         verify(mocked_comparator1, times=1).compare(solution1, solution2)
         verify(mocked_comparator2, times=1).compare(solution1, solution2)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `jmetalpy-1.5.5/jmetal/util/test/test_constraint_handling.py` & `jmetalpy-1.6.0/jmetal/util/test/test_constraint_handling.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import unittest
 
 from jmetal.core.solution import Solution
-from jmetal.util.constraint_handling import is_feasible, number_of_violated_constraints, \
-    overall_constraint_violation_degree, feasibility_ratio
+from jmetal.util.constraint_handling import (
+    feasibility_ratio,
+    is_feasible,
+    number_of_violated_constraints,
+    overall_constraint_violation_degree,
+)
 
 
 class ConstraintHandlingTestCases(unittest.TestCase):
-
     def test_should_is_feasible_return_true_if_the_solution_has_no_constraints(self) -> None:
         solution = Solution(number_of_variables=2, number_of_objectives=2, number_of_constraints=0)
 
         self.assertEqual(True, is_feasible(solution))
 
     def test_should_is_feasible_return_true_if_the_solution_has_constraints_and_is_feasible(self) -> None:
         solution = Solution(number_of_variables=2, number_of_objectives=2, number_of_constraints=1)
@@ -25,15 +28,17 @@
         self.assertEqual(False, is_feasible(solution))
 
     def test_should_number_of_violated_constraints_return_zero_if_the_solution_has_no_constraints(self) -> None:
         solution = Solution(number_of_variables=2, number_of_objectives=2, number_of_constraints=0)
 
         self.assertEqual(0, number_of_violated_constraints(solution))
 
-    def test_should_number_of_violated_constraints_return_zero_if_the_solution_has_not_violated_constraints(self) -> None:
+    def test_should_number_of_violated_constraints_return_zero_if_the_solution_has_not_violated_constraints(
+        self,
+    ) -> None:
         solution = Solution(number_of_variables=2, number_of_objectives=2, number_of_constraints=2)
 
         self.assertEqual(0, number_of_violated_constraints(solution))
 
     def test_should_number_of_violated_constraints_return_the_right_number_of_violated_constraints(self) -> None:
         solution = Solution(number_of_variables=2, number_of_objectives=2, number_of_constraints=2)
         solution.constraints[0] = 0
@@ -86,12 +91,12 @@
         solution1 = Solution(2, 2, 1)
         solution2 = Solution(2, 2, 1)
         solution3 = Solution(2, 2, 1)
         solution1.constraints[0] = -1
         solution2.constraints[0] = 0
         solution3.constraints[0] = -2
 
-        self.assertEqual(1/3, feasibility_ratio([solution1, solution2, solution3]))
+        self.assertEqual(1 / 3, feasibility_ratio([solution1, solution2, solution3]))
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `jmetalpy-1.5.5/jmetal/util/test/test_density_estimator.py` & `jmetalpy-1.6.0/jmetal/util/test/test_density_estimator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import unittest
 from math import sqrt
 
 from jmetal.core.solution import Solution
-from jmetal.util.density_estimator import CrowdingDistance, KNearestNeighborDensityEstimator
+from jmetal.util.density_estimator import (
+    CrowdingDistance,
+    KNearestNeighborDensityEstimator,
+)
 
 
 class CrowdingDistanceTestCases(unittest.TestCase):
-
     def setUp(self):
         self.crowding = CrowdingDistance()
 
     def test_should_the_crowding_distance_of_an_empty_set_do_nothing(self):
         solution_list = []
         self.crowding.compute_density_estimator(solution_list)
 
@@ -85,58 +87,57 @@
 
         self.assertEqual(float("inf"), value_from_solution1)
         self.assertEqual(float("inf"), value_from_solution2)
         self.assertGreater(value_from_solution3, value_from_solution4)
 
 
 class KNearestNeighborDensityEstimatorTest(unittest.TestCase):
-
     def setUp(self):
         self.knn = KNearestNeighborDensityEstimator()
 
     def test_should_the_density_estimator_compute_the_right_distances_case1(self):
         """
-         5 1
-         4   2
-         3     3
-         2
-         1         4
-         0 1 2 3 4 5
+        5 1
+        4   2
+        3     3
+        2
+        1         4
+        0 1 2 3 4 5
         """
         solution1 = Solution(2, 2)
         solution1.objectives = [1, 5]
         solution2 = Solution(2, 2)
         solution2.objectives = [2, 4]
         solution3 = Solution(2, 2)
         solution3.objectives = [3, 3]
         solution4 = Solution(2, 2)
         solution4.objectives = [5, 1]
 
         solution_list = [solution1, solution2, solution3, solution4]
 
         self.knn.compute_density_estimator(solution_list)
 
-        self.assertEqual(sqrt(2), solution1.attributes['knn_density'])
-        self.assertEqual(sqrt(2), solution2.attributes['knn_density'])
-        self.assertEqual(sqrt(2), solution3.attributes['knn_density'])
-        self.assertEqual(sqrt(2 * 2 + 2 * 2), solution4.attributes['knn_density'])
+        self.assertEqual(sqrt(2), solution1.attributes["knn_density"])
+        self.assertEqual(sqrt(2), solution2.attributes["knn_density"])
+        self.assertEqual(sqrt(2), solution3.attributes["knn_density"])
+        self.assertEqual(sqrt(2 * 2 + 2 * 2), solution4.attributes["knn_density"])
 
         # self.knn.sort(solution_list)
 
     def test_should_the_density_estimator_sort_the_solution_list(self):
         """
-         5 1
-         4   2
-         3     3
-         2     5
-         1         4
-         0 1 2 3 4 5
+        5 1
+        4   2
+        3     3
+        2     5
+        1         4
+        0 1 2 3 4 5
 
-         List: 1,2,3,4,5
-         Expected result: 4, 1, 2, 5, 3
+        List: 1,2,3,4,5
+        Expected result: 4, 1, 2, 5, 3
         """
         solution1 = Solution(2, 2)
         solution1.objectives = [1, 5]
         solution2 = Solution(2, 2)
         solution2.objectives = [2, 4]
         solution3 = Solution(2, 2)
         solution3.objectives = [3, 3]
@@ -153,22 +154,22 @@
         self.assertEqual(solution_list[0], solution4)
         self.assertEqual(solution_list[1], solution1)
         self.assertEqual(solution_list[2], solution2)
         self.assertEqual(solution_list[3], solution5)
 
     def test_should_the_density_estimator_sort_the_solution_list_considering_the_draws(self):
         """
-         5 1
-         4   2
-         3     3
-         2
-         1         4
-         0 1 2 3 4 5
+        5 1
+        4   2
+        3     3
+        2
+        1         4
+        0 1 2 3 4 5
 
-         Expected result after sort: 4, 3, 1, 2
+        Expected result after sort: 4, 3, 1, 2
         """
         solution1 = Solution(2, 2)
         solution1.objectives = [1, 5]
         solution2 = Solution(2, 2)
         solution2.objectives = [2, 4]
         solution3 = Solution(2, 2)
         solution3.objectives = [3, 3]
@@ -190,19 +191,21 @@
         0.13436424411240122 4.323216008886963
         0.020818108509287336 5.1051826661880515
         0.1028341459863098 4.9409270526888935
         0.8967291504209932 2.506948771242972
         0.25529404008730594 2.922302861104415
         """
 
-        points = [[0.13436424411240122, 4.323216008886963],
-                  [0.020818108509287336, 5.1051826661880515],
-                  [0.1028341459863098, 4.9409270526888935],
-                  [0.8967291504209932, 2.506948771242972],
-                  [0.25529404008730594, 2.922302861104415]]
+        points = [
+            [0.13436424411240122, 4.323216008886963],
+            [0.020818108509287336, 5.1051826661880515],
+            [0.1028341459863098, 4.9409270526888935],
+            [0.8967291504209932, 2.506948771242972],
+            [0.25529404008730594, 2.922302861104415],
+        ]
 
         population = []
         for i in range(len(points)):
             population.append(Solution(2, 2))
             population[i].objectives = points[i]
 
         self.knn.compute_density_estimator(population)
```

### Comparing `jmetalpy-1.5.5/jmetal/util/test/test_distance.py` & `jmetalpy-1.6.0/jmetal/util/test/test_distance.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 import unittest
 
 from jmetal.util.distance import EuclideanDistance
 
 
 class EuclideanDistanceTestCases(unittest.TestCase):
-
     def test_should_get_distance_work_properly_case_1(self):
-        """ Case 1: [1], [1] -> distance == 0 """
+        """Case 1: [1], [1] -> distance == 0"""
         distance = EuclideanDistance()
 
         self.assertEqual(0, distance.get_distance([1], [1]))
 
     def test_should_get_distance_work_properly_case_2(self):
-        """ Case 2: [1, 0, 0], [0, 1, 0] -> distance == 1.4142135623730951 """
+        """Case 2: [1, 0, 0], [0, 1, 0] -> distance == 1.4142135623730951"""
         distance = EuclideanDistance()
 
         self.assertEqual(1.4142135623730951, distance.get_distance([1, 0, 0], [0, 1, 0]))
 
     def test_should_get_distance_work_properly_case_3(self):
-        """ Case 3: [1, 1, 0], [0, 1, 0] -> distance == 1.0 """
+        """Case 3: [1, 1, 0], [0, 1, 0] -> distance == 1.0"""
         distance = EuclideanDistance()
 
         self.assertEqual(1.0, distance.get_distance([1, 1, 0], [0, 1, 0]))
 
 
 """
 class CosineDistanceTestCases(unittest.TestCase):
@@ -41,9 +40,9 @@
     def test_should_two_perpendicular_points_have_a_distance_of_one(self):
         reference_point = [0.0, 0.0]
         distance = CosineDistance(reference_point)
 
         self.assertEqual(1.0, distance.get_distance([0.0, 1.0], [1.0, 0.0]))
 """
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `jmetalpy-1.5.5/jmetal/util/test/test_neighborhood.py` & `jmetalpy-1.6.0/jmetal/util/test/test_neighborhood.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import unittest
 
 import numpy
 
 from jmetal.core.solution import Solution
-from jmetal.util.ckecking import NoneParameterException, InvalidConditionException
-from jmetal.util.neighborhood import WeightVectorNeighborhood, TwoDimensionalMesh, L5
+from jmetal.util.ckecking import InvalidConditionException, NoneParameterException
+from jmetal.util.neighborhood import L5, TwoDimensionalMesh, WeightVectorNeighborhood
 
 
 class WeightVectorNeighborhoodTestCases(unittest.TestCase):
-
     def test_should_constructor_work_properly(self) -> None:
         number_of_weight_vectors = 100
         neighborhood_size = 20
         neighborhood: WeightVectorNeighborhood = WeightVectorNeighborhood(number_of_weight_vectors, neighborhood_size)
 
         self.assertEqual(number_of_weight_vectors, neighborhood.number_of_weight_vectors)
         self.assertEqual(neighborhood_size, neighborhood.neighborhood_size)
@@ -21,18 +20,26 @@
         self.assertEqual(0.0, neighborhood.weight_vectors[0][0])
         self.assertEqual(1.0, neighborhood.weight_vectors[0][1])
         self.assertEqual(0.0101010101010101010101, neighborhood.weight_vectors[1][0])
         self.assertEqual(0.989898989898989898, neighborhood.weight_vectors[1][1])
         self.assertEqual(1.0, neighborhood.weight_vectors[99][0])
         self.assertEqual(0.0, neighborhood.weight_vectors[99][1])
 
-        self.assertTrue(numpy.array_equal(numpy.array([0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19]),
-                         neighborhood.neighborhood[0]))
-        self.assertTrue(numpy.array_equal(numpy.array([69, 70, 68, 71, 67, 72, 66, 73, 65, 64, 74, 75, 63, 76, 62, 77, 61, 78, 60, 79]),
-                         neighborhood.neighborhood[69]))
+        self.assertTrue(
+            numpy.array_equal(
+                numpy.array([0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19]),
+                neighborhood.neighborhood[0],
+            )
+        )
+        self.assertTrue(
+            numpy.array_equal(
+                numpy.array([69, 70, 68, 71, 67, 72, 66, 73, 65, 64, 74, 75, 63, 76, 62, 77, 61, 78, 60, 79]),
+                neighborhood.neighborhood[69],
+            )
+        )
 
     def test_should_get_neighbors_work_properly_with_two_objectives(self):
         number_of_weight_vectors = 100
         neighborhood_size = 20
         neighborhood: WeightVectorNeighborhood = WeightVectorNeighborhood(number_of_weight_vectors, neighborhood_size)
 
         solution_list = [Solution(2, 2) for _ in range(number_of_weight_vectors)]
@@ -221,15 +228,15 @@
         Solution location: 0; the neighborhood is: 0, 1
         """
         rows = 1
         columns = 2
         solution_list = []
         for i in range(rows * columns):
             solution = Solution(i, 2)
-            solution.variables = [i, i+1]
+            solution.variables = [i, i + 1]
             solution_list.append(solution)
         neighborhood = L5(rows, columns)
 
         result = neighborhood.get_neighbors(0, solution_list)
         self.assertEqual(4, len(result))
         self.assertTrue(solution_list[0] in result)
         self.assertTrue(solution_list[1] in result)
@@ -272,9 +279,9 @@
         self.assertTrue(solution_list[3] not in result)
         self.assertTrue(solution_list[0] not in result)
 
         self.assertEqual(2, result.count(solution_list[1]))
         self.assertEqual(2, result.count(solution_list[2]))
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `jmetalpy-1.5.5/jmetal/util/test/test_point.py` & `jmetalpy-1.6.0/jmetal/util/test/test_point.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import unittest
 
 from jmetal.util.point import IdealPoint
 
 
 class IdealPointTestCases(unittest.TestCase):
-
     def test_should_constructor_create_a_correctly_initialized_point(self) -> None:
         point = IdealPoint(2)
 
         self.assertEqual(2, len(point.point))
         self.assertEqual(2 * [float("inf")], point.point)
 
     def test_should_update_with_one_point_work_properly(self) -> None:
@@ -36,9 +35,9 @@
         point.update([3.0, 1.0, 2.0])
         point.update([0.2, 4.0, 5.5])
         point.update([5.0, 6.0, 1.5])
 
         self.assertEqual([0.2, 1.0, 1.5], point.point)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `jmetalpy-1.5.5/jmetal/util/test/test_ranking.py` & `jmetalpy-1.6.0/jmetal/util/test/test_ranking.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import unittest
 
 from jmetal.core.solution import Solution
-from jmetal.util.ranking import FastNonDominatedRanking, StrengthRanking, Ranking
+from jmetal.util.ranking import FastNonDominatedRanking, Ranking, StrengthRanking
 
 
 class FastNonDominatedRankingTestCases(unittest.TestCase):
-
     def setUp(self):
         self.ranking = FastNonDominatedRanking()
 
     def test_should_constructor_create_a_valid_object(self):
         self.assertIsNotNone(self.ranking)
 
     def test_should_compute_ranking_of_an_emtpy_solution_list_return_a_empty_list_of_subranks(self):
@@ -37,16 +36,15 @@
 
         self.assertEqual(1, self.ranking.get_number_of_subfronts())
         self.assertEqual(2, len(self.ranking.get_subfront(0)))
         self.assertEqual(solution, ranking[0][0])
         self.assertEqual(solution2, ranking[0][1])
 
     def test_should_compute_ranking_work_properly_case1(self):
-        """ The list contains two solutions and one of them is dominated by the other one.
-        """
+        """The list contains two solutions and one of them is dominated by the other one."""
         solution = Solution(2, 2)
         solution.objectives = [2, 3]
         solution2 = Solution(2, 2)
         solution2.objectives = [3, 6]
         solution_list = [solution, solution2]
 
         ranking = self.ranking.compute_ranking(solution_list)
@@ -105,16 +103,15 @@
         self.assertEqual(solution1, ranking[0][0])
         self.assertEqual(solution2, ranking[0][1])
         self.assertEqual(solution3, ranking[0][2])
         self.assertEqual(solution4, ranking[1][0])
         self.assertEqual(solution5, ranking[1][1])
 
     def test_should_compute_ranking_work_properly_with_constraints_case1(self):
-        """ The list contains two solutions and one is infeasible
-        """
+        """The list contains two solutions and one is infeasible"""
         solution = Solution(2, 2, 1)
         solution.objectives = [2, 3]
         solution.constraints[0] = -1
         solution2 = Solution(2, 2, 1)
         solution2.objectives = [3, 6]
         solution2.constraints[0] = 0
         solution_list = [solution, solution2]
@@ -122,16 +119,15 @@
         ranking = self.ranking.compute_ranking(solution_list)
 
         self.assertEqual(2, self.ranking.get_number_of_subfronts())
         self.assertEqual(solution2, ranking[0][0])
         self.assertEqual(solution, ranking[1][0])
 
     def test_should_compute_ranking_work_properly_with_constraints_case2(self):
-        """ The list contains two solutions and both are infeasible with different violation degree
-        """
+        """The list contains two solutions and both are infeasible with different violation degree"""
         solution = Solution(2, 2, 1)
         solution.objectives = [2, 3]
         solution.constraints[0] = -1
         solution2 = Solution(2, 2, 1)
         solution2.objectives = [3, 6]
         solution2.constraints[0] = -2
         solution_list = [solution, solution2]
@@ -139,16 +135,15 @@
         ranking = self.ranking.compute_ranking(solution_list)
 
         self.assertEqual(2, self.ranking.get_number_of_subfronts())
         self.assertEqual(solution, ranking[0][0])
         self.assertEqual(solution2, ranking[1][0])
 
     def test_should_compute_ranking_work_properly_with_constraints_case3(self):
-        """ The list contains two solutions and both are infeasible with equal violation degree
-        """
+        """The list contains two solutions and both are infeasible with equal violation degree"""
         solution = Solution(2, 2, 1)
         solution.objectives = [2, 3]
         solution.constraints[0] = -1
         solution2 = Solution(2, 2, 1)
         solution2.objectives = [3, 6]
         solution2.constraints[0] = -1
         solution_list = [solution, solution2]
@@ -157,28 +152,27 @@
 
         self.assertEqual(2, self.ranking.get_number_of_subfronts())
         self.assertEqual(solution, ranking[0][0])
         self.assertEqual(solution2, ranking[1][0])
 
 
 class StrengthRankingTestCases(unittest.TestCase):
-
     def setUp(self):
-        self.ranking:Ranking = StrengthRanking()
+        self.ranking: Ranking = StrengthRanking()
 
     def test_should_ranking_assing_zero_to_all_the_solutions_if_they_are_nondominated(self):
         """
-          5 1
-          4   2
-          3     3
-          2
-          1         4
-          0 1 2 3 4 5
+        5 1
+        4   2
+        3     3
+        2
+        1         4
+        0 1 2 3 4 5
 
-          Points 1, 2, 3 and 4 are nondominated
+        Points 1, 2, 3 and 4 are nondominated
         """
         solution1 = Solution(2, 2)
         solution1.objectives = [1, 5]
         solution2 = Solution(2, 2)
         solution2.objectives = [2, 4]
         solution3 = Solution(2, 2)
         solution3.objectives = [3, 3]
@@ -193,23 +187,23 @@
         self.assertTrue(solution1 in ranking[0])
         self.assertTrue(solution2 in ranking[0])
         self.assertTrue(solution3 in ranking[0])
         self.assertTrue(solution4 in ranking[0])
 
     def test_should_ranking_work_properly(self):
         """
-          5 1
-          4   2
-          3     3
-          2     5
-          1         4
-          0 1 2 3 4 5
+        5 1
+        4   2
+        3     3
+        2     5
+        1         4
+        0 1 2 3 4 5
 
-          Solutions: 1, 2, 3, 4, 5
-          Expected result: two ranks (rank 0: 1, 2, 5, 4; rank 1: 3)
+        Solutions: 1, 2, 3, 4, 5
+        Expected result: two ranks (rank 0: 1, 2, 5, 4; rank 1: 3)
         """
 
         solution1 = Solution(2, 2)
         solution1.objectives = [1, 5]
         solution2 = Solution(2, 2)
         solution2.objectives = [2, 4]
         solution3 = Solution(2, 2)
@@ -225,16 +219,16 @@
 
         self.assertEqual(2, self.ranking.get_number_of_subfronts())
         self.assertTrue(solution1 in self.ranking.get_subfront(0))
         self.assertTrue(solution2 in self.ranking.get_subfront(0))
         self.assertTrue(solution3 in self.ranking.get_subfront(1))
         self.assertTrue(solution4 in self.ranking.get_subfront(0))
         self.assertTrue(solution5 in self.ranking.get_subfront(0))
-        self.assertEqual(0, solution1.attributes['strength_ranking'])
-        self.assertEqual(0, solution2.attributes['strength_ranking'])
-        self.assertEqual(1, solution3.attributes['strength_ranking'])
-        self.assertEqual(0, solution4.attributes['strength_ranking'])
-        self.assertEqual(0, solution5.attributes['strength_ranking'])
+        self.assertEqual(0, solution1.attributes["strength_ranking"])
+        self.assertEqual(0, solution2.attributes["strength_ranking"])
+        self.assertEqual(1, solution3.attributes["strength_ranking"])
+        self.assertEqual(0, solution4.attributes["strength_ranking"])
+        self.assertEqual(0, solution5.attributes["strength_ranking"])
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `jmetalpy-1.5.5/jmetal/util/test/test_replacement.py` & `jmetalpy-1.6.0/jmetal/util/test/test_replacement.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 import unittest
 
 from jmetal.core.solution import Solution
 from jmetal.util.density_estimator import KNearestNeighborDensityEstimator
-from jmetal.util.ranking import StrengthRanking, FastNonDominatedRanking
+from jmetal.util.ranking import FastNonDominatedRanking, StrengthRanking
 from jmetal.util.replacement import RankingAndDensityEstimatorReplacement
 
 
 class RankingAndDensityEstimatorReplacementTestCases(unittest.TestCase):
-
     def test_should_replacement_return_the_list_if_the_offspring_list_is_empty(self):
         """
-         5 1
-         4   2
-         3     3
-         2
-         1         4
-         0 1 2 3 4 5
+        5 1
+        4   2
+        3     3
+        2
+        1         4
+        0 1 2 3 4 5
         """
         ranking = StrengthRanking()
         density_estimator = KNearestNeighborDensityEstimator(1)
 
         replacement = RankingAndDensityEstimatorReplacement(ranking, density_estimator)
 
         solution1 = Solution(2, 2)
@@ -31,30 +30,30 @@
         solution4 = Solution(2, 2)
         solution4.objectives = [5, 1]
 
         solution_list = [solution1, solution2, solution3, solution4]
         result_list = replacement.replace(solution_list, [])
 
         self.assertEqual(4, len(result_list))
-        self.assertEqual(0, solution1.attributes['strength_ranking'])
-        self.assertEqual(0, solution2.attributes['strength_ranking'])
-        self.assertEqual(0, solution3.attributes['strength_ranking'])
-        self.assertEqual(0, solution4.attributes['strength_ranking'])
+        self.assertEqual(0, solution1.attributes["strength_ranking"])
+        self.assertEqual(0, solution2.attributes["strength_ranking"])
+        self.assertEqual(0, solution3.attributes["strength_ranking"])
+        self.assertEqual(0, solution4.attributes["strength_ranking"])
 
     def test_should_replacement_return_the_right_value_case1(self):
         """
-         5 1
-         4   2
-         3     3
-         2
-         1         4
-         0 1 2 3 4 5
+        5 1
+        4   2
+        3     3
+        2
+        1         4
+        0 1 2 3 4 5
 
-         List: 1,2,3   OffspringList: 4
-         Expected result: 4, 1, 3
+        List: 1,2,3   OffspringList: 4
+        Expected result: 4, 1, 3
         """
         ranking = StrengthRanking()
         density_estimator = KNearestNeighborDensityEstimator(1)
 
         replacement = RankingAndDensityEstimatorReplacement(ranking, density_estimator)
 
         solution1 = Solution(2, 2)
@@ -73,23 +72,23 @@
         self.assertEqual(3, len(result_list))
         self.assertTrue(solution1 in result_list)
         self.assertTrue(solution3 in result_list)
         self.assertTrue(solution4 in result_list)
 
     def test_should_replacement_return_the_right_value_case2(self):
         """
-         5 1
-         4   2
-         3     3
-         2    5
-         1         4
-         0 1 2 3 4 5
+        5 1
+        4   2
+        3     3
+        2    5
+        1         4
+        0 1 2 3 4 5
 
-         List: 1,2,4   OffspringList: 3,5
-         Expected result: 1, 5, 4
+        List: 1,2,4   OffspringList: 3,5
+        Expected result: 1, 5, 4
         """
         ranking = StrengthRanking()
         density_estimator = KNearestNeighborDensityEstimator(1)
 
         replacement = RankingAndDensityEstimatorReplacement(ranking, density_estimator)
 
         solution1 = Solution(2, 2)
@@ -103,50 +102,53 @@
         solution5 = Solution(2, 2)
         solution5.objectives = [2.5, 2.5]
 
         solution_list = [solution1, solution2, solution4]
         offspring_list = [solution3, solution5]
         result_list = replacement.replace(solution_list, offspring_list)
 
-        self.assertEqual(0, solution1.attributes['strength_ranking'])
-        self.assertEqual(0, solution2.attributes['strength_ranking'])
-        self.assertEqual(1, solution3.attributes['strength_ranking'])
-        self.assertEqual(0, solution4.attributes['strength_ranking'])
-        self.assertEqual(0, solution5.attributes['strength_ranking'])
+        self.assertEqual(0, solution1.attributes["strength_ranking"])
+        self.assertEqual(0, solution2.attributes["strength_ranking"])
+        self.assertEqual(1, solution3.attributes["strength_ranking"])
+        self.assertEqual(0, solution4.attributes["strength_ranking"])
+        self.assertEqual(0, solution5.attributes["strength_ranking"])
 
         self.assertEqual(3, len(result_list))
         self.assertTrue(solution1 in result_list)
         self.assertTrue(solution5 in result_list)
         self.assertTrue(solution4 in result_list)
 
     def test_should_replacement_return_the_right_value_case3(self):
-        """
-         """
+        """"""
 
-        points_population = [[0.13436424411240122, 4.323216008886963],
-                             [0.23308445025757263, 4.574937990387161],
-                             [0.17300740157905092, 4.82329350808847],
-                             [0.9571162814602269, 3.443495331489301],
-                             [0.25529404008730594, 3.36387501100745],
-                             [0.020818108509287336, 5.1051826661880515],
-                             [0.8787178982088466, 3.2716009445324103],
-                             [0.6744550697237632, 3.901350307095427],
-                             [0.7881164487252263, 3.1796004913916516],
-                             [0.1028341459863098, 4.9409270526888935]]
-
-        points_offspring_population = [[0.3150521745650882, 4.369120371847888],
-                                       [0.8967291504209932, 2.506948771242972],
-                                       [0.6744550697237632, 3.9361442668874504],
-                                       [0.9571162814602269, 3.4388386707431433],
-                                       [0.13436424411240122, 4.741872175943253],
-                                       [0.25529404008730594, 2.922302861104415],
-                                       [0.23308445025757263, 4.580180404770213],
-                                       [0.23308445025757263, 4.591260299892424],
-                                       [0.9571162814602269, 2.9865495383518694],
-                                       [0.25529404008730594, 3.875587748122183]]
+        points_population = [
+            [0.13436424411240122, 4.323216008886963],
+            [0.23308445025757263, 4.574937990387161],
+            [0.17300740157905092, 4.82329350808847],
+            [0.9571162814602269, 3.443495331489301],
+            [0.25529404008730594, 3.36387501100745],
+            [0.020818108509287336, 5.1051826661880515],
+            [0.8787178982088466, 3.2716009445324103],
+            [0.6744550697237632, 3.901350307095427],
+            [0.7881164487252263, 3.1796004913916516],
+            [0.1028341459863098, 4.9409270526888935],
+        ]
+
+        points_offspring_population = [
+            [0.3150521745650882, 4.369120371847888],
+            [0.8967291504209932, 2.506948771242972],
+            [0.6744550697237632, 3.9361442668874504],
+            [0.9571162814602269, 3.4388386707431433],
+            [0.13436424411240122, 4.741872175943253],
+            [0.25529404008730594, 2.922302861104415],
+            [0.23308445025757263, 4.580180404770213],
+            [0.23308445025757263, 4.591260299892424],
+            [0.9571162814602269, 2.9865495383518694],
+            [0.25529404008730594, 3.875587748122183],
+        ]
 
         ranking = FastNonDominatedRanking()
         density_estimator = KNearestNeighborDensityEstimator(1)
 
         population = []
         for i in range(len(points_population)):
             population.append(Solution(2, 2))
@@ -156,19 +158,17 @@
         for i in range(len(points_offspring_population)):
             offspring_population.append(Solution(2, 2))
             offspring_population[i].objectives = points_offspring_population[i]
 
         replacement = RankingAndDensityEstimatorReplacement(ranking, density_estimator)
         result_list = replacement.replace(population, offspring_population)
 
-        self.assertEqual(10,len(result_list))
+        self.assertEqual(10, len(result_list))
 
         for solution in result_list[0:4]:
-            self.assertEqual(0, solution.attributes['dominance_ranking'])
+            self.assertEqual(0, solution.attributes["dominance_ranking"])
         for solution in result_list[5:9]:
-            self.assertEqual(1, solution.attributes['dominance_ranking'])
-
-
+            self.assertEqual(1, solution.attributes["dominance_ranking"])
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `jmetalpy-1.5.5/jmetalpy.egg-info/PKG-INFO` & `jmetalpy-1.6.0/jmetalpy.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,147 +1,155 @@
 Metadata-Version: 2.1
 Name: jmetalpy
-Version: 1.5.5
+Version: 1.6.0
 Summary: Python version of the jMetal framework
 Home-page: https://github.com/jMetal/jMetalPy
 Author: Antonio J. Nebro
 Author-email: antonio@lcc.uma.es
-Maintainer: Antonio J. Nebro, Antonio Benitez-Hidalgo
-Maintainer-email: antonio@lcc.uma.es, antonio.benitez@lcc.uma.es
 License: MIT
-Description: ![jMetalPy](docs/source/jmetalpy.png)
-        
-        [![Build Status](https://img.shields.io/travis/jMetal/jMetalPy/master.svg?style=flat-square)](https://travis-ci.org/jMetal/jMetalPy)
-        [![Documentation](https://img.shields.io/badge/docs-online-success?style=flat-square)](https://jmetal.github.io/jMetalPy/index.html)
-        [![PyPI License](https://img.shields.io/pypi/l/jMetalPy.svg?style=flat-square)]()
-        [![PyPI version](https://img.shields.io/pypi/v/jMetalPy.svg?style=flat-square)]()
-        [![PyPI Python version](https://img.shields.io/pypi/pyversions/jMetalPy.svg?style=flat-square)]()
-        
-        A paper introducing jMetalPy is available at: https://doi.org/10.1016/j.swevo.2019.100598
-        
-        ### Table of Contents
-        - [Installation](#installation)
-        - [Usage](#hello-world-)
-        - [Features](#features)
-        - [Changelog](#changelog)
-        - [License](#license)
-        
-        ## Installation
-        
-        You can install the latest version of jMetalPy with `pip`, 
-        
-        ```console
-        pip install jmetalpy  # or "jmetalpy[distributed]"
-        ```
-        
-        <details><summary><b>Notes on installing with <tt>pip</tt></b></summary>
-        <p>
-        
-        jMetalPy includes features for parallel and distributed computing based on [pySpark](https://spark.apache.org/docs/latest/api/python/index.html) and [Dask](https://dask.org/).
-        
-        These (extra) dependencies are *not* automatically installed when running `pip`, which only comprises the core functionality of the framework (enough for most users):
-        
-        ```console
-        pip install jmetalpy
-        ```
-        
-        This is the equivalent of running: 
-        
-        ```console
-        pip install "jmetalpy[core]"
-        ```
-        
-        Other supported commands are listed next:
-        
-        ```console
-        pip install "jmetalpy[docs]"  # Install requirements for building docs
-        pip install "jmetalpy[distributed]"  # Install requirements for parallel/distributed computing
-        pip install "jmetalpy[complete]"  # Install all requirements
-        ```
-        
-        </p>
-        </details>
-        
-        ## Hello, world! 👋
-        
-        Examples of configuring and running all the included algorithms are located [in the documentation](https://jmetal.github.io/jMetalPy/multiobjective.algorithms.html).
-        
-        ```python
-        from jmetal.algorithm.multiobjective import NSGAII
-        from jmetal.operator import SBXCrossover, PolynomialMutation
-        from jmetal.problem import ZDT1
-        from jmetal.util.termination_criterion import StoppingByEvaluations
-        
-        problem = ZDT1()
-        
-        algorithm = NSGAII(
-            problem=problem,
-            population_size=100,
-            offspring_population_size=100,
-            mutation=PolynomialMutation(probability=1.0 / problem.number_of_variables, distribution_index=20),
-            crossover=SBXCrossover(probability=1.0, distribution_index=20),
-            termination_criterion=StoppingByEvaluations(max_evaluations=25000)
-        )
-        
-        algorithm.run()
-        ```
-        
-        We can then proceed to explore the results:
-        
-        ```python
-        from jmetal.util.solution import get_non_dominated_solutions, print_function_values_to_file, \ 
-            print_variables_to_file
-        
-        front = get_non_dominated_solutions(algorithm.get_result())
-        
-        # save to files
-        print_function_values_to_file(front, 'FUN.NSGAII.ZDT1')
-        print_variables_to_file(front, 'VAR.NSGAII.ZDT1')
-        ```
-        
-        Or visualize the Pareto front approximation produced by the algorithm:
-        
-        ```python
-        from jmetal.lab.visualization import Plot
-        
-        plot_front = Plot(title='Pareto front approximation', axis_labels=['x', 'y'])
-        plot_front.plot(front, label='NSGAII-ZDT1', filename='NSGAII-ZDT1', format='png')
-        ```
-        
-        <img src=docs/source/_static/NSGAII-ZDT1.png width=450 alt="Pareto front approximation">
-        
-        ## Features
-        The current release of jMetalPy (v1.5.5) contains the following components:
-        
-        * Algorithms: local search, genetic algorithm, evolution strategy, simulated annealing, random search, NSGA-II, NSGA-III, SMPSO, OMOPSO, MOEA/D, MOEA/D-DRA, MOEA/D-IEpsilon, GDE3, SPEA2, HYPE, IBEA. Preference articulation-based algorithms (G-NSGA-II, G-GDE3, G-SPEA2, SMPSO/RP); Dynamic versions of NSGA-II, SMPSO, and GDE3.
-        * Parallel computing based on Apache Spark and Dask.
-        * Benchmark problems: ZDT1-6, DTLZ1-2, FDA, LZ09, LIR-CMOP, unconstrained (Kursawe, Fonseca, Schaffer, Viennet2), constrained (Srinivas, Tanaka).
-        * Encodings: real, binary, permutations.
-        * Operators: selection (binary tournament, ranking and crowding distance, random, nary random, best solution), crossover (single-point, SBX), mutation (bit-blip, polynomial, uniform, random).
-        * Quality indicators: hypervolume, additive epsilon, GD, IGD.
-        * Pareto front approximation plotting in real-time, static or interactive.
-        * Experiment class for performing studies either alone or alongside [jMetal](https://github.com/jMetal/jMetal).
-        * Pairwise and multiple hypothesis testing for statistical analysis, including several frequentist and Bayesian testing methods, critical distance plots and posterior diagrams.
-        
-        | ![Scatter plot 2D](docs/source/_static/2D.gif) | ![Scatter plot 3D](docs/source/_static/3D.gif) |
-        |-------------- | ----------------  |
-        | ![Parallel coordinates](docs/source/_static/p-c.gif) | ![Interactive chord plot](docs/source/_static/chordplot.gif) |
-        
-        ## Changelog
-        
-        * [v1.5.5] Minor bug fixes.
-        * [v1.5.4] Refactored quality indicators to accept numpy array as input parameter.
-        * [v1.5.4] Added [CompositeSolution](https://github.com/jMetal/jMetalPy/blob/master/jmetal/core/solution.py#L111) class to support mixed combinatorial problems. [#69](https://github.com/jMetal/jMetalPy/issues/69)
-        
-        ## License
-        This project is licensed under the terms of the MIT - see the [LICENSE](LICENSE) file for details.
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Project-URL: Source, https://github.com/jMetal/jMetalPy
+Project-URL: Tracker, https://github.com/jMetal/jMetalPy/issues
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Programming Language :: Python :: 3.6
-Description-Content-Type: text/markdown
-Provides-Extra: core
-Provides-Extra: docs
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown; charset=UTF-8
 Provides-Extra: distributed
-Provides-Extra: complete
+Provides-Extra: dev
+Provides-Extra: test
+Provides-Extra: all
+License-File: LICENSE
+
+![jMetalPy](docs/source/jmetalpy.png)
+
+[![CI](https://github.com/jMetal/jMetalPy/actions/workflows/ci.yml/badge.svg)](https://github.com/jMetal/jMetalPy/actions/workflows/ci.yml)
+[![PyPI Python version](https://img.shields.io/pypi/pyversions/jMetalPy.svg)]()
+[![DOI](https://img.shields.io/badge/DOI-10.1016%2Fj.swevo.2019.100598-blue)](https://doi.org/10.1016/j.swevo.2019.100598)
+[![PyPI License](https://img.shields.io/pypi/l/jMetalPy.svg)]()
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+A paper introducing jMetalPy is available at: https://doi.org/10.1016/j.swevo.2019.100598
+
+### Table of Contents
+- [Installation](#installation)
+- [Usage](#hello-world-)
+- [Features](#features)
+- [Changelog](#changelog)
+- [License](#license)
+
+## Installation
+
+You can install the latest version of jMetalPy with `pip`, 
+
+```console
+pip install jmetalpy  # or "jmetalpy[distributed]"
+```
+
+<details><summary><b>Notes on installing with <tt>pip</tt></b></summary>
+<p>
+
+jMetalPy includes features for parallel and distributed computing based on [pySpark](https://spark.apache.org/docs/latest/api/python/index.html) and [Dask](https://dask.org/).
+
+These (extra) dependencies are *not* automatically installed when running `pip`, which only comprises the core functionality of the framework (enough for most users):
+
+```console
+pip install jmetalpy
+```
+
+This is the equivalent of running: 
+
+```console
+pip install "jmetalpy[core]"
+```
+
+Other supported commands are listed next:
+
+```console
+pip install "jmetalpy[dev]"  # Install requirements for development
+pip install "jmetalpy[distributed]"  # Install requirements for parallel/distributed computing
+pip install "jmetalpy[complete]"  # Install all requirements
+```
+
+</p>
+</details>
+
+## Hello, world! 👋
+
+Examples of configuring and running all the included algorithms are located [in the documentation](https://jmetal.github.io/jMetalPy/multiobjective.algorithms.html).
+
+```python
+from jmetal.algorithm.multiobjective import NSGAII
+from jmetal.operator import SBXCrossover, PolynomialMutation
+from jmetal.problem import ZDT1
+from jmetal.util.termination_criterion import StoppingByEvaluations
+
+problem = ZDT1()
+
+algorithm = NSGAII(
+    problem=problem,
+    population_size=100,
+    offspring_population_size=100,
+    mutation=PolynomialMutation(probability=1.0 / problem.number_of_variables, distribution_index=20),
+    crossover=SBXCrossover(probability=1.0, distribution_index=20),
+    termination_criterion=StoppingByEvaluations(max_evaluations=25000)
+)
+
+algorithm.run()
+```
+
+We can then proceed to explore the results:
+
+```python
+from jmetal.util.solution import get_non_dominated_solutions, print_function_values_to_file, \ 
+    print_variables_to_file
+
+front = get_non_dominated_solutions(algorithm.get_result())
+
+# save to files
+print_function_values_to_file(front, 'FUN.NSGAII.ZDT1')
+print_variables_to_file(front, 'VAR.NSGAII.ZDT1')
+```
+
+Or visualize the Pareto front approximation produced by the algorithm:
+
+```python
+from jmetal.lab.visualization import Plot
+
+plot_front = Plot(title='Pareto front approximation', axis_labels=['x', 'y'])
+plot_front.plot(front, label='NSGAII-ZDT1', filename='NSGAII-ZDT1', format='png')
+```
+
+<img src=docs/source/_static/NSGAII-ZDT1.png width=450 alt="Pareto front approximation">
+
+## Features
+The current release of jMetalPy (v1.5.7) contains the following components:
+
+* Algorithms: local search, genetic algorithm, evolution strategy, simulated annealing, random search, NSGA-II, NSGA-III, SMPSO, OMOPSO, MOEA/D, MOEA/D-DRA, MOEA/D-IEpsilon, GDE3, SPEA2, HYPE, IBEA. Preference articulation-based algorithms (G-NSGA-II, G-GDE3, G-SPEA2, SMPSO/RP); Dynamic versions of NSGA-II, SMPSO, and GDE3.
+* Parallel computing based on Apache Spark and Dask.
+* Benchmark problems: ZDT1-6, DTLZ1-2, FDA, LZ09, LIR-CMOP, unconstrained (Kursawe, Fonseca, Schaffer, Viennet2), constrained (Srinivas, Tanaka).
+* Encodings: real, binary, permutations.
+* Operators: selection (binary tournament, ranking and crowding distance, random, nary random, best solution), crossover (single-point, SBX), mutation (bit-blip, polynomial, uniform, random).
+* Quality indicators: hypervolume, additive epsilon, GD, IGD.
+* Pareto front approximation plotting in real-time, static or interactive.
+* Experiment class for performing studies either alone or alongside [jMetal](https://github.com/jMetal/jMetal).
+* Pairwise and multiple hypothesis testing for statistical analysis, including several frequentist and Bayesian testing methods, critical distance plots and posterior diagrams.
+
+| ![Scatter plot 2D](docs/source/_static/2D.gif) | ![Scatter plot 3D](docs/source/_static/3D.gif) |
+|-------------- | ----------------  |
+| ![Parallel coordinates](docs/source/_static/p-c.gif) | ![Interactive chord plot](docs/source/_static/chordplot.gif) |
+
+## Changelog
+
+* [v1.6.0] Refactor class Problem, the single-objective genetic algorithm can solve constrained problems, performance improvements in NSGA-II, generation of Latex tables summarizing the results of the Wilcoxon rank sum test, added a notebook folder with examples.
+* [v1.5.7] Use of linters for catching errors and formatters to fix style, minor bug fixes.
+* [v1.5.6] Removed warnings when using Python 3.8.
+* [v1.5.5] Minor bug fixes.
+* [v1.5.4] Refactored quality indicators to accept numpy array as input parameter.
+* [v1.5.4] Added [CompositeSolution](https://github.com/jMetal/jMetalPy/blob/master/jmetal/core/solution.py#L111) class to support mixed combinatorial problems. [#69](https://github.com/jMetal/jMetalPy/issues/69)
+
+## License
+
+This project is licensed under the terms of the MIT - see the [LICENSE](LICENSE) file for details.
```

### Comparing `jmetalpy-1.5.5/jmetalpy.egg-info/SOURCES.txt` & `jmetalpy-1.6.0/jmetalpy.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+LICENSE
 README.md
+pyproject.toml
 setup.cfg
 setup.py
 examples/__init__.py
 examples/experiment/__init__.py
 examples/experiment/comparison.py
+examples/experiment/generateMedianAndWilcoxonLatexTables.py
 examples/experiment/statistical_analysis.py
 examples/multiobjective/__init__.py
 examples/multiobjective/gde3/__init__.py
 examples/multiobjective/gde3/dynamic_gde3.py
 examples/multiobjective/gde3/gde3_spark_evaluator.py
 examples/multiobjective/gde3/gde3_zdt1.py
 examples/multiobjective/gde3/ggde3_zdt2.py
@@ -23,15 +26,14 @@
 examples/multiobjective/moead/moead_lz09.py
 examples/multiobjective/moead/moeaddra_lz09.py
 examples/multiobjective/nsgaii/__init__.py
 examples/multiobjective/nsgaii/distributed_nsgaii_with_dask.py
 examples/multiobjective/nsgaii/distributed_nsgaii_with_dask_evaluator.py
 examples/multiobjective/nsgaii/distributed_nsgaii_with_spark_evaluator.py
 examples/multiobjective/nsgaii/dynamic_nsgaii_solving_fda2.py
-examples/multiobjective/nsgaii/gnsgaii_solving_zdt2_with_reference_point.py
 examples/multiobjective/nsgaii/nsgaii_defining_schaffer_problem_on_the_fly.py
 examples/multiobjective/nsgaii/nsgaii_defining_srinivas_problem_on_the_fly.py
 examples/multiobjective/nsgaii/nsgaii_solving_3D_problem.py
 examples/multiobjective/nsgaii/nsgaii_solving_binary_problem.py
 examples/multiobjective/nsgaii/nsgaii_solving_constrained_srinivas_problem.py
 examples/multiobjective/nsgaii/nsgaii_solving_mixed_encoding_problem.py
 examples/multiobjective/nsgaii/nsgaii_ssp.py
@@ -41,51 +43,58 @@
 examples/multiobjective/nsgaii/nsgaii_steady_state_with_real_time_plotting.py
 examples/multiobjective/nsgaii/parallel_nsgaii_with_multiprocess_evaluator.py
 examples/multiobjective/nsgaiii/__init__.py
 examples/multiobjective/nsgaiii/nsgaiii_dtlz2.py
 examples/multiobjective/omopso/__init__.py
 examples/multiobjective/omopso/omopso_spark_evaluator.py
 examples/multiobjective/omopso/omopso_zdt1.py
+examples/multiobjective/preferences/__init__.py
+examples/multiobjective/preferences/ggde3_zdt2.py
+examples/multiobjective/preferences/gnsgaii_solving_zdt2_with_reference_point.py
 examples/multiobjective/random_search/__init__.py
 examples/multiobjective/random_search/random_search_zdt1.py
 examples/multiobjective/smpso/__init__.py
 examples/multiobjective/smpso/dynamic_smpso.py
 examples/multiobjective/smpso/smpso_schaffer_on_the_fly.py
 examples/multiobjective/smpso/smpso_spark_evaluator.py
-examples/multiobjective/smpso/smpso_srinivas.py
 examples/multiobjective/smpso/smpso_srinivas_on_the_fly.py
+examples/multiobjective/smpso/smpso_tanaka.py
 examples/multiobjective/smpso/smpso_zdt4.py
 examples/multiobjective/smpso/smpsorp_zdt4.py
 examples/multiobjective/spea2/__init__.py
 examples/multiobjective/spea2/gspea2_zdt1.py
 examples/multiobjective/spea2/spea2_dtlz1.py
 examples/multiobjective/spea2/spea2_zdt1.py
 examples/singleobjective/__init__.py
 examples/singleobjective/evolution_strategy/__init__.py
 examples/singleobjective/evolution_strategy/evolution_strategy_binary.py
 examples/singleobjective/evolution_strategy/evolution_strategy_float.py
+examples/singleobjective/evolution_strategy/evolution_strategy_permutation.py
 examples/singleobjective/gde3/__init__.py
 examples/singleobjective/gde3/gde3_single_objective.py
 examples/singleobjective/genetic_algorithm/__init__.py
 examples/singleobjective/genetic_algorithm/generational_genetic_algorithm_binary.py
 examples/singleobjective/genetic_algorithm/generational_genetic_algorithm_float.py
 examples/singleobjective/genetic_algorithm/generational_genetic_algorithm_tsp.py
+examples/singleobjective/genetic_algorithm/generational_genetic_algorithm_tsp_with_contraints.py
 examples/singleobjective/genetic_algorithm/steady_state_genetic_algorithm.py
 examples/singleobjective/genetic_algorithm/steady_state_genetic_algorithm_with_knapsack_problem.py
 examples/singleobjective/local_search/__init__.py
 examples/singleobjective/local_search/local_search_binary.py
 examples/singleobjective/local_search/local_search_float.py
 examples/singleobjective/nsgaii/__init__.py
 examples/singleobjective/nsgaii/nsgaii_single_objective_binary.py
 examples/singleobjective/nsgaii/nsgaii_single_objective_float.py
 examples/singleobjective/simulated_annealing/__init__.py
 examples/singleobjective/simulated_annealing/simulated_annealing_binary.py
 examples/singleobjective/simulated_annealing/simulated_annealing_float.py
+examples/singleobjective/simulated_annealing/simulated_annealing_permutation.py
 jmetal/__init__.py
 jmetal/config.py
+jmetal/logger.py
 jmetal/algorithm/__init__.py
 jmetal/algorithm/multiobjective/__init__.py
 jmetal/algorithm/multiobjective/gde3.py
 jmetal/algorithm/multiobjective/hype.py
 jmetal/algorithm/multiobjective/ibea.py
 jmetal/algorithm/multiobjective/mocell.py
 jmetal/algorithm/multiobjective/moead.py
@@ -144,14 +153,16 @@
 jmetal/problem/multiobjective/lircmop.py
 jmetal/problem/multiobjective/lz09.py
 jmetal/problem/multiobjective/uf.py
 jmetal/problem/multiobjective/unconstrained.py
 jmetal/problem/multiobjective/zdt.py
 jmetal/problem/multiobjective/test/__init__.py
 jmetal/problem/multiobjective/test/test_constrained.py
+jmetal/problem/multiobjective/test/test_dtlz.py
+jmetal/problem/multiobjective/test/test_lz09.py
 jmetal/problem/multiobjective/test/test_unconstrained.py
 jmetal/problem/multiobjective/test/test_zdt.py
 jmetal/problem/singleobjective/__init__.py
 jmetal/problem/singleobjective/knapsack.py
 jmetal/problem/singleobjective/tsp.py
 jmetal/problem/singleobjective/unconstrained.py
 jmetal/problem/singleobjective/test/__init__.py
@@ -187,9 +198,10 @@
 jmetal/util/test/test_neighborhood.py
 jmetal/util/test/test_point.py
 jmetal/util/test/test_ranking.py
 jmetal/util/test/test_replacement.py
 jmetalpy.egg-info/PKG-INFO
 jmetalpy.egg-info/SOURCES.txt
 jmetalpy.egg-info/dependency_links.txt
+jmetalpy.egg-info/not-zip-safe
 jmetalpy.egg-info/requires.txt
 jmetalpy.egg-info/top_level.txt
```

