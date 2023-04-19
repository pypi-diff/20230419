# Comparing `tmp/mobspy-1.1.3.tar.gz` & `tmp/mobspy-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mobspy-1.1.3.tar", last modified: Tue Aug  9 11:05:54 2022, max compression
+gzip compressed data, was "mobspy-2.0.1.tar", last modified: Wed Apr 19 11:46:42 2023, max compression
```

## Comparing `mobspy-1.1.3.tar` & `mobspy-2.0.1.tar`

### file list

```diff
@@ -1,100 +1,125 @@
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2022-08-09 11:05:54.449363 mobspy-1.1.3/
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2022-08-09 11:05:54.365393 mobspy-1.1.3/.github/
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2022-08-09 11:05:54.383268 mobspy-1.1.3/.github/workflows/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1201 2022-05-09 13:33:55.000000 mobspy-1.1.3/.github/workflows/python-app.yml
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      145 2022-07-19 13:10:01.000000 mobspy-1.1.3/.gitignore
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1068 2022-03-29 10:50:57.000000 mobspy-1.1.3/LICENSE
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6581 2022-08-09 11:05:54.449021 mobspy-1.1.3/PKG-INFO
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5423 2022-05-11 13:37:51.000000 mobspy-1.1.3/README.md
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2022-08-09 11:05:54.366817 mobspy-1.1.3/example_models/
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2022-08-09 11:05:54.394054 mobspy-1.1.3/example_models/application_models/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      573 2022-05-10 16:12:42.000000 mobspy-1.1.3/example_models/application_models/AB_2CD.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1446 2022-05-10 16:12:42.000000 mobspy-1.1.3/example_models/application_models/AND_gate.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2653 2022-05-10 16:12:42.000000 mobspy-1.1.3/example_models/application_models/CRISPR_Oscillator.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1435 2022-06-17 09:01:31.000000 mobspy-1.1.3/example_models/application_models/For_The_Trees.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1294 2022-05-10 16:12:42.000000 mobspy-1.1.3/example_models/application_models/NOR_gate.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1244 2022-05-10 16:12:42.000000 mobspy-1.1.3/example_models/application_models/donor_receptor.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1372 2022-05-10 16:12:42.000000 mobspy-1.1.3/example_models/application_models/oscillator.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2863 2022-05-10 16:12:42.000000 mobspy-1.1.3/example_models/application_models/random_walk.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      565 2022-05-10 16:12:42.000000 mobspy-1.1.3/example_models/application_models/simple_repressor.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     3855 2022-05-10 16:12:42.000000 mobspy-1.1.3/example_models/application_models/toggle_switch.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2022-08-09 11:05:54.412955 mobspy-1.1.3/example_models/tutorial_models/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1602 2022-05-11 13:37:51.000000 mobspy-1.1.3/example_models/tutorial_models/01_Getting_Started.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1863 2022-05-11 13:37:51.000000 mobspy-1.1.3/example_models/tutorial_models/02_Reaction_Inheritance.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1013 2022-05-11 13:37:51.000000 mobspy-1.1.3/example_models/tutorial_models/02_Reaction_Inheritance_Model.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1769 2022-05-12 10:51:20.000000 mobspy-1.1.3/example_models/tutorial_models/03_Queries.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      946 2022-05-11 13:37:51.000000 mobspy-1.1.3/example_models/tutorial_models/03_Queries.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      989 2022-05-19 14:18:28.000000 mobspy-1.1.3/example_models/tutorial_models/04_Characteristic_Restriction.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1121 2022-05-19 14:18:28.000000 mobspy-1.1.3/example_models/tutorial_models/05_C_Query.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2284 2022-05-19 14:18:28.000000 mobspy-1.1.3/example_models/tutorial_models/06_Round_Robin.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2255 2022-05-19 14:18:28.000000 mobspy-1.1.3/example_models/tutorial_models/07_Rates.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2125 2022-05-19 14:18:28.000000 mobspy-1.1.3/example_models/tutorial_models/08_Units.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      866 2022-05-12 10:51:20.000000 mobspy-1.1.3/example_models/tutorial_models/09_Count_Assignment.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1042 2022-05-11 13:37:51.000000 mobspy-1.1.3/example_models/tutorial_models/09_Count_Assignment.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1589 2022-05-12 10:51:20.000000 mobspy-1.1.3/example_models/tutorial_models/10_Species_Loop.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2074 2022-05-12 10:51:20.000000 mobspy-1.1.3/example_models/tutorial_models/11_Results.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2128 2022-05-12 10:51:20.000000 mobspy-1.1.3/example_models/tutorial_models/12_Hierarchical_plot.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      982 2022-05-15 18:48:36.000000 mobspy-1.1.3/example_models/tutorial_models/13_Born_Species.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       59 2022-05-21 18:55:53.000000 mobspy-1.1.3/for_local_use.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2022-08-09 11:05:54.414254 mobspy-1.1.3/images/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    18566 2022-04-08 15:15:44.000000 mobspy-1.1.3/images/img.png
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2022-08-09 11:05:54.417839 mobspy-1.1.3/mobspy/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       95 2022-05-04 17:32:05.000000 mobspy-1.1.3/mobspy/__init__.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       22 2022-08-09 11:05:20.000000 mobspy-1.1.3/mobspy/_version.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2022-08-09 11:05:54.422487 mobspy-1.1.3/mobspy/data_handler/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2022-03-29 10:50:57.000000 mobspy-1.1.3/mobspy/data_handler/__init__.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2884 2022-05-12 14:09:11.000000 mobspy-1.1.3/mobspy/data_handler/process_result_data.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2022-08-09 11:05:54.430496 mobspy-1.1.3/mobspy/modules/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2022-03-29 10:50:57.000000 mobspy-1.1.3/mobspy/modules/__init__.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    11802 2022-05-19 14:18:28.000000 mobspy-1.1.3/mobspy/modules/function_rate_code.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    41088 2022-07-19 13:23:47.000000 mobspy-1.1.3/mobspy/modules/meta_class.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     7705 2022-05-13 15:25:15.000000 mobspy-1.1.3/mobspy/modules/meta_class_utils.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    14768 2022-05-14 15:01:12.000000 mobspy-1.1.3/mobspy/modules/order_operators.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    15478 2022-05-19 14:18:28.000000 mobspy-1.1.3/mobspy/modules/reaction_construction_nb.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     5349 2022-05-15 14:29:40.000000 mobspy-1.1.3/mobspy/modules/unit_handler.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2022-08-09 11:05:54.431850 mobspy-1.1.3/mobspy/parameter_scripts/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2022-03-29 10:50:57.000000 mobspy-1.1.3/mobspy/parameter_scripts/__init__.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     3196 2022-05-15 14:29:40.000000 mobspy-1.1.3/mobspy/parameter_scripts/parameter_reader.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2022-08-09 11:05:54.435342 mobspy-1.1.3/mobspy/parameters/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1463 2022-05-11 13:37:51.000000 mobspy-1.1.3/mobspy/parameters/README.md
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2022-03-29 10:50:57.000000 mobspy-1.1.3/mobspy/parameters/__init__.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      904 2022-05-15 14:29:40.000000 mobspy-1.1.3/mobspy/parameters/default_reader.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      895 2022-05-15 14:29:40.000000 mobspy-1.1.3/mobspy/parameters/example_reader.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2022-08-09 11:05:54.437259 mobspy-1.1.3/mobspy/plot_params/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2022-03-29 10:50:57.000000 mobspy-1.1.3/mobspy/plot_params/__init__.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      184 2022-03-24 09:14:00.000000 mobspy-1.1.3/mobspy/plot_params/default_plot_reader.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1232 2022-05-15 14:29:40.000000 mobspy-1.1.3/mobspy/plot_params/example_plot_reader.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2022-08-09 11:05:54.440759 mobspy-1.1.3/mobspy/plot_scripts/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2022-03-29 10:50:57.000000 mobspy-1.1.3/mobspy/plot_scripts/__init__.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6498 2022-05-15 14:43:05.000000 mobspy-1.1.3/mobspy/plot_scripts/default_plots.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    14971 2022-05-15 15:24:15.000000 mobspy-1.1.3/mobspy/plot_scripts/hierarchical_plot.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2703 2022-05-15 15:38:18.000000 mobspy-1.1.3/mobspy/plot_scripts/process_plot_data.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2416 2022-05-15 15:50:46.000000 mobspy-1.1.3/mobspy/plot_scripts/statistics_calculations.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2022-08-09 11:05:54.443493 mobspy-1.1.3/mobspy/sbml_simulator/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     8146 2022-05-15 15:50:46.000000 mobspy-1.1.3/mobspy/sbml_simulator/SBMLWriter.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2022-03-29 10:50:57.000000 mobspy-1.1.3/mobspy/sbml_simulator/__init__.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      483 2022-05-15 15:50:46.000000 mobspy-1.1.3/mobspy/sbml_simulator/builder.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     7413 2022-07-19 13:11:52.000000 mobspy-1.1.3/mobspy/sbml_simulator/run.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)    13217 2022-07-19 15:43:22.000000 mobspy-1.1.3/mobspy/simulation.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2022-08-09 11:05:54.444355 mobspy-1.1.3/mobspy/simulation_logging/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2022-03-29 10:50:57.000000 mobspy-1.1.3/mobspy/simulation_logging/__init__.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      707 2022-07-19 13:03:54.000000 mobspy-1.1.3/mobspy/simulation_logging/log_scripts.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2022-08-09 11:05:54.421698 mobspy-1.1.3/mobspy.egg-info/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     6581 2022-08-09 11:05:54.000000 mobspy-1.1.3/mobspy.egg-info/PKG-INFO
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     2889 2022-08-09 11:05:54.000000 mobspy-1.1.3/mobspy.egg-info/SOURCES.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        1 2022-08-09 11:05:54.000000 mobspy-1.1.3/mobspy.egg-info/dependency_links.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       76 2022-08-09 11:05:54.000000 mobspy-1.1.3/mobspy.egg-info/requires.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)        7 2022-08-09 11:05:54.000000 mobspy-1.1.3/mobspy.egg-info/top_level.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       77 2022-05-04 18:06:18.000000 mobspy-1.1.3/requirements.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       38 2022-08-09 11:05:54.449483 mobspy-1.1.3/setup.cfg
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      767 2022-03-29 10:50:57.000000 mobspy-1.1.3/setup.py
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     4525 2022-07-19 15:49:40.000000 mobspy-1.1.3/test_script.py
-drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2022-08-09 11:05:54.448103 mobspy-1.1.3/test_tools/
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      170 2022-05-08 19:17:17.000000 mobspy-1.1.3/test_tools/model_1.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      396 2022-05-09 09:35:00.000000 mobspy-1.1.3/test_tools/model_2.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     3154 2022-05-09 11:02:28.000000 mobspy-1.1.3/test_tools/model_3.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      727 2022-05-09 11:27:45.000000 mobspy-1.1.3/test_tools/model_4.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      559 2022-05-09 11:47:47.000000 mobspy-1.1.3/test_tools/model_5.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)      353 2022-05-13 16:22:03.000000 mobspy-1.1.3/test_tools/model_6.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)     1352 2022-07-19 15:49:36.000000 mobspy-1.1.3/test_tools/model_7.txt
--rw-r--r--   0 fabriciocravo   (501) staff       (20)       60 2022-04-13 12:52:19.000000 mobspy-1.1.3/useful_parameters.json
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-19 11:46:42.917449 mobspy-2.0.1/
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-19 11:46:42.767707 mobspy-2.0.1/.github/
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-19 11:46:42.776416 mobspy-2.0.1/.github/workflows/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1201 2023-04-03 11:45:17.000000 mobspy-2.0.1/.github/workflows/python-app.yml
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      265 2023-04-05 11:22:48.000000 mobspy-2.0.1/.gitignore
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1068 2023-03-26 13:05:39.000000 mobspy-2.0.1/LICENSE
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     7015 2023-04-19 11:46:42.915662 mobspy-2.0.1/PKG-INFO
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5825 2023-03-29 14:16:39.000000 mobspy-2.0.1/README.md
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-19 11:46:42.768156 mobspy-2.0.1/example_models/
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-19 11:46:42.785863 mobspy-2.0.1/example_models/application_models/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      573 2023-03-26 13:05:39.000000 mobspy-2.0.1/example_models/application_models/AB_2CD.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1446 2023-03-26 13:05:39.000000 mobspy-2.0.1/example_models/application_models/AND_gate.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2653 2023-03-26 13:05:39.000000 mobspy-2.0.1/example_models/application_models/CRISPR_Oscillator.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1435 2023-04-18 11:26:50.000000 mobspy-2.0.1/example_models/application_models/For_The_Trees.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1297 2023-03-31 13:18:09.000000 mobspy-2.0.1/example_models/application_models/NOR_gate.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1244 2023-03-26 13:05:39.000000 mobspy-2.0.1/example_models/application_models/donor_receptor.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1372 2023-03-26 13:05:39.000000 mobspy-2.0.1/example_models/application_models/oscillator.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2901 2023-04-18 11:26:50.000000 mobspy-2.0.1/example_models/application_models/random_walk.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      565 2023-03-26 13:05:39.000000 mobspy-2.0.1/example_models/application_models/simple_repressor.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     3855 2023-03-26 13:05:39.000000 mobspy-2.0.1/example_models/application_models/toggle_switch.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-19 11:46:42.803619 mobspy-2.0.1/example_models/tutorial_models/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1602 2023-03-26 13:05:39.000000 mobspy-2.0.1/example_models/tutorial_models/01_Getting_Started.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1863 2023-03-26 13:05:39.000000 mobspy-2.0.1/example_models/tutorial_models/02_Reaction_Inheritance.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1013 2023-03-26 13:05:39.000000 mobspy-2.0.1/example_models/tutorial_models/02_Reaction_Inheritance_Model.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1769 2023-03-26 13:05:39.000000 mobspy-2.0.1/example_models/tutorial_models/03_Queries.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      946 2023-03-26 13:05:39.000000 mobspy-2.0.1/example_models/tutorial_models/03_Queries.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      989 2023-03-26 13:05:39.000000 mobspy-2.0.1/example_models/tutorial_models/04_Characteristic_Restriction.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1121 2023-03-31 13:18:09.000000 mobspy-2.0.1/example_models/tutorial_models/05_C_Query.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2284 2023-03-31 13:18:09.000000 mobspy-2.0.1/example_models/tutorial_models/06_Round_Robin.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2255 2023-03-26 13:05:39.000000 mobspy-2.0.1/example_models/tutorial_models/07_Rates.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2125 2023-03-31 13:18:09.000000 mobspy-2.0.1/example_models/tutorial_models/08_Units.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      866 2023-03-26 13:05:39.000000 mobspy-2.0.1/example_models/tutorial_models/09_Count_Assignment.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1042 2023-03-26 13:05:39.000000 mobspy-2.0.1/example_models/tutorial_models/09_Count_Assignment.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1589 2023-03-26 13:05:39.000000 mobspy-2.0.1/example_models/tutorial_models/10_Species_Loop.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2074 2023-03-26 13:05:39.000000 mobspy-2.0.1/example_models/tutorial_models/11_Results.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2128 2023-03-26 13:05:39.000000 mobspy-2.0.1/example_models/tutorial_models/12_Hierarchical_plot.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      982 2023-03-26 13:05:39.000000 mobspy-2.0.1/example_models/tutorial_models/13_Born_Species.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      101 2023-04-19 11:43:11.000000 mobspy-2.0.1/for_local_use.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-19 11:46:42.804603 mobspy-2.0.1/images/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    18566 2023-03-26 13:05:39.000000 mobspy-2.0.1/images/img.png
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-19 11:46:42.807293 mobspy-2.0.1/mobspy/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       95 2023-03-26 13:05:39.000000 mobspy-2.0.1/mobspy/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       22 2023-03-26 13:05:39.000000 mobspy-2.0.1/mobspy/_version.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-19 11:46:42.813584 mobspy-2.0.1/mobspy/data_handler/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-03-26 13:05:39.000000 mobspy-2.0.1/mobspy/data_handler/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2207 2023-04-05 18:57:56.000000 mobspy-2.0.1/mobspy/data_handler/process_result_data.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5233 2023-04-19 11:42:57.000000 mobspy-2.0.1/mobspy/data_handler/time_series_object.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-19 11:46:42.833692 mobspy-2.0.1/mobspy/modules/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-03-26 13:05:39.000000 mobspy-2.0.1/mobspy/modules/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4355 2023-04-17 14:42:37.000000 mobspy-2.0.1/mobspy/modules/event_functions.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    12456 2023-04-18 20:56:31.000000 mobspy-2.0.1/mobspy/modules/function_rate_code.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    12663 2023-04-12 21:11:32.000000 mobspy-2.0.1/mobspy/modules/logic_operator_objects.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    57088 2023-04-18 20:51:04.000000 mobspy-2.0.1/mobspy/modules/meta_class.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     5239 2023-04-13 11:40:51.000000 mobspy-2.0.1/mobspy/modules/meta_class_utils.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    14961 2023-04-13 12:13:54.000000 mobspy-2.0.1/mobspy/modules/order_operators.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    16482 2023-04-13 12:24:44.000000 mobspy-2.0.1/mobspy/modules/reaction_construction_nb.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     3988 2023-04-17 11:11:45.000000 mobspy-2.0.1/mobspy/modules/set_counts_module.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     4143 2023-04-11 11:59:50.000000 mobspy-2.0.1/mobspy/modules/species_string_generator.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     6615 2023-04-18 21:25:28.000000 mobspy-2.0.1/mobspy/modules/unit_handler.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-19 11:46:42.834921 mobspy-2.0.1/mobspy/parameter_scripts/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-03-26 13:05:39.000000 mobspy-2.0.1/mobspy/parameter_scripts/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     2211 2023-04-07 15:35:28.000000 mobspy-2.0.1/mobspy/parameter_scripts/parameter_reader.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-19 11:46:42.839087 mobspy-2.0.1/mobspy/parameters/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1463 2023-03-26 13:05:39.000000 mobspy-2.0.1/mobspy/parameters/README.md
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-03-26 13:05:39.000000 mobspy-2.0.1/mobspy/parameters/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1035 2023-03-28 13:07:30.000000 mobspy-2.0.1/mobspy/parameters/default_reader.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1117 2023-04-07 15:35:28.000000 mobspy-2.0.1/mobspy/parameters/example_reader.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-19 11:46:42.843351 mobspy-2.0.1/mobspy/plot_params/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-03-26 13:05:39.000000 mobspy-2.0.1/mobspy/plot_params/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      184 2023-03-26 13:05:39.000000 mobspy-2.0.1/mobspy/plot_params/default_plot_reader.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1232 2023-03-26 13:05:39.000000 mobspy-2.0.1/mobspy/plot_params/example_plot_reader.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-19 11:46:42.850288 mobspy-2.0.1/mobspy/plot_scripts/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-03-26 13:05:39.000000 mobspy-2.0.1/mobspy/plot_scripts/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     6445 2023-04-19 11:27:03.000000 mobspy-2.0.1/mobspy/plot_scripts/default_plots.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    14387 2023-04-17 13:43:18.000000 mobspy-2.0.1/mobspy/plot_scripts/hierarchical_plot.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1736 2023-04-18 13:30:54.000000 mobspy-2.0.1/mobspy/plot_scripts/process_plot_data.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     3566 2023-04-08 16:53:54.000000 mobspy-2.0.1/mobspy/plot_scripts/statistics_calculations.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-19 11:46:42.855000 mobspy-2.0.1/mobspy/sbml_simulator/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     8118 2023-04-08 16:53:54.000000 mobspy-2.0.1/mobspy/sbml_simulator/SBMLWriter.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-03-26 13:05:39.000000 mobspy-2.0.1/mobspy/sbml_simulator/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      936 2023-04-08 16:40:14.000000 mobspy-2.0.1/mobspy/sbml_simulator/builder.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    12536 2023-04-17 15:49:48.000000 mobspy-2.0.1/mobspy/sbml_simulator/run.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    26192 2023-04-19 08:48:20.000000 mobspy-2.0.1/mobspy/simulation.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-19 11:46:42.856697 mobspy-2.0.1/mobspy/simulation_logging/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        0 2023-03-26 13:05:39.000000 mobspy-2.0.1/mobspy/simulation_logging/__init__.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1013 2023-04-13 12:13:25.000000 mobspy-2.0.1/mobspy/simulation_logging/log_scripts.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-19 11:46:42.811622 mobspy-2.0.1/mobspy.egg-info/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     7015 2023-04-19 11:46:42.000000 mobspy-2.0.1/mobspy.egg-info/PKG-INFO
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     3563 2023-04-19 11:46:42.000000 mobspy-2.0.1/mobspy.egg-info/SOURCES.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        1 2023-04-19 11:46:42.000000 mobspy-2.0.1/mobspy.egg-info/dependency_links.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       76 2023-04-19 11:46:42.000000 mobspy-2.0.1/mobspy.egg-info/requires.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)        7 2023-04-19 11:46:42.000000 mobspy-2.0.1/mobspy.egg-info/top_level.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       77 2023-03-26 13:05:39.000000 mobspy-2.0.1/requirements.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       38 2023-04-19 11:46:42.918064 mobspy-2.0.1/setup.cfg
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      767 2023-03-26 13:05:39.000000 mobspy-2.0.1/setup.py
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)    18793 2023-04-18 21:34:52.000000 mobspy-2.0.1/test_script.py
+drwxr-xr-x   0 fabriciocravo   (501) staff       (20)        0 2023-04-19 11:46:42.910475 mobspy-2.0.1/test_tools/
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      170 2023-03-26 13:05:39.000000 mobspy-2.0.1/test_tools/model_1.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      239 2023-03-28 14:54:04.000000 mobspy-2.0.1/test_tools/model_10.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      299 2023-03-29 10:35:15.000000 mobspy-2.0.1/test_tools/model_11.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      393 2023-03-31 14:53:54.000000 mobspy-2.0.1/test_tools/model_12.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      490 2023-03-31 16:58:04.000000 mobspy-2.0.1/test_tools/model_13.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      487 2023-03-31 17:23:20.000000 mobspy-2.0.1/test_tools/model_14.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      550 2023-04-03 08:42:24.000000 mobspy-2.0.1/test_tools/model_15.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      286 2023-04-04 18:39:28.000000 mobspy-2.0.1/test_tools/model_16.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      273 2023-04-05 14:12:52.000000 mobspy-2.0.1/test_tools/model_17.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      118 2023-04-06 11:09:14.000000 mobspy-2.0.1/test_tools/model_18.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      970 2023-04-06 13:23:26.000000 mobspy-2.0.1/test_tools/model_19.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      396 2023-03-26 13:05:39.000000 mobspy-2.0.1/test_tools/model_2.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      326 2023-04-06 13:24:46.000000 mobspy-2.0.1/test_tools/model_20.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1453 2023-04-11 12:17:19.000000 mobspy-2.0.1/test_tools/model_21.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      435 2023-04-11 15:31:51.000000 mobspy-2.0.1/test_tools/model_22.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      186 2023-04-12 16:26:56.000000 mobspy-2.0.1/test_tools/model_23.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      605 2023-04-17 14:45:24.000000 mobspy-2.0.1/test_tools/model_24.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       81 2023-04-18 11:30:58.000000 mobspy-2.0.1/test_tools/model_25.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      507 2023-04-18 20:45:48.000000 mobspy-2.0.1/test_tools/model_26.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      145 2023-04-18 21:30:11.000000 mobspy-2.0.1/test_tools/model_27.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     3154 2023-03-26 13:05:39.000000 mobspy-2.0.1/test_tools/model_3.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      727 2023-03-26 13:05:39.000000 mobspy-2.0.1/test_tools/model_4.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      559 2023-03-26 13:05:39.000000 mobspy-2.0.1/test_tools/model_5.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      353 2023-03-26 13:05:39.000000 mobspy-2.0.1/test_tools/model_6.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)     1352 2023-03-26 13:05:39.000000 mobspy-2.0.1/test_tools/model_7.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      443 2023-03-28 21:23:58.000000 mobspy-2.0.1/test_tools/model_8.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)      736 2023-03-28 08:26:08.000000 mobspy-2.0.1/test_tools/model_9.txt
+-rw-r--r--   0 fabriciocravo   (501) staff       (20)       60 2023-03-26 13:05:39.000000 mobspy-2.0.1/useful_parameters.json
```

### Comparing `mobspy-1.1.3/.github/workflows/python-app.yml` & `mobspy-2.0.1/.github/workflows/python-app.yml`

 * *Files 2% similar despite different names*

```diff
@@ -30,10 +30,10 @@
         if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
     - name: Lint with flake8
       run: |
         # stop the build if there are Python syntax errors or undefined names
         flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics
         # exit-zero treats all errors as warnings. The GitHub editor is 127 chars wide
         flake8 . --count --exit-zero --max-complexity=10 --max-line-length=127 --statistics
