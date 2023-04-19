# Comparing `tmp/sberpm-2.3.3.tar.gz` & `tmp/sberpm-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sberpm-2.3.3.tar", last modified: Wed Apr  5 21:36:44 2023, max compression
+gzip compressed data, was "sberpm-2.4.0.tar", last modified: Wed Apr 19 07:37:05 2023, max compression
```

## Comparing `sberpm-2.3.3.tar` & `sberpm-2.4.0.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxrwxrwx   0        0        0        0 2023-04-05 21:36:44.599895 sberpm-2.3.3/
--rw-rw-rw-   0        0        0      274 2023-03-14 12:01:36.000000 sberpm-2.3.3/.gitignore
--rw-rw-rw-   0        0        0    29507 2023-01-26 18:07:31.000000 sberpm-2.3.3/LICENSE
--rw-rw-rw-   0        0        0    62148 2023-01-26 18:07:31.000000 sberpm-2.3.3/LICENSE_RUS
--rw-rw-rw-   0        0        0      242 2023-01-26 18:07:31.000000 sberpm-2.3.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2660 2023-04-05 21:36:44.599895 sberpm-2.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     2213 2023-04-05 21:34:08.000000 sberpm-2.3.3/README.md
--rw-rw-rw-   0        0        0     1147 2023-01-26 18:07:31.000000 sberpm-2.3.3/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-04-05 21:36:42.944046 sberpm-2.3.3/sberpm/
--rw-rw-rw-   0        0        0      542 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/__init__.py
--rw-rw-rw-   0        0        0    31800 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/_holder.py
--rw-rw-rw-   0        0        0      947 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/_utils.py
--rw-rw-rw-   0        0        0       21 2023-04-05 21:32:51.000000 sberpm-2.3.3/sberpm/_version.py
-drwxrwxrwx   0        0        0        0 2023-04-05 21:36:42.996235 sberpm-2.3.3/sberpm/autoinsights/
--rw-rw-rw-   0        0        0      120 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/autoinsights/__init__.py
--rw-rw-rw-   0        0        0      188 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/autoinsights/_influencing_activities.py
-drwxrwxrwx   0        0        0        0 2023-04-05 21:36:43.022428 sberpm-2.3.3/sberpm/autoinsights/file_obf/
--rw-rw-rw-   0        0        0    12828 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/autoinsights/file_obf/_influencing_activities.obfsbpm
-drwxrwxrwx   0        0        0        0 2023-04-05 21:36:43.055860 sberpm-2.3.3/sberpm/bpmn/
--rw-rw-rw-   0        0        0      177 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/bpmn/__init__.py
--rw-rw-rw-   0        0        0    26484 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/bpmn/_bpmn_file_to_graph.py
-drwxrwxrwx   0        0        0        0 2023-04-05 21:36:43.168609 sberpm-2.3.3/sberpm/bpmn/_bpmn_graph_to_file/
--rw-rw-rw-   0        0        0      103 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/bpmn/_bpmn_graph_to_file/__init__.py
--rw-rw-rw-   0        0        0     4093 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/bpmn/_bpmn_graph_to_file/_bpmn_exporter.py
--rw-rw-rw-   0        0        0     6642 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/bpmn/_bpmn_graph_to_file/_bpmn_xml_maker.py
--rw-rw-rw-   0        0        0     4680 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/bpmn/_bpmn_graph_to_file/_petri_net_to_bpmn.py
--rw-rw-rw-   0        0        0     1545 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/bpmn/_bpmn_graph_to_file/grandalf.py
--rw-rw-rw-   0        0        0     5350 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/bpmn/_bpmn_graph_to_file/graphviz.py
-drwxrwxrwx   0        0        0        0 2023-04-05 21:36:43.182612 sberpm-2.3.3/sberpm/column_matching/
--rw-rw-rw-   0        0        0      102 2023-03-14 12:01:36.000000 sberpm-2.3.3/sberpm/column_matching/__init__.py
--rw-rw-rw-   0        0        0      182 2023-03-14 12:01:36.000000 sberpm-2.3.3/sberpm/column_matching/_column_matching.py
-drwxrwxrwx   0        0        0        0 2023-04-05 21:36:43.207617 sberpm-2.3.3/sberpm/column_matching/file_obf/
--rw-rw-rw-   0        0        0     5710 2023-03-14 12:01:36.000000 sberpm-2.3.3/sberpm/column_matching/file_obf/_column_matching_.obfsbpm
-drwxrwxrwx   0        0        0        0 2023-04-05 21:36:43.272624 sberpm-2.3.3/sberpm/conformance_checking/
--rw-rw-rw-   0        0        0      202 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/conformance_checking/__init__.py
--rw-rw-rw-   0        0        0     6061 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/conformance_checking/_conformance_checking.py
--rw-rw-rw-   0        0        0     9883 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/conformance_checking/_token_replay.py
-drwxrwxrwx   0        0        0        0 2023-04-05 21:36:43.311607 sberpm-2.3.3/sberpm/decision_mining/
--rw-rw-rw-   0        0        0      100 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/decision_mining/__init__.py
--rw-rw-rw-   0        0        0    33758 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/decision_mining/_decision_mining.py
-drwxrwxrwx   0        0        0        0 2023-04-05 21:36:43.359626 sberpm-2.3.3/sberpm/graph_stats/
--rw-rw-rw-   0        0        0      146 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/graph_stats/__init__.py
--rw-rw-rw-   0        0        0     3336 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/graph_stats/centrality.py
-drwxrwxrwx   0        0        0        0 2023-04-05 21:36:43.428617 sberpm-2.3.3/sberpm/imitation/
--rw-rw-rw-   0        0        0      160 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/imitation/__init__.py
--rw-rw-rw-   0        0        0    30041 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/imitation/_simulation.py
--rw-rw-rw-   0        0        0    13518 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/imitation/_validation.py
-drwxrwxrwx   0        0        0        0 2023-04-05 21:36:43.590629 sberpm-2.3.3/sberpm/metrics/
--rw-rw-rw-   0        0        0      371 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/metrics/__init__.py
--rw-rw-rw-   0        0        0     5524 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/metrics/_activity_metric.py
--rw-rw-rw-   0        0        0     6918 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/metrics/_base_metric.py
--rw-rw-rw-   0        0        0     4077 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/metrics/_id_metric.py
--rw-rw-rw-   0        0        0     5173 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/metrics/_trace_metric.py
--rw-rw-rw-   0        0        0     6093 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/metrics/_transition_metric.py
--rw-rw-rw-   0        0        0     3995 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/metrics/_user_metric.py
--rw-rw-rw-   0        0        0      389 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/metrics/_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-05 21:36:43.926658 sberpm-2.3.3/sberpm/miners/
--rw-rw-rw-   0        0        0     1374 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/miners/__init__.py
--rw-rw-rw-   0        0        0     9571 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/miners/_abstract_miner.py
--rw-rw-rw-   0        0        0    19774 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/miners/_alpha_miner.py
--rw-rw-rw-   0        0        0    10578 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/miners/_alpha_plus_miner.py
--rw-rw-rw-   0        0        0      174 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/miners/_auto_miner.py
--rw-rw-rw-   0        0        0     3153 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/miners/_causal_miner.py
--rw-rw-rw-   0        0        0    18462 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/miners/_correlation_miner.py
--rw-rw-rw-   0        0        0     9122 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/miners/_heu_miner.py
--rw-rw-rw-   0        0        0     3896 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/miners/_inductive_miner.py
--rw-rw-rw-   0        0        0     8354 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/miners/_inductive_utils.py
--rw-rw-rw-   0        0        0      174 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/miners/_ml_miner.py
--rw-rw-rw-   0        0        0     7306 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/miners/_parallel_miner.py
--rw-rw-rw-   0        0        0     2678 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/miners/_simple_miner.py
-drwxrwxrwx   0        0        0        0 2023-04-05 21:36:43.969660 sberpm-2.3.3/sberpm/miners/file_obf/
--rw-rw-rw-   0        0        0     3192 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/miners/file_obf/_auto_miner.obfsbpm
--rw-rw-rw-   0        0        0     5082 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/miners/file_obf/_ml_miner.obfsbpm
-drwxrwxrwx   0        0        0        0 2023-04-05 21:36:44.022665 sberpm-2.3.3/sberpm/miners/mining_utils/
--rw-rw-rw-   0        0        0     8347 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/miners/mining_utils/_inductive_utils.py
--rw-rw-rw-   0        0        0    25893 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/miners/mining_utils/_node_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-05 21:36:44.038849 sberpm-2.3.3/sberpm/ml/
--rw-rw-rw-   0        0        0      179 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/ml/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-05 21:36:44.202863 sberpm-2.3.3/sberpm/ml/anomaly_detection/
--rw-rw-rw-   0        0        0      571 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/ml/anomaly_detection/__init__.py
--rw-rw-rw-   0        0        0    11459 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/ml/anomaly_detection/_outlier_detector.py
--rw-rw-rw-   0        0        0     4669 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/ml/anomaly_detection/_outlier_detector_ensemble.py
--rw-rw-rw-   0        0        0     5295 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/ml/anomaly_detection/_outliercblof.py
--rw-rw-rw-   0        0        0     2404 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/ml/anomaly_detection/_outliercustom.py
--rw-rw-rw-   0        0        0     4911 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/ml/anomaly_detection/_outlierforest.py
--rw-rw-rw-   0        0        0     6340 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/ml/anomaly_detection/_outlierlof.py
--rw-rw-rw-   0        0        0     4804 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/ml/anomaly_detection/_outlierocsvm.py
-drwxrwxrwx   0        0        0        0 2023-04-05 21:36:44.226866 sberpm-2.3.3/sberpm/ml/chronometrage/
--rw-rw-rw-   0        0        0       76 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/ml/chronometrage/__init__.py
--rw-rw-rw-   0        0        0     6531 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/ml/chronometrage/_chronometrage.py
-drwxrwxrwx   0        0        0        0 2023-04-05 21:36:44.249868 sberpm-2.3.3/sberpm/ml/stages_clustering/
--rw-rw-rw-   0        0        0      111 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/ml/stages_clustering/__init__.py
--rw-rw-rw-   0        0        0      183 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/ml/stages_clustering/_stages_clustering.py
-drwxrwxrwx   0        0        0        0 2023-04-05 21:36:44.275869 sberpm-2.3.3/sberpm/ml/stages_clustering/file_obf/
--rw-rw-rw-   0        0        0     5116 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/ml/stages_clustering/file_obf/_stages_clustering.obfsbpm
-drwxrwxrwx   0        0        0        0 2023-04-05 21:36:44.307872 sberpm-2.3.3/sberpm/ml/utils/
--rw-rw-rw-   0        0        0      107 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/ml/utils/__init__.py
--rw-rw-rw-   0        0        0     3935 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/ml/utils/_perm_importance.py
-drwxrwxrwx   0        0        0        0 2023-04-05 21:36:44.340873 sberpm-2.3.3/sberpm/models/
--rw-rw-rw-   0        0        0      300 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/models/__init__.py
--rw-rw-rw-   0        0        0     1846 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/models/_check_models.py
-drwxrwxrwx   0        0        0        0 2023-04-05 21:36:44.484886 sberpm-2.3.3/sberpm/visual/
--rw-rw-rw-   0        0        0      608 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/visual/__init__.py
--rw-rw-rw-   0        0        0    76564 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/visual/_chart_painter.py
--rw-rw-rw-   0        0        0    18529 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/visual/_graph.py
--rw-rw-rw-   0        0        0    12406 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/visual/_graphviz_painter.py
--rw-rw-rw-   0        0        0    25598 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/visual/_matplotlib_painter.py
--rw-rw-rw-   0        0        0      594 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/visual/_types.py
--rw-rw-rw-   0        0        0     6935 2023-01-26 18:07:31.000000 sberpm-2.3.3/sberpm/visual/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-05 21:36:42.977234 sberpm-2.3.3/sberpm.egg-info/
--rw-rw-rw-   0        0        0     2660 2023-04-05 21:36:42.000000 sberpm-2.3.3/sberpm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3186 2023-04-05 21:36:42.000000 sberpm-2.3.3/sberpm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-05 21:36:42.000000 sberpm-2.3.3/sberpm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      814 2023-04-05 21:36:42.000000 sberpm-2.3.3/sberpm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-05 21:36:42.000000 sberpm-2.3.3/sberpm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-05 21:36:44.603898 sberpm-2.3.3/setup.cfg
--rw-rw-rw-   0        0        0     2377 2023-01-26 18:07:31.000000 sberpm-2.3.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-05 21:36:44.595895 sberpm-2.3.3/tutorials/
--rw-rw-rw-   0        0        0    19319 2023-01-26 18:07:31.000000 sberpm-2.3.3/tutorials/chrono_data.xlsx
--rw-rw-rw-   0        0        0   132942 2023-01-26 18:07:31.000000 sberpm-2.3.3/tutorials/example.xlsx
--rw-rw-rw-   0        0        0    92872 2023-03-14 16:20:33.000000 sberpm-2.3.3/tutorials/tutorial_en.ipynb
--rw-rw-rw-   0        0        0   124935 2023-03-14 16:20:11.000000 sberpm-2.3.3/tutorials/tutorial_ru.ipynb
+drwxrwxrwx   0        0        0        0 2023-04-19 07:37:05.306032 sberpm-2.4.0/
+-rw-rw-rw-   0        0        0      274 2023-03-14 12:01:36.000000 sberpm-2.4.0/.gitignore
+-rw-rw-rw-   0        0        0    29507 2023-01-26 18:07:31.000000 sberpm-2.4.0/LICENSE
+-rw-rw-rw-   0        0        0    62148 2023-01-26 18:07:31.000000 sberpm-2.4.0/LICENSE_RUS
+-rw-rw-rw-   0        0        0      242 2023-01-26 18:07:31.000000 sberpm-2.4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2887 2023-04-19 07:37:05.306032 sberpm-2.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2213 2023-04-05 21:34:08.000000 sberpm-2.4.0/README.md
+-rw-rw-rw-   0        0        0     1147 2023-01-26 18:07:31.000000 sberpm-2.4.0/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-04-19 07:37:05.053391 sberpm-2.4.0/sberpm/
+-rw-rw-rw-   0        0        0      542 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/__init__.py
+-rw-rw-rw-   0        0        0    31800 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/_holder.py
+-rw-rw-rw-   0        0        0      947 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/_utils.py
+-rw-rw-rw-   0        0        0       21 2023-04-19 07:20:10.000000 sberpm-2.4.0/sberpm/_version.py
+drwxrwxrwx   0        0        0        0 2023-04-19 07:37:05.092759 sberpm-2.4.0/sberpm/autoinsights/
+-rw-rw-rw-   0        0        0      120 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/autoinsights/__init__.py
+-rw-rw-rw-   0        0        0      188 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/autoinsights/_influencing_activities.py
+drwxrwxrwx   0        0        0        0 2023-04-19 07:37:05.094850 sberpm-2.4.0/sberpm/autoinsights/file_obf/
+-rw-rw-rw-   0        0        0    12828 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/autoinsights/file_obf/_influencing_activities.obfsbpm
+drwxrwxrwx   0        0        0        0 2023-04-19 07:37:05.099986 sberpm-2.4.0/sberpm/bpmn/
+-rw-rw-rw-   0        0        0      177 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/bpmn/__init__.py
+-rw-rw-rw-   0        0        0    26484 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/bpmn/_bpmn_file_to_graph.py
+drwxrwxrwx   0        0        0        0 2023-04-19 07:37:05.115873 sberpm-2.4.0/sberpm/bpmn/_bpmn_graph_to_file/
+-rw-rw-rw-   0        0        0      103 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/bpmn/_bpmn_graph_to_file/__init__.py
+-rw-rw-rw-   0        0        0     4093 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/bpmn/_bpmn_graph_to_file/_bpmn_exporter.py
+-rw-rw-rw-   0        0        0     6642 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/bpmn/_bpmn_graph_to_file/_bpmn_xml_maker.py
+-rw-rw-rw-   0        0        0     4680 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/bpmn/_bpmn_graph_to_file/_petri_net_to_bpmn.py
+-rw-rw-rw-   0        0        0     1545 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/bpmn/_bpmn_graph_to_file/grandalf.py
+-rw-rw-rw-   0        0        0     5350 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/bpmn/_bpmn_graph_to_file/graphviz.py
+drwxrwxrwx   0        0        0        0 2023-04-19 07:37:05.119873 sberpm-2.4.0/sberpm/column_matching/
+-rw-rw-rw-   0        0        0      102 2023-03-14 12:01:36.000000 sberpm-2.4.0/sberpm/column_matching/__init__.py
+-rw-rw-rw-   0        0        0      182 2023-03-14 12:01:36.000000 sberpm-2.4.0/sberpm/column_matching/_column_matching.py
+drwxrwxrwx   0        0        0        0 2023-04-19 07:37:05.122011 sberpm-2.4.0/sberpm/column_matching/file_obf/
+-rw-rw-rw-   0        0        0     5710 2023-03-14 12:01:36.000000 sberpm-2.4.0/sberpm/column_matching/file_obf/_column_matching_.obfsbpm
+drwxrwxrwx   0        0        0        0 2023-04-19 07:37:05.130130 sberpm-2.4.0/sberpm/conformance_checking/
+-rw-rw-rw-   0        0        0      202 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/conformance_checking/__init__.py
+-rw-rw-rw-   0        0        0     6061 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/conformance_checking/_conformance_checking.py
+-rw-rw-rw-   0        0        0     9883 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/conformance_checking/_token_replay.py
+drwxrwxrwx   0        0        0        0 2023-04-19 07:37:05.134322 sberpm-2.4.0/sberpm/decision_mining/
+-rw-rw-rw-   0        0        0      100 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/decision_mining/__init__.py
+-rw-rw-rw-   0        0        0    33758 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/decision_mining/_decision_mining.py
+drwxrwxrwx   0        0        0        0 2023-04-19 07:37:05.139320 sberpm-2.4.0/sberpm/graph_stats/
+-rw-rw-rw-   0        0        0      146 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/graph_stats/__init__.py
+-rw-rw-rw-   0        0        0     3336 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/graph_stats/centrality.py
+drwxrwxrwx   0        0        0        0 2023-04-19 07:37:05.146593 sberpm-2.4.0/sberpm/imitation/
+-rw-rw-rw-   0        0        0      160 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/imitation/__init__.py
+-rw-rw-rw-   0        0        0    30041 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/imitation/_simulation.py
+-rw-rw-rw-   0        0        0    13518 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/imitation/_validation.py
+drwxrwxrwx   0        0        0        0 2023-04-19 07:37:05.165887 sberpm-2.4.0/sberpm/metrics/
+-rw-rw-rw-   0        0        0      371 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/metrics/__init__.py
+-rw-rw-rw-   0        0        0     5524 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/metrics/_activity_metric.py
+-rw-rw-rw-   0        0        0     6918 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/metrics/_base_metric.py
+-rw-rw-rw-   0        0        0     4077 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/metrics/_id_metric.py
+-rw-rw-rw-   0        0        0     5173 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/metrics/_trace_metric.py
+-rw-rw-rw-   0        0        0     6093 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/metrics/_transition_metric.py
+-rw-rw-rw-   0        0        0     3995 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/metrics/_user_metric.py
+-rw-rw-rw-   0        0        0      389 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/metrics/_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-19 07:37:05.199371 sberpm-2.4.0/sberpm/miners/
+-rw-rw-rw-   0        0        0     1374 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/miners/__init__.py
+-rw-rw-rw-   0        0        0     9571 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/miners/_abstract_miner.py
+-rw-rw-rw-   0        0        0    19774 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/miners/_alpha_miner.py
+-rw-rw-rw-   0        0        0    10578 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/miners/_alpha_plus_miner.py
+-rw-rw-rw-   0        0        0      174 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/miners/_auto_miner.py
+-rw-rw-rw-   0        0        0     3153 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/miners/_causal_miner.py
+-rw-rw-rw-   0        0        0    18462 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/miners/_correlation_miner.py
+-rw-rw-rw-   0        0        0     9122 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/miners/_heu_miner.py
+-rw-rw-rw-   0        0        0     3896 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/miners/_inductive_miner.py
+-rw-rw-rw-   0        0        0     8354 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/miners/_inductive_utils.py
+-rw-rw-rw-   0        0        0      174 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/miners/_ml_miner.py
+-rw-rw-rw-   0        0        0     7306 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/miners/_parallel_miner.py
+-rw-rw-rw-   0        0        0     2678 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/miners/_simple_miner.py
+drwxrwxrwx   0        0        0        0 2023-04-19 07:37:05.204538 sberpm-2.4.0/sberpm/miners/file_obf/
+-rw-rw-rw-   0        0        0     3192 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/miners/file_obf/_auto_miner.obfsbpm
+-rw-rw-rw-   0        0        0     5082 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/miners/file_obf/_ml_miner.obfsbpm
+drwxrwxrwx   0        0        0        0 2023-04-19 07:37:05.210679 sberpm-2.4.0/sberpm/miners/mining_utils/
+-rw-rw-rw-   0        0        0     8347 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/miners/mining_utils/_inductive_utils.py
+-rw-rw-rw-   0        0        0    25893 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/miners/mining_utils/_node_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-19 07:37:05.213675 sberpm-2.4.0/sberpm/ml/
+-rw-rw-rw-   0        0        0      179 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/ml/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 07:37:05.237048 sberpm-2.4.0/sberpm/ml/anomaly_detection/
+-rw-rw-rw-   0        0        0      571 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/ml/anomaly_detection/__init__.py
+-rw-rw-rw-   0        0        0    11459 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/ml/anomaly_detection/_outlier_detector.py
+-rw-rw-rw-   0        0        0     4669 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/ml/anomaly_detection/_outlier_detector_ensemble.py
+-rw-rw-rw-   0        0        0     5295 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/ml/anomaly_detection/_outliercblof.py
+-rw-rw-rw-   0        0        0     2404 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/ml/anomaly_detection/_outliercustom.py
+-rw-rw-rw-   0        0        0     4911 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/ml/anomaly_detection/_outlierforest.py
+-rw-rw-rw-   0        0        0     6340 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/ml/anomaly_detection/_outlierlof.py
+-rw-rw-rw-   0        0        0     4804 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/ml/anomaly_detection/_outlierocsvm.py
+drwxrwxrwx   0        0        0        0 2023-04-19 07:37:05.242219 sberpm-2.4.0/sberpm/ml/chronometrage/
+-rw-rw-rw-   0        0        0       76 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/ml/chronometrage/__init__.py
+-rw-rw-rw-   0        0        0     6531 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/ml/chronometrage/_chronometrage.py
+drwxrwxrwx   0        0        0        0 2023-04-19 07:37:05.247200 sberpm-2.4.0/sberpm/ml/stages_clustering/
+-rw-rw-rw-   0        0        0      111 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/ml/stages_clustering/__init__.py
+-rw-rw-rw-   0        0        0      183 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/ml/stages_clustering/_stages_clustering.py
+drwxrwxrwx   0        0        0        0 2023-04-19 07:37:05.250198 sberpm-2.4.0/sberpm/ml/stages_clustering/file_obf/
+-rw-rw-rw-   0        0        0     5116 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/ml/stages_clustering/file_obf/_stages_clustering.obfsbpm
+drwxrwxrwx   0        0        0        0 2023-04-19 07:37:05.255323 sberpm-2.4.0/sberpm/ml/utils/
+-rw-rw-rw-   0        0        0      107 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/ml/utils/__init__.py
+-rw-rw-rw-   0        0        0     3935 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/ml/utils/_perm_importance.py
+drwxrwxrwx   0        0        0        0 2023-04-19 07:37:05.260324 sberpm-2.4.0/sberpm/models/
+-rw-rw-rw-   0        0        0      300 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/models/__init__.py
+-rw-rw-rw-   0        0        0     1846 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/models/_check_models.py
+drwxrwxrwx   0        0        0        0 2023-04-19 07:37:05.279576 sberpm-2.4.0/sberpm/visual/
+-rw-rw-rw-   0        0        0      608 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/visual/__init__.py
+-rw-rw-rw-   0        0        0    76564 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/visual/_chart_painter.py
+-rw-rw-rw-   0        0        0    18529 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/visual/_graph.py
+-rw-rw-rw-   0        0        0    12406 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/visual/_graphviz_painter.py
+-rw-rw-rw-   0        0        0    25598 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/visual/_matplotlib_painter.py
+-rw-rw-rw-   0        0        0      594 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/visual/_types.py
+-rw-rw-rw-   0        0        0     6935 2023-01-26 18:07:31.000000 sberpm-2.4.0/sberpm/visual/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-19 07:37:05.086598 sberpm-2.4.0/sberpm.egg-info/
+-rw-rw-rw-   0        0        0     2887 2023-04-19 07:37:04.000000 sberpm-2.4.0/sberpm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3186 2023-04-19 07:37:04.000000 sberpm-2.4.0/sberpm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 07:37:04.000000 sberpm-2.4.0/sberpm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      814 2023-04-19 07:37:04.000000 sberpm-2.4.0/sberpm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-19 07:37:04.000000 sberpm-2.4.0/sberpm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 07:37:05.310029 sberpm-2.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     2606 2023-04-19 07:36:42.000000 sberpm-2.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 07:37:05.290887 sberpm-2.4.0/tutorials/
+-rw-rw-rw-   0        0        0    19319 2023-01-26 18:07:31.000000 sberpm-2.4.0/tutorials/chrono_data.xlsx
+-rw-rw-rw-   0        0        0   132942 2023-01-26 18:07:31.000000 sberpm-2.4.0/tutorials/example.xlsx
+-rw-rw-rw-   0        0        0    92872 2023-03-14 16:20:33.000000 sberpm-2.4.0/tutorials/tutorial_en.ipynb
+-rw-rw-rw-   0        0        0   124935 2023-03-14 16:20:11.000000 sberpm-2.4.0/tutorials/tutorial_ru.ipynb
```

### Comparing `sberpm-2.3.3/LICENSE` & `sberpm-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sberpm-2.3.3/LICENSE_RUS` & `sberpm-2.4.0/LICENSE_RUS`

 * *Files identical despite different names*

### Comparing `sberpm-2.3.3/PKG-INFO` & `sberpm-2.4.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: sberpm
-Version: 2.3.3
-Summary: Library that is intended to operate with various process mining tasks.
-Author: Sberbank Process Mining Team
-Author-email: AABugaenko@sberbank.ru
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: LICENSE_RUS
-
 # SberProcessMining (SberPM) – Process Mining Python framework
 SberPM is an open-source Python library for conducting a comprehensive analysis of business processes with the use of process mining and machine learning techniques. By implementing this tool, objective and deep insights into the process on all levels can be revealed. These insights are then used to detect problems such as bottlenecks and deviations and identify potential opportunities for process improvement and optimization.
 
 With SberPM you can:
 - **Discover the real process flow and create visualization of the generated model**
     Having the event log of a business process, you can build the process model in the form of a graph by using the algorithms called miners and visualize it. In order to do this, the library provides a number of algorithms, that is Simple Miner, Causal Miner, Heuristic Miner, Alpha/Alpha+ Miners, and Inductive Miner. Thus different process weaknesses such as bottlenecks, loops, and deviations can be identified.
 - **Calculate process performance indicators**