-    - name: Test with pytest
+    - name: Test with script
       run: |
-        pytest test_script.py
+        python test_script.py
```

### Comparing `mobspy-1.1.3/LICENSE` & `mobspy-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mobspy-1.1.3/PKG-INFO` & `mobspy-2.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mobspy
-Version: 1.1.3
+Version: 2.0.1
 Summary: A Query-Based Language for Chemical Reaction Networks
 Home-page: https://github.com/ROBACON/mobspy
 License: UNKNOWN
 Description: ![Alt text](/images/img.png "MobsPy")
         
         # MobsPy
         
@@ -105,14 +105,18 @@
         
         For now MobsPy is not thread-safe and it's not compatible with numpy and deepcopy
         
         # Release info
         
         Version 1.1 added automated testing to git pushes with test_script.py
         
+        Version 2.0.1 added events, ability to concatenate simulations, and changed the structure of output data to be more 
+        user-friendly. Now MySim.results["data"]["runs"]["MetaSpeciesName"] has been deprecated. It has been replaced by 
+        MySim.results["MetaSpeciesName"] or MySim.results[MetaSpeciesObject]. It will return only one run if there are no 
+        repetitions and multiple runs with several repetitions.
```

### Comparing `mobspy-1.1.3/README.md` & `mobspy-2.0.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -99,13 +99,17 @@
 
 For now MobsPy is not thread-safe and it's not compatible with numpy and deepcopy
 
 # Release info
 
 Version 1.1 added automated testing to git pushes with test_script.py
 
+Version 2.0.1 added events, ability to concatenate simulations, and changed the structure of output data to be more 
+user-friendly. Now MySim.results["data"]["runs"]["MetaSpeciesName"] has been deprecated. It has been replaced by 
+MySim.results["MetaSpeciesName"] or MySim.results[MetaSpeciesObject]. It will return only one run if there are no 
+repetitions and multiple runs with several repetitions.
```

### Comparing `mobspy-1.1.3/example_models/application_models/AB_2CD.py` & `mobspy-2.0.1/example_models/application_models/AB_2CD.py`

 * *Files identical despite different names*

### Comparing `mobspy-1.1.3/example_models/application_models/AND_gate.py` & `mobspy-2.0.1/example_models/application_models/AND_gate.py`

 * *Files identical despite different names*

### Comparing `mobspy-1.1.3/example_models/application_models/CRISPR_Oscillator.py` & `mobspy-2.0.1/example_models/application_models/CRISPR_Oscillator.py`

 * *Files identical despite different names*

### Comparing `mobspy-1.1.3/example_models/application_models/For_The_Trees.py` & `mobspy-2.0.1/example_models/application_models/For_The_Trees.py`

 * *Files identical despite different names*

### Comparing `mobspy-1.1.3/example_models/application_models/NOR_gate.py` & `mobspy-2.0.1/example_models/application_models/NOR_gate.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,17 @@
     If any of them bind to the Promoter the protein can no longer be expressed
 """
 
 
 def NOR_GATE(A_conc, B_conc):
     # Here we define the Protein to be produced, the Promoter that will act as the gate
     # A and B are the inputs any of them can inactivate the Promoter so they inherit from Repressor
-    Repressor, Promoter, Protein = BaseSpecies(4)
+    Repressor, Promoter, Protein = BaseSpecies(3)
     Repressor + Promoter.active >> Promoter.inactive [0.5]
-    A, B = New(Repressor)
+    A, B = New(Repressor, 2)
     Promoter >> Promoter + Protein [lambda promoter: 1 if promoter.active else 0]
     Protein >> Zero [2]
 
     Promoter(100)
     A(A_conc), B(B_conc)
     MySim = Simulation(A | B | Promoter | Protein)
     MySim.duration = 10
```

### Comparing `mobspy-1.1.3/example_models/application_models/donor_receptor.py` & `mobspy-2.0.1/example_models/application_models/donor_receptor.py`

 * *Files identical despite different names*

### Comparing `mobspy-1.1.3/example_models/application_models/oscillator.py` & `mobspy-2.0.1/example_models/application_models/oscillator.py`

 * *Files identical despite different names*

### Comparing `mobspy-1.1.3/example_models/application_models/random_walk.py` & `mobspy-2.0.1/example_models/application_models/random_walk.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 import sys, os
 import matplotlib.pyplot as plt
 from mobspy import *
+import time
 
 
 """
     This is a geometry-based model
     Here the Meta-Species Mesh is used to represent the positions in a grid
     And their transitions using a CRN
     Here we have a bacteria and a phage that move through a Mesh and once they encounter the bacteria becomes infected
     Although the movement is not realistic, it shows MobsPy geometry capabilities 
     In future work we hope to implement different type movements or grids
 """
 
+start_time = time.time()
+
 Mesh = BaseSpecies(1)
 n = 10
 for i in range(n):
     for j in range(n):
         coordinate = 'p_' + str(i) + '_' + str(j)
 
         if i + 1 < n:
```

### Comparing `mobspy-1.1.3/example_models/application_models/simple_repressor.py` & `mobspy-2.0.1/example_models/application_models/simple_repressor.py`

 * *Files identical despite different names*

### Comparing `mobspy-1.1.3/example_models/application_models/toggle_switch.py` & `mobspy-2.0.1/example_models/application_models/toggle_switch.py`

 * *Files identical despite different names*

### Comparing `mobspy-1.1.3/example_models/tutorial_models/01_Getting_Started.py` & `mobspy-2.0.1/example_models/tutorial_models/01_Getting_Started.py`

 * *Files identical despite different names*

### Comparing `mobspy-1.1.3/example_models/tutorial_models/02_Reaction_Inheritance.py` & `mobspy-2.0.1/example_models/tutorial_models/02_Reaction_Inheritance.py`

 * *Files identical despite different names*

### Comparing `mobspy-1.1.3/example_models/tutorial_models/02_Reaction_Inheritance_Model.txt` & `mobspy-2.0.1/example_models/tutorial_models/02_Reaction_Inheritance_Model.txt`

 * *Files identical despite different names*

### Comparing `mobspy-1.1.3/example_models/tutorial_models/03_Queries.py` & `mobspy-2.0.1/example_models/tutorial_models/03_Queries.py`

 * *Files identical despite different names*

### Comparing `mobspy-1.1.3/example_models/tutorial_models/03_Queries.txt` & `mobspy-2.0.1/example_models/tutorial_models/03_Queries.txt`

 * *Files identical despite different names*

### Comparing `mobspy-1.1.3/example_models/tutorial_models/04_Characteristic_Restriction.py` & `mobspy-2.0.1/example_models/tutorial_models/04_Characteristic_Restriction.py`

 * *Files identical despite different names*

### Comparing `mobspy-1.1.3/example_models/tutorial_models/05_C_Query.py` & `mobspy-2.0.1/example_models/tutorial_models/05_C_Query.py`

 * *Files identical despite different names*

### Comparing `mobspy-1.1.3/example_models/tutorial_models/06_Round_Robin.py` & `mobspy-2.0.1/example_models/tutorial_models/06_Round_Robin.py`

 * *Files identical despite different names*

### Comparing `mobspy-1.1.3/example_models/tutorial_models/07_Rates.py` & `mobspy-2.0.1/example_models/tutorial_models/07_Rates.py`

 * *Files identical despite different names*

### Comparing `mobspy-1.1.3/example_models/tutorial_models/08_Units.py` & `mobspy-2.0.1/example_models/tutorial_models/08_Units.py`

 * *Files identical despite different names*

### Comparing `mobspy-1.1.3/example_models/tutorial_models/09_Count_Assignment.py` & `mobspy-2.0.1/example_models/tutorial_models/09_Count_Assignment.py`

 * *Files identical despite different names*

### Comparing `mobspy-1.1.3/example_models/tutorial_models/09_Count_Assignment.txt` & `mobspy-2.0.1/example_models/tutorial_models/09_Count_Assignment.txt`

 * *Files identical despite different names*

### Comparing `mobspy-1.1.3/example_models/tutorial_models/10_Species_Loop.py` & `mobspy-2.0.1/example_models/tutorial_models/10_Species_Loop.py`

 * *Files identical despite different names*

### Comparing `mobspy-1.1.3/example_models/tutorial_models/11_Results.py` & `mobspy-2.0.1/example_models/tutorial_models/11_Results.py`

 * *Files identical despite different names*

### Comparing `mobspy-1.1.3/example_models/tutorial_models/12_Hierarchical_plot.py` & `mobspy-2.0.1/example_models/tutorial_models/12_Hierarchical_plot.py`

 * *Files identical despite different names*

### Comparing `mobspy-1.1.3/example_models/tutorial_models/13_Born_Species.py` & `mobspy-2.0.1/example_models/tutorial_models/13_Born_Species.py`

 * *Files identical despite different names*

### Comparing `mobspy-1.1.3/images/img.png` & `mobspy-2.0.1/images/img.png`

 * *Files identical despite different names*

### Comparing `mobspy-1.1.3/mobspy/modules/function_rate_code.py` & `mobspy-2.0.1/mobspy/modules/function_rate_code.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,26 +13,20 @@
 import mobspy.modules.meta_class as mc
 import mobspy.modules.unit_handler as uh
 from pint import Quantity
 
 
 class Bool_Override:
     """
-        Just a base class for implementing the . operation in the rate function arguments
-        through boolean overriding
+            Just a base class for implementing the . operation in the rate function arguments
+            through boolean overriding. It is responsible for returning true when the reactant
+            has the specified characteristic when using the dot notation
 
-        Attributes:
-            _stocked_characteristics (str) = stocks the characteristics of the queries performed by the user
-            species_string (str) = string value from an individual species in MobsPY format
-
-        Methods:
-            __bool__
-
-        related classes:
-            Specific_Species_Operator - inherits from it for the __bool__ method
+            :param _stocked_characteristics: (str) stocks the characteristics of the queries performed by the user
+            :param species_string: (str) string value from an individual species in MobsPY format
     """
 
     def __bool__(self):
         """
             The implementation of the .dot operation for rate function arguments
             Returns true when the argument possesses the characteristics
             Bool is called after the .dot operations
@@ -59,44 +53,37 @@
 
 class Specific_Species_Operator(Bool_Override):
     """
         This class creates objects from the species strings from the meta-species to pass them to the rate functions
         as arguments. It uses the Bool_Override class to return true or false to the .dot operation inside the rate
         functions
 
-        Attributes:
-            species_string (str) = A string from MobsPy meta-species format
-            species_object (Species) = Meta-species set for which the species_string is contained in
-            _stocked_characteristics (str) = stocks the characteristics of the queries performed by the user
-
-        Methods:
-            __getattr__, __str__, is_a, add
 
+        :param _stocked_characteristics: (str) stocks the characteristics of the queries performed by the user
+        :param species_string: (str) string value from an individual species in MobsPY format
+        :param species_object: (Species) Meta-species object which originated the meta-species str
     """
 
     def __init__(self, species_string, species_object):
         """
             Constructs the object from the species strings from the meta-species to pass them to the rate functions
             as arguments.
 
-            Parameters:
-                species_string (str) = A string from MobsPy meta-species format
-                species_object (Species) = Meta-species set for which the species_string is contained in
-
+            :param species_string: (str) A string from MobsPy meta-species format
+            :param species_object: (Species) = Meta-species set for which the species_string is contained in
         """
         self.species_string = species_string
         self._stocked_characteristics = set()
         self._species_object = species_object
 
     def __getattr__(self, characteristic):
         """
             Stores the characteristics for the boolean query inside the rate function by adding them to the set
 
-            Parameters:
-                characteristic (str) = characteristic being queried
+            :param characteristic: (str) characteristic being queried
         """
         self._stocked_characteristics.add(characteristic)
         return self
 
     def __str__(self):
         """
             Returns the species_string from the MobsPy meta-species used in the object construction
@@ -104,105 +91,117 @@
         return self.species_string
 
     def is_a(self, reference):
         """
             This function checks to see if the meta-species the species_string belong to has inherited from the
             parameter reference (reminder: every meta-species inherits from itself)
 
-            Parameters:
-                reference (Species) = Meta-species object
-
-            Returns:
-                True if the meta-species in Specific_Species_Operator has inherited from the reference
-                False otherwise
+            :param reference: (Species) Meta-species object
+            :return: (bool) True if the meta-species in Specific_Species_Operator has inherited from the reference
+            False otherwise
         """
         if not self._stocked_characteristics:
             if reference in self._species_object.get_references():
                 return True
             else:
                 return False
         else:
-            simlog.error('Concatenation of is_a and dot operator still not supported. Please use them separately')
+            simlog.error('Concatenation of is_a and dot operator not supported. Please use them separately',
+                         stack_index=2)
 
     def add(self, characteristic):
         """
-            Adds characteristics to the set of characteristics
+            Adds characteristic to the set of characteristics when checking for all
+            referred characteristics by the user
 
-            Parameters:
-                characteristic (str) = characteristic to add to the set
+            :param characteristic: (str) characteristic to add to the set
         """
         self._stocked_characteristics.add(characteristic)
 
 
 def extract_reaction_rate(combination_of_reactant_species, reactant_string_list
-                          , reaction_rate_function, type_of_model, dimension):
+                          , reaction_rate_function, type_of_model, dimension, function_rate_arguments=None):
     """
         This function is responsible for returning the reaction rate string for the model construction. To do this it
         does a different action depending on the type of the reaction_rate_function (we consider constants as functions)
         It passes the rate as a string expression in MobsPy standard units
 
-        Parameters:
-            combination_of_reactant_species (list of Species) = Meta-species currently being used in this reaction
-            reactant_string_list (list of strings) = list of species strings in order they apear in the reaction
-            reaction_rate_function (float, callable, Quantity) = rate stored in the reaction object
-            dimension (int) = system dimension (for the rate conversion)
-
-        Returns:
-            reaction_rate_string (str) = the reaction kinetics as a string for SBML
-            extra_species (list) = species that appear in the rate but are not reactants (COPASI will throw an error)
-    """
-    extra_species = []
-    if type(reaction_rate_function) == int or type(reaction_rate_function) == float or isinstance(reaction_rate_function, Quantity):
-        reaction_rate_function = uh.convert_rate(reaction_rate_function, len(reactant_string_list), dimension)
+        :param  function_rate_arguments: list of strings of the function rate argument ex:['r1', 'r2', ....]
+        :param  combination_of_reactant_species: (list of Species) Meta-species currently being used in this reaction
+        :param  reactant_string_list: (list of strings) list of species strings in order they apear in the reaction
+        :param  reaction_rate_function: (float, callable, Quantity) rate stored in the reaction object
+        :param  dimension: (int) system dimension (for the rate conversion)
+
+        :return: reaction_rate_string (str) the reaction kinetics as a string for SBML
+    """
+
+    if type(reaction_rate_function) == int or type(reaction_rate_function) == float or \
+            isinstance(reaction_rate_function, Quantity):
+        # Function is a constant function number int here
+        reaction_rate_function, dimension = uh.convert_rate(reaction_rate_function, len(reactant_string_list),
+                                                            dimension)
+        if reaction_rate_function == 0:
+            return 0
         reaction_rate_string = basic_kinetics_string(reactant_string_list,
                                                      reaction_rate_function, type_of_model)
 
-    elif callable(reaction_rate_function):
-        arguments = prepare_arguments_for_callable(combination_of_reactant_species,
-                                                   reactant_string_list, reaction_rate_function.__code__.co_varnames)
-        rate = reaction_rate_function(**arguments)
-        rate = uh.convert_rate(rate, len(reactant_string_list), dimension)
+    elif function_rate_arguments is not None:
+
+        # [''] means that it is a function that takes no arguments (empty signature)
+        if function_rate_arguments != ['']:
+            arguments = prepare_arguments_for_callable(combination_of_reactant_species,
+                                                       reactant_string_list, function_rate_arguments)
+
+            rate = reaction_rate_function(**arguments)
+        else:
+            rate = reaction_rate_function()
+
+        rate, dimension = uh.convert_rate(rate, len(reactant_string_list), dimension)
+        if rate == 0:
+            return 0
 
         if type(rate) == int or type(rate) == float:
             reaction_rate_string = basic_kinetics_string(reactant_string_list,
                                                          rate, type_of_model)
         elif type(rate) == str:
             reaction_rate_string = rate
         elif rate is None:
             simlog.error('There is a reaction rate missing for the following reactants: \n'
                          + str(reactant_string_list))
         else:
-            simlog.error('The function return a non-valid value')
+            simlog.error(f'The rate function {reaction_rate_function}, returned a non-valid value. \n' +
+                         f'Only int, floats and str are accepted')
     elif reaction_rate_function is None:
         simlog.error('There is a reaction rate missing for the following reactants: \n'
                      + str(reactant_string_list))
+    elif type(reaction_rate_function) == str:
+        return reaction_rate_function
     else:
         simlog.debug(type(reaction_rate_function))
-        simlog.error('The rate type is not supported')
+        simlog.error(f'The {type(reaction_rate_function)}, from {reaction_rate_function} is not supported')
 
     return reaction_rate_string
 
 
 def basic_kinetics_string(reactants, reaction_rate, type_of_model):
     """
         This constructs the bases for mass-action kinetics. Both for stochastic and deterministic depending on the type
         of model
 
-        Parameters:
-            reactants (list of str) = list of reactants in MobsPy str format
-            reaction_rate (float) = reaction constant
-            type_of_model (str) = stochastic or deterministic - rate expressions are different depending on each case
+        :params reactants: (list of str) list of reactants in MobsPy str format
+        :params reaction_rate: (float) reaction constant
+        :params type_of_model: (str) stochastic or deterministic - rate expressions are different depending on each case
 
-        Returns:
-            kinetics_string (str) = mass action kinetics expression for the reaction
+        :return:  kinetics_string (str) mass action kinetics expression for the reaction
     """
     counts = rc.count_string_dictionary(reactants)
 
     if type_of_model.lower() not in ['stochastic', 'deterministic']:
-        simlog.error('Type of model not supported. Only stochastic or deterministic')
+        simlog.error(f'The following method for simulation {type_of_model} is not supported.\n' +
+                     f'Only stochastic or deterministic')
 
     kinetics_string = ""
     for name, number in counts.items():
         if type_of_model.lower() == 'stochastic':
             kinetics_string += stochastic_string(name, number)
         elif type_of_model.lower() == 'deterministic':
             kinetics_string += deterministic_string(name, number)
@@ -219,20 +218,18 @@
 
 def stochastic_string(reactant_name, number):
     """
         This function returns the stochastic string expression for mass action kinetics
         For instance the reaction 2A -> 3A would imply A*(A-1)/2
         It only does so for one reactant, so it must be called for all reactants in the reaction
 
-        Parameters:
-            reactant_name (str) = species string involved in the reaction
-            number (int) = stoichiometry (number of times it appears)
+        :params reactant_name: (str) species string involved in the reaction
+        :params number: (int) stoichiometry (number of times it appears)
 
-        Returns:
-            to_return_string (str) = the mass action kinetics string expression for only that species
+        :return: to_return_string (str) the mass action kinetics string expression for only that species
     """
     to_return_string = ''
     for i in range(number):
         if i == 0:
             to_return_string = reactant_name
         else:
             to_return_string += f' * ({reactant_name} - {i})/{i + 1}'
@@ -242,20 +239,18 @@
 
 def deterministic_string(reactant_name, number):
     """
         This function returns the deterministic string expression for mass action kinetics
         For instance the reaction 2A -> 3A would imply A*A
         It only does so for one reactant, so it must be called for all reactants in the reaction
 
-        Parameters:
-            reactant_name (str) = species string involved in the reaction
-            number (int) = stoichiometry (number of times it appears)
+        :params reactant_name: (str) species string involved in the reaction
+        :params number: (int) stoichiometry (number of times it appears)
 
-        Returns:
-            to_return_string (str) = the mass action kinetics string expression for only that species
+        :return: to_return_string (str) the mass action kinetics string expression for only that species
     """
     to_return_string = ''
     for i in range(number):
         if i == 0:
             to_return_string = reactant_name
         else:
             to_return_string += f' * {reactant_name}'
@@ -263,31 +258,31 @@
 
 
 def prepare_arguments_for_callable(combination_of_reactant_species, reactant_string_list, rate_function_arguments):
     """
         This function prepares the requested arguments to the rate function for a given reaction by creating objects
         of the Specific_Species_Operator class
 
-        Parameters:
-            combination_of_reactant_species : meta-species involved in the reaction
-            reactant_string_list : species strings involved in the reaction
-            rate_function_arguments : arguments received by the rate function
+        :params combination_of_reactant_species: meta-species involved in the reaction
+        :params reactant_string_list: species strings involved in the reaction
+        :params rate_function_arguments: arguments received by the rate function
     """
     argument_dict = {}
-    i = 0
-    for i, (species, reactant_string) in enumerate(zip(combination_of_reactant_species, reactant_string_list)):
-        try:
-            species = species['object']
-            argument_dict[rate_function_arguments[i]] = Specific_Species_Operator(species_string=reactant_string,
-                                                                                  species_object=species)
-        except IndexError:
-            continue
-
-    while len(argument_dict) < len(rate_function_arguments):
-        argument_dict[rate_function_arguments[i]] = Specific_Species_Operator('$Null', mc.Zero)
-        i += 1
+    if rate_function_arguments is not None:
+        i = 0
+        for i, (species, reactant_string) in enumerate(zip(combination_of_reactant_species, reactant_string_list)):
+            try:
+                species = species['object']
+                argument_dict[rate_function_arguments[i]] = Specific_Species_Operator(species_string=reactant_string,
+                                                                                      species_object=species)
+            except IndexError:
+                continue
+
+        while len(argument_dict) < len(rate_function_arguments):
+            i += 1
+            argument_dict[rate_function_arguments[i]] = Specific_Species_Operator('$Null', mc.Zero)
 
     return argument_dict
 
 
 if __name__ == '__main__':
     pass
```

### Comparing `mobspy-1.1.3/mobspy/modules/meta_class_utils.py` & `mobspy-2.0.1/mobspy/modules/meta_class_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,78 +2,58 @@
     This model stores function used by the meta_class.py module
 """
 import copy
 import itertools
 import mobspy.simulation_logging.log_scripts as simlog
 
 
-def unite_dictionaries(first_dict, second_dict):
-    """
-        Performs the union of two dictionaries whose values are sets.
-
-        Parameters:
-            first_dict (dict)
-            second_dict (dict)
-    """
-    for key in second_dict:
-        try:
-            first_dict[key].union(second_dict[key])
-        except KeyError:
-            first_dict[key] = second_dict[key]
-
-
 def combine_references(species1, species2):
     """
         Combine the sets of references of two species
 