```

### Comparing `sberpm-2.3.3/README.md` & `sberpm-2.4.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: sberpm
+Version: 2.4.0
+Summary: Library that is intended to operate with various process mining tasks.
+Author: Sberbank Process Mining Team
+Author-email: AABugaenko@sberbank.ru
+Classifier: Programming Language :: Python
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: LICENSE_RUS
+
 # SberProcessMining (SberPM) – Process Mining Python framework
 SberPM is an open-source Python library for conducting a comprehensive analysis of business processes with the use of process mining and machine learning techniques. By implementing this tool, objective and deep insights into the process on all levels can be revealed. These insights are then used to detect problems such as bottlenecks and deviations and identify potential opportunities for process improvement and optimization.
 
 With SberPM you can:
 - **Discover the real process flow and create visualization of the generated model**
     Having the event log of a business process, you can build the process model in the form of a graph by using the algorithms called miners and visualize it. In order to do this, the library provides a number of algorithms, that is Simple Miner, Causal Miner, Heuristic Miner, Alpha/Alpha+ Miners, and Inductive Miner. Thus different process weaknesses such as bottlenecks, loops, and deviations can be identified.
 - **Calculate process performance indicators**
```

### Comparing `sberpm-2.3.3/requirements.txt` & `sberpm-2.4.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `sberpm-2.3.3/sberpm/__init__.py` & `sberpm-2.4.0/sberpm/__init__.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.3.3/sberpm/_holder.py` & `sberpm-2.4.0/sberpm/_holder.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.3.3/sberpm/_utils.py` & `sberpm-2.4.0/sberpm/_utils.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.3.3/sberpm/autoinsights/file_obf/_influencing_activities.obfsbpm` & `sberpm-2.4.0/sberpm/autoinsights/file_obf/_influencing_activities.obfsbpm`

 * *Files identical despite different names*