-        Parameters:
-            species1 (Meta-species object)
-            species2 (Meta-species object)
+        :param species1: (Meta-species object)
+        :param species2: (Meta-species object)
     """
-    #if species1.get_references().intersection(species2.get_references()):
-    #    simlog.warning(f'A product was executed between species with a common meta-species\n')
-
     return species1.get_references().union(species2.get_references())
 
 
 def check_orthogonality_between_references(references):
     """
         Check if meta-species objects inside a reference do not have characteristics in common
         The sets of characteristics directly added to species must be independent
 
-        Parameter:
-            references (set) =  set of meta-species objects to check for independence
+        :param references: (set) set of meta-species objects to check for independence
+        :raise simlog.error: raises error if there are repeated characteristics in different meta-species
     """
     for i, reference1 in enumerate(references):
         for j, reference2 in enumerate(references):
 
             if i == j:
                 continue
 
             if len(reference1.get_characteristics().intersection(reference2.get_characteristics())) != 0:
-                simlog.error(f'A characteristic must be unique for species construction'
+                simlog.error(f'The same characteristic can only be shared through inheritance. ' +
+                             f'There are two characteristics directly added to two meta-species \n'
                              f'Repetition in: {reference1}, {reference2}'
                              f'Characteristics: {reference1.get_characteristics()}, {reference2.get_characteristics()}')
 
 
 def complete_characteristics_with_first_values(spe_object, characteristics, characteristics_to_object):
     """
         This creates a string with the species object name and the set of all first characteristics added
         to it's base species used to construct it
         It allows us to search for the proper string in the model using the result of this function
         It's used to set the quantities using the call method in Species and Reacting_Species
 
-        Parameters:
-            spe_object (meta-species object) = meta-species to generate the species states with the first values
-            characteristics (str) = if there are characteristics to use instead of the default
-            characteristics_to_object (dict) = dictionary with characteristics as keys and the meta-species which
-            they have been added to directly as value (no inheritance or New)
+        :param spe_object: (meta-species object) meta-species to generate the species states with the first values
+        :param characteristics: (str) if there are characteristics to use instead of the default
+        :param characteristics_to_object: (dict) dictionary with characteristics as keys and the meta-species which
+        they have been added to directly as value (no inheritance or New)
 
-        Returns:
-            Set with the species name and characteristics
+        :return: Set with the species name and characteristics
     """
     if characteristics == 'std$':
         characteristics = set()
 
     vector_elements = {}
     for cha in characteristics:
         vector = characteristics_to_object[cha]
@@ -86,120 +66,56 @@
     for reference in spe_object.get_references() - set(vector_elements.keys()):
         if reference.first_characteristic:
             first_characteristics.add(reference.first_characteristic)
 
     return {spe_object.get_name()}.union(first_characteristics).union(characteristics)
 
 
-def extract_characteristics_from_string(species_string):
-    """
-        Species are named for the SBML as species_name_dot_characteristic1_dot_characteristic2
-        So this transforms them into a set
-
-        Parameters:
-            species_string (str) = species string in MobsPy for SBML format (with _dot_ instead of .)
-    """
-    return set(species_string.split('_dot_'))
-
-
-def turn_set_into_0_value_dict(set):
-    to_return = {}
-    for e in set:
-        to_return[e] = 0
-    return to_return
-
-
 def unite_characteristics(species):
     """
         This function unites the characteristics of all the given species
 
-        Parameters:
-            species (list of species or ParallelSpecies object)
+        :param species: (list of species or List_Species object)
     """
     characteristics = set()
 
     if species is not None:
         for spe in species:
             characteristics = characteristics.union(spe.get_characteristics())
 
     return characteristics
 
 
-def extract_characteristics(spe):
-    """
-        Extracts all the characteristics from a species and it's references
-
-        Parameters:
-            spe (meta-species object)
-    """
-    lists_of_characteristics = []
-    for reference in spe.get_references():
-        lists_of_characteristics.append(reference.get_characteristics())
-
-    return lists_of_characteristics
-
-
 def create_orthogonal_vector_structure(species):
     """
         This creates the independent state-structure for the model
         It is just a dictionary where the keys are characteristics and the values are meta-species objects that have
         been directly added to that object (no inheritance or New)
         It simplifies the code by allowing to easily keep track of the 'axis' of each characteristic. Allowing
         for easy transformation on the products and others
 
-        Parameters:
-            species (meta-species objects) - meta-species objects used in a model
+        :param species: (meta-species objects) - meta-species objects used in a model
 
-        Returns:
-            ref_characteristics_to_object (dict) = a dictionary where the keys are characteristics and the
-            values are meta-species objects that have been directly added to that object
+        :return ref_characteristics_to_object: (dict) a dictionary where the keys are characteristics and the
+        values are meta-species objects that have been directly added to that object
     """
     ref_characteristics_to_object = {}
     for spe in species:
         for prop in spe.get_references():
             for cha in prop.get_characteristics():
 
                 if cha not in ref_characteristics_to_object:
                     ref_characteristics_to_object[cha] = prop
                 elif ref_characteristics_to_object[cha] == prop:
                     pass
                 else:
-                    simlog.error(f'A characteristic must be unique for each species \n'
+                    simlog.error(f'The same characteristic can only be shared through inheritance. ' +
+                                 f'There are two characteristics directly added to two meta-species \n'
                                 f'Repetition in: {spe}, {ref_characteristics_to_object[cha] } \n'
-                                f'Characteristics: {spe.get_characteristics()}, {ref_characteristics_to_object[cha].get_characteristics()} \n')
+                                f'Characteristics: {spe.get_characteristics()}, '
+                                 f'{ref_characteristics_to_object[cha].get_characteristics()} \n')
 
     return ref_characteristics_to_object
 
 
-def create_species_strings(spe_object, sets_of_characteristics):
-    """
-        This function combines the species name with all the characteristics of it's references.
-        This way it creates the strings that will be used for the SBML
-        All possible combinations are created, with no intersections between characteristics of
-        a same referenced species
-
-        Parameters:
-            spe_object (meta-species object) = received species object
-            sets_of_characteristics (set of sets (thus not a set)) = all sets of characteristics from the
-            referenced objects
-
-        Returns:
-            set_of_species (set) = set of species from the meta-species object
-    """
-
-    # Remove empty sets from the list and transform sets in lists
-    # Sort the lists so the characteristics will appear in the same order e
-    lists_of_definitions = [sorted(list(i)) for i in sets_of_characteristics if i != set()]
-    set_of_species = set()
-    lists_of_definitions = sorted(lists_of_definitions)
-
-    for i in itertools.product(*lists_of_definitions):
-        if lists_of_definitions:
-            set_of_species.add(spe_object.get_name() + '_dot_' + '_dot_'.join(i))
-        else:
-            set_of_species.add(spe_object.get_name())
-
-    return set_of_species
-
-
 if __name__ == '__main__':
     pass
```

### Comparing `mobspy-1.1.3/mobspy/modules/order_operators.py` & `mobspy-2.0.1/mobspy/modules/order_operators.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,272 +4,265 @@
     are not referenced in the reactants (Born Species)
     It has also the implementation of the Rev operator, since that is a also a reaction operator
 """
 from copy import deepcopy
 import mobspy.modules.meta_class_utils as mcu
 import mobspy.modules.meta_class as mc
 import mobspy.simulation_logging.log_scripts as simlog
+import mobspy.modules.species_string_generator as ssg
 
 
 class __Operator_Base:
     """
         This is the order operator base. It contains some functions that can be useful the reaction operators defined
         Reaction Operators are now responsible for order assignment and how to deal with species in the products that
         are not referenced in the reactants (Born Species)
         It also overrides the getitem method so we can use:
         Operator[Reaction] to assign an order to the reaction
     """
 
     # Assign order structure
     def __getitem__(self, item):
-        item.order = self
+        try:
+            if type(item) == str:
+                return item + '.all$'
+
+            if item.is_species():
+                return item.c('all$')
+            elif not item.is_species():
+                for reactant in item.list_of_reactants:
+                    reactant['characteristics'].add('all$')
+                return item
+        except AttributeError:
+            simlog.error('All can only be used on species, reacting species and strings under set_count',
+                         stack_index=2)
 
     # Transform product function
     @staticmethod
     def transform_species_string(species_string, characteristics_to_transform,
                                  ref_characteristics_to_object):
         """
             This function handles the characteristic change due to a chemical reaction. It receives a string in the
             MobsPy format and the characteristic one has written on the product side of the reaction
             MobsPy them converts the characteristics in the same position as that one (that have been directly
             added to the same meta-species) to the one in the characteristics_to_transform variable
 
-            Parameters:
-                species_string (str) = A string associated with a species in the MobsPy format
-                characteristics_to_transform (str) = Characteristics received by the species object in the product
-                ref_characteristics_to_object (dict) = Dictionary with the characteristics as keys and meta-species
-                objects as values
-        """
-        species_to_return = deepcopy(species_string)
-        for characteristic in characteristics_to_transform:
-            replaceable_characteristics = ref_characteristics_to_object[characteristic].get_characteristics()
+            :param  species_string: (str) A string associated with a species in the MobsPy format
+            :param  characteristics_to_transform: (str) Characteristics received by the species object in the product
+            :param ref_characteristics_to_object: (dict) Dictionary with the characteristics as keys and meta-species
+            objects as values
+        """
+        species_object = species_string[0]
+        species_to_return = [species_object.get_name()] + deepcopy(species_string[1:]) \
+            if len(species_string) > 1 else [species_object.get_name()]
 
-            for rep_cha in replaceable_characteristics:
-                species_to_return = species_to_return.replace('_dot_' + rep_cha, '_dot_' + characteristic)
+        for characteristic in characteristics_to_transform:
+            obj = ref_characteristics_to_object[characteristic]
+            i = species_object.get_index_from_reference_dict(obj)
+            species_to_return[i] = characteristic
+        species_to_return = '_dot_'.join(species_to_return)
 
         return species_to_return
 
     @staticmethod
-    def find_all_string_references_to_born_species(species_referenced_by, characteristics, species_string_dictionary):
+    def find_all_string_references_to_born_species(species_referenced_by, characteristics,
+                                                   ref_characteristics_to_object):
         """
             Finds all the string species that reference the born-meta species, including inheritors
             Returns them all in a list for the product construction
 
-            Parameters:
-                species_referenced_by (meta-species list) = List of species that inherit from the born-meta species
-                in the reaction
-                characteristics (str) = List of characteristics queried on the born species in the product
-                species_string_dictionary (dict) = Dictionary with meta-species as keys and a list of species strings
-                as values
+            :param species_referenced_by: (meta-species list) List of species that inherit from the born-meta species
+            in the reaction
+            :param characteristics: (str) List of characteristics queried on the born species in the product
+            :param meta_species_in_model: (list) list of meta-species in model
+            as values
         """
         to_return = []
         for species in species_referenced_by:
-            for key in species_string_dictionary:
-                if species in key.get_references():
-                    for species_string in species_string_dictionary[key]:
-                        species_string_split = species_string.split('_dot_')[1:]
-                        if all([char in species_string_split for char in characteristics]):
-                            to_return.append(species_string)
-
+            to_return += ssg.construct_all_combinations(species, characteristics,
+                                                        ref_characteristics_to_object, symbol='_dot_')
         return to_return
 
     @staticmethod
-    def find_all_default_references_to_born_species(species_referenced_by, characteristics, species_string_dictionary,
+    def find_all_default_references_to_born_species(species_referenced_by, characteristics,
                                                     ref_characteristics_to_object):
         """
             Finds only the DEFAULT string species that reference the born-meta species, including inheritors
             Returns them all in a list for the product construction.
 
-            Parameters:
-                species_referenced_by (meta-species list) = List of species that inherit from the born-meta species
-                in the reaction
-                characteristics (str) = List of characteristics queried on the born species in the product
-                species_string_dictionary (dict) = Dictionary with meta-species as keys and a list of species strings
-                as values
-                ref_characteristics_to_object (dict) =  Dictionary with the characteristics as keys and meta-species
-                objects that they have been directly added to as values
+            :param species_referenced_by: (meta-species list) List of species that inherit from the born-meta species
+            in the reaction
+            :param characteristics: (str) List of characteristics queried on the born species in the product
+            :param meta_species_in_model: (list) list of meta-species in model
+            :param ref_characteristics_to_object: (dict) Dictionary with the characteristics as keys and meta-species
+            objects that they have been directly added to as values
         """
         to_return = []
-
         for species in species_referenced_by:
-            characteristics_to_find = mcu.complete_characteristics_with_first_values(species, characteristics,
-                                                                                     ref_characteristics_to_object)
-
-            characteristics_to_find.remove(species.get_name())
-            characteristics_to_find.union(characteristics)
-
-            for key in species_string_dictionary:
-                if species in key.get_references():
-                    for species_string in species_string_dictionary[key]:
-                        species_string_split = species_string.split('_dot_')[1:]
-                        if all([char in species_string_split for char in characteristics_to_find]):
-                            to_return.append(species_string)
+            to_return += [ssg.construct_species_char_list(species, characteristics,
+                                                          ref_characteristics_to_object, symbol='_dot_')]
 
         return to_return
 
-
-class __Round_Robin_Base(__Operator_Base):
-    """
-        Here we have the implementation of the round robin order it goes like this:
-
-        2*Ecoli >> 4*Ecoli
-
-        Since an Ecoli is a generic object that refers to all types of Ecoli
-        This object refers to multiple reactions and to multiple strings
-        Therefore we follow this rule to know which string goes where:
-        1 Ecoli reactant >> 1 Ecoli product
-        2 Ecoli reactant >> 2 Ecoli product
-        1 Ecoli reactant >> 3 Ecoli product
-        2 Ecoli reactant >> 4 Ecoli product
-        This is a cycle (round robin) between the reactants to be assigned positions in the product
-        The products will keep the characteristics of the reactants except if stated otherwise with .
-        For completely new species (no reactant of the same species) we use ALL possible combinations
-        For only the default option see the code bellow
-
-        Methods:
-            __call__
-    """
-
     def __call__(self, order_dictionary, product_species,
-                 species_string_dictionary,
-                 ref_characteristics_to_object):
+                 model, ref_characteristics_to_object, all_reactions=False):
         """
             This function is responsible for parrying the products with the reactants according to their meta-species
             It parries them using the order_dictionary and an index-system for the round-robin application
             If it cannot find a parrying it considers it a born species
 