### Comparing `sberpm-2.3.3/sberpm/bpmn/_bpmn_file_to_graph.py` & `sberpm-2.4.0/sberpm/bpmn/_bpmn_file_to_graph.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.3.3/sberpm/bpmn/_bpmn_graph_to_file/_bpmn_exporter.py` & `sberpm-2.4.0/sberpm/bpmn/_bpmn_graph_to_file/_bpmn_exporter.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.3.3/sberpm/bpmn/_bpmn_graph_to_file/_bpmn_xml_maker.py` & `sberpm-2.4.0/sberpm/bpmn/_bpmn_graph_to_file/_bpmn_xml_maker.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.3.3/sberpm/bpmn/_bpmn_graph_to_file/_petri_net_to_bpmn.py` & `sberpm-2.4.0/sberpm/bpmn/_bpmn_graph_to_file/_petri_net_to_bpmn.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.3.3/sberpm/bpmn/_bpmn_graph_to_file/grandalf.py` & `sberpm-2.4.0/sberpm/bpmn/_bpmn_graph_to_file/grandalf.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.3.3/sberpm/bpmn/_bpmn_graph_to_file/graphviz.py` & `sberpm-2.4.0/sberpm/bpmn/_bpmn_graph_to_file/graphviz.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.3.3/sberpm/column_matching/file_obf/_column_matching_.obfsbpm` & `sberpm-2.4.0/sberpm/column_matching/file_obf/_column_matching_.obfsbpm`

 * *Files identical despite different names*