-            Parameters:
-                order_dictionary (dict) = Dictionary with the meta-species as keys and the list of meta-species strings
-                product_species (dict) = Product species dict with the meta-species object (key: species),
-                label (key: label), and characteristics (key: characteristics)
-                ref_characteristics_to_object (dict) =  Dictionary with the characteristics as keys and meta-species
-                objects that they have been directly added to as values
+            :param order_dictionary: (dict) Dictionary with the meta-species as keys and the list of 
+            meta-species strings
+            :param product_species: (dict) Product species dict with the meta-species object (key: species),
+            label (key: label), and characteristics (key: characteristics)
+            :param ref_characteristics_to_object: (dict) Dictionary with the characteristics as keys and meta-species
+            objects that they have been directly added to as values
         """
         round_robin_index = {}
         for species, label in [(e['species'], e['label']) for e in product_species]:
             round_robin_index[(species, label)] = 0
 
         products = []
         for species, label, characteristics in [(e['species'], e['label'], e['characteristics']) for e in
                                                 product_species]:
 
+            if 'all$' in characteristics:
+                species_is_referenced_by = []
+                for spe_obe in model:
+                    if species in spe_obe.get_references():
+                        species_is_referenced_by.append(spe_obe)
+                products.append(self.find_all_string_references_to_born_species(species_is_referenced_by,
+                                                                                characteristics,
+                                                                                ref_characteristics_to_object))
+                continue
+
             # Simple round robin
             try:
                 species_to_transform_string = order_dictionary[(species, label)][round_robin_index[(species, label)]]
                 round_robin_index[(species, label)] = (round_robin_index[(species, label)] + 1) % len(
                     order_dictionary[(species, label)])
 
                 # Return in list of lists format for combination later
                 products.append([self.transform_species_string(species_to_transform_string, characteristics,
                                                                ref_characteristics_to_object)])
 
             # If the species is not on the reactants - order_dictionary
             except KeyError:
-
-                # Find all the species that reference the one in the reaction
                 species_is_referenced_by = []
-                for key in species_string_dictionary:
-                    if species in key.get_references():
-                        species_is_referenced_by.append(key)
+                for spe_obe in model:
+                    if species in spe_obe.get_references():
+                        species_is_referenced_by.append(spe_obe)
 
                 if len(species_is_referenced_by) == 0:
-                    simlog.error(f'{species} or inheritors are not in the model. Please add at least one')
+                    simlog.error(f'Species {species} was used in a reaction '
+                                 f'but itself or any inheritors are not in the model. Please add at least one')
 
-                products.append(self.find_all_string_references_to_born_species(species_is_referenced_by,
-                                                                                characteristics,
-                                                                                species_string_dictionary))
+                if all_reactions:
+                    # Find all the species that reference the one in the reaction
+                    products.append(self.find_all_string_references_to_born_species(species_is_referenced_by,
+                                                                                    characteristics,
+                                                                                    ref_characteristics_to_object))
+                else:
+                    # Find only default state of the species
+                    products.append(self.find_all_default_references_to_born_species(species_is_referenced_by,
+                                                                                     characteristics,
+                                                                                     ref_characteristics_to_object))
 
         return products
 
 
+class __Round_Robin_Base(__Operator_Base):
+    """
+        Here we have the implementation of the round robin order it goes like this:
+
+        2*Ecoli >> 4*Ecoli
+
+        Since an Ecoli is a generic object that refers to all types of Ecoli
+        This object refers to multiple reactions and to multiple strings
+        Therefore we follow this rule to know which string goes where:
+        1 Ecoli reactant >> 1 Ecoli product
+        2 Ecoli reactant >> 2 Ecoli product
+        1 Ecoli reactant >> 3 Ecoli product
+        2 Ecoli reactant >> 4 Ecoli product
+        This is a cycle (round robin) between the reactants to be assigned positions in the product
+        The products will keep the characteristics of the reactants except if stated otherwise with .
+        For completely new species (no reactant of the same species) we use ALL possible combinations
+        For only the default option see the code bellow
+    """
+
+    def __call__(self, order_dictionary, product_species,
+                 meta_species_in_model,
+                 ref_characteristics_to_object, all_reactions=True):
+        """
+            This function is responsible for parrying the products with the reactants according to their meta-species
+            It parries them using the order_dictionary and an index-system for the round-robin application
+            If it cannot find a parrying it considers it a born species
+
+            :param order_dictionary: (dict) Dictionary with the meta-species as keys and the list of 
+            meta-species strings
+            :param product_species: (dict) Product species dict with the meta-species object (key: species),
+            label (key: label), and characteristics (key: characteristics)
+            :param ref_characteristics_to_object: (dict)  Dictionary with the characteristics as keys and meta-species
+            objects that they have been directly added to as values
+        """
+        return super().__call__(order_dictionary, product_species, meta_species_in_model,
+                                ref_characteristics_to_object, all_reactions)
+
+
 # Define class to override the operators
 All = __Round_Robin_Base()
 
 
 class __RR_Default_Base(__Operator_Base):
     """
         Only default options for born species (no reference in reactant)
         See __Round_Robin_Base for clarification
-
-        Methods:
-            __call__
     """
 
     # Here is the default order requested by Thomas
     def __call__(self, order_dictionary, product_species,
-                 species_string_dictionary,
-                 ref_characteristics_to_object):
+                 meta_species_in_model,
+                 ref_characteristics_to_object, all_reactions=False):
         """
             This function is responsible for parrying the products with the reactants according to their meta-species
             It parries them using the order_dictionary and an index-system for the round-robin application
             If it cannot find a parrying it considers it a born species
 
-            Parameters:
-                order_dictionary (dict) = Dictionary with the meta-species as keys and the list of meta-species strings
-                product_species (dict) = Product species dict with the meta-species object (key: species),
-                label (key: label), and characteristics (key: characteristics)
-                ref_characteristics_to_object (dict) =  Dictionary with the characteristics as keys and meta-species
-                objects that they have been directly added to as values
+            :param order_dictionary: (dict) Dictionary with the meta-species as keys and the list of meta-species
+            strings
+            :param product_species: (dict) Product species dict with the meta-species object (key: species),
+            label (key: label), and characteristics (key: characteristics)
+            :param ref_characteristics_to_object: (dict) Dictionary with the characteristics as keys and meta-species
+            objects that they have been directly added to as values
         """
-        round_robin_index = {}
-        for species, label in [(e['species'], e['label']) for e in product_species]:
-            round_robin_index[(species, label)] = 0
-
-        products = []
-        for species, label, characteristics in [(e['species'], e['label'], e['characteristics']) for e in
-                                                product_species]:
-
-            # Simple round robin
-            try:
-                species_to_transform_string = order_dictionary[(species, label)][round_robin_index[(species, label)]]
-                round_robin_index[(species, label)] = (round_robin_index[(species, label)] + 1) % len(
-                    order_dictionary[(species, label)])
-
-                # Return in list of lists format for combination later
-                products.append([self.transform_species_string(species_to_transform_string, characteristics,
-                                                               ref_characteristics_to_object)])
-
-            # If the species is not on the reactants - order_dictionary
-            except KeyError:
-
-                # Find all the species that reference the one in the reaction
-                species_is_referenced_by = []
-                for key in species_string_dictionary:
-                    if species in key.get_references():
-                        species_is_referenced_by.append(key)
-
-                if len(species_is_referenced_by) == 0:
-                    simlog.error(f'{species} or inheritors are not in the model. Please add at least one')
-
-                products.append(self.find_all_default_references_to_born_species(species_is_referenced_by,
-                                                                                 characteristics,
-                                                                                 species_string_dictionary,
-                                                                                 ref_characteristics_to_object))
-
-        return products
+        return super().__call__(order_dictionary, product_species, meta_species_in_model,
+                                ref_characteristics_to_object, all_reactions)
 
 
 Default = __RR_Default_Base()
 
 
 class __Set_Reversible_Rate:
     """
         This class is responsible for dealing with reversible reactions
         Since reversible reactions have too rates
         The process is in __getitem__
     """
+
     def __getitem__(self, both_rates):
         """
             This function extracts both reaction rates from a tuple
 
-            Parameters:
-                both_rates (rate functions) = rate function from the direct and reverse reaction
+            :param both_rates: (rate functions) rate function from the direct and reverse reaction
         """
-        if len(both_rates) != 2:
-            simlog.error('The reversible reaction must receive 2 rates')
+        try:
+            if len(both_rates) != 2:
+                simlog.error('The reversible reaction must receive 2 rates', stack_index=2)
+        except TypeError:
+            simlog.error('The reversible reaction must receive 2 rates', stack_index=2)
 
         self.reaction_direct.rate = both_rates[0]
         self.reaction_reverse.rate = both_rates[1]
 
     def __init__(self):
         """
             This a dummy constructor, the class object Rev is the one with the __getitem__ overridden
@@ -286,16 +279,15 @@
 class __Reversible_Base:
 
     def __getitem__(self, reaction):
         """
             This __getitem__ uses the rate setter which is a instance of __Set_Reversible_Rate to set the reversible
             reaction rates. It also creates the reverse reaction with the constructor
 
-            Parameters:
-                reaction (Reaction object) = object from the reaction class
+            :param reaction: (Reaction object) object from the reaction class
         """
         reaction_direct = reaction
         reaction_reverse = mc.Reactions(reaction_direct.products, reaction_direct.reactants)
         self.rate_setter.set_reactions(reaction_direct, reaction_reverse)
         return self.rate_setter
 
     def __init__(self, rate_setter):
```

### Comparing `mobspy-1.1.3/mobspy/modules/reaction_construction_nb.py` & `mobspy-2.0.1/mobspy/modules/reaction_construction_nb.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,14 +2,17 @@
     This module is responsible for the construction of all individual reactions from a meta-reaction
 """
 from copy import deepcopy
 import mobspy.modules.function_rate_code as fr
 import itertools
 import mobspy.modules.meta_class as mc
 import mobspy.simulation_logging.log_scripts as simlog
+import mobspy.modules.species_string_generator as ssg
+from inspect import signature
+from mobspy.modules.order_operators import Default
 
 
 def iterator_for_combinations(list_of_lists):
     """
         Iterate through all the combinations of a list of lists
         [[A,B,C], [D, F, E], [G]] means:
         ADG, AFG, AEG, BDG, BFG, BEG, CDG, CFG, CEG .....
@@ -52,35 +55,35 @@
 
 def check_for_invalid_reactions(reactions, ref_characteristics_to_object):
     """
         If query references two independent characteristics from the in meta-species it would result in an empty set
         Like Ecoli.live.dead - (assuming live and dead belong to the same meta-species characteristics set)
         If that ever happens inside a meta-reaction we just pop an error
 
-        Parameters:
-            reactions (set of meta-reactions) = set of meta-reactions inside the model
-            ref_characteristics_to_object (dict) = dictionary where the characteristics are the keys and the values
-            are the meta-species objects that they have been directly added to
+        :param reactions: (set of meta-reactions) set of meta-reactions inside the model
+        :param ref_characteristics_to_object: (dict) dictionary with the characteristics as keys and their respective
+        object as values
     """
     for reaction in reactions:
         for reactant in reaction.reactants:
 
             check_for_duplicates = {}
             for cha in reactant['characteristics']:
 
                 # Ok I love try catches for checking if something is in a dict. Don't judge me
                 try:
                     check_for_duplicates[ref_characteristics_to_object[cha]]
-                    simlog.error('Illegal reaction, there is a product with multiple '
-                                 'characteristics from the same Species referenced \n'
-                                 'Please divide the reaction accordingly \n'
-                                 f'Error in {ref_characteristics_to_object[cha]} both {cha} and '
-                                 f'{check_for_duplicates[ref_characteristics_to_object[cha]]}'
-                                 f' referenced at the same time \n'
-                                 f'The characteristics: {ref_characteristics_to_object[cha].get_characteristics()}')
+                    simlog.error(f'Illegal reaction: {reaction}. \n'
+                                 'There is a query with two characteristics '
+                                 f'{ref_characteristics_to_object[cha].get_characteristics()} from the same'
+                                 f' vector axis resulting in an impossible query. \n'
+                                 f'As all those characteristics have been directly added to'
+                                 f'{ref_characteristics_to_object[cha]}, they are located in the same vector axis. \n'
+                                 f'To solve this either assign the characteristics to new meta-species and use '
+                                 f'inheritance or create a new reaction for each desired query.')
                 except KeyError:
                     try:
                         check_for_duplicates[ref_characteristics_to_object[cha]] = cha
                     except KeyError:
                         simlog.error(
                             'The characteristic\'s object was not found in the species supplied to the simulator \n'
                             'Perhaps a species is missing ?')
@@ -89,81 +92,81 @@
 
             check_for_duplicates = {}
             for cha in product['characteristics']:
 
                 # Ok I love try catches for checking if something is in a dict. Don't judge me
                 try:
                     check_for_duplicates[ref_characteristics_to_object[cha]]
-                    simlog.error('Illegal reaction, there is a product with multiple '
-                                 'characteristics from the same Species referenced \n'
-                                 'Please divide the reaction accordingly \n'
-                                 f'Error in {ref_characteristics_to_object[cha]} both {cha} and '
-                                 f'{check_for_duplicates[ref_characteristics_to_object[cha]]}'
-                                 f' referenced at the same time \n'
-                                 f'The characteristics: {ref_characteristics_to_object[cha].get_characteristics()}')
+                    simlog.error(f'Illegal reaction: {reaction}. \n'
+                                 'There is a transformation with two characteristics '
+                                 f'{ref_characteristics_to_object[cha].get_characteristics()} from the same'
+                                 f' vector axis resulting in an undefinable transformation. \n'
+                                 f'As all those characteristics have been directly added to '
+                                 f'{ref_characteristics_to_object[cha]}, they are located in the same vector axis. \n'
+                                 f'To solve this either assign the characteristics to new meta-species and use '
+                                 f'inheritance or create a new reaction for each desired query.')
                 except KeyError:
-                    check_for_duplicates[ref_characteristics_to_object[cha]] = cha
+                    if '$' not in cha:
+                        check_for_duplicates[ref_characteristics_to_object[cha]] = cha
 
 
-def construct_reactant_structures(reactant_species, species_string_dict):
+def construct_reactant_structures(reactant_species, ref_characteristics_to_object):
     """
         This function finds the corresponding strings according to the reactant meta-species with or without a query
         pack then in a list and return
 
-        Parameters:
-            reactant_species (meta-species object) = species objects of the involved species
-            species_string_dict (dict)=  dictionary with species objects as keys and corresponding species strings
+        :param reactant_species: (meta-species object) species objects of the involved species
+        :param ref_characteristics_to_object: (dict) dictionary with characteristics as keys and species objects as
+        values
     """
     species_string_combinations = []
 
     for reactant in reactant_species:
-        species_string_combinations.append(extract_species_strings(reactant['object'],
-                                                                   reactant['characteristics'], species_string_dict))
+        species_string_combinations.append(ssg.construct_all_combinations(reactant['object'],
+                                                                          reactant['characteristics'],
+                                                                          ref_characteristics_to_object))
 
     return species_string_combinations
 
 
 def construct_order_structure(species_order_list, current_species_string_list):
     """
         Order structure for reaction order operations. Returns the cyclic_dictionary to be used by the order operator.
         The meta-species objects are the keys of this dictionary and a lists of species strings currently being used
         in the reaction are the values - Allowing the product to find it's corresponding species-string in a future
         step
 
-        Parameters:
-            species_order_list (list of meta-species objects): list of meta-species objects as they appear in the
-            meta-reaction
-            current_species_string_list (list of strings): list of strings in MobsPy format of the species currently
-            in this specific reaction
+        :param species_order_list: (list of meta-species objects) list of meta-species objects as they appear in the
+        meta-reaction
+        :param current_species_string_list: (list of strings) list of strings in MobsPy format of the species
+        currently in this specific reaction
 
-        Returns:
-            cyclic_dict (dict) = Dictionary where the keys are meta-species objects and the values are lists of species
+        :return: cyclic_dict (dict) Dictionary where the keys are meta-species objects and the values are
+        lists of species
     """
     cyclic_dict = {}
     for species_object, species_string in zip(species_order_list, current_species_string_list):
 
         try:
             cyclic_dict[species_object].append(species_string)
         except KeyError:
             cyclic_dict[species_object] = [species_string]
 
     return cyclic_dict
 
 
 def construct_product_structure(reaction):
-    '''
+    """
         This function unpacks the products in a meta-reaction
 
-        Parameters:
-            reaction = meta-reaction currently being analysed
+        :param: reaction meta-reaction currently being analysed
 
-        Returns:
-            product_list: A list of dictionaries for each product with the meta-species object, the label and the
-            characteristics
-    '''
+        :return: product_list = A list of dictionaries for each product with the meta-species object, the label and the
+        characteristics
+    """
     product_list = []
     for product in reaction.products:
         for _ in range(product['stoichiometry']):
             product_list.append({'species': product['object'], 'label': product['label'],
                                  'characteristics': product['characteristics']})
 
     return product_list
@@ -172,21 +175,19 @@
 def construct_single_reaction_for_sbml(reactant_species_string_list, product_species_string_list, reaction_rate):
     """
         This function constructs the reactions for SBML for the conversion by the model builder script
         It follows the following structure 're':[('stoichmetry', reactantant_string) ....
         The reaction rate must be a string containing the reaction kinetics
         This returns a single reaction to be appended by the reactions_for_sbml dictionary
 
-        Parameters:
-            reactant_species_string_list (list of strings) = list of reactants in MobsPy format
-            product_species_string_list (list of strings) = list of products in MobsPy format
-            reaction_rate (str) = reaction rate expression as a string
+        :param reactant_species_string_list: (list of strings) list of reactants in MobsPy format
+        :param product_species_string_list: (list of strings) list of products in MobsPy format
+        :param reaction_rate: (str) reaction rate expression as a string
 
-        Returns:
-            to_return (dict) = dictionary that packs the reactants products and rate
+        :return: to_return (dict) = dictionary that packs the reactants products and rate
     """
     to_return = {'re': [], 'pr': [], 'kin': reaction_rate}
 
     reactant_count_dict = count_string_dictionary(reactant_species_string_list)
     product_count_dict = count_string_dictionary(product_species_string_list)
 
     for key in reactant_count_dict:
@@ -210,133 +211,134 @@
             to_return[e] += 1
         except KeyError:
             to_return[e] = 1
 
     return to_return
 
 
-def extract_species_strings(species, characteristics, species_string_dict):
-    """
-        Extract the species strings from the species_string_dict based on the meta-species and characteristics given
-
-        Parameters:
-            species (meta-species object) = Instance of the meta-species to obtain the species strings for
-            characteristics (str) = Characteristics to filter through
-            species_string_dict (dict) = Dictionary where the meta-species are the keys and the values all their
-            species
-
-        Returns:
-            species_strings_list (list of str) = species strings filtered from the meta-species
-    """
-    species_strings_list = []
-    species_strings_to_filter = set()
-
-    species_strings_to_filter = species_strings_to_filter.union(species_string_dict[species])
-
-    for species_string in species_strings_to_filter:
-        species_string_split = species_string.split('_dot_')[1:]
-        if all([char in species_string_split for char in characteristics]):
-            species_strings_list.append(species_string)
-
-    return species_strings_list
-
-
-def get_involved_species(reaction, species_string_dict):
+def get_involved_species(reaction, meta_species_in_model):
     """
         This extracts all the involved meta-species inside a reaction
         This function is responsible for implementing the inheritance mechanism, by finding within each meta-species
         references set, if they reference the meta-species in the reaction
 
-        Parameters:
-            reaction (meta-reaction object)
-            species_string_dict (dict) = dictionary where the keys are meta-species and the values are
-            lists of species they contain (used only for the keys here)
-
-        Returns:
-            base_species_order (list of meta-species objects): order that the meta-species appear in the meta-reaction
-            reactant_species_combination_list (list of lists of meta-species): list of lists of all meta-species that
-            have inherited from the meta-species in the meta-reaction
+        :param reaction: (meta-reaction object)
+        :param meta_species_in_model: (list) list of meta-species used in the model
+
+        :return: base_species_order (list of meta-species objects) = order that the meta-species appear in the
+        meta-reaction, reactant_species_combination_list (list of lists of meta-species) = list of lists of all
+        meta-species that have inherited from the meta-species in the meta-reaction
     """
     reactant_species_combination_list = []
     base_species_order = []
 
     for reactant in reaction.reactants:
         flag_absent_reactant = False
         for _ in range(reactant['stoichiometry']):
 
             species_for_reactant = []
             base_species_order.append((reactant['object'], reactant['label']))
 
-            for species in species_string_dict:
+            for species in meta_species_in_model:
                 if reactant['object'] in species.get_references():
                     species_for_reactant.append({'object': species,
                                                  'characteristics': reactant['characteristics']})
                     flag_absent_reactant = True
 
             if not flag_absent_reactant:
-                simlog.error(f'Species {reactant["object"]} was not found in model \n'
+                simlog.error(f'Species {reactant["object"]} or any inheritors were not found in model \n'
                              f'For reaction {reaction} \n'
                              f'Please add the species or remove the reaction')
 
             reactant_species_combination_list.append(species_for_reactant)
 
     return base_species_order, reactant_species_combination_list
 
 
-def create_all_reactions(reactions, species_string_dict,
+def construct_rate_function_arguments(rate_function, reaction):
+    rate_function_arguments = str(signature(rate_function))
+
+    black_list = ['*', '=']
+    if any(i in rate_function_arguments for i in black_list):
+        simlog.error(f'Rate arguments must not contain = or *. \n'
+                     f'Error in reaction {reaction}. \n'
+                     f'Error in rate function {rate_function} in signature {str(signature(rate_function))}')
+
+    rate_function_arguments = str(rate_function_arguments).replace('(', '')
+    rate_function_arguments = str(rate_function_arguments).replace(')', '')
+    rate_function_arguments = str(rate_function_arguments).replace(' ', '')
+    rate_function_arguments = rate_function_arguments.split(',')
+    return rate_function_arguments
+
+
+def create_all_reactions(reactions, meta_species_in_model,
                          ref_characteristics_to_object,
                          type_of_model, dimension):
     """
         This function creates all reactions
         Returns the reactions_for_sbml and parameters_for_sbml dictionary
         Those will be used by another module to create the SBML file
 
-        Parameters:
-            reactions (meta-reaction objects) = reactions objects constructed by the meta_class module
-            species_string_dict (dict) = Meta-species object keys and respective species strings values
-            ref_characteristics_to_object (dict) =  Characteristics as keys objects as values
-            type_of_model (str) = stochastic or deterministic
-            dimension (int) = model dimension 1D, 2D, 3D, .....
-
-        Returns:
-            reactions_for_sbml (dict) = dictionary with all reactions that will be added to the sbml model file
-            parameters_for_sbml (dict) = parameters for the sbml model file
-    """
+        :param reactions: (meta-reaction objects) reactions objects constructed by the meta_class module
+        :param meta_species_in_model: (list) list of meta-species in model
+        :param ref_characteristics_to_object: (dict) Characteristics as keys objects as values
+        :param type_of_model: (str) stochastic or deterministic
+        :param dimension: (int) model dimension 1D, 2D, 3D, .....
 
+        :returns: reactions_for_sbml (dict) = dictionary with all reactions that will be added to the sbml model file,
+        parameters_for_sbml (dict) = parameters for the sbml model file
+    """
     reactions_for_sbml = {}
     parameters_for_sbml = {}
 
     check_for_invalid_reactions(reactions, ref_characteristics_to_object)
 
     for reaction in reactions:
 
-        base_species_order, reactant_species_combination_list = get_involved_species(reaction, species_string_dict)
+        base_species_order, reactant_species_combination_list = get_involved_species(reaction, meta_species_in_model)
 
         for combination_of_reactant_species in iterator_for_combinations(reactant_species_combination_list):
 
             reactant_species_string_combination_list = \
-                construct_reactant_structures(combination_of_reactant_species, species_string_dict)
+                construct_reactant_structures(combination_of_reactant_species, ref_characteristics_to_object)
 
             for reactant_string_list in iterator_for_combinations(reactant_species_string_combination_list):
 
                 product_object_list = construct_product_structure(reaction)
                 order_structure = construct_order_structure(base_species_order, reactant_string_list)
 
-                product_species_species_string_combination_list = reaction.order(order_structure, product_object_list,
-                                                                                 species_string_dict,
-                                                                                 ref_characteristics_to_object)
+                if reaction.order is None:
+                    product_species_species_string_combination_list = Default(order_structure, product_object_list,
+                                                                              meta_species_in_model,
+                                                                              ref_characteristics_to_object)
+                else:
+                    product_species_species_string_combination_list = reaction.order(order_structure,
+                                                                                     product_object_list,
+                                                                                     meta_species_in_model,
+                                                                                     ref_characteristics_to_object)
 
                 for product_string_list in iterator_for_combinations(product_species_species_string_combination_list):
+
+                    reactant_strings = ['_dot_'.join([reactant[0].get_name()] + reactant[1:])
+                                        if len(reactant) > 1 else reactant[0].get_name()
+                                        for reactant in reactant_string_list]
+
+                    reaction_rate_arguments = None
+                    if callable(reaction.rate):
+                        reaction_rate_arguments = construct_rate_function_arguments(reaction.rate, reaction)
+
                     rate_string = fr.extract_reaction_rate(combination_of_reactant_species,
-                                                           reactant_string_list
+                                                           reactant_strings
                                                            , reaction.rate, type_of_model,
-                                                           dimension)
+                                                           dimension, reaction_rate_arguments)
+                    if rate_string == 0:
+                        continue
 
                     reactions_for_sbml['reaction_' + str(len(reactions_for_sbml))] = \