### Comparing `sberpm-2.3.3/sberpm/conformance_checking/_conformance_checking.py` & `sberpm-2.4.0/sberpm/conformance_checking/_conformance_checking.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.3.3/sberpm/conformance_checking/_token_replay.py` & `sberpm-2.4.0/sberpm/conformance_checking/_token_replay.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.3.3/sberpm/decision_mining/_decision_mining.py` & `sberpm-2.4.0/sberpm/decision_mining/_decision_mining.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.3.3/sberpm/graph_stats/centrality.py` & `sberpm-2.4.0/sberpm/graph_stats/centrality.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.3.3/sberpm/imitation/_simulation.py` & `sberpm-2.4.0/sberpm/imitation/_simulation.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.3.3/sberpm/imitation/_validation.py` & `sberpm-2.4.0/sberpm/imitation/_validation.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.3.3/sberpm/metrics/_activity_metric.py` & `sberpm-2.4.0/sberpm/metrics/_activity_metric.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.3.3/sberpm/metrics/_base_metric.py` & `sberpm-2.4.0/sberpm/metrics/_base_metric.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.3.3/sberpm/metrics/_id_metric.py` & `sberpm-2.4.0/sberpm/metrics/_id_metric.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.3.3/sberpm/metrics/_trace_metric.py` & `sberpm-2.4.0/sberpm/metrics/_trace_metric.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.3.3/sberpm/metrics/_transition_metric.py` & `sberpm-2.4.0/sberpm/metrics/_transition_metric.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.3.3/sberpm/metrics/_user_metric.py` & `sberpm-2.4.0/sberpm/metrics/_user_metric.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.3.3/sberpm/miners/__init__.py` & `sberpm-2.4.0/sberpm/miners/__init__.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.3.3/sberpm/miners/_abstract_miner.py` & `sberpm-2.4.0/sberpm/miners/_abstract_miner.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.3.3/sberpm/miners/_alpha_miner.py` & `sberpm-2.4.0/sberpm/miners/_alpha_miner.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.3.3/sberpm/miners/_alpha_plus_miner.py` & `sberpm-2.4.0/sberpm/miners/_alpha_plus_miner.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.3.3/sberpm/miners/_causal_miner.py` & `sberpm-2.4.0/sberpm/miners/_causal_miner.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.3.3/sberpm/miners/_correlation_miner.py` & `sberpm-2.4.0/sberpm/miners/_correlation_miner.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.3.3/sberpm/miners/_heu_miner.py` & `sberpm-2.4.0/sberpm/miners/_heu_miner.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.3.3/sberpm/miners/_inductive_miner.py` & `sberpm-2.4.0/sberpm/miners/_inductive_miner.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.3.3/sberpm/miners/_inductive_utils.py` & `sberpm-2.4.0/sberpm/miners/_inductive_utils.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.3.3/sberpm/miners/_parallel_miner.py` & `sberpm-2.4.0/sberpm/miners/_parallel_miner.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.3.3/sberpm/miners/_simple_miner.py` & `sberpm-2.4.0/sberpm/miners/_simple_miner.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.3.3/sberpm/miners/file_obf/_auto_miner.obfsbpm` & `sberpm-2.4.0/sberpm/miners/file_obf/_auto_miner.obfsbpm`

 * *Files identical despite different names*