-                        construct_single_reaction_for_sbml(reactant_string_list,
+                        construct_single_reaction_for_sbml(reactant_strings,
                                                            product_string_list,
                                                            rate_string)
 
     return reactions_for_sbml, parameters_for_sbml
 
 
 if __name__ == '__main__':
```

### Comparing `mobspy-1.1.3/mobspy/modules/unit_handler.py` & `mobspy-2.0.1/mobspy/modules/unit_handler.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,143 +3,166 @@
     MobsPy standard units are Decimeter (Liter) - Second - Count
 """
 from pint import UnitRegistry, Quantity
 from scipy.constants import N_A
 from copy import deepcopy
 import os, sys
 import mobspy.simulation_logging.log_scripts as simlog
+import mobspy.modules.unit_handler as uh
 
 
 def convert_rate(quantity, reaction_order, dimension):
     """
         This function converts the rate from the users given unit to MobsPy standard units
 
-        Parameters:
-            quantity (int, float, Quantity) = If it is a quantity object convert, otherwise it remains the same
-            reaction_order (int) = number of reactants in the reaction, to check if the rate is in the correct unit
-            dimension (int) = model's dimension (1D, 2D, 3D, ... )
+        :param quantity: (int, float, Quantity) If it is a quantity object convert, otherwise it remains the same
+        :param reaction_order: (int) number of reactants in the reaction, to check if the rate is in the correct unit
+        :param dimension: (int) model's dimension (1D, 2D, 3D, ... )
 
-        Returns:
-            quantity (int, float) = converted unit into MobsPy standard units
+        :param quantity: (int, float) converted unit into MobsPy standard units
     """
     volume_power = reaction_order - 1
     converted_quantity = deepcopy(quantity)
+
+    # Dimension arrives as none but there is a rate
+    if dimension is None and isinstance(quantity, Quantity) and reaction_order > 1:
+        dimension = uh.extract_length_dimension(str(quantity.dimensionality), dimension,
+                                                reaction_order)
+
     if isinstance(quantity, Quantity):
         try:
             if volume_power <= 0:
-                converted_quantity.ito_base_units()
-                converted_quantity.ito(f'1/seconds')
-                return converted_quantity.magnitude
-
-            if '[substance]' in quantity.dimensionality:
-                converted_quantity.ito_base_units()
-                converted_quantity.ito(f'decimeters ** {dimension*volume_power}/(moles ** {volume_power} * seconds)')
-                return converted_quantity.magnitude / (N_A ** volume_power)
+                if '[substance]' in str(quantity.dimensionality):
+                    converted_quantity.ito(f'moles/seconds')
+                    return converted_quantity.magnitude, dimension
+                else:
+                    converted_quantity.ito(f'1/seconds')
+                    return converted_quantity.magnitude, dimension
             else:
-                converted_quantity.ito_base_units()
-                converted_quantity.ito(f'decimeters ** {dimension*volume_power}/seconds')
-                return converted_quantity.magnitude
+                if '[substance]' in str(quantity.dimensionality):
+                    converted_quantity.ito(f'decimeters ** {dimension*volume_power}/(moles ** {volume_power} * seconds)')
+                    return converted_quantity.magnitude / (N_A ** volume_power), dimension
+                else:
+                    converted_quantity.ito(f'decimeters ** {dimension*volume_power}/seconds')
+                    return converted_quantity.magnitude, dimension
         except Exception as e:
-            print(e)
-            simlog.error(f'Problem converting rate {quantity} \n'
-                         f'Is the rate in the form [volume] ** (order - 1)/[time]?')
+            simlog.error(str(e) + '\n' +
+                         f'Problem converting rate {quantity} \n'
+                         f'Is the rate in the form [volume]**{volume_power}/[time]?')
 
     else:
-        return quantity
+        return quantity, dimension
 
 
 def convert_counts(quantity, volume, dimension):
     """
         This function converts the counts from the users given unit to MobsPy standard units. It also converts
         concentrations into counts
 
-        Parameters:
-            quantity (int, float, Quantity) = If it is a quantity object convert, otherwise it remains the same
-            volume (int, float) = volume in liters (converted beforehand)
-            dimension (int) = model's dimension (1D, 2D, 3D, ... )
+        :param quantity: (int, float, Quantity) If it is a quantity object convert, otherwise it remains the same
+        :param volume: (int, float) volume in liters (converted beforehand)
+        :param dimension: (int) model's dimension (1D, 2D, 3D, ... )
 
-        Returns:
-            converted_quantity (int, float) = converted unit into MobsPy standard units
+        :return: converted_quantity (int, float) = converted unit into MobsPy standard units
     """
     converted_quantity = deepcopy(quantity)
+
     if isinstance(quantity, Quantity):
+        if '[length]' not in str(quantity.dimensionality) and '[substance]' not in quantity.dimensionality:
+            simlog.error(f'The assigned quantity {quantity} is neither a count or concentration')
+
         try:
             if '[substance]' in quantity.dimensionality:
-                converted_quantity.ito_base_units()
-                if '[length] ** 3' in str(quantity.dimensionality):
+                if '[length]' in str(quantity.dimensionality):
                     converted_quantity.ito(f'moles/(decimeter ** {dimension})')
                     converted_quantity = converted_quantity*volume
 
                 converted_quantity = converted_quantity.magnitude * N_A
             else:
-                converted_quantity.ito_base_units()
-                if '[length] ** 3' in str(quantity.dimensionality):
+                if '[length]' in str(quantity.dimensionality):
                     converted_quantity.ito(f'1/(decimeter ** {dimension})')
                     converted_quantity = converted_quantity*volume
                 converted_quantity = converted_quantity.magnitude
-
         except Exception as e:
-            print(e)
-            simlog.error(f'Problem converting rate {quantity} \n'
-                         f'Is it really a count? Concentrations must be converted')
+            simlog.error(str(e) + '\n' +
+                         f'Problem converting rate {quantity} \n'
+                         f'Is it really a count or concentration?')
     return converted_quantity
 
 
 def check_dimension(dimension, value):
     """
         Checks for dimension consistency. It "stores" the first dimension it was given by returning it
 
-        Parameters:
-            dimension (int) = model's dimension (1D, 2D, 3D ...)
-            value (int) = dimension value being analysed
+        :param dimension: (int) model's dimension (1D, 2D, 3D ...)
+        :param value: (int) dimension value being analysed
+
+        :raise simlog.error: If dimensions are not consistent through the given units (units in 1D with 2D mixed)
 
-        Returns:
-            dimension (int) = model's dimension (1D, 2D, 3D ...)
+        :return: dimension (int) = model's dimension (1D, 2D, 3D ...)
     """
     if dimension is None:
         dimension = int(value)
     else:
         if dimension != int(value):
-            simlog.error('The dimensions are not consistent')
+            simlog.error('The dimensions are not consistent. There are at least two units given for different '
+                         'dimension models')
     return dimension
 
 
-def extract_length_dimension(unit_string, dimension):
+def extract_length_dimension(unit_string, dimension, reaction_order=None):
     """
         Extracts the volume dimension from a Quantity object from Pint
 
-        Parameters:
-            unit_string (str) = unit in str format
-            dimension (int) = model's dimension (1D, 2D, 3D ...)
+        :param unit_string: (str) unit in str format
+        :param dimension: (int) model's dimension (1D, 2D, 3D ...)
     """
     temp_list = unit_string.split()
     try:
         position = temp_list.index('[length]')
     except ValueError:
         position = -1
 
     if position == -1:
         return False
     if temp_list[position + 1] == '**':
-        dimension = check_dimension(dimension, temp_list[position + 2])
+        if reaction_order is None:
+            dimension = check_dimension(dimension, temp_list[position + 2])
+        else:
+            temp_int = int(int(temp_list[position + 2])/(reaction_order - 1))
+            dimension = check_dimension(dimension, temp_int)
     else:
         dimension = check_dimension(dimension, 1)
     return dimension
 
 
 def convert_volume(volume, dimension):
     """
         Converts volume to decimetre**dimension
 
-        Parameters:
-            volume (int, float, Quantity) = volume used in simulation
+        :param volume: (int, float, Quantity) volume used in simulation
+
+        :return: the converted volume in MobsPy units
     """
     if isinstance(volume, Quantity):
         dimension = extract_length_dimension(str(volume.dimensionality), dimension)
         volume = volume.to(f'decimeter ** {dimension}').magnitude
         return volume
     else:
         return volume
 
 
+def convert_time(time):
+    """
+        Converts time into seconds
+
+        :param time: (int, float, Quantity) any time used
+    """
+    if isinstance(time, Quantity):
+        if str(time.dimensionality) == '[time]':
+            return time.to('second').magnitude
+    else:
+        return time
+
+
 if __name__ == '__main__':
     pass
```

### Comparing `mobspy-1.1.3/mobspy/parameter_scripts/parameter_reader.py` & `mobspy-2.0.1/mobspy/parameter_scripts/parameter_reader.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 from pint import Quantity
 
 
 def read_json(json_file_name):
     """
         Reads json file
 
-        Parameters:
-            plot_json_filename: json file name
+        :param plot_json_filename: json file name
 
-        Returns:
-            plot parameter dictionary
+        :raise simlog.error: If the file was not able to be read
+
+        :return: plot parameter dictionary
     """
     with open(json_file_name, 'r') as file:
         try:
             json_data = json.load(file)
         except json.decoder.JSONDecodeError as e:
             simlog.error('Error reading file')
             exit(1)
@@ -31,78 +31,48 @@
     return json_data
 
 
 def __name_output_file(params):
     """
         Gives a name to the output file - just date time in case the user has not specified one
 
-        Parameters:
-            params (dict) = Dictionary with simulation parameters
+        :param params: (dict) Dictionary with simulation parameters
     """
-    if params['output_dir'][0] == '/':
-        params['output_dir'] = params['output_dir'][1:]
 
-    try:
-        main_directory = os.path.abspath(sys.modules['__main__'].__file__)
-        save_dir = os.path.join(Path(main_directory).parent.absolute(), params['output_dir'])
-
-        if params['output_file'] is None:
-            file_name = "r_"
-            file_name += str(datetime.now()) + '.json'
-        else:
-            file_name = params['output_file']
-
-        params['output_absolute_directory'] = save_dir
-        params['output_absolute_file'] = os.path.join(params['output_absolute_directory'], file_name)
-
-    except:
-        simlog.warning('Automatic data-saving setup failed. Please save manually')
-        params['save_data'] = False
+    file_name = "r_"
+    file_name += str(datetime.now()) + '.json'
+    params["absolute_output_file"] = params["output_dir"] + file_name
 
 
 def __check_stochastic_repetitions_seeds(params):
     """
         The list of seeds must be equal to the number of repetitions specified
 
-        Parameters:
-            params (dict) = Dictionary with simulation parameters
+        :param params (dict) = Dictionary with simulation parameters
     """
     if 'seeds' in params:
         try:
             if params['repetitions'] != len(params['seeds']):
                 simlog.error('Seeds must be equal to the number of repetitions')
         except Exception:
             simlog.error('Parameter seeds must be a list')
 
 
-def __check_ode_repetitions(params):
-    """
-        If the method is deterministic MobsPy sets the number of repetitions to one
-
-        Parameters:
-            params (dict) = Dictionary with simulation parameters
-    """
-    if params["simulation_method"].lower() == 'deterministic':
-        params["repetitions"] = 1
-
-
 def __convert_parameters_for_COPASI(params):
     """
         Converts parameters units to MobsPy standard units (basiCO needs seconds for simulation duration)
 
-        Parameters:
-            params (dict) = Dictionary with simulation parameters
+        :param params: (dict) = Dictionary with simulation parameters
     """
     for key, p in params.items():
         if isinstance(p, Quantity):
             if str(p.dimensionality) == '[time]':
                 params[key] = p.to('second').magnitude
                 continue
 
 
 def parameter_process(params):
     __name_output_file(params)
     __check_stochastic_repetitions_seeds(params)
-    __check_ode_repetitions(params)
     __convert_parameters_for_COPASI(params)
```

### Comparing `mobspy-1.1.3/mobspy/parameters/README.md` & `mobspy-2.0.1/mobspy/parameters/README.md`

 * *Files identical despite different names*

### Comparing `mobspy-1.1.3/mobspy/parameters/default_reader.py` & `mobspy-2.0.1/mobspy/parameters/default_reader.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,31 +6,35 @@
 
 # This was just created to avoid potential directory compatibilities
 def get_default_parameters():
     default_parameters = {
         "__comment_1": "Model parameters - Repetitions only for stochastic",
 
         "volume": 1,
-        "repetitions": 3,
+        "repetitions": 1,
         "level": 3,
 
         "__comment_2": "basiCO parameters",
 
         "simulation_method": "deterministic",
+        "method": None,
         "start_time": 0,
         "duration": 60,
         "r_tol": 1e-8,
         "a_tol": 1e-10,
 
         "__comment_3": "OUTPUT",
 
         "output_dir": "outputs/",
         "output_file": None,
         "output_event": False,
-        "unit_x":None,
-        "unit_y":None,
-        "output_concentration":False,
-        "save_data": True,
-        "plot_data": True
-
+        "unit_x": None,
+        "unit_y": None,
+        "output_concentration": False,
+        "save_data": False,
+        "plot_data": True,
+
+        "_continuous_simulation": False,
+        "_end_condition": None,
+        "_with_event": False
     }
     return default_parameters
```

### Comparing `mobspy-1.1.3/mobspy/parameters/example_reader.py` & `mobspy-2.0.1/mobspy/parameters/example_reader.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 """
     This model is responsible for storing example parameters
-    It's used by the simulation to check which parameters exist or not
+    It's used by the simulation to check which parameters exist or not.
+    If a new parameter is added, they key must be added here as an example.
+    Otherwise the simulation object will throw a compilation error, telling the user that the parameter is not
+    supported,
 """
 
 
 def get_example_parameters():
     example_parameters = {
         "__comment_1": "Model parameters - Repetitions only for stochastic",
 
         "volume": 1,
         "repetitions": 3,
         "level": 0,
 
         "__comment_2": "basiCO parameters",
 
         "simulation_method": "stochastic",
+        "method": None,
         "start_time": 0,
         "duration": None,
         "r_tol": 1e-8,
         "a_tol": 1e-10,
         "seeds": [1, 2, 3],
         "step_size": 1,
 
         "__comment_3": "OUTPUT",
 
-        "unit_x":"year",
-        "unit_y":"nanomolar",
-        "output_concentration":True,
-        "output_dir": "outputs/",
+        "unit_x": "year",
+        "unit_y": "nanomolar",
+        "output_concentration": True,
+        "output_dir": "",
         "output_event": False,
         "output_file": None,
         "save_data": False,
         "plot_data": True
 
     }
     return example_parameters
```

### Comparing `mobspy-1.1.3/mobspy/plot_params/example_plot_reader.py` & `mobspy-2.0.1/mobspy/plot_params/example_plot_reader.py`

 * *Files identical despite different names*

### Comparing `mobspy-1.1.3/mobspy/plot_scripts/default_plots.py` & `mobspy-2.0.1/mobspy/plot_scripts/default_plots.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,122 +6,121 @@
 import mobspy.plot_scripts.process_plot_data as ppd
 
 
 def read_plot_json(plot_json_filename):
     """
         This function converts a plot_json file into a dictionary
 
-        Parameters:
-            plot_json_filename (str) = JSON file name
+        :param plot_json_filename: (str) JSON file name
 
-        Returns:
-            json_data (dict) = Converted JSON as dictionary
+        :return: json_data (dict) converted JSON as dictionary
     """
     with open(plot_json_filename, 'r') as file:
         try:
             json_data = json.load(file)
         except Exception:
             simlog.error(f'Error while decoding json file "{plot_json_filename}".')
 
     return json_data
 
 
 def set_plot_units(new_plot_params):
     """
         Sets the plot labels to the unit names by adding to the xlabel and ylabel
 
-        Parameters:
-            new_plot_params (dict) = plot parameters after some changes
+        :param new_plot_params: (dict) plot parameters after some changes
     """
     new_plot_params['xlabel'] = 'Time'
     if new_plot_params['unit_x'] is not None:
         new_plot_params['xlabel'] += f'({new_plot_params["unit_x"]})'
     else:
-        new_plot_params['xlabel'] += '(second)'
+        new_plot_params['xlabel'] += '(s)'
 
     if new_plot_params['output_concentration']:
         new_plot_params['ylabel'] = 'Conc.'
     else:
         new_plot_params['ylabel'] = 'Counts'
 
     if new_plot_params['unit_y'] is not None:
         new_plot_params['ylabel'] += f'({new_plot_params["unit_y"]})'
     else:
         if new_plot_params['output_concentration']:
-            new_plot_params['ylabel'] += '(molar)'
+            new_plot_params['ylabel'] += '(mol/L)'
 
 
 def stochastic_plot(species, data, plot_params):
     """
         Design default stochastic plot using MobsPy plotting hierarchy. It them passes the parameters for plotting
         in the hierarchical plot module
 
-        Parameters:
-            species (list of str) = list of species names in MobsPy str format (queries are performed with the query plot
-            data function)
-            data (dict) = data in MobsPy format Simulation.results['data']
-            plot_params (dict) = dictionary with the plot parameters supplied by the user before the modifications
-            from this function
+        :param species: (list of str) list of species names in MobsPy str format (queries are performed with the
+        query plot data function)
+        :param data: (dict) data in MobsPy format Simulation.results['data']
+        :param plot_params: (dict) dictionary with the plot parameters supplied by the user before the modifications
+        from this function
     """
-    # Data Handling
+
+    # Data Handling - Copy data object to not interfere with simulation data
     species, data = ppd.query_plot_data(species, data)
     ppd.check_plot_parameters(species, plot_params)
 
-    data_to_plot = deepcopy(data)
+    data_to_plot = data
+
     new_plot_params = deepcopy(plot_params)
     set_plot_units(new_plot_params)
 
     # Plot config
     new_plot_params['frameon'] = False
     new_plot_params['figures'] = []
     new_plot_params['pad'] = 1.5
     color_cycler = hp.Color_cycle()
     for spe in species:
         # We define new 'mappings' with the resulting runs for the statics for the plot structure
         try:
             plots_for_spe_i = []
             plots_for_spe_i_sta = []
-            for i, time_series in enumerate(data):
-                if len(time_series) == 1:
-                    i = ''
-
-                processed_runs = sc.average_plus_standard_deviation(time_series[spe]['runs'])
-                key_average = spe + '$' + 'average'
-                key_dev = spe + '$' + 'deviation'
-                data_to_plot[i][key_average] = {'runs': [processed_runs[0]]}
-                data_to_plot[i][key_dev] = {'runs': [processed_runs[1], processed_runs[2]]}
-
-                # We define the standard plot for the average and deviation
-                color = color_cycler(1)
-                plots_for_spe_i.append({'species_to_plot': [spe], 'time_series': i + 1,
-                                        spe: {'color': color, 'label': spe}})
-
-                plots_for_spe_i_sta.append({'species_to_plot': [key_average], 'time_series': i + 1,
-                                            key_average: {'color': color, 'linestyle': '-', 'label': 'mean'}})
-                plots_for_spe_i_sta.append({'species_to_plot': [key_dev], 'time_series': i + 1, 'fill_between': True,
-                                            key_dev: {'color': (0.8, 0.8, 0.8), 'linestyle': ':', 'label': 'std. dev'}})
-        except KeyError:
+
+            processed_runs = sc.average_plus_standard_deviation(spe, data_to_plot)
+
+            key_average = spe + '$' + 'average'
+            key_dev = spe + '$' + 'deviation'
+
+            average_and_deviation_ts = {'Time': data_to_plot.get_max_time_for_species(spe),
+                                        key_average: processed_runs[0],
+                                        key_dev: [processed_runs[1], processed_runs[2]]}
+            data_to_plot.add_ts_to_data(average_and_deviation_ts)
+
+            # We define the standard plot for the average and deviation
+            color = color_cycler(1)
+            plots_for_spe_i.append({'species_to_plot': [spe],
+                                    spe: {'color': color, 'label': spe}})
+
+            plots_for_spe_i_sta.append({'species_to_plot': [key_average],
+                                        key_average: {'color': color, 'linestyle': '-', 'label': 'mean'}})
+            plots_for_spe_i_sta.append({'species_to_plot': [key_dev], 'fill_between': True,
+                                        key_dev: {'color': (0.8, 0.8, 0.8), 'linestyle': ':', 'label': 'std. dev'}})
+        except ValueError:
             simlog.error(f'{spe} species not found in data')
-        new_plot_params['figures'].append({'ylabel': spe + ' ' + new_plot_params['ylabel'], 'plots': plots_for_spe_i })
-        new_plot_params['figures'].append({'ylabel': spe + ' ' + new_plot_params['ylabel'], 'plots': plots_for_spe_i_sta})
+        new_plot_params['figures'].append({'ylabel': spe + ' ' + new_plot_params['ylabel'], 'plots': plots_for_spe_i})
+        new_plot_params['figures'].append(
+            {'ylabel': spe + ' ' + new_plot_params['ylabel'], 'plots': plots_for_spe_i_sta})
 
     hp.plot_data(data_to_plot, new_plot_params)
 
 
 def deterministic_plot(species, data, plot_params):
     """
         Design default deterministic plot using MobsPy plotting hierarchy. It them passes the parameters for plotting
         in the hierarchical plot module
 
-        Parameters:
-            species (list of str) = list of species names in MobsPy str format (queries are performed with the query plot
-            data function)
-            data (dict) = data in MobsPy format Simulation.results['data']
-            plot_params (dict) = dictionary with the plot parameters supplied by the user before the modifications
-            from this function
+        :param species: (list of str) list of species names in MobsPy str format (queries are performed
+        with the query plot data function)
+        :param data: (dict) data in MobsPy format Simulation.results['data']
+        :param plot_params: (dict) dictionary with the plot parameters supplied by the user before the modifications
+        from this function
     """
     # Data Handling
     species, data = ppd.query_plot_data(species, data)
     ppd.check_plot_parameters(species, plot_params)
 
     new_plot_params = deepcopy(plot_params)
     set_plot_units(new_plot_params)
@@ -136,25 +135,26 @@
 
 
 def raw_plot(data, parameters_or_file):
     """
         Plots data from a json or parameter dictionary configured according to the hierarchical plot structure
         Does not accept parameters from a Simulation object, it must be given the parameters in it's entirety
 
-        Parameters:
-            data (dict) = data in MobsPy format Simulation.results['data']
-            parameters_or_file (dict, str) = Dictionary originated from a JSON or JSON file name
+        :param data: (dict) data in MobsPy format Simulation.results['data']
+        :param parameters_or_file: (dict, str) Dictionary originated from a JSON or JSON file name
     """
     if type(parameters_or_file) == str and parameters_or_file[-5:] == '.json':
         plot_params = read_plot_json(parameters_or_file)
     elif type(parameters_or_file) == dict:
         plot_params = parameters_or_file
     else:
         simlog.error('Raw plot only takes json files or parameters for configuration')
 
-    species = list(data[0].keys())
+    species = list(data.ts_data[0].keys())
     ppd.check_plot_parameters(species, plot_params)
+
+    # Here we add some base data just in case the user has not supplied it
     hp.plot_data(data, plot_params)
 
 
 if __name__ == '__main__':
     raw_plot({}, 'default_parameters.json')
```

### Comparing `mobspy-1.1.3/mobspy/plot_scripts/hierarchical_plot.py` & `mobspy-2.0.1/mobspy/plot_scripts/hierarchical_plot.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,66 +12,58 @@
 
 
 ####################### PRACTICAL FUNCTIONS
 class Color_cycle:
     """
         This class is responsible for cycling through the different colors for different curves
 
-        Attributes:
-            index (int) = Current position in the color cycle
-            color_list (list) = list of available colors
+        :param index: (int) Current position in the color cycle
+        :param color_list: (list) = list of available colors
     """
+
     def __init__(self):
         self.index = 0
         self.color_list = ['b', 'g', 'r', 'c', 'm', 'y', 'k']
 
     def __call__(self, n):
         """
             Call updates the index and returns the next color in the list
             Normally n is set to 1
 
-            Parameters:
-                n (int) = number of positions to skip
-
-            Returns:
-                color (str) = color name for pyplot
+            :param n: (int) number of positions to skip
+            :return: color (str) = color name for pyplot
         """
         self.index = (self.index + n) % len(self.color_list)
         return self.color_list[self.index]
 
 
 def find_species_time_series(spe, data):
     """
         There can be different time-series in MobsPy data (even experimental data, as long as it is in MobPy format)
         This function finds all the time-series the species is present in and returns it for looping thorugh all of
         them
         This function is implemented to allow for the comparison of models with experimental data or other models
 
-        Parameters:
-            spe (str) = Species name
-
-        Data:
-            data (dict) = Data in MobsPy format
+        :param spe: (str) Species name
+        :pram  data: (dict) Data in MobsPy format
     """
     for time_series in data:
         if spe in time_series:
             yield time_series
 
 
 def get_total_figure_number(axis_matrix):
     """
         Gets the number of figures from an axis_matrix generated by pyplot. Used by the hash to place configs in the
         correct part of the axis_matrix
 
-        Parameters:
-            axis_matrix (1D or 2D numpy array) = Array returned by pyplot once multiple figures are introduced into
-            a single plot
+        :param axis_matrix: (1D or 2D numpy array) Array returned by pyplot once multiple figures are introduced into
+        a single plot
 
-        Returns:
-            total_figure_number (int) = Total number of figures
+        :return: total_figure_number (int) Total number of figures
     """
     # Get the number of figures, using the axis_matrix
     try:
         total_figure_number = axis_matrix.shape[0] * axis_matrix.shape[1]
     except IndexError:
         total_figure_number = axis_matrix.shape[0]
     return total_figure_number
@@ -83,20 +75,18 @@
         This function allows one to acess the figure grid with a linear input
         For instance one can access a 2x2 grid using 0, 1, 2, 3
         0 becomes 0,0
         1 becomes 1,0
         2 becomes 0,1
         3 becomes 1,1
 
-        Parameters:
-            current_figure (int) = linear number of the figure
-            axis_matrix (1D or 2D numpy array) =  a list with all the created axis on the multiple figure subplot
+        :param current_figure: (int) linear number of the figure
+        :param axis_matrix: (1D or 2D numpy array) a list with all the created axis on the multiple figure subplot
 
-        Returns:
-            the correct axis based on the number provided
+        :return: the correct axis based on the number provided
     """
 
     # Get the number of lines
     max_lines = len(axis_matrix)
     total_figure_number = get_total_figure_number(axis_matrix)
 
     # Correction for index purposes
@@ -115,20 +105,18 @@
     """
 
         This is hash used to create the figure grid automatically according to the number of figures desired by the
         user and the maximum number of lines
 
         For instance 4 figures with 2 as max_lines creates a 2x2 figure grid automatically
 
-        Parameters:
-            total_figure_number (int) = Number of total figures to create
-            max_lines (int) = Maximum number of lines in the grid
+        :param total_figure_number: (int) Number of total figures to create
+        :param max_lines: (int) Maximum number of lines in the grid
 
-        Returns:
-            fig and axs = Figures grid will all the respective axis
+        :return: fig and axs = Figures grid will all the respective axis
     """
 
     # Default value if nothing is set up
     if max_lines is None:
         max_lines = 2
 
     if total_figure_number <= max_lines:
@@ -152,21 +140,19 @@
         The priority for parameter search is plots => figures => global, with plot overriding others and so on
 
         If a parameter is defined globally it will be applied to all figures, if it defined inside a figure element
         it will only apply to that figure, if it is defined in a plot element it will only apply to that curve
 
         Check the readme or the tutorials for more details on the plotting structure. It is simple and versatile
 
-        Parameters:
-            params (dict) = Plot parameters from python dictionary (after json conversion)
-            key (str) = Key necessary to access the parameters
-            index (int) = None for global search, one index for figure search, and two for figure curve search
+        :param params: (dict) Plot parameters from python dictionary (after json conversion)
+        :param key: (str) Key necessary to access the parameters
+        :param index: (int) None for global search, one index for figure search, and two for figure curve search
 
-        Returns:
-            The parameter if found, and None if nothing is found
+        :return: The parameter if found, and None if nothing is found
     """
 
     # No index is given, look global
     if index is None:
         try:
             return params[key]
         except (KeyError, IndexError):
@@ -208,19 +194,18 @@
 
 ####################### PLOTING FUNCTIONS
 
 def plot_curves(data, axs, figure_index, plot_params):
     """
         This function plots the programmed curves in the assigned figure
 
-        Params:
-            axs (pyplot axe) = axs to plot the data in
-            data (dict) = data given in MobsPy format results['data']
-            figure_index (int) = index of the current figure to plot curves in
-            plot_params: parameters for plotting
+        :param axs: (pyplot axe) axs to plot the data in
+        :param data: (dict) data given in MobsPy format results['data']
+        :param figure_index: (int) index of the current figure to plot curves in
+        :param plot_params: parameters for plotting
     """
 
     # Get the plot number from the list of plots
     try:
         plot_number = len(find_parameter(plot_params, 'plots', figure_index))
     except TypeError:
         # No figures plot only the default
@@ -243,83 +228,79 @@
         if find_parameter(plot_params, key='time_series', index=(figure_index, plot_index)) is not None:
             time_series = find_parameter(plot_params, key='time_series', index=(figure_index, plot_index))
             if type(time_series) == int:
                 time_series = [time_series]
         else:
             time_series = list(range(len(data)))
 
-        for ts in time_series:
-            ts = data[ts - 1]
+        for spe in species:
 
-            for spe in species:
+            color_index = 0
 
-                color_index = 0
+            # Get the parameters assigned to the species, if not assign empty for None returns
+            if find_parameter(plot_params, key=spe, index=(figure_index, plot_index)) is not None:
+                species_characteristics = find_parameter(plot_params, key=spe, index=(figure_index, plot_index))
+            else:
+                species_characteristics = {}
+
+            # Now we search the species characteristics for parameters
+            if find_parameter(species_characteristics, key='color') is not None:
+                curve_color = find_parameter(species_characteristics, key='color')
+            else:
+                color_index = (color_index + 1) % len(Color_cycle().color_list)
+                curve_color = Color_cycle()(color_index)
+
+            if find_parameter(species_characteristics, key='linestyle') is not None:
+                linestyle = find_parameter(species_characteristics, key='linestyle')
+            else:
+                linestyle = '-'
+
+            if find_parameter(species_characteristics, key='linewidth') is not None:
+                linewidth = find_parameter(species_characteristics, key='linewidth')
+            else:
+                linewidth = None
+
+            if find_parameter(species_characteristics, key='label') is not None:
+                label = find_parameter(species_characteristics, key='label')
+                legend_flag = True
+            else:
+                label = None
 
-                # Get the parameters assigned to the species, if not assign empty for None returns
-                if find_parameter(plot_params, key=spe, index=(figure_index, plot_index)) is not None:
-                    species_characteristics = find_parameter(plot_params, key=spe, index=(figure_index, plot_index))
-                else:
-                    species_characteristics = {}
-
-                # Now we search the species characteristics for parameters
-                if find_parameter(species_characteristics, key='color') is not None:
-                    curve_color = find_parameter(species_characteristics, key='color')
-                else:
-                    color_index = (color_index + 1) % len(Color_cycle().color_list)
-                    curve_color = Color_cycle()(color_index)
-
-                if find_parameter(species_characteristics, key='linestyle') is not None:
-                    linestyle = find_parameter(species_characteristics, key='linestyle')
-                else:
-                    linestyle = '-'
-
-                if find_parameter(species_characteristics, key='linewidth') is not None:
-                    linewidth = find_parameter(species_characteristics, key='linewidth')
-                else:
-                    linewidth = None
-
-                if find_parameter(species_characteristics, key='label') is not None:
-                    label = find_parameter(species_characteristics, key='label')
-                    legend_flag = True
-                else:
-                    label = None
-
-                if find_parameter(plot_params, key='runs', index=(figure_index, plot_index)) is not None:
-                    runs = find_parameter(plot_params, key='runs', index=(figure_index, plot_index))
-                else:
-                    runs = range(len(ts[spe]['runs']))
-
-                if find_parameter(plot_params, key='fill_between', index=(figure_index, plot_index)) is not None and \
-                        find_parameter(plot_params, key='fill_between', index=(figure_index, plot_index)):
-                    try:
-                        axs.fill_between(ts['Time'], ts[spe]['runs'][0], ts[spe]['runs'][1], color=curve_color,
-                                         label=label)
-                    except IndexError:
-                        simlog.error('Fill_between must only have two or less runs referring to it')
-                else:
-                    for run in runs:
-                        axs.plot(ts['Time'], ts[spe]['runs'][run], color=curve_color,
-                            linestyle=linestyle, linewidth=linewidth, label=label)
+            for ts in time_series:
+                ts = data[ts]
+
+                try:
+                    if find_parameter(plot_params, key='fill_between', index=(figure_index, plot_index)) is not None \
+                            and find_parameter(plot_params, key='fill_between', index=(figure_index, plot_index)):
+                        try:
+                            axs.fill_between(ts['Time'], ts[spe][0], ts[spe][1], color=curve_color,
+                                             label=label)
+                        except IndexError:
+                            simlog.error('Fill_between must only have two or less runs referring to it')
+                    else:
+                        axs.plot(ts['Time'], ts[spe], color=curve_color,
+                                 linestyle=linestyle, linewidth=linewidth, label=label)
                         label = None
+                except KeyError:
+                    pass
 
     if legend_flag:
         if find_parameter(plot_params, key='frameon', index=figure_index) is not None:
             frameon = find_parameter(plot_params, key='frameon', index=figure_index)
         else:
             frameon = True
         axs.legend(frameon=frameon)
 
 
 def set_figure_characteristics(axis_matrix, plot_params):
     """
         Sets the characteristics for each figure
 
-        Params:
-            axis_matrix (axis from pyplot subplot) = Array of all axis in the grid
-            plot_params (dict) = Plot parameters received
+        :param axis_matrix: (axis from pyplot subplot) Array of all axis in the grid
+        :param plot_params: (dict) Plot parameters received
     """
     total_figure_number = get_total_figure_number(axis_matrix)
     # Loop through all axis
     for i in range(total_figure_number):
 
         if find_parameter(plot_params, 'xlim', i) is not None:
             figure_hash(i, axis_matrix).set_xlim(find_parameter(plot_params, 'xlim', i))
@@ -347,17 +328,16 @@
                 figure_hash(i, axis_matrix).text(annotations[0], annotations[1], annotations[2])
 
 
 def set_global_parameters(fig, plot_params):
     """
         Sets the characteristics the plot window
 
-        Params:
-            fig (fig from pyplot subplot) = Array of all axis in the grid
-            plot_params (dict) = Plot parameters received
+        :param fig: (fig from pyplot subplot) Array of all axis in the grid
+        :param plot_params: (dict) Plot parameters received
     """
     if find_parameter(plot_params, 'pad') is not None:
         fig.tight_layout(pad=find_parameter(plot_params, 'pad'))
 
     if find_parameter(plot_params, 'figsize') is not None:
         fig.set_size_inches(plot_params['figsize'][0], plot_params['figsize'][1])
 
@@ -365,17 +345,16 @@
         fig.set_dpi(plot_params['dpi'])
 
 
 def plot_data(data, plot_params):
     """
         This function plots the simulation results according to the specifications
 
-        Parameters:
-            data (dict) = Data in MobsPy format
-            plot_params (dict) = Plot parameters received
+        :param data: (dict) Data in MobsPy format
+        :param plot_params: (dict) Plot parameters received
     """
 
     # Get the figure number from the list of figures
     # Add it to parameters
     try:
         figure_number = len(find_parameter(plot_params, 'figures'))
     except TypeError:
```

### Comparing `mobspy-1.1.3/mobspy/sbml_simulator/SBMLWriter.py` & `mobspy-2.0.1/mobspy/sbml_simulator/SBMLWriter.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,39 +31,35 @@
             )
             raise RuntimeError(err_msg)
     else:
         return
 
 
 def create_model(species={}, parameters={}, reactions={}, events={}):
-    """Returns an SBML Level 3 model.
-
+    """
+    Returns an SBML Level 3 model.
     Example:
-
-    species = { 'E': 1, \
-                'EM': 0, \
-                'EM2': 0, \
-                'F': 100, \
-                }
-
-    parameters = {'k': (1e-06,'per_min'), \
+    species = { 'E': 1,
+                'EM': 0,
+                'EM2': 0,
+                'F': 100,
+                },
+    parameters = {'k': (1e-06,'per_min'),
                  }
-
-    reactions = { 'Production_E': \
-                        { 're': [(1,'E'),(1,'F')], \
-                          'pr': [(2,'E')], \
-                          'kin' : 'k * E * F' \
-                        }, \
-                }
-
-    events = {'e': \
-              { 'trigger': 'true', \
-                'delay': '10', \
-                'assignments': [('M','1'),], \
-              }, \
+    reactions = { 'Production_E':
+                        { 're': [(1,'E'),(1,'F')],
+                          'pr': [(2,'E')],
+                          'kin' : 'k * E * F'
+                        },
+                },
+    events = {'e':
+              { 'trigger': 'true',
+                'delay': '10',
+                'assignments': [('M','1'),],
+              },
     }
     """
 
     # Create an empty SBMLDocument object.  It's a good idea to check for
     # possible errors.  Even when the parameter values are hardwired like
     # this, it is still possible for a failure to occur (e.g., if the
     # operating system runs out of memory).
```

### Comparing `mobspy-1.1.3/mobspy.egg-info/PKG-INFO` & `mobspy-2.0.1/mobspy.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mobspy
-Version: 1.1.3
+Version: 2.0.1
 Summary: A Query-Based Language for Chemical Reaction Networks
 Home-page: https://github.com/ROBACON/mobspy
 License: UNKNOWN
 Description: ![Alt text](/images/img.png "MobsPy")
         
         # MobsPy
         
@@ -105,14 +105,18 @@
         
         For now MobsPy is not thread-safe and it's not compatible with numpy and deepcopy
         
         # Release info
         
         Version 1.1 added automated testing to git pushes with test_script.py
         
+        Version 2.0.1 added events, ability to concatenate simulations, and changed the structure of output data to be more 
+        user-friendly. Now MySim.results["data"]["runs"]["MetaSpeciesName"] has been deprecated. It has been replaced by 
+        MySim.results["MetaSpeciesName"] or MySim.results[MetaSpeciesObject]. It will return only one run if there are no 
+        repetitions and multiple runs with several repetitions.
```

### Comparing `mobspy-1.1.3/setup.py` & `mobspy-2.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `mobspy-1.1.3/test_tools/model_3.txt` & `mobspy-2.0.1/test_tools/model_3.txt`

 * *Files identical despite different names*

### Comparing `mobspy-1.1.3/test_tools/model_4.txt` & `mobspy-2.0.1/test_tools/model_4.txt`

 * *Files identical despite different names*

### Comparing `mobspy-1.1.3/test_tools/model_5.txt` & `mobspy-2.0.1/test_tools/model_5.txt`

 * *Files identical despite different names*

### Comparing `mobspy-1.1.3/test_tools/model_7.txt` & `mobspy-2.0.1/test_tools/model_7.txt`

 * *Files identical despite different names*