### Comparing `sberpm-2.3.3/sberpm/miners/file_obf/_ml_miner.obfsbpm` & `sberpm-2.4.0/sberpm/miners/file_obf/_ml_miner.obfsbpm`

 * *Files identical despite different names*

### Comparing `sberpm-2.3.3/sberpm/miners/mining_utils/_inductive_utils.py` & `sberpm-2.4.0/sberpm/miners/mining_utils/_inductive_utils.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.3.3/sberpm/miners/mining_utils/_node_utils.py` & `sberpm-2.4.0/sberpm/miners/mining_utils/_node_utils.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.3.3/sberpm/ml/anomaly_detection/__init__.py` & `sberpm-2.4.0/sberpm/ml/anomaly_detection/__init__.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.3.3/sberpm/ml/anomaly_detection/_outlier_detector.py` & `sberpm-2.4.0/sberpm/ml/anomaly_detection/_outlier_detector.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.3.3/sberpm/ml/anomaly_detection/_outlier_detector_ensemble.py` & `sberpm-2.4.0/sberpm/ml/anomaly_detection/_outlier_detector_ensemble.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.3.3/sberpm/ml/anomaly_detection/_outliercblof.py` & `sberpm-2.4.0/sberpm/ml/anomaly_detection/_outliercblof.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.3.3/sberpm/ml/anomaly_detection/_outliercustom.py` & `sberpm-2.4.0/sberpm/ml/anomaly_detection/_outliercustom.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.3.3/sberpm/ml/anomaly_detection/_outlierforest.py` & `sberpm-2.4.0/sberpm/ml/anomaly_detection/_outlierforest.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.3.3/sberpm/ml/anomaly_detection/_outlierlof.py` & `sberpm-2.4.0/sberpm/ml/anomaly_detection/_outlierlof.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.3.3/sberpm/ml/anomaly_detection/_outlierocsvm.py` & `sberpm-2.4.0/sberpm/ml/anomaly_detection/_outlierocsvm.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.3.3/sberpm/ml/chronometrage/_chronometrage.py` & `sberpm-2.4.0/sberpm/ml/chronometrage/_chronometrage.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.3.3/sberpm/ml/stages_clustering/file_obf/_stages_clustering.obfsbpm` & `sberpm-2.4.0/sberpm/ml/stages_clustering/file_obf/_stages_clustering.obfsbpm`

 * *Files identical despite different names*

### Comparing `sberpm-2.3.3/sberpm/ml/utils/_perm_importance.py` & `sberpm-2.4.0/sberpm/ml/utils/_perm_importance.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.3.3/sberpm/models/_check_models.py` & `sberpm-2.4.0/sberpm/models/_check_models.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.3.3/sberpm/visual/__init__.py` & `sberpm-2.4.0/sberpm/visual/__init__.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.3.3/sberpm/visual/_chart_painter.py` & `sberpm-2.4.0/sberpm/visual/_chart_painter.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.3.3/sberpm/visual/_graph.py` & `sberpm-2.4.0/sberpm/visual/_graph.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.3.3/sberpm/visual/_graphviz_painter.py` & `sberpm-2.4.0/sberpm/visual/_graphviz_painter.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.3.3/sberpm/visual/_matplotlib_painter.py` & `sberpm-2.4.0/sberpm/visual/_matplotlib_painter.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.3.3/sberpm/visual/_types.py` & `sberpm-2.4.0/sberpm/visual/_types.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.3.3/sberpm/visual/utils.py` & `sberpm-2.4.0/sberpm/visual/utils.py`

 * *Files identical despite different names*

### Comparing `sberpm-2.3.3/sberpm.egg-info/PKG-INFO` & `sberpm-2.4.0/sberpm.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 Metadata-Version: 2.1
 Name: sberpm
-Version: 2.3.3
+Version: 2.4.0
 Summary: Library that is intended to operate with various process mining tasks.
 Author: Sberbank Process Mining Team
 Author-email: AABugaenko@sberbank.ru
+Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE_RUS
 
 # SberProcessMining (SberPM) – Process Mining Python framework
 SberPM is an open-source Python library for conducting a comprehensive analysis of business processes with the use of process mining and machine learning techniques. By implementing this tool, objective and deep insights into the process on all levels can be revealed. These insights are then used to detect problems such as bottlenecks and deviations and identify potential opportunities for process improvement and optimization.
```

### Comparing `sberpm-2.3.3/sberpm.egg-info/SOURCES.txt` & `sberpm-2.4.0/sberpm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sberpm-2.3.3/sberpm.egg-info/requires.txt` & `sberpm-2.4.0/sberpm.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `sberpm-2.3.3/setup.py` & `sberpm-2.4.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -59,13 +59,18 @@
     long_description_content_type="text/markdown",
 
     author="Sberbank Process Mining Team",
     author_email="AABugaenko@sberbank.ru",
     packages=get_packages(),
     include_package_data=True,
     classifiers=[
+        "Programming Language :: Python",
         "Intended Audience :: Developers",
+        "Programming Language :: Python :: 3 :: Only",
+        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
         "Operating System :: OS Independent",
     ],
+    python_requires=">=3.7",
     install_requires=parse_requirements("requirements.txt"),
 )
```

### Comparing `sberpm-2.3.3/tutorials/chrono_data.xlsx` & `sberpm-2.4.0/tutorials/chrono_data.xlsx`

 * *Files identical despite different names*

### Comparing `sberpm-2.3.3/tutorials/example.xlsx` & `sberpm-2.4.0/tutorials/example.xlsx`

 * *Files identical despite different names*

### Comparing `sberpm-2.3.3/tutorials/tutorial_en.ipynb` & `sberpm-2.4.0/tutorials/tutorial_en.ipynb`

 * *Files identical despite different names*

### Comparing `sberpm-2.3.3/tutorials/tutorial_ru.ipynb` & `sberpm-2.4.0/tutorials/tutorial_ru.ipynb`

 * *Files identical despite different names*

