# Comparing `tmp/geochemistrypi-0.1.0.tar.gz` & `tmp/geochemistrypi-0.2.0.tar.gz`

## Comparing `geochemistrypi-0.1.0.tar` & `geochemistrypi-0.2.0.tar`

### file list

```diff
@@ -1,70 +1,74 @@
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 geochemistrypi-0.1.0/requirements.txt
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 geochemistrypi-0.1.0/.github/workflows/geochemistrypy.yml
--rw-r--r--   0        0        0   285992 2020-02-02 00:00:00.000000 geochemistrypi-0.1.0/docs/Geochemistry π.png
--rw-r--r--   0        0        0   255925 2020-02-02 00:00:00.000000 geochemistrypi-0.1.0/docs/Geochemistryπ-Activity Diagram_v1.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geochemistrypi-0.1.0/geochemistrypi/__init__.py
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 geochemistrypi-0.1.0/geochemistrypi/cli.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 geochemistrypi-0.1.0/geochemistrypi/main.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 geochemistrypi-0.1.0/geochemistrypi/data_mining/__init__.py
--rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 geochemistrypi-0.1.0/geochemistrypi/data_mining/global_variable.py
--rw-r--r--   0        0        0    13917 2020-02-02 00:00:00.000000 geochemistrypi-0.1.0/geochemistrypi/data_mining/pipeline.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 geochemistrypi-0.1.0/geochemistrypi/data_mining/data/__init__.py
--rw-r--r--   0        0        0    10755 2020-02-02 00:00:00.000000 geochemistrypi-0.1.0/geochemistrypi/data_mining/data/data_readiness.py
--rw-r--r--   0        0        0     7143 2020-02-02 00:00:00.000000 geochemistrypi-0.1.0/geochemistrypi/data_mining/data/feature_engineering.py
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 geochemistrypi-0.1.0/geochemistrypi/data_mining/data/imputation.py
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 geochemistrypi-0.1.0/geochemistrypi/data_mining/data/preprocessing.py
--rw-r--r--   0        0        0     3492 2020-02-02 00:00:00.000000 geochemistrypi-0.1.0/geochemistrypi/data_mining/data/statistic.py
--rw-r--r--   0        0        0   225291 2020-02-02 00:00:00.000000 geochemistrypi-0.1.0/geochemistrypi/data_mining/data/dataset/Data_Classification.xlsx
--rw-r--r--   0        0        0   225363 2020-02-02 00:00:00.000000 geochemistrypi-0.1.0/geochemistrypi/data_mining/data/dataset/Data_Clustering.xlsx
--rw-r--r--   0        0        0    44562 2020-02-02 00:00:00.000000 geochemistrypi-0.1.0/geochemistrypi/data_mining/data/dataset/Data_Decomposition.xlsx
--rw-r--r--   0        0        0    44562 2020-02-02 00:00:00.000000 geochemistrypi-0.1.0/geochemistrypi/data_mining/data/dataset/Data_Regression.xlsx
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 geochemistrypi-0.1.0/geochemistrypi/data_mining/model/__init__.py
--rw-r--r--   0        0        0    10420 2020-02-02 00:00:00.000000 geochemistrypi-0.1.0/geochemistrypi/data_mining/model/_base.py
--rw-r--r--   0        0        0    64821 2020-02-02 00:00:00.000000 geochemistrypi-0.1.0/geochemistrypi/data_mining/model/classification.py
--rw-r--r--   0        0        0    16255 2020-02-02 00:00:00.000000 geochemistrypi-0.1.0/geochemistrypi/data_mining/model/clustering.py
--rw-r--r--   0        0        0    11317 2020-02-02 00:00:00.000000 geochemistrypi-0.1.0/geochemistrypi/data_mining/model/decomposition.py
--rw-r--r--   0        0        0    86210 2020-02-02 00:00:00.000000 geochemistrypi-0.1.0/geochemistrypi/data_mining/model/regression.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 geochemistrypi-0.1.0/geochemistrypi/data_mining/model/func/__init__.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 geochemistrypi-0.1.0/geochemistrypi/data_mining/model/func/algo_classification/__init__.py
--rw-r--r--   0        0        0     4417 2020-02-02 00:00:00.000000 geochemistrypi-0.1.0/geochemistrypi/data_mining/model/func/algo_classification/_common.py
--rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 geochemistrypi-0.1.0/geochemistrypi/data_mining/model/func/algo_classification/_decision_tree.py
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 geochemistrypi-0.1.0/geochemistrypi/data_mining/model/func/algo_classification/_logistic.py
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 geochemistrypi-0.1.0/geochemistrypi/data_mining/model/func/algo_classification/_rf.py
--rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 geochemistrypi-0.1.0/geochemistrypi/data_mining/model/func/algo_classification/_svm.py
--rw-r--r--   0        0        0     5943 2020-02-02 00:00:00.000000 geochemistrypi-0.1.0/geochemistrypi/data_mining/model/func/algo_classification/_xgboost.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 geochemistrypi-0.1.0/geochemistrypi/data_mining/model/func/algo_clustering/__init__.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 geochemistrypi-0.1.0/geochemistrypi/data_mining/model/func/algo_clustering/_common.py
--rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 geochemistrypi-0.1.0/geochemistrypi/data_mining/model/func/algo_clustering/_dbscan.py
--rw-r--r--   0        0        0     6015 2020-02-02 00:00:00.000000 geochemistrypi-0.1.0/geochemistrypi/data_mining/model/func/algo_clustering/_kmeans.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 geochemistrypi-0.1.0/geochemistrypi/data_mining/model/func/algo_decomposition/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 geochemistrypi-0.1.0/geochemistrypi/data_mining/model/func/algo_decomposition/_common.py
--rw-r--r--   0        0        0     4752 2020-02-02 00:00:00.000000 geochemistrypi-0.1.0/geochemistrypi/data_mining/model/func/algo_decomposition/_pca.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 geochemistrypi-0.1.0/geochemistrypi/data_mining/model/func/algo_regression/__init__.py
--rw-r--r--   0        0        0     3659 2020-02-02 00:00:00.000000 geochemistrypi-0.1.0/geochemistrypi/data_mining/model/func/algo_regression/_common.py
--rw-r--r--   0        0        0     2554 2020-02-02 00:00:00.000000 geochemistrypi-0.1.0/geochemistrypi/data_mining/model/func/algo_regression/_decision_tree.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 geochemistrypi-0.1.0/geochemistrypi/data_mining/model/func/algo_regression/_dnn.py
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 geochemistrypi-0.1.0/geochemistrypi/data_mining/model/func/algo_regression/_extra_tree.py
--rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 geochemistrypi-0.1.0/geochemistrypi/data_mining/model/func/algo_regression/_linear.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 geochemistrypi-0.1.0/geochemistrypi/data_mining/model/func/algo_regression/_polynomial.py
--rw-r--r--   0        0        0     3730 2020-02-02 00:00:00.000000 geochemistrypi-0.1.0/geochemistrypi/data_mining/model/func/algo_regression/_rf.py
--rw-r--r--   0        0        0     2548 2020-02-02 00:00:00.000000 geochemistrypi-0.1.0/geochemistrypi/data_mining/model/func/algo_regression/_xgboost.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geochemistrypi-0.1.0/geochemistrypi/data_mining/plot/__init__.py
--rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 geochemistrypi-0.1.0/geochemistrypi/data_mining/plot/geochemistry_plot.py
--rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 geochemistrypi-0.1.0/geochemistrypi/data_mining/plot/map_plot.py
--rw-r--r--   0        0        0     4354 2020-02-02 00:00:00.000000 geochemistrypi-0.1.0/geochemistrypi/data_mining/plot/statistic_plot.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 geochemistrypi-0.1.0/geochemistrypi/data_mining/process/__init__.py
--rw-r--r--   0        0        0     4336 2020-02-02 00:00:00.000000 geochemistrypi-0.1.0/geochemistrypi/data_mining/process/classify.py
--rw-r--r--   0        0        0     2907 2020-02-02 00:00:00.000000 geochemistrypi-0.1.0/geochemistrypi/data_mining/process/cluster.py
--rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 geochemistrypi-0.1.0/geochemistrypi/data_mining/process/decompose.py
--rw-r--r--   0        0        0     6487 2020-02-02 00:00:00.000000 geochemistrypi-0.1.0/geochemistrypi/data_mining/process/regress.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geochemistrypi-0.1.0/geochemistrypi/data_mining/tests/__init__.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 geochemistrypi-0.1.0/geochemistrypi/data_mining/tests/test_data/__init__.py
--rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 geochemistrypi-0.1.0/geochemistrypi/data_mining/tests/test_data/test_data_readiness.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 geochemistrypi-0.1.0/geochemistrypi/data_mining/utils/__init__.py
--rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 geochemistrypi-0.1.0/geochemistrypi/data_mining/utils/base.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 geochemistrypi-0.1.0/geochemistrypi/data_mining/utils/exceptions.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 geochemistrypi-0.1.0/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 geochemistrypi-0.1.0/LICENSE
--rw-r--r--   0        0        0     8360 2020-02-02 00:00:00.000000 geochemistrypi-0.1.0/README.md
--rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 geochemistrypi-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    10786 2020-02-02 00:00:00.000000 geochemistrypi-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/requirements.txt
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/.github/workflows/geochemistrypy.yml
+-rw-r--r--   0        0        0   285992 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/docs/Geochemistry π.png
+-rw-r--r--   0        0        0   255925 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/docs/Geochemistryπ-Activity Diagram_v1.png
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/__init__.py
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/cli.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/main.py
+-rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/UI.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/__init__.py
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/global_variable.py
+-rw-r--r--   0        0        0    15242 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/pipeline.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/data/__init__.py
+-rw-r--r--   0        0        0    12027 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/data/data_readiness.py
+-rw-r--r--   0        0        0     7620 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/data/feature_engineering.py
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/data/imputation.py
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/data/preprocessing.py
+-rw-r--r--   0        0        0     3492 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/data/statistic.py
+-rw-r--r--   0        0        0   225291 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/data/dataset/Data_Classification.xlsx
+-rw-r--r--   0        0        0   225363 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/data/dataset/Data_Clustering.xlsx
+-rw-r--r--   0        0        0    44562 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/data/dataset/Data_Decomposition.xlsx
+-rw-r--r--   0        0        0    44562 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/data/dataset/Data_Regression.xlsx
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/model/__init__.py
+-rw-r--r--   0        0        0    10732 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/model/_base.py
+-rw-r--r--   0        0        0   106659 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/model/classification.py
+-rw-r--r--   0        0        0    17294 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/model/clustering.py
+-rw-r--r--   0        0        0    11942 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/model/decomposition.py
+-rw-r--r--   0        0        0    94512 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/model/regression.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/__init__.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_classification/__init__.py
+-rw-r--r--   0        0        0     4417 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_classification/_common.py
+-rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_classification/_decision_tree.py
+-rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_classification/_deep_neural_network.py
+-rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_classification/_extra_trees.py
+-rw-r--r--   0        0        0     4940 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_classification/_logistic_regression.py
+-rw-r--r--   0        0        0     4541 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_classification/_rf.py
+-rw-r--r--   0        0        0     6967 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_classification/_svm.py
+-rw-r--r--   0        0        0     8499 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_classification/_xgboost.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_clustering/__init__.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_clustering/_common.py
+-rw-r--r--   0        0        0     5818 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_clustering/_dbscan.py
+-rw-r--r--   0        0        0     8184 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_clustering/_kmeans.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_decomposition/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_decomposition/_common.py
+-rw-r--r--   0        0        0     5729 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_decomposition/_pca.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_regression/__init__.py
+-rw-r--r--   0        0        0     3659 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_regression/_common.py
+-rw-r--r--   0        0        0     5188 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_regression/_decision_tree.py
+-rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_regression/_deep_neural_network.py
+-rw-r--r--   0        0        0     5712 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_regression/_extra_tree.py
+-rw-r--r--   0        0        0     3621 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_regression/_linear_regression.py
+-rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_regression/_polynomial_regression.py
+-rw-r--r--   0        0        0     7273 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_regression/_rf.py
+-rw-r--r--   0        0        0     6807 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_regression/_svr.py
+-rw-r--r--   0        0        0     5104 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_regression/_xgboost.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/plot/__init__.py
+-rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/plot/geochemistry_plot.py
+-rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/plot/map_plot.py
+-rw-r--r--   0        0        0     4354 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/plot/statistic_plot.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/process/__init__.py
+-rw-r--r--   0        0        0     8069 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/process/classify.py
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/process/cluster.py
+-rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/process/decompose.py
+-rw-r--r--   0        0        0     8420 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/process/regress.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/tests/__init__.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/tests/test_data/__init__.py
+-rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/tests/test_data/test_data_readiness.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/utils/__init__.py
+-rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/utils/base.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/utils/exceptions.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/LICENSE
+-rw-r--r--   0        0        0     9971 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/README.md
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    12426 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/PKG-INFO
```

### Comparing `geochemistrypi-0.1.0/.github/workflows/geochemistrypy.yml` & `geochemistrypi-0.2.0/.github/workflows/geochemistrypy.yml`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.1.0/docs/Geochemistry π.png` & `geochemistrypi-0.2.0/docs/Geochemistry π.png`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.1.0/docs/Geochemistryπ-Activity Diagram_v1.png` & `geochemistrypi-0.2.0/docs/Geochemistryπ-Activity Diagram_v1.png`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.1.0/geochemistrypi/cli.py` & `geochemistrypi-0.2.0/geochemistrypi/cli.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.1.0/geochemistrypi/data_mining/global_variable.py` & `geochemistrypi-0.2.0/geochemistrypi/data_mining/global_variable.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 
 # current working directory in which the user activates the application
 WORKING_PATH = os.getcwd()
 
-# the directory in which the package(application) s installed
+# the directory in which the package(application) is installed
 PACKAGEDIR = os.path.dirname(os.path.realpath(__file__))
 
 # the directory where the built-in data set to be processed stays
 BUILT_IN_DATASET_PATH = os.path.join(PACKAGEDIR, "data", "dataset")
 
 # the root directory where all the output stays
 OUTPUT_PATH = os.path.join(WORKING_PATH, "output")
@@ -32,17 +32,20 @@
 DATA_OPTION = ['Own Data', 'Testing Data (Built-in)']
 TEST_DATA_OPTION = ['Data For Regression', 'Data For Classification',
                     'Data For Clustering', 'Data For Dimensional Reduction']
 MODE_OPTION = ['Regression', 'Classification', 'Clustering', 'Dimensional Reduction']
 
 # The model provided to use
 REGRESSION_MODELS = ['Linear Regression', 'Polynomial Regression', 'Support Vector Machine', 'Decision Tree',
-                     'Random Forest', 'Extra-Trees', 'Xgboost', 'Deep Neural Networks']
-CLASSIFICATION_MODELS = ['Logistic Regression', 'Support Vector Machine', 'Decision Tree', 'Random Forest', 'Xgboost']
+                     'Random Forest', 'Extra-Trees', 'Xgboost', 'Deep Neural Network']
+CLASSIFICATION_MODELS = ['Logistic Regression', 'Support Vector Machine', 'Decision Tree', 'Random Forest', 'Extra-Trees', 
+                         'Xgboost', 'Deep Neural Network']
 CLUSTERING_MODELS = ['KMeans', 'DBSCAN']
 DECOMPOSITION_MODELS = ['Principal Component Analysis']
+
+# Special AutoML models
 NON_AUTOML_MODELS = ['Linear Regression', 'Polynomial Regression']
-RAY_FLAML = ['Deep Neural Networks']
+RAY_FLAML = ['Deep Neural Network']
 
-IMPUTING_STRATEGY = ['Mean', 'Median', 'Most Frequent']
+IMPUTING_STRATEGY = ['Mean Value', 'Median Value', 'Most Frequent Value', 'Constant(Specified Value)']
 
 FEATURE_SCALING_STRATEGY = ['Min-max Scaling', 'Standardization']
```

### Comparing `geochemistrypi-0.1.0/geochemistrypi/data_mining/pipeline.py` & `geochemistrypi-0.2.0/geochemistrypi/data_mining/pipeline.py`

 * *Files 8% similar despite different names*

```diff
@@ -58,29 +58,54 @@
         data = read_data(file_name=file_name)
         print(f"Successfully loading the built-in data set '{file_name}'.")
     show_data_columns(data.columns)
     clear_output()
 
     # World map projection for a specific element
     logger.debug("World Map Projection")
+    print("-*-*- World Map -*-*-")
     map_flag = 0
     is_map_projection = 0
-    while True:
+    detection_index = 0
+    if ('LATITUDE' not in data.columns) and ('latitude' not in data.columns):
+        detection_index += 1
+    if ('LONGITUDE' not in data.columns) and ('longitude' not in data.columns):
+        detection_index += 2
+    if detection_index == 1:
+        print("The provided data set is lack of 'LATITUDE' data.")
+    elif detection_index == 2:
+        print("The provided data set is lack of 'LONGITUDE' data.")
+    elif detection_index == 3:
+        print("The provided data set is lack of 'LONGITUDE' and 'LATITUDE' data.")
+    if detection_index != 0:
+        print("Hence, world map projection functionality will be skipped!")
+        clear_output()
+    while detection_index == 0:
         if map_flag != 1:
             # option selection
             print("World Map Projection for A Specific Element Option:")
             num2option(OPTION)
             is_map_projection = limit_num_input(OPTION, SECTION[3], num_input)
             clear_output()
         if is_map_projection == 1:
             print("-*-*- Distribution in World Map -*-*-")
             print("Select one of the elements below to be projected in the World Map: ")
             show_data_columns(data.columns)
             elm_num = limit_num_input(data.columns, SECTION[3], num_input)
-            map_projected(data.iloc[:, elm_num - 1], data)
+            clear_output()
+            if 'LONGITUDE' in data.columns:
+                longitude = data.loc[:, 'LONGITUDE']
+            else:
+                longitude = data.loc[:, 'longitude']
+            if 'LATITUDE' in data.columns:
+                latitude = data.loc[:, 'LATITUDE']
+            else:
+                latitude = data.loc[:, 'latitude']
+            print("Longitude and latitude data are selected from the provided data set.")
+            map_projected(data.iloc[:, elm_num - 1], longitude, latitude)
             clear_output()
             print("Do you want to continue to project a new element in the World Map?")
             num2option(OPTION)
             map_flag = limit_num_input(OPTION, SECTION[3], num_input)
             if map_flag == 1:
                 clear_output()
                 continue
@@ -88,16 +113,16 @@
                 print('Exit Map Projection Mode.')
                 clear_output()
                 break
         elif is_map_projection == 2:
             break
 
     # Create the processing data set
-    logger.debug("Data Selected")
-    print("-*-*- Data Selected -*-*-")
+    logger.debug("Data Selection")
+    print("-*-*- Data Selection -*-*-")
     show_data_columns(data.columns)
     data_processed = create_sub_data_set(data)
     clear_output()
     print("The Selected Data Set:")
     print(data_processed)
     clear_output()
     print('Basic Statistical Information: ')
@@ -230,27 +255,28 @@
         clear_output()
 
         # create Y data set
         print("-*-*- Data Split - X Set and Y Set-*-*-")
         print("Selected sub data set to create Y data set:")
         show_data_columns(data_processed_imputed.columns)
         print('The selected Y data set:')
-        print('Note: Normally, only one column is allowed to be tag column, not multiple columns.')
+        print('Notice: Normally, please choose only one column to be tag column Y, not multiple columns.')
+        print('Notice: For classification model training, please choose the label column which has distinctive integers.')
         y = create_sub_data_set(data_processed_imputed)
         print('Successfully create Y data set.')
         print("The Selected Data Set:")
         print(y)
         print('Basic Statistical Information: ')
         basic_statistic(y)
         save_data(y, "y", DATASET_OUTPUT_PATH)
         clear_output()
 
         # create training data and testing data
         print("-*-*- Data Split - Train Set and Test Set -*-*-")
-        print('Note: Normally, set 20% of the dataset aside as test set, such as 0.2')
+        print('Notice: Normally, set 20% of the dataset aside as test set, such as 0.2')
         test_ratio = float_input(default=0.2, prefix=SECTION[1], slogan="@Test Ratio: ")
         train_test_data = data_split(X, y, test_ratio)
         for key, value in train_test_data.items():
             print("-" * 25)
             print(f"The Selected Data Set: {key}")
             print(value)
             print(f'Basic Statistical Information: {key}')
```

### Comparing `geochemistrypi-0.1.0/geochemistrypi/data_mining/data/data_readiness.py` & `geochemistrypi-0.2.0/geochemistrypi/data_mining/data/data_readiness.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 import re
 import openpyxl.utils.exceptions
 from sklearn.model_selection import train_test_split
 from ..global_variable import BUILT_IN_DATASET_PATH
 import pandas as pd
 from typing import Optional, List, Tuple, Union
 
-
 # from utils.exceptions import InvalidFileError
 
 
 def read_data(file_name: Optional[str] = None, is_own_data: int = 2, prefix: Optional[str] = None,
               slogan: Optional[str] = "@File: "):
     """Read the data set."""
     if is_own_data == 1:
         while True:
             # Capture exception: The path is invalid -> doesn't exist or not xlsx format
             if os.path.exists(file_name):
                 if '.xlsx' in re.findall(r'.xlsx.*', file_name):
+                # if True:
                     data_path = file_name
                     break
                 else:
                     print("Caution: Please make sure the data is stored in xlsx format!")
             else:
                 print("Caution: The path is invalid. Please input the correct path including the"
                       " stored path and suffix!")
@@ -118,17 +118,34 @@
             print("Warning: Please follow the rules and re-enter.")
             judge = True
             sub_data_set_columns_range = input('@input: ')
         except TypeError:
             print("Warning: Please follow the rules and re-enter.")
             judge = True
             sub_data_set_columns_range = input('@input: ')
+        else:
+            data_checking = data.iloc[:, sub_data_set_columns_selected]
+            for i in data_checking.columns.values:
+                df_test = pd.DataFrame(data_checking[i])
+                test_columns = df_test.columns
+                v_value = int(df_test.isnull().sum())
+                if v_value == len(df_test):
+                    print(f"Warning: The selected column {df_test.columns.values} is an empty column!")
+                    judge = True
+                elif df_test[test_columns[0]].dtype in ['int64', 'float64']:
+                    continue
+                else:
+                    print(f"Warning: The data type of selected column {df_test.columns.values} is not numeric!"
+                          " Please make sure that the selected data type is numeric and re-enter.")
+                    judge = True
+            if judge == True:
+                sub_data_set_columns_range = input('@input: ')
         if judge == False:
             break
-          
+
     # select designated column
     sub_data_set = data.iloc[:, sub_data_set_columns_selected]
     show_data_columns(sub_data_set.columns, sub_data_set_columns_selected)
     return sub_data_set
 
 
 def data_split(X: pd.DataFrame, y: Union[pd.DataFrame, pd.Series], test_size: float = 0.2) -> dict:
@@ -236,15 +253,29 @@
             break
         else:
             print("Caution: The input is not a positive number. Please input the right number again!")
     return option
 
 
 def str_input(option_list: List[str], prefix: Optional[str] = None) -> str:
-    # TODO (Sany sanyhew1097618435@163,com): Test this function and add the docstring.
+    """Get the string of the desired option.
+    
+    Parameters
+    ----------
+    option_list : list
+        All the options provided are stored in a list.
+
+    prefix : str, default=None
+        It indicates which section the user currently is in on the UML, which is shown on the command-line console.
+    
+    Returns
+    -------
+    option: str
+        A string of the desired option.
+    """
     num2option(option_list)
     option_num = limit_num_input(option_list, prefix, num_input)
     option = option_list[option_num-1]
     return option
 
 
 def tuple_input(default: Tuple[int], prefix: Optional[str] = None, slogan: Optional[str] = None) -> Tuple[int]:
@@ -267,21 +298,22 @@
         A numeric tuple.
     """
     while True:
         option = input('Determine the architecture of the deep neural network.\n'
                        'Input format:\n'
                        'Format 1: "(**,)", such as "(100,)"\n'
                        '--> You want to set one hidden layer with 100 neurons for the deep neural network.\n'
-                       'Format 2: "(**, **)", such as "(50,25)"\n'
+                       'Format 2: "(**, **)", such as "(50, 25)"\n'
                        '--> You want to set two hidden layers in order with 50 neurons and 25 neurons respectively'
                        ' for the deep neural network.\n'
                        'Format 3: "(**, **, **)", such as "(64, 32, 8)"\n'
                        '--> You want to set three hidden layers in order 64 neurons, 32 neurons and 8 neurons'
                        ' respectively for the deep neural network.\n'
                        f"({prefix}) ➜ {slogan}").strip()
         if len(option) == 0:
              option = default
              break
         else:
              option = eval(option)
              break
     return option
+
```

### Comparing `geochemistrypi-0.1.0/geochemistrypi/data_mining/data/feature_engineering.py` & `geochemistrypi-0.2.0/geochemistrypi/data_mining/data/feature_engineering.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,20 +2,22 @@
 import string
 import operator
 import gc
 import pandas
 
 
 class Stack(object):
+    """Create a stack."""
+
     Error = -1
 
     def __init__(self, MaxSize):
-        # the size of the stack
+        # The size of the stack.
         self.MaxSize = MaxSize
-        # pointer indicates the position of the top element
+        # Pointer indicates the position of the top element.
         self.Top = -1
         self.Data = [None for _ in range(self.MaxSize)]
 
     def is_empty(self):
         return self.Top == -1
 
     def push(self, item):
@@ -48,40 +50,45 @@
         self.data = data
         self._infix_expr = []
         self._postfix_expr = []
         self.map_dict = {}
         self._result = None
 
     def index2name(self):
-        """pattern: [letter : column name], e.g. a : 1st column name; b : 2nd column name
+        """Pattern: [letter : column name], e.g. a : 1st column name; b : 2nd column name
 
         :return: index : column name, dict
         """
         columns_name = self.data.columns
         print("Selected data set:")
         for i in range(len(columns_name)):
             print(FeatureConstructor.alphabet[i] + ' - ' + columns_name[i])
             self.map_dict[FeatureConstructor.alphabet[i]] = columns_name[i]
 
     def _get_column(self, index):
         return self.data[self.map_dict[index]]
 
     def name_feature(self):
-        self.feature_name = input("Name the constructed feature (column name): \n"
+        self.feature_name = input("Name the constructed feature (column name), like 'NEW-COMPOUND': \n"
                                   "@input: ")
 
     def input_expression(self):
-        expression = input("Build up new feature with the combination of 4 basic arithmatic operator.\n"
+        expression = input("Build up new feature with the combination of 4 basic arithmatic operator,"
+                           " including '+', '-', '*', '/', '()'.\n"
                            "Input example 1: a * b - c \n"
                            "--> Step 1: Multiply a column with b column; \n"
                            "--> Step 2: Subtract c from the result of Step 1; \n"
                            "Input example 2: (d + 5 * f) / g \n"
-                           "--> Step 1: multiply 5 with f; \n"
+                           "--> Step 1: Multiply 5 with f; \n"
                            "--> Step 2: Plus d column with the result of Step 1;\n"
                            "--> Step 3: Divide the result of Step 1 by g; \n"
+                           # "Input example 3: (h ** 3) / (i ** (1/2)) \n"
+                           # "--> Step 1: Exponent calculation, h raised to the power of 3; \n"
+                           # "--> Step 2: Root calculation, find the square root of i; \n"
+                           # "--> Step 3: Divide the result of Step 1 by the result of Step 2; \n"
                            "@input: ")
         self._infix_expr = list(expression.replace(' ', ''))
 
     @staticmethod
     def _oper_priority_out(oper):
         return {
             '+': 1, '-': 1,
```

### Comparing `geochemistrypi-0.1.0/geochemistrypi/data_mining/data/preprocessing.py` & `geochemistrypi-0.2.0/geochemistrypi/data_mining/data/preprocessing.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.1.0/geochemistrypi/data_mining/data/statistic.py` & `geochemistrypi-0.2.0/geochemistrypi/data_mining/data/statistic.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.1.0/geochemistrypi/data_mining/data/dataset/Data_Classification.xlsx` & `geochemistrypi-0.2.0/geochemistrypi/data_mining/data/dataset/Data_Classification.xlsx`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.1.0/geochemistrypi/data_mining/data/dataset/Data_Clustering.xlsx` & `geochemistrypi-0.2.0/geochemistrypi/data_mining/data/dataset/Data_Clustering.xlsx`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.1.0/geochemistrypi/data_mining/data/dataset/Data_Decomposition.xlsx` & `geochemistrypi-0.2.0/geochemistrypi/data_mining/data/dataset/Data_Decomposition.xlsx`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.1.0/geochemistrypi/data_mining/data/dataset/Data_Regression.xlsx` & `geochemistrypi-0.2.0/geochemistrypi/data_mining/data/dataset/Data_Regression.xlsx`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.1.0/geochemistrypi/data_mining/model/_base.py` & `geochemistrypi-0.2.0/geochemistrypi/data_mining/model/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # -*- coding: utf-8 -*-
 import os
 import pandas as pd
 import numpy as np
 import joblib
 import pickle
-from typing import Optional
-from ..data.data_readiness import num2option, num_input, limit_num_input, create_sub_data_set, show_data_columns
-from ..global_variable import SECTION, MODEL_PATH
-from ..utils.base import save_data
+from typing import Dict, Optional
 from typing import Tuple, List, Union
 from abc import ABCMeta, abstractmethod
 from multipledispatch import dispatch
 from datetime import date
 
+from ..data.data_readiness import num2option, num_input, limit_num_input, create_sub_data_set, show_data_columns
+from ..global_variable import SECTION, MODEL_PATH
+from ..utils.base import save_data
+
 
 class WorkflowBase(metaclass=ABCMeta):
     """Base class for all workflow classes in geochemistry π."""
 
     # Default for child class. They need to be overwritten in child classes.
     name = None
     common_function = []
@@ -115,14 +116,25 @@
         """The interface for the child classes."""
         return pd.DataFrame()
 
     def transform(self, X: pd.DataFrame) -> pd.DataFrame:
         """The interface for the child classes."""
         return pd.DataFrame()
 
+    @abstractmethod
+    def manual_hyper_parameters(cls) -> Dict:
+        """Placeholder for manual_hyper_parameters. child classes should implement this method!
+
+        Parameters
+        ----------
+        kwargs : dict
+            The hyper parameters of the model.
+        """
+        return dict()
+
     @staticmethod
     def score(y_true: Union[pd.DataFrame, np.ndarray], y_predict: Union[pd.DataFrame, np.ndarray])\
             -> Union[int, float]:
         """The interface for the child classes."""
         return float()
 
     @staticmethod
```

### Comparing `geochemistrypi-0.1.0/geochemistrypi/data_mining/model/classification.py` & `geochemistrypi-0.2.0/geochemistrypi/data_mining/model/classification.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 # -*- coding: utf-8 -*-
 # import sys
 import numpy as np
 import pandas as pd
 from sklearn.svm import SVC
 from sklearn.metrics import classification_report
-from ..utils.base import save_fig
-from ..global_variable import MODEL_OUTPUT_IMAGE_PATH
 from sklearn.tree import DecisionTreeClassifier
-from sklearn.ensemble import RandomForestClassifier
-import xgboost
+from sklearn.ensemble import RandomForestClassifier, ExtraTreesClassifier
+from sklearn.neural_network import MLPClassifier
 from sklearn.linear_model import LogisticRegression
 from typing import Union, Optional, List, Dict, Callable, Tuple, Any, Sequence, Set, Literal
+import xgboost
 from multipledispatch import dispatch
 from flaml import AutoML
+
+from ..utils.base import save_fig
+from ..global_variable import MODEL_OUTPUT_IMAGE_PATH, RAY_FLAML
 from ._base import WorkflowBase
 from .func.algo_classification._common import confusion_matrix_plot, contour_data, plot_precision_recall, plot_ROC,\
     cross_validation
-from .func.algo_classification._svm import plot_2d_decision_boundary
+from .func.algo_classification._svm import plot_2d_decision_boundary, svc_manual_hyper_parameters
 from .func.algo_classification._xgboost import feature_importance_map, feature_importance_value, \
-    feature_weights_histograms
-from .func.algo_classification._decision_tree import decision_tree_plot
-from .func.algo_classification._logistic import logistic_importance_plot
-from .func.algo_classification._rf import feature_importances
-
+    feature_weights_histograms, xgboost_manual_hyper_parameters
+from .func.algo_classification._decision_tree import decision_tree_plot, decision_tree_manual_hyper_parameters
+from .func.algo_classification._logistic_regression import logistic_importance_plot, logistic_regression_manual_hyper_parameters
+from .func.algo_classification._rf import feature_importances, random_forest_manual_hyper_parameters
+from .func.algo_classification._extra_trees import extra_trees_manual_hyper_parameters
+from .func.algo_classification._deep_neural_network import deep_neural_network_manual_hyper_parameters
 
 class ClassificationWorkflowBase(WorkflowBase):
     """The base workflow class of classification algorithms."""
 
     common_function = ["Model Score", "Confusion Matrix", 'Cross Validation', 'Model Prediction', 'Model Persistence']
 
     def __init__(self) -> None:
@@ -39,62 +42,83 @@
     def fit(self, X: pd.DataFrame, y: Optional[pd.DataFrame] = None) -> None:
         """Fit the model by Scikit-learn framework."""
         self.model.fit(X, y)
 
     @dispatch(object, object, bool)
     def fit(self, X: pd.DataFrame, y: Optional[pd.DataFrame] = None, is_automl: bool = False) -> None:
         """Fit the model by FLAML framework."""
-        self.automl = AutoML()
-        if self.customized:  # When the model is not built-in in FLAML framwork
-            self.automl.add_learner(learner_name=self.customized_name, learner_class=self.customization)
-        if y.shape[1] == 1:  # FLAML's data format validation mechanism
-            y = y.squeeze()  # Convert a single dataFrame column into a series
-        self.automl.fit(X_train=X, y_train=y, **self.settings)
+        if self.naming not in RAY_FLAML:
+            self.automl = AutoML()
+            if self.customized:  # When the model is not built-in in FLAML framwork
+                self.automl.add_learner(learner_name=self.customized_name, learner_class=self.customization)
+            if y.shape[1] == 1:  # FLAML's data format validation mechanism
+                y = y.squeeze()  # Convert a single dataFrame column into a series
+            self.automl.fit(X_train=X, y_train=y, **self.settings)
+        else:
+            # When the model is not built-in in FLAML framework, use RAY + FLAML customization.
+            self.ray_tune(ClassificationWorkflowBase.X_train, ClassificationWorkflowBase.X_test,
+                          ClassificationWorkflowBase.y_train, ClassificationWorkflowBase.y_test)
+            self.ray_best_model.fit(X, y)
 
     @dispatch(object)
     def predict(self, X: pd.DataFrame) -> np.ndarray:
         """Perform classification on samples in X by Scikit-learn framework."""
         y_predict = self.model.predict(X)
         return y_predict
 
     @dispatch(object, bool)
     def predict(self, X: pd.DataFrame, is_automl: bool = False) -> np.ndarray:
         """Perform classification on samples in X by FLAML framework."""
-        y_predict = self.automl.predict(X)
-        return y_predict
+        if self.naming not in RAY_FLAML:
+            y_predict = self.automl.predict(X)
+            return y_predict
+        else:
+            y_predict = self.ray_best_model.predict(X)
+            return y_predict
 
     @property
     def settings(self) -> Dict:
         """The configuration to implement AutoML by FLAML framework."""
         return dict()
 
     @property
     def customization(self) -> object:
         """The customized model of FLAML framework."""
         return object
 
     @property
     def auto_model(self) -> object:
         """Get AutoML trained model by FLAML framework."""
-        return self.automl.model.estimator
+        if self.naming not in RAY_FLAML:
+            return self.automl.model.estimator
+        else:
+            return self.ray_best_model
+
+    @classmethod
+    def manual_hyper_parameters(cls) -> Dict:
+        """Manual hyper-parameters specification."""
+        return dict()
 
     @staticmethod
     def _score(y_true: pd.DataFrame, y_predict: pd.DataFrame) -> None:
+        """Print the classification score report of the model."""
         print("-----* Model Score *-----")
         print(classification_report(y_true, y_predict))
 
     @staticmethod
     def _cross_validation(trained_model: object, X_train: pd.DataFrame, y_train: pd.DataFrame, cv_num: int = 10) -> None:
+        """Perform cross validation on the model."""
         print("-----* Cross Validation *-----")
         print(f"K-Folds: {cv_num}")
         cross_validation(trained_model, X_train, y_train, cv_num=cv_num)
 
     @staticmethod
     def _confusion_matrix_plot(y_test: pd.DataFrame, y_test_predict: pd.DataFrame,
                                trained_model: object, algorithm_name: str, store_path: str) -> None:
+        """Plot the confusion matrix of the model."""
         print("-----* Confusion Matrix *-----")
         confusion_matrix_plot(y_test, y_test_predict, trained_model)
         save_fig(f"Confusion Matrix - {algorithm_name}", store_path)
 
     @staticmethod
     def _contour_data(X: pd.DataFrame, trained_model: Any) -> Tuple[List[np.ndarray], np.ndarray]:
         """Build up coordinate matrices as the data of contour plot."""
@@ -120,30 +144,30 @@
 class SVMClassification(ClassificationWorkflowBase):
     """The automation workflow of using SVC algorithm to make insightful products."""
 
     name = "Support Vector Machine"
     special_function = ['Two-dimensional Decision Boundary Diagram', 'Precision_Recall_Curve', 'ROC Curve']
 
     def __init__(
-            self,
-            C: float = 1.0,
-            kernel: Union[str, Callable] = 'rbf',
-            degree: int = 3,
-            gamma: Union[str, float] = "scale",
-            coef0: float = 0.0,
-            shrinking: bool = True,
-            probability: bool = False,
-            tol: float = 1e-3,
-            cache_size: float = 200,
-            class_weight: Union[dict, str, None] = None,
-            verbose: bool = False,
-            max_iter: int = -1,
-            decision_function_shape: Literal['ovo', 'ovr'] = "ovr",
-            break_ties: bool = False,
-            random_state: Optional[int] = None
+        self,
+        C: float = 1.0,
+        kernel: Union[str, Callable] = 'rbf',
+        degree: int = 3,
+        gamma: Union[str, float] = "scale",
+        coef0: float = 0.0,
+        shrinking: bool = True,
+        probability: bool = False,
+        tol: float = 1e-3,
+        cache_size: float = 200,
+        class_weight: Union[dict, str, None] = None,
+        verbose: bool = False,
+        max_iter: int = -1,
+        decision_function_shape: Literal['ovo', 'ovr'] = "ovr",
+        break_ties: bool = False,
+        random_state: Optional[int] = None
     ) -> None:
         """
         Parameters
         ----------
         C : float, default=1.0
             Regularization parameter. The strength of the regularization is
             inversely proportional to C. Must be strictly positive. The penalty
@@ -237,15 +261,15 @@
             Controls the pseudo random number generation for shuffling the data for
             probability estimates. Ignored when `probability` is False.
             Pass an int for reproducible output across multiple function calls.
             See :term:`Glossary <random_state>`.
 
         References
         ----------
-        scikit API: sklearn.svm.SVC
+        Scikit-learn API: sklearn.svm.SVC
         https://scikit-learn.org/stable/modules/generated/sklearn.svm.SVC.html
         """
 
         super().__init__()
         self.C = C
         self.kernel = kernel
         self.degree = degree
@@ -257,29 +281,32 @@
         self.cache_size = cache_size
         self.class_weight = class_weight
         self.verbose = verbose
         self.max_iter = max_iter
         self.decision_function_shape = decision_function_shape
         self.break_ties = break_ties
 
-        self.model = SVC(C=self.C,
-                         kernel=self.kernel,
-                         degree=self.degree,
-                         gamma=self.gamma,
-                         coef0=self.coef0,
-                         shrinking=self.shrinking,
-                         probability=self.probability,
-                         tol=self.tol,
-                         cache_size=self.cache_size,
-                         class_weight=self.class_weight,
-                         verbose=self.verbose,
-                         max_iter=self.max_iter,
-                         decision_function_shape=self.decision_function_shape,
-                         break_ties=self.break_ties,
-                         random_state=self.random_state)
+        self.model = SVC(
+            C=self.C,
+            kernel=self.kernel,
+            degree=self.degree,
+            gamma=self.gamma,
+            coef0=self.coef0,
+            shrinking=self.shrinking,
+            probability=self.probability,
+            tol=self.tol,
+            cache_size=self.cache_size,
+            class_weight=self.class_weight,
+            verbose=self.verbose,
+            max_iter=self.max_iter,
+            decision_function_shape=self.decision_function_shape,
+            break_ties=self.break_ties,
+            random_state=self.random_state
+        )
+        
         self.naming = SVMClassification.name
         self.customized = True
         self.customized_name = 'SVC'
 
     @property
     def settings(self) -> Dict:
         """The configuration of SVC to implement AutoML by FLAML framework."""
@@ -306,22 +333,48 @@
                 super().__init__(task, **config)
                 if task in CLASSIFICATION:
                     self.estimator_class = SVC
 
             @classmethod
             def search_space(cls, data_size, task):
                 space = {
-                    'C': {'domain': tune.uniform(lower=1, upper=data_size[0]),
-                          'init_value': 1,
-                          'low_cost_init_value': 1}
+                    'C': {
+                        'domain': tune.uniform(lower=1, upper=data_size[0]),
+                        'init_value': 1,
+                        'low_cost_init_value': 1
+                    },
+                    'kernel': {'domain': tune.choice(['poly', 'rbf', 'sigmoid'])},
+                    'gamma': {
+                        'domain': tune.uniform(lower=1e-5, upper=10),
+                        'init_value': 1e-1,
+                        'low_cost_init_value': 1e-1
+                    },
+                    'degree': {
+                        'domain': tune.quniform(lower=1, upper=5, q=1),
+                        'init_value': 3,
+                        'low_cost_init_value': 3
+                    },
+                    'coef0': {
+                        'domain': tune.uniform(lower=0, upper=1),
+                        'init_value': 0,
+                        'low_cost_init_value': 0
+                    },
+                    'shrinking': {'domain': tune.choice([True, False])},
                 }
                 return space
 
         return MySVMClassification
 
+    @classmethod
+    def manual_hyper_parameters(cls) -> Dict:
+        """Manual hyper-parameters specification."""
+        print(f"-*-*- {cls.name} - Hyper-parameters Specification -*-*-")
+        hyper_parameters = svc_manual_hyper_parameters()
+        return hyper_parameters
+
     @staticmethod
     def _plot_2d_decision_boundary(X: pd.DataFrame, X_test: pd.DataFrame, y_test: pd.DataFrame, trained_model: Any,
                                    image_config: dict, algorithm_name: str, store_path: str,
                                    contour_data: Optional[List[np.ndarray]] = None,
                                    labels: Optional[np.ndarray] = None) -> None:
         """Plot the decision boundary of the trained model with the testing data set below."""
         print("-----* Two-dimensional Decision Boundary Diagram *-----")
@@ -370,33 +423,33 @@
                        self.auto_model, self.naming, MODEL_OUTPUT_IMAGE_PATH)
         if SVMClassification.X.shape[1] == 2:
             self._plot_2d_decision_boundary(SVMClassification.X, SVMClassification.X_test, SVMClassification.y_test,
                                             self.auto_model, self.image_config, self.naming, MODEL_OUTPUT_IMAGE_PATH)
 
 
 class DecisionTreeClassification(ClassificationWorkflowBase):
-    """A decision tree classifier"""
+    """The automation workflow of using Decision Tree algorithm to make insightful products."""
 
     name = "Decision Tree"
     special_function = ["Decision Tree Plot"]
 
     def __init__(
-            self,
-            criterion: str = 'gini',
-            splitter: str = 'best',
-            max_depth: Optional[int] = 3,
-            min_samples_split: Union[int, float] = 2,
-            min_samples_leaf: Union[int, float] = 1,
-            min_weight_fraction_leaf: float = 0.0,
-            max_features: Union[int, float, str, None] = None,
-            random_state: Optional[int] = None,
-            max_leaf_nodes: Optional[int] = None,
-            min_impurity_decrease: float = 0.0,
-            class_weight: Union[dict, list[dict], str, None] = None,
-            ccp_alpha: float = 0.0
+        self,
+        criterion: str = 'gini',
+        splitter: str = 'best',
+        max_depth: Optional[int] = 3,
+        min_samples_split: Union[int, float] = 2,
+        min_samples_leaf: Union[int, float] = 1,
+        min_weight_fraction_leaf: float = 0.0,
+        max_features: Union[int, float, str, None] = None,
+        random_state: Optional[int] = None,
+        max_leaf_nodes: Optional[int] = None,
+        min_impurity_decrease: float = 0.0,
+        class_weight: Union[dict, List[dict], str, None] = None,
+        ccp_alpha: float = 0.0
     ) -> None:
         """
         Parameters
         ----------
         criterion : {"gini", "entropy"}, default="gini"
             The function to measure the quality of a split. Supported criteria are
             "gini" for the Gini impurity and "entropy" for the information gain.
@@ -520,42 +573,104 @@
             ``ccp_alpha`` will be chosen. By default, no pruning is performed. See
             :ref:`minimal_cost_complexity_pruning` for details.
 
             .. versionadded:: 0.22
 
         References
         ----------
-        sklearn.tree.DecisionTreeClassifier
+        Scikit-learn API: sklearn.tree.DecisionTreeClassifier
         https://scikit-learn.org/stable/modules/generated/sklearn.tree.DecisionTreeClassifier.html?highlight=decisiontreeclassifier#sklearn.tree.DecisionTreeClassifier
         """
+
         super().__init__()
         self.criterion = criterion
         self.splitter = splitter
         self.max_depth = max_depth
         self.min_samples_split = min_samples_split
         self.min_samples_leaf = min_samples_leaf
         self.min_weight_fraction_leaf = min_weight_fraction_leaf
         self.max_features = max_features
         self.max_leaf_nodes = max_leaf_nodes
         self.min_impurity_decrease = min_impurity_decrease
         self.class_weight = class_weight
         self.ccp_alpha = ccp_alpha
-        self.model = DecisionTreeClassifier(criterion=self.criterion,
-                                            splitter=self.splitter,
-                                            max_depth=self.max_depth,
-                                            min_samples_split=self.min_samples_split,
-                                            min_samples_leaf=self.min_samples_leaf,
-                                            min_weight_fraction_leaf=self.min_weight_fraction_leaf,
-                                            max_features=self.max_features,
-                                            random_state=self.random_state,
-                                            max_leaf_nodes=self.max_leaf_nodes,
-                                            min_impurity_decrease=self.min_impurity_decrease,
-                                            class_weight=self.class_weight,
-                                            ccp_alpha=self.ccp_alpha)
+
+        self.model = DecisionTreeClassifier(
+            criterion=self.criterion,
+            splitter=self.splitter,
+            max_depth=self.max_depth,
+            min_samples_split=self.min_samples_split,
+            min_samples_leaf=self.min_samples_leaf,
+            min_weight_fraction_leaf=self.min_weight_fraction_leaf,
+            max_features=self.max_features,
+            random_state=self.random_state,
+            max_leaf_nodes=self.max_leaf_nodes,
+            min_impurity_decrease=self.min_impurity_decrease,
+            class_weight=self.class_weight,
+            ccp_alpha=self.ccp_alpha
+        )
+
         self.naming = DecisionTreeClassification.name
+        self.customized = True
+        self.customized_name = 'Decision Tree'
+
+    @property
+    def settings(self) -> Dict:
+        """The configuration of Decision Tree to implement AutoML by FLAML framework."""
+        configuration = {
+            "time_budget": 10,  # total running time in seconds
+            "metric": 'accuracy',
+            "estimator_list": [self.customized_name],  # list of ML learners
+            "task": 'classification',  # task type
+            # "log_file_name": f'{self.naming} - automl.log',  # flaml log file
+            # "log_training_metric": True,  # whether to log training metric
+        }
+        return configuration
+    
+    @property
+    def customization(self) -> object:
+        """The customized Decision Tree of FLAML framework."""
+        from flaml.model import SKLearnEstimator
+        from flaml import tune
+        from flaml.data import CLASSIFICATION
+        from sklearn.tree import DecisionTreeClassifier
+
+        class MyDTClassification(SKLearnEstimator):
+            def __init__(self, task='binary', n_jobs=None, **config):
+                super().__init__(task, **config)
+                if task in CLASSIFICATION:
+                    self.estimator_class = DecisionTreeClassifier
+
+            @classmethod
+            def search_space(cls, data_size, task):
+                space = {
+                    'criterion': {'domain': tune.choice(['gini', 'entropy', 'log_loss'])},
+                    'max_depth': {'domain': tune.randint(lower=2, upper=20),
+                                  'init_value': 1,
+                                  'low_cost_init_value': 1},
+                    'min_samples_split': {'domain': tune.randint(lower=2, upper=10),
+                                          'init_value': 2,
+                                          'low_cost_init_value': 2},
+                    'min_samples_leaf': {'domain': tune.randint(lower=1, upper=10),
+                                         'init_value': 1,
+                                         'low_cost_init_value': 1},
+                    'max_features': {'domain': tune.randint(lower=1, upper=10),
+                                     'init_value': 1,
+                                     'low_cost_init_value': 1},
+                }
+                return space
+
+        return MyDTClassification
+
+    @classmethod
+    def manual_hyper_parameters(cls) -> Dict:
+        """Manual hyper-parameters specification."""
+        print(f"-*-*- {cls.name} - Hyper-parameters Specification -*-*-")
+        hyper_parameters = decision_tree_manual_hyper_parameters()
+        return hyper_parameters
 
     def plot_tree_function(self, trained_model: object, image_config: dict, algorithm_name: str, store_path: str) -> None:
         """Drawing decision tree diagrams."""
         print("-----* Decision Tree Plot *-----")
         decision_tree_plot(trained_model, image_config)
         save_fig(f"Classification - {algorithm_name} - Tree Graph", store_path)
 
@@ -565,48 +680,59 @@
                                    contour_data: Optional[List[np.ndarray]] = None,
                                    labels: Optional[np.ndarray] = None) -> None:
         """Plot the decision boundary of the trained model with the testing data set below."""
         print("-----* Two-dimensional Decision Boundary Diagram *-----")
         plot_2d_decision_boundary(X, X_test, y_test, trained_model, image_config, algorithm_name)
         save_fig(f'Classification - {algorithm_name} - Decision Boundary', store_path)
 
+    @dispatch()
     def special_components(self, **kwargs) -> None:
+        """Invoke all special application functions for this algorithms by Scikit-learn framework."""
         self.plot_tree_function(self.model, self.image_config, self.naming, MODEL_OUTPUT_IMAGE_PATH)
         if DecisionTreeClassification.X.shape[1] == 2:
             self._plot_2d_decision_boundary(DecisionTreeClassification.X, DecisionTreeClassification.X_test,
                                               DecisionTreeClassification.y_test,
                                               self.model, self.image_config, self.naming, MODEL_OUTPUT_IMAGE_PATH)
 
+    @dispatch(bool)
+    def special_components(self, is_automl: bool, **kwargs) -> None:
+        """Invoke all special application functions for this algorithms by FLAML framework."""
+        self.plot_tree_function(self.auto_model, self.image_config, self.naming, MODEL_OUTPUT_IMAGE_PATH)
+        if DecisionTreeClassification.X.shape[1] == 2:
+            self._plot_2d_decision_boundary(DecisionTreeClassification.X, DecisionTreeClassification.X_test,
+                                              DecisionTreeClassification.y_test,
+                                              self.auto_model, self.image_config, self.naming, MODEL_OUTPUT_IMAGE_PATH)
+
 
 class RandomForestClassification(ClassificationWorkflowBase):
     """The automation workflow of using Random Forest algorithm to make insightful products."""
 
     name = "Random Forest"
     special_function = ['Feature Importance', "Random Forest's Tree Plot", "Drawing Decision Surfaces Plot"]
 
     def __init__(
-            self,
-            n_estimators: int = 100,
-            criterion: str = 'gini',
-            max_depth: Optional[int] = 4,
-            min_samples_split: Union[int, float] = 4,
-            min_samples_leaf: Union[int, float] = 1,
-            min_weight_fraction_leaf: float = 0.0,
-            max_features: Union[str, int, float] = 'sqrt',
-            max_leaf_nodes: Optional[int] = 3,
-            min_impurity_decrease: float = 0.0,
-            bootstrap: bool = True,
-            oob_score: bool = False,
-            n_jobs: Optional[int] = -1,
-            random_state: Optional[int] = 42,
-            verbose: int = 0,
-            warm_start: bool = False,
-            class_weight: Union[str, dict, list[dict], None] = None,
-            ccp_alpha: float = 0.0,
-            max_samples: Union[int, float] = 10
+        self,
+        n_estimators: int = 100,
+        criterion: str = 'gini',
+        max_depth: Optional[int] = 4,
+        min_samples_split: Union[int, float] = 4,
+        min_samples_leaf: Union[int, float] = 1,
+        min_weight_fraction_leaf: float = 0.0,
+        max_features: Union[str, int, float] = 'sqrt',
+        max_leaf_nodes: Optional[int] = 3,
+        min_impurity_decrease: float = 0.0,
+        bootstrap: bool = True,
+        oob_score: bool = False,
+        n_jobs: Optional[int] = -1,
+        random_state: Optional[int] = 42,
+        verbose: int = 0,
+        warm_start: bool = False,
+        class_weight: Union[str, dict, list[dict], None] = None,
+        ccp_alpha: float = 0.0,
+        max_samples: Union[int, float] = 10
     ) -> None:
         """
         A random forest classifier.
 
         A random forest is a meta estimator that fits a number of decision tree
         classifiers on various sub-samples of the dataset and uses averaging to
         improve the predictive accuracy and control over-fitting.
@@ -778,17 +904,18 @@
             - If float, then draw `max_samples * X.shape[0]` samples. Thus,
               `max_samples` should be in the interval `(0.0, 1.0]`.
 
             .. versionadded:: 0.22
 
         References
         ----------
-        scikit API: sklearn.ensemble.RandomForestClassifier
+        Scikit-learn API: sklearn.ensemble.RandomForestClassifier
         https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html?highlight=randomforestclassifier#sklearn.ensemble.RandomForestClassifier
         """
+
         super().__init__()
         self.n_estimators = n_estimators
         self.criterion = criterion
         self.max_depth = max_depth
         self.min_samples_split = min_samples_split
         self.min_samples_leaf = min_samples_leaf
         self.min_weight_fraction_leaf = min_weight_fraction_leaf
@@ -800,32 +927,36 @@
         self.n_jobs = n_jobs
         self.random_state = random_state
         self.verbose = verbose
         self.warm_start = warm_start
         self.class_weight = class_weight
         self.ccp_alpha = ccp_alpha
         self.max_samples = max_samples
-        self.model = RandomForestClassifier(n_estimators=self.n_estimators,
-                                            criterion=self.criterion,
-                                            max_depth=self.max_depth,
-                                            min_samples_split=self.min_samples_split,
-                                            min_samples_leaf=self.min_samples_leaf,
-                                            min_weight_fraction_leaf=self.min_weight_fraction_leaf,
-                                            max_features=self.max_features,
-                                            max_leaf_nodes=self.max_leaf_nodes,
-                                            min_impurity_decrease=self.min_impurity_decrease,
-                                            bootstrap=self.bootstrap,
-                                            oob_score=self.oob_score,
-                                            n_jobs=self.n_jobs,
-                                            random_state=self.random_state,
-                                            verbose=self.verbose,
-                                            warm_start=self.warm_start,
-                                            class_weight=self.class_weight,
-                                            ccp_alpha=self.ccp_alpha,
-                                            max_samples=self.max_samples)
+        
+        self.model = RandomForestClassifier(
+            n_estimators=self.n_estimators,
+            criterion=self.criterion,
+            max_depth=self.max_depth,
+            min_samples_split=self.min_samples_split,
+            min_samples_leaf=self.min_samples_leaf,
+            min_weight_fraction_leaf=self.min_weight_fraction_leaf,
+            max_features=self.max_features,
+            max_leaf_nodes=self.max_leaf_nodes,
+            min_impurity_decrease=self.min_impurity_decrease,
+            bootstrap=self.bootstrap,
+            oob_score=self.oob_score,
+            n_jobs=self.n_jobs,
+            random_state=self.random_state,
+            verbose=self.verbose,
+            warm_start=self.warm_start,
+            class_weight=self.class_weight,
+            ccp_alpha=self.ccp_alpha,
+            max_samples=self.max_samples
+        )
+
         self.naming = RandomForestClassification.name
 
     @property
     def settings(self) -> Dict:
         """The configuration to implement AutoML by FLAML framework."""
         configuration = {
             "time_budget": 10,  # total running time in seconds
@@ -833,14 +964,21 @@
             "estimator_list": ['rf'],  # list of ML learners
             "task": 'classification',  # task type
             # "log_file_name": f'{self.naming} - automl.log',  # flaml log file
             # "log_training_metric": True,  # whether to log training metric
         }
         return configuration
 
+    @classmethod
+    def manual_hyper_parameters(cls) -> Dict:
+        """Manual hyper-parameters specification."""
+        print(f"-*-*- {cls.name} - Hyper-parameters Specification -*-*-")
+        hyper_parameters = random_forest_manual_hyper_parameters()
+        return hyper_parameters
+
     @staticmethod
     def _feature_importances(X_train: pd.DataFrame, trained_model: object, algorithm_name: str,
                              store_path: str) -> None:
         """Draw the feature importance bar diagram."""
         print("-----* Feature Importance *-----")
         feature_importances(X_train, trained_model)
         save_fig(f"Feature Importance - {algorithm_name}", store_path)
@@ -891,51 +1029,218 @@
             str, Callable[[np.ndarray, np.ndarray], Tuple[np.ndarray, np.ndarray]]
         ]
     ]
     name = "Xgboost"
     special_function = ['Feature Importance']
 
     def __init__(
-            self,
-            n_estimators: int = 100,
-            max_depth: Optional[int] = None,
-            max_leaves: Optional[int] = None,
-            max_bin: Optional[int] = None,
-            grow_policy=1,
-            learning_rate: Optional[float] = None,
-            verbosity: Optional[int] = None,
-            objective: _SklObjective = None,
-            booster: Optional[str] = None,
-            tree_method: Optional[str] = None,
-            n_jobs: Optional[int] = None,
-            gamma: Optional[float] = None,
-            min_child_weight: Optional[float] = None,
-            max_delta_step: Optional[float] = None,
-            subsample: Optional[float] = None,
-            colsample_bytree: Optional[float] = None,
-            colsample_bylevel: Optional[float] = None,
-            colsample_bynode: Optional[float] = None,
-            reg_alpha: Optional[float] = None,
-            reg_lambda: Optional[float] = None,
-            scale_pos_weight: Optional[float] = None,
-            base_score: Optional[float] = None,
-            random_state: Optional[Union[np.random.RandomState, int]] = None,
-            missing: float = np.nan,
-            num_parallel_tree: Optional[int] = None,
-            monotone_constraints: Optional[Union[Dict[str, int], str]] = None,
-            interaction_constraints: Optional[Union[str, Sequence[Sequence[str]]]] = None,
-            importance_type: Optional[str] = 'weight',
-            gpu_id: Optional[int] = None,
-            validate_parameters: Optional[bool] = None,
-            predictor: Optional[str] = None,
-            # enable_categorical: bool = False,
-            eval_metric: Optional[Union[str, List[str], Callable]] = None,
-            early_stopping_rounds: Optional[int] = None,
-            **kwargs: Any
+        self,
+        n_estimators: int = 100,
+        max_depth: Optional[int] = None,
+        max_leaves: Optional[int] = None,
+        max_bin: Optional[int] = None,
+        grow_policy=1,
+        learning_rate: Optional[float] = None,
+        verbosity: Optional[int] = None,
+        objective: _SklObjective = None,
+        booster: Optional[str] = None,
+        tree_method: Optional[str] = None,
+        n_jobs: Optional[int] = None,
+        gamma: Optional[float] = None,
+        min_child_weight: Optional[float] = None,
+        max_delta_step: Optional[float] = None,
+        subsample: Optional[float] = None,
+        colsample_bytree: Optional[float] = None,
+        colsample_bylevel: Optional[float] = None,
+        colsample_bynode: Optional[float] = None,
+        reg_alpha: Optional[float] = None,
+        reg_lambda: Optional[float] = None,
+        scale_pos_weight: Optional[float] = None,
+        base_score: Optional[float] = None,
+        random_state: Optional[Union[np.random.RandomState, int]] = None,
+        missing: float = np.nan,
+        num_parallel_tree: Optional[int] = None,
+        monotone_constraints: Optional[Union[Dict[str, int], str]] = None,
+        interaction_constraints: Optional[Union[str, Sequence[Sequence[str]]]] = None,
+        importance_type: Optional[str] = 'weight',
+        gpu_id: Optional[int] = None,
+        validate_parameters: Optional[bool] = None,
+        predictor: Optional[str] = None,
+        # enable_categorical: bool = False,
+        eval_metric: Optional[Union[str, List[str], Callable]] = None,
+        early_stopping_rounds: Optional[int] = None,
+        **kwargs: Any
     ):
+        """
+        Parameters
+        ----------
+        max_depth [default=6]
+            Maximum depth of a tree. Increasing this value will make the model more complex and more likely to overfit.
+            0 indicates no limit on depth. Beware that XGBoost aggressively consumes memory when training a deep tree.
+            exact tree method requires non-zero value.
+            range: [0,∞]
+
+        learning_rate [default=0.3]
+            Step size shrinkage used in update to prevents overfitting.
+            After each boosting step, we can directly get the weights of new features,
+            and eta shrinks the feature weights to make the boosting process more conservative.
+            range: [0,1]
+
+        n_estimators : int
+        Number of gradient boosted trees.  Equivalent to number of boosting rounds.
+
+        objective : {SklObjective}
+            Specify the learning task and the corresponding learning objective or
+            a custom objective function to be used (see note below).
+
+        verbosity [default=1]
+            Verbosity of printing messages. Valid values are 0 (silent), 1 (warning), 2 (info), 3 (debug).
+            Sometimes XGBoost tries to change configurations based on heuristics,
+            which is displayed as warning message.
+            If there’s unexpected behaviour, please try to increase value of verbosity.
+
+        booster [default= gbtree ]
+            Which booster to use. Can be gbtree, gblinear or dart;
+            gbtree and dart use tree based models while gblinear uses linear functions.
+
+        tree_method string [default= auto]
+            The tree construction algorithm used in XGBoost. See description in the reference paper and Tree Methods.
+            XGBoost supports approx, hist and gpu_hist for distributed training. Experimental support for external memory is available for approx and gpu_hist.
+            Choices: auto, exact, approx, hist, gpu_hist, this is a combination of commonly used updaters. For other updaters like refresh, set the parameter updater directly.
+                auto: Use heuristic to choose the fastest method.
+                    For small dataset, exact greedy (exact) will be used.
+                    For larger dataset, approximate algorithm (approx) will be chosen. It’s recommended to try hist and gpu_hist for higher performance with large dataset. (gpu_hist)has support for external memory.
+                    Because old behavior is always use exact greedy in single machine, user will get a message when approximate algorithm is chosen to notify this choice.
+                exact: Exact greedy algorithm. Enumerates all split candidates.
+                approx: Approximate greedy algorithm using quantile sketch and gradient histogram.
+                hist: Faster histogram optimized approximate greedy algorithm.
+                gpu_hist: GPU implementation of hist algorithm.
+
+        n_jobs : Optional[int]
+            Number of parallel threads used to run xgboost.  When used with other
+            Scikit-Learn algorithms like grid search, you may choose which algorithm to
+            parallelize and balance the threads.  Creating thread contention will
+            significantly slow down both algorithms.
+
+        gamma [default=0, alias: min_split_loss]
+            Minimum loss reduction required to make a further partition on a leaf node of the tree.
+            The larger gamma is, the more conservative the algorithm will be.
+            range: [0,∞]
+
+        min_child_weight [default=1]
+            Minimum sum of instance weight (hessian) needed in a child.
+            If the tree partition step results in a leaf node with the sum of instance weight less than min_child_weight,
+            then the building process will give up further partitioning. In linear regression task,
+            this simply corresponds to minimum number of instances needed to be in each node.
+            The larger min_child_weight is, the more conservative the algorithm will be.
+            range: [0,∞]
+
+        max_delta_step [default=0]
+            Maximum delta step we allow each leaf output to be.
+            If the value is set to 0, it means there is no constraint.
+            If it is set to a positive value, it can help making the update step more conservative.
+            Usually this parameter is not needed, but it might help in logistic regression
+            when class is extremely imbalanced. Set it to value of 1-10 might help control the update.
+            range: [0,∞]
+
+        subsample [default=1]
+            Subsample ratio of the training instances.
+            Setting it to 0.5 means that XGBoost would randomly sample half of the training data prior to growing trees.
+            and this will prevent overfitting.
+            Subsampling will occur once in every boosting iteration.
+            range: (0,1]
+
+        colsample_bytree [default=1]
+            colsample_bytree is the subsample ratio of columns when constructing each tree.
+            Subsampling occurs once for every tree constructed.
+
+        colsample_bylevel [default=1]
+            colsample_bylevel is the subsample ratio of columns for each level.
+            Subsampling occurs once for every new depth level reached in a tree.
+            Columns are subsampled from the set of columns chosen for the current tree.
+
+        colsample_bynode [default=1]
+            colsample_bynode is the subsample ratio of columns for each node (split).
+            Subsampling occurs once every time a new split is evaluated.
+            Columns are subsampled from the set of columns chosen for the current level.
+
+        reg_alpha [default=0]
+            L1 regularization term on weights.
+            Increasing this value will make model more conservative.
+
+        reg_lambda [default=1, alias: reg_lambda]
+            L2 regularization term on weights.
+            Increasing this value will make model more conservative.
+
+        scale_pos_weight [default=1]
+            Control the balance of positive and negative weights, useful for unbalanced classes.
+
+        predictor, [default= auto]
+            The type of predictor algorithm to use.
+            Provides the same results but allows the use of GPU or CPU.
+                auto: Configure predictor based on heuristics.
+                cpu_predictor: Multicore CPU prediction algorithm.
+                gpu_predictor: Prediction using GPU. Used when tree_method is gpu_hist.
+                    When predictor is set to default value auto, the gpu_hist tree method is able to provide GPU based prediction
+                    without copying training data to GPU memory. If gpu_predictor is explicitly specified,
+                    then all data is copied into GPU, only recommended for performing prediction tasks.
+
+        base_score : Optional[float]
+            The initial prediction score of all instances, global bias.
+
+        random_state : Optional[Union[numpy.random.RandomState, int]]
+            Random number seed.
+            .. note::
+
+               Using gblinear booster with shotgun updater is nondeterministic as
+               it uses Hogwild algorithm.
+
+        missing : float, default np.nan
+        Value in the data which needs to be present as a missing value.
+
+        num_parallel_tree: Optional[int]
+            Used for boosting random forest.
+
+        monotone_constraints : Optional[Union[Dict[str, int], str]]
+            Constraint of variable monotonicity.  See :doc:`tutorial </tutorials/monotonic>`
+            for more information.
+
+        interaction_constraints : Optional[Union[str, List[Tuple[str]]]]
+            Constraints for interaction representing permitted interactions.  The
+            constraints must be specified in the form of a nested list, e.g. ``[[0, 1], [2,
+            3, 4]]``, where each inner list is a group of indices of features that are
+            allowed to interact with each other.  See :doc:`tutorial
+            </tutorials/feature_interaction_constraint>` for more information
+
+        importance_type: Optional[str]
+            The feature importance type for the feature_importances\\_ property:
+
+            * For tree model, it's either "gain", "weight", "cover", "total_gain" or
+              "total_cover".
+            * For linear model, only "weight" is defined and it's the normalized coefficients
+              without bias.
+
+        gpu_id : Optional[int]
+            Device ordinal.
+
+        validate_parameters : Optional[bool]
+            Give warnings for unknown parameter.
+
+        eval_metric : Optional[Union[str, List[str], Callable]]
+
+        early_stopping_rounds : Optional[int]
+
+        References
+        ----------
+        [1] Xgboost Python API Reference - Scikit-Learn API
+            https://xgboost.readthedocs.io/en/latest/python/python_api.html#module-xgboost.sklearn
+
+        [2] Xgboost API for the scikit-learn wrapper:
+            https://github.com/dmlc/xgboost/blob/master/python-package/xgboost/sklearn.py
+        """
         super().__init__()
         self.n_estimators = n_estimators
         self.learning_rate = learning_rate
         self.objective = objective
         self.max_depth = max_depth
         self.max_leaves = max_leaves
         self.max_bin = max_bin
@@ -1001,14 +1306,15 @@
             gpu_id=self.gpu_id,
             validate_parameters=self.validate_parameters,
             predictor=self.predictor,
             # enable_categorical=self.enable_categorical,
             eval_metric=self.eval_metric,
             early_stopping_rounds=self.early_stopping_rounds,
         )
+
         self.naming = XgboostClassification.name
 
     @property
     def settings(self) -> Dict:
         """The configuration to implement AutoML by FLAML framework."""
         configuration = {
             "time_budget": 10,  # total running time in seconds
@@ -1016,17 +1322,25 @@
             "estimator_list": ['xgboost'],  # list of ML learners
             "task": 'classification',  # task type
             # "log_file_name": f'{self.naming} - automl.log',  # flaml log file
             # "log_training_metric": True,  # whether to log training metric
         }
         return configuration
 
+    @classmethod
+    def manual_hyper_parameters(cls) -> Dict:
+        """Manual hyper-parameters specification."""
+        print(f"-*-*- {cls.name} - Hyper-parameters Specification -*-*-")
+        hyper_parameters = xgboost_manual_hyper_parameters()
+        return hyper_parameters
+
     @staticmethod
     def _feature_importance_series(data: pd.DataFrame, trained_model: any, algorithm_name: str, image_config: dict,
                                    store_path: str) -> None:
+        """Plot feature importance series."""
         print("-----* Feature Importance *-----")
         feature_importance_value(data, trained_model)
         feature_weights_histograms(trained_model, image_config, algorithm_name)
         save_fig(f"Classification - {algorithm_name} - Feature Weights Histograms Plot", store_path)
         feature_importance_map(trained_model, image_config,algorithm_name)
         save_fig(f"Classification - {algorithm_name} - Feature Importance Map Plot", store_path)
 
@@ -1059,30 +1373,30 @@
 class LogisticRegressionClassification(ClassificationWorkflowBase):
     """The automation workflow of using Logistic Regression algorithm to make insightful products."""
 
     name = "Logistic Regression"
     special_function = ['Feature Importance', 'Precision_Recall_Curve', 'ROC Curve']
 
     def __init__(
-            self,
-            penalty: str = 'l2',
-            dual: bool = False,
-            tol: float = 0.0001,
-            C: float = 1.0,
-            fit_intercept: bool = True,
-            intercept_scaling: float = 1,
-            class_weight: Optional[Union[Dict, str]] = None,
-            random_state: Optional[int] = None,
-            solver: str = 'lbfgs',
-            max_iter: int = 100,
-            multi_class: str = 'auto',
-            verbose: int = 0,
-            warm_start: bool = False,
-            n_jobs: int = None,
-            l1_ratio: float = None
+        self,
+        penalty: str = 'l2',
+        dual: bool = False,
+        tol: float = 0.0001,
+        C: float = 1.0,
+        fit_intercept: bool = True,
+        intercept_scaling: float = 1,
+        class_weight: Optional[Union[Dict, str]] = None,
+        random_state: Optional[int] = None,
+        solver: str = 'lbfgs',
+        max_iter: int = 100,
+        multi_class: str = 'auto',
+        verbose: int = 0,
+        warm_start: bool = False,
+        n_jobs: int = None,
+        l1_ratio: float = None
     ) -> None:
         """
         Parameters
         ----------
         penalty : {'l1', 'l2', 'elasticnet', 'none'}, default='l2'
             Specify the norm of the penalty:
 
@@ -1222,15 +1536,15 @@
             used if ``penalty='elasticnet'``. Setting ``l1_ratio=0`` is equivalent
             to using ``penalty='l2'``, while setting ``l1_ratio=1`` is equivalent
             to using ``penalty='l1'``. For ``0 < l1_ratio <1``, the penalty is a
             combination of L1 and L2.
 
         References
         ----------
-        scikit API: sklearn.linear_model.LogisticRegression
+        Scikit-learn API: sklearn.linear_model.LogisticRegression
         https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LogisticRegression.html
         """
         super().__init__()
         self.penalty = penalty
         self.dual = dual
         self.tol = tol
         self.C = C
@@ -1277,31 +1591,40 @@
             "estimator_list": ['lrl2'],  # list of ML learners
             "task": 'classification',  # task type
             # "log_file_name": f'{self.naming} - automl.log',  # flaml log file
             # "log_training_metric": True,  # whether to log training metric
         }
         return configuration
 
+    @classmethod
+    def manual_hyper_parameters(cls) -> Dict:
+        """Manual hyper-parameters specification."""
+        print(f"-*-*- {cls.name} - Hyper-parameters Specification -*-*-")
+        hyper_parameters = logistic_regression_manual_hyper_parameters()
+        return hyper_parameters
+
     @staticmethod
     def _feature_importance(data: pd.DataFrame, trained_model: any, algorithm_name: str, store_path: str) -> None:
         """Print the feature coefficient value orderly."""
         print("-----* Feature Importance *-----")
         logistic_importance_plot(data, trained_model, algorithm_name)
         save_fig("LogisticRegression_feature_importance", store_path)
 
     @staticmethod
     def _plot_precision_recall(X_train: pd.DataFrame, y_train: pd.DataFrame,
                                trained_model: object, algorithm_name: str, store_path: str) -> None:
+        """Plot the precision-recall curve."""
         print("-----* Precision and Recall Versus the Decision Threshold *-----")
         plot_precision_recall(X_train, y_train, trained_model, algorithm_name)
         save_fig(f'Precision_Recall_Curve - {algorithm_name}', store_path)
 
     @staticmethod
     def _plot_ROC(X_train: pd.DataFrame, y_train: pd.DataFrame,
                   trained_model: object, algorithm_name: str, store_path: str) -> None:
+        """Plot the ROC curve."""
         print("-----* ROC Curve *-----")
         plot_ROC(X_train, y_train, trained_model, algorithm_name)
         save_fig(f'ROC_Curve - {algorithm_name}', store_path)
 
     @dispatch()
     def special_components(self, **kwargs) -> None:
         """Invoke all special application functions for this algorithms by Scikit-learn framework."""
@@ -1314,8 +1637,592 @@
     @dispatch(bool)
     def special_components(self, is_automl: bool = False, **kwargs) -> None:
         """Invoke all special application functions for this algorithms by FLAML framework."""
         self._feature_importance(LogisticRegressionClassification.X, self.auto_model, self.naming, MODEL_OUTPUT_IMAGE_PATH)
         self._plot_precision_recall(LogisticRegressionClassification.X_train, LogisticRegressionClassification.y_train,
                                     self.auto_model, self.naming, MODEL_OUTPUT_IMAGE_PATH)
         self._plot_ROC(LogisticRegressionClassification.X_train, LogisticRegressionClassification.y_train,
-                       self.auto_model, self.naming, MODEL_OUTPUT_IMAGE_PATH)
+                       self.auto_model, self.naming, MODEL_OUTPUT_IMAGE_PATH)
+        
+
+class DNNClassification(ClassificationWorkflowBase):
+    """The automation workflow of using Deep Neural Network algorithm to make insightful products."""
+
+    name = "Deep Neural Network"
+    special_function = []
+
+    def __init__(
+        self,
+        hidden_layer_sizes: tuple = (100,),
+        activation: str = "relu",
+        *,
+        solver: str = "adam",
+        alpha: float = 0.0001,
+        batch_size: Union[int, str] = "auto",
+        learning_rate: str = "constant",
+        learning_rate_init: float = 0.001,
+        power_t: float = 0.5,
+        max_iter: int = 200,
+        shuffle: bool = True,
+        random_state: Optional[int] = None,
+        tol: float = 1e-4,
+        verbose: bool = False,
+        warm_start: bool = False,
+        momentum: float = 0.9,
+        nesterovs_momentum: bool = True,
+        early_stopping: bool = False,
+        validation_fraction: float = 0.1,
+        beta_1: float = 0.9,
+        beta_2: float = 0.999,
+        epsilon: float = 1e-8,
+        n_iter_no_change: int = 10,
+        max_fun: int = 15000,
+    ):
+        """
+        Parameters
+        ----------
+        hidden_layer_sizes : array-like of shape(n_layers - 2,), default=(100,)
+            The ith element represents the number of neurons in the ith
+            hidden layer.
+
+        activation : {'identity', 'logistic', 'tanh', 'relu'}, default='relu'
+            Activation function for the hidden layer.
+            - 'identity', no-op activation, useful to implement linear bottleneck,
+            returns f(x) = x
+            - 'logistic', the logistic sigmoid function,
+            returns f(x) = 1 / (1 + exp(-x)).
+            - 'tanh', the hyperbolic tan function,
+            returns f(x) = tanh(x).
+            - 'relu', the rectified linear unit function,
+            returns f(x) = max(0, x)
+
+        solver : {'lbfgs', 'sgd', 'adam'}, default='adam'
+            The solver for weight optimization.
+            - 'lbfgs' is an optimizer in the family of quasi-Newton methods.
+            - 'sgd' refers to stochastic gradient descent.
+            - 'adam' refers to a stochastic gradient-based optimizer proposed
+            by Kingma, Diederik, and Jimmy Ba
+            Note: The default solver 'adam' works pretty well on relatively
+            large datasets (with thousands of training samples or more) in terms of
+            both training time and validation score.
+            For small datasets, however, 'lbfgs' can converge faster and perform
+            better.
+
+        alpha : float, default=0.0001
+            Strength of the L2 regularization term. The L2 regularization term
+            is divided by the sample size when added to the loss.
+        
+        batch_size : int, default='auto'
+            Size of minibatches for stochastic optimizers.
+            If the solver is 'lbfgs', the classifier will not use minibatch.
+            When set to "auto", `batch_size=min(200, n_samples)`.
+        
+        learning_rate : {'constant', 'invscaling', 'adaptive'}, default='constant'
+            Learning rate schedule for weight updates.
+            - 'constant' is a constant learning rate given by
+            'learning_rate_init'.
+            - 'invscaling' gradually decreases the learning rate at each
+            time step 't' using an inverse scaling exponent of 'power_t'.
+            effective_learning_rate = learning_rate_init / pow(t, power_t)
+            - 'adaptive' keeps the learning rate constant to
+            'learning_rate_init' as long as training loss keeps decreasing.
+            Each time two consecutive epochs fail to decrease training loss by at
+            least tol, or fail to increase validation score by at least tol if
+            'early_stopping' is on, the current learning rate is divided by 5.
+            Only used when ``solver='sgd'``.
+        
+        learning_rate_init : float, default=0.001
+            The initial learning rate used. It controls the step-size
+            in updating the weights. Only used when solver='sgd' or 'adam'.
+        
+        power_t : float, default=0.5
+            The exponent for inverse scaling learning rate.
+            It is used in updating effective learning rate when the learning_rate
+            is set to 'invscaling'. Only used when solver='sgd'.
+        
+        max_iter : int, default=200
+            Maximum number of iterations. The solver iterates until convergence
+            (determined by 'tol') or this number of iterations. For stochastic
+            solvers ('sgd', 'adam'), note that this determines the number of epochs
+            (how many times each data point will be used), not the number of
+            gradient steps.
+        
+        shuffle : bool, default=True
+            Whether to shuffle samples in each iteration. Only used when
+            solver='sgd' or 'adam'.
+        
+        random_state : int, RandomState instance, default=None
+            Determines random number generation for weights and bias
+            initialization, train-test split if early stopping is used, and batch
+            sampling when solver='sgd' or 'adam'.
+            Pass an int for reproducible results across multiple function calls.
+            See :term:`Glossary <random_state>`.
+        
+        tol : float, default=1e-4
+            Tolerance for the optimization. When the loss or score is not improving
+            by at least ``tol`` for ``n_iter_no_change`` consecutive iterations,
+            unless ``learning_rate`` is set to 'adaptive', convergence is
+            considered to be reached and training stops.
+        
+        verbose : bool, default=False
+            Whether to print progress messages to stdout.
+        
+        warm_start : bool, default=False
+            When set to True, reuse the solution of the previous
+            call to fit as initialization, otherwise, just erase the
+            previous solution. See :term:`the Glossary <warm_start>`.
+        
+        momentum : float, default=0.9
+            Momentum for gradient descent update. Should be between 0 and 1. Only
+            used when solver='sgd'.
+        
+        nesterovs_momentum : bool, default=True
+            Whether to use Nesterov's momentum. Only used when solver='sgd' and
+            momentum > 0.
+        
+        early_stopping : bool, default=False
+            Whether to use early stopping to terminate training when validation
+            score is not improving. If set to true, it will automatically set
+            aside 10% of training data as validation and terminate training when
+            validation score is not improving by at least tol for
+            ``n_iter_no_change`` consecutive epochs. The split is stratified,
+            except in a multilabel setting.
+            If early stopping is False, then the training stops when the training
+            loss does not improve by more than tol for n_iter_no_change consecutive
+            passes over the training set.
+            Only effective when solver='sgd' or 'adam'.
+        
+        validation_fraction : float, default=0.1
+            The proportion of training data to set aside as validation set for
+            early stopping. Must be between 0 and 1.
+            Only used if early_stopping is True.
+        
+        beta_1 : float, default=0.9
+            Exponential decay rate for estimates of first moment vector in adam,
+            should be in [0, 1). Only used when solver='adam'.
+        
+        beta_2 : float, default=0.999
+            Exponential decay rate for estimates of second moment vector in adam,
+            should be in [0, 1). Only used when solver='adam'.
+        
+        epsilon : float, default=1e-8
+            Value for numerical stability in adam. Only used when solver='adam'.
+        
+        n_iter_no_change : int, default=10
+            Maximum number of epochs to not meet ``tol`` improvement.
+            Only effective when solver='sgd' or 'adam'.
+            .. versionadded:: 0.20
+        
+        max_fun : int, default=15000
+            Only used when solver='lbfgs'. Maximum number of loss function calls.
+            The solver iterates until convergence (determined by 'tol'), number
+            of iterations reaches max_iter, or this number of loss function calls.
+            Note that number of loss function calls will be greater than or equal
+            to the number of iterations for the `MLPClassifier`.
+            .. versionadded:: 0.22
+
+        References
+        ----------
+        Scikit-learn API: sklearn.neural_network.MLPClassifier
+        https://scikit-learn.org/stable/modules/generated/sklearn.neural_network.MLPClassifier.html
+        """
+
+        super().__init__()
+        self.hidden_layer_sizes = hidden_layer_sizes,
+        self.activation = activation,
+        self.solver = solver,
+        self.alpha = alpha,
+        self.batch_size = batch_size,
+        self.learning_rate = learning_rate,
+        self.learning_rate_init = learning_rate_init,
+        self.power_t = power_t,
+        self.max_iter = max_iter,
+        self.shuffle = shuffle,
+        self.random_state = random_state,
+        self.tol = tol,
+        self.verbose = verbose,
+        self.warm_start = warm_start,
+        self.momentum = momentum,
+        self.nesterovs_momentum = nesterovs_momentum,
+        self.early_stopping = early_stopping,
+        self.validation_fraction = validation_fraction,
+        self.beta_1 = beta_1,
+        self.beta_2 = beta_2,
+        self.epsilon = epsilon,
+        self.n_iter_no_change = n_iter_no_change,
+        self.max_fun = max_fun,
+
+        # FIXME (Sany sanyhew1097618435@163.com): figure out why data type changes after assignment.
+        self.model = MLPClassifier(
+            hidden_layer_sizes = self.hidden_layer_sizes[0],
+            activation = self.activation[0],
+            alpha = self.alpha[0],
+            batch_size = self.batch_size[0],
+            learning_rate = self.learning_rate[0],
+            learning_rate_init = self.learning_rate_init[0],
+            power_t = self.power_t[0],
+            max_iter = self.max_iter[0],
+            shuffle = self.shuffle[0],
+            random_state = self.random_state[0],
+            tol = self.tol[0],
+            verbose = self.verbose[0],
+            warm_start = self.warm_start[0],
+            momentum = self.momentum[0],
+            solver = self.solver[0],
+            nesterovs_momentum = self.nesterovs_momentum[0],
+            early_stopping = self.early_stopping[0],
+            validation_fraction = self.validation_fraction[0],
+            beta_1 = self.beta_1[0],
+            beta_2 = self.beta_2[0],
+            epsilon = self.epsilon[0],
+            n_iter_no_change = self.n_iter_no_change[0],
+            max_fun = self.max_fun[0],
+        )
+
+        self.naming = DNNClassification.name
+
+    def ray_tune(self, X_train: pd.DataFrame, X_test: pd.DataFrame, y_train: pd.DataFrame, y_test: pd.DataFrame) -> None:
+        """The customized DNN of the combinations of Ray, FLAML and Scikit-learn framework."""
+
+        from ray import tune
+        from ray.air import session
+        from ray.tune.search import ConcurrencyLimiter
+        from ray.tune.search.flaml import BlendSearch
+        from sklearn.metrics import accuracy_score
+
+        def customized_model(l1: int, l2: int, l3: int, batch: int) -> object:
+            """The customized model by Scikit-learn framework."""
+            return MLPClassifier(hidden_layer_sizes=(l1, l2, l3), batch_size=batch)
+
+        def evaluate(l1: int, l2: int, l3: int, batch: int) -> float:
+            """The evaluation function by simulating a long-running ML experiment
+             to get the model's performance at every epoch."""
+            clfr = customized_model(l1, l2, l3, batch)
+            clfr.fit(X_train, y_train)
+            y_pred = clfr.predict(X_test)
+            acc = accuracy_score(y_test, y_pred)
+            return acc
+
+        def objective(config: Dict) -> None:
+            """Objective function takes a Tune config, evaluates the score of your experiment in a training loop,
+             and uses session.report to report the score back to Tune."""
+            for step in range(config["steps"]):
+                score = evaluate(config["l1"], config["l2"], config["l3"], config["batch"])
+                session.report({"iterations": step, "mean_loss": score})
+
+        # Search space: The critical assumption is that the optimal hyper-parameters live within this space.
+        search_config = {
+            "l1": tune.randint(1, 20),
+            "l2": tune.randint(1, 30),
+            "l3": tune.randint(1, 20),
+            "batch": tune.randint(20, 100)
+        }
+
+        # Define the time budget in seconds.
+        time_budget_s = 30
+
+        # Integrate with FLAML's BlendSearch to implement hyper-parameters optimization .
+        algo = BlendSearch(
+            metric="mean_loss",
+            mode="min",
+            space=search_config)
+        algo.set_search_properties(config={"time_budget_s": time_budget_s})
+        algo = ConcurrencyLimiter(algo, max_concurrent=4)
+
+        # Use Ray Tune to  run the experiment to "min"imize the “mean_loss” of the "objective"
+        # by searching "search_config" via "algo", "num_samples" times.
+        tuner = tune.Tuner(
+            objective,
+            tune_config=tune.TuneConfig(
+                metric="mean_loss",
+                mode="min",
+                search_alg=algo,
+                num_samples=-1,
+                time_budget_s=time_budget_s,
+            ),
+            param_space={"steps": 100},
+        )
+        results = tuner.fit()
+
+        # The hyper-parameters found to minimize the mean loss of the defined objective and the corresponding model.
+        best_result = results.get_best_result(metric='mean_loss', mode='min')
+        self.ray_best_model = customized_model(best_result.config['l1'], best_result.config['l2'],
+                                               best_result.config['l3'], best_result.config['batch'])
+
+
+    @classmethod
+    def manual_hyper_parameters(cls) -> Dict:
+        """Manual hyper-parameters specification."""
+        print(f"-*-*- {cls.name} - Hyper-parameters Specification -*-*-")
+        hyper_parameters = deep_neural_network_manual_hyper_parameters()
+        return hyper_parameters
+
+    @dispatch()
+    def special_components(self, **kwargs) -> None:
+        """Invoke all special application functions for this algorithms by Scikit-learn framework."""
+        pass
+
+    @dispatch(bool)
+    def special_components(self, is_automl: bool, **kwargs) -> None:
+        """Invoke all special application functions for this algorithms by FLAML framework."""
+        pass
+
+
+class ExtraTreesClassification(ClassificationWorkflowBase):
+    """The automation workflow of using Extra-Trees algorithm to make insightful products."""
+
+    name = "Extra-Trees"
+    special_function = []
+
+    def __init__(
+        self,
+        n_estimators=100,
+        criterion="gini",
+        max_depth=None,
+        min_samples_split=2,
+        min_samples_leaf=1,
+        min_weight_fraction_leaf=0.0,
+        max_features="sqrt",
+        max_leaf_nodes=None,
+        min_impurity_decrease=0.0,
+        bootstrap=False,
+        oob_score=False,
+        n_jobs=None,
+        random_state=None,
+        verbose=0,
+        warm_start=False,
+        class_weight=None,
+        ccp_alpha=0.0,
+        max_samples=None,
+    ) -> None:
+        """
+        Parameters
+        ----------
+        n_estimators : int, default=100
+            The number of trees in the forest.
+            .. versionchanged:: 0.22
+            The default value of ``n_estimators`` changed from 10 to 100
+            in 0.22.
+            
+        criterion : {"gini", "entropy", "log_loss"}, default="gini"
+            The function to measure the quality of a split. Supported criteria are
+            "gini" for the Gini impurity and "log_loss" and "entropy" both for the
+            Shannon information gain, see :ref:`tree_mathematical_formulation`.
+            Note: This parameter is tree-specific.
+        
+        max_depth : int, default=None
+            The maximum depth of the tree. If None, then nodes are expanded until
+            all leaves are pure or until all leaves contain less than
+            min_samples_split samples.
+        
+        min_samples_split : int or float, default=2
+            The minimum number of samples required to split an internal node:
+            - If int, then consider `min_samples_split` as the minimum number.
+            - If float, then `min_samples_split` is a fraction and
+            `ceil(min_samples_split * n_samples)` are the minimum
+            number of samples for each split.
+            .. versionchanged:: 0.18
+            Added float values for fractions.
+        
+        min_samples_leaf : int or float, default=1
+            The minimum number of samples required to be at a leaf node.
+            A split point at any depth will only be considered if it leaves at
+            least ``min_samples_leaf`` training samples in each of the left and
+            right branches.  This may have the effect of smoothing the model,
+            especially in regression.
+            - If int, then consider `min_samples_leaf` as the minimum number.
+            - If float, then `min_samples_leaf` is a fraction and
+            `ceil(min_samples_leaf * n_samples)` are the minimum
+            number of samples for each node.
+            .. versionchanged:: 0.18
+            Added float values for fractions.
+        
+        min_weight_fraction_leaf : float, default=0.0
+            The minimum weighted fraction of the sum total of weights (of all
+            the input samples) required to be at a leaf node. Samples have
+            equal weight when sample_weight is not provided.
+        
+        max_features : {"sqrt", "log2", None}, int or float, default="sqrt"
+            The number of features to consider when looking for the best split:
+            - If int, then consider `max_features` features at each split.
+            - If float, then `max_features` is a fraction and
+            `max(1, int(max_features * n_features_in_))` features are considered at each
+            split.
+            - If "auto", then `max_features=sqrt(n_features)`.
+            - If "sqrt", then `max_features=sqrt(n_features)`.
+            - If "log2", then `max_features=log2(n_features)`.
+            - If None, then `max_features=n_features`.
+            .. versionchanged:: 1.1
+                The default of `max_features` changed from `"auto"` to `"sqrt"`.
+            .. deprecated:: 1.1
+                The `"auto"` option was deprecated in 1.1 and will be removed
+                in 1.3.
+            Note: the search for a split does not stop until at least one
+            valid partition of the node samples is found, even if it requires to
+            effectively inspect more than ``max_features`` features.
+        
+        max_leaf_nodes : int, default=None
+            Grow trees with ``max_leaf_nodes`` in best-first fashion.
+            Best nodes are defined as relative reduction in impurity.
+            If None then unlimited number of leaf nodes.
+        
+        min_impurity_decrease : float, default=0.0
+            A node will be split if this split induces a decrease of the impurity
+            greater than or equal to this value.
+            The weighted impurity decrease equation is the following::
+                N_t / N * (impurity - N_t_R / N_t * right_impurity
+                                    - N_t_L / N_t * left_impurity)
+            where ``N`` is the total number of samples, ``N_t`` is the number of
+            samples at the current node, ``N_t_L`` is the number of samples in the
+            left child, and ``N_t_R`` is the number of samples in the right child.
+            ``N``, ``N_t``, ``N_t_R`` and ``N_t_L`` all refer to the weighted sum,
+            if ``sample_weight`` is passed.
+            .. versionadded:: 0.19
+        
+        bootstrap : bool, default=False
+            Whether bootstrap samples are used when building trees. If False, the
+            whole dataset is used to build each tree.
+        
+        oob_score : bool, default=False
+            Whether to use out-of-bag samples to estimate the generalization score.
+            Only available if bootstrap=True.
+        
+        n_jobs : int, default=None
+            The number of jobs to run in parallel. :meth:`fit`, :meth:`predict`,
+            :meth:`decision_path` and :meth:`apply` are all parallelized over the
+            trees. ``None`` means 1 unless in a :obj:`joblib.parallel_backend`
+            context. ``-1`` means using all processors. See :term:`Glossary
+            <n_jobs>` for more details.
+        
+        random_state : int, RandomState instance or None, default=None
+            Controls 3 sources of randomness:
+            - the bootstrapping of the samples used when building trees
+            (if ``bootstrap=True``)
+            - the sampling of the features to consider when looking for the best
+            split at each node (if ``max_features < n_features``)
+            - the draw of the splits for each of the `max_features`
+            See :term:`Glossary <random_state>` for details.
+        
+        verbose : int, default=0
+            Controls the verbosity when fitting and predicting.
+        
+        warm_start : bool, default=False
+            When set to ``True``, reuse the solution of the previous call to fit
+            and add more estimators to the ensemble, otherwise, just fit a whole
+            new forest. See :term:`Glossary <warm_start>` and
+            :ref:`gradient_boosting_warm_start` for details.
+        
+        class_weight : {"balanced", "balanced_subsample"}, dict or list of dicts, \
+                default=None
+            Weights associated with classes in the form ``{class_label: weight}``.
+            If not given, all classes are supposed to have weight one. For
+            multi-output problems, a list of dicts can be provided in the same
+            order as the columns of y.
+            Note that for multioutput (including multilabel) weights should be
+            defined for each class of every column in its own dict. For example,
+            for four-class multilabel classification weights should be
+            [{0: 1, 1: 1}, {0: 1, 1: 5}, {0: 1, 1: 1}, {0: 1, 1: 1}] instead of
+            [{1:1}, {2:5}, {3:1}, {4:1}].
+            The "balanced" mode uses the values of y to automatically adjust
+            weights inversely proportional to class frequencies in the input data
+            as ``n_samples / (n_classes * np.bincount(y))``
+            The "balanced_subsample" mode is the same as "balanced" except that
+            weights are computed based on the bootstrap sample for every tree
+            grown.
+            For multi-output, the weights of each column of y will be multiplied.
+            Note that these weights will be multiplied with sample_weight (passed
+            through the fit method) if sample_weight is specified.
+        
+        ccp_alpha : non-negative float, default=0.0
+            Complexity parameter used for Minimal Cost-Complexity Pruning. The
+            subtree with the largest cost complexity that is smaller than
+            ``ccp_alpha`` will be chosen. By default, no pruning is performed. See
+            :ref:`minimal_cost_complexity_pruning` for details.
+            .. versionadded:: 0.22
+        
+        max_samples : int or float, default=None
+            If bootstrap is True, the number of samples to draw from X
+            to train each base estimator.
+            - If None (default), then draw `X.shape[0]` samples.
+            - If int, then draw `max_samples` samples.
+            - If float, then draw `max_samples * X.shape[0]` samples. Thus,
+            `max_samples` should be in the interval `(0.0, 1.0]`.
+            .. versionadded:: 0.22
+        
+        References
+        ----------
+        Scikit-learn API: sklearn.ensemble.ExtraTreesClassifier
+        https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.ExtraTreesClassifier.html#sklearn-ensemble-extratreesclassifier
+        """
+
+        super().__init__()
+        self.n_estimators = n_estimators
+        self.criterion = criterion
+        self.max_depth = max_depth
+        self.min_samples_split = min_samples_split
+        self.min_samples_leaf = min_samples_leaf
+        self.min_weight_fraction_leaf = min_weight_fraction_leaf
+        self.max_features = max_features
+        self.max_leaf_nodes = max_leaf_nodes
+        self.min_impurity_decrease = min_impurity_decrease
+        self.bootstrap = bootstrap
+        self.oob_score = oob_score
+        self.n_jobs = n_jobs
+        self.random_state = random_state
+        self.verbose = verbose
+        self.warm_start = warm_start
+        self.class_weight = class_weight
+        self.ccp_alpha = ccp_alpha
+        self.max_samples = max_samples
+
+        self.model = ExtraTreesClassifier(
+            n_estimators=self.n_estimators,
+            criterion=self.criterion,
+            max_depth=self.max_depth,
+            min_samples_split=self.min_samples_split,
+            min_samples_leaf=self.min_samples_leaf,
+            min_weight_fraction_leaf=self.min_weight_fraction_leaf,
+            max_features=self.max_features,
+            max_leaf_nodes=self.max_leaf_nodes,
+            min_impurity_decrease=self.min_impurity_decrease,
+            bootstrap=self.bootstrap,
+            oob_score=self.oob_score,
+            n_jobs=self.n_jobs,
+            random_state=self.random_state,
+            verbose=self.verbose,
+            warm_start=self.warm_start,
+            class_weight=self.class_weight,
+            ccp_alpha=self.ccp_alpha,
+            max_samples=self.max_samples,
+        )
+
+        self.naming = ExtraTreesClassification.name
+
+    @property
+    def settings(self) -> Dict:
+        """The configuration to implement AutoML by FLAML framework."""
+        configuration = {
+            "time_budget": 10,  # total running time in seconds
+            "metric": 'accuracy',
+            "estimator_list": ['extra_tree'],  # list of ML learners
+            "task": 'classification',  # task type
+            # "log_file_name": f'{self.naming} - automl.log',  # flaml log file
+            # "log_training_metric": True,  # whether to log training metric
+        }
+        return configuration
+
+    @classmethod
+    def manual_hyper_parameters(cls) -> Dict:
+        """Manual hyper-parameters specification."""
+        print(f"-*-*- {cls.name} - Hyper-parameters Specification -*-*-")
+        hyper_parameters = extra_trees_manual_hyper_parameters()
+        return hyper_parameters
+
+    @dispatch()
+    def special_components(self, **kwargs) -> None:
+        """Invoke all special application functions for this algorithms by Scikit-learn framework."""
+        pass
+
+    @dispatch(bool)
+    def special_components(self, is_automl: bool, **kwargs) -> None:
+        """Invoke all special application functions for this algorithms by FLAML framework."""
+        pass
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `geochemistrypi-0.1.0/geochemistrypi/data_mining/model/clustering.py` & `geochemistrypi-0.2.0/geochemistrypi/data_mining/model/clustering.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,72 +1,79 @@
 # -*- coding: utf-8 -*-
+import numpy as np
+import pandas as pd
 from sklearn import metrics
 from sklearn.cluster import KMeans
 from sklearn.cluster import DBSCAN
-import numpy as np
-import pandas as pd
 from sklearn.cluster import AffinityPropagation
+from typing import Optional, Union, Dict
+
 from ..utils.base import save_data
 from ..utils.base import save_fig
 from ..global_variable import MODEL_OUTPUT_IMAGE_PATH
 from ..global_variable import DATASET_OUTPUT_PATH
 from ._base import WorkflowBase
-from .func.algo_clustering._kmeans import plot_silhouette_diagram, scatter2d, scatter3d
-from .func.algo_clustering._dbscan import dbscan_result_plot
-from typing import Optional, Union, Dict
+from .func.algo_clustering._kmeans import plot_silhouette_diagram, scatter2d, scatter3d, kmeans_manual_hyper_parameters
+from .func.algo_clustering._dbscan import dbscan_result_plot, dbscan_manual_hyper_parameters
 
 
 class ClusteringWorkflowBase(WorkflowBase):
-    """Base class for Cluster.
+    """The base workflow class of clustering algorithms."""
 
-    Warning: This class should not be used directly.
-    Use derived classes instead.
-    """
     common_function = ['Cluster Centers', 'Cluster Labels', 'Model Persistence']
 
     def __init__(self):
         super().__init__()
         self.clustering_result = None
 
     def fit(self, X: pd.DataFrame, y: Optional[pd.DataFrame] = None) -> None:
+        """Fit the model according to the given training data."""
         self.X = X
         self.model.fit(X)
 
+    @classmethod
+    def manual_hyper_parameters(cls) -> Dict:
+        """Manual hyper-parameters specification."""
+        return dict()
+
     # TODO(Samson 1057266013@qq.com): This function might need to be rethought.
     def get_cluster_centers(self) -> np.ndarray:
+        """Get the cluster centers."""
         print("-----* Clustering Centers *-----")
         print(getattr(self.model, 'cluster_centers_', 'This class don not have cluster_centers_'))
         return getattr(self.model, 'cluster_centers_', 'This class don not have cluster_centers_')
 
     def get_labels(self):
+        """Get the cluster labels."""
         print("-----* Clustering Labels *-----")
         #self.X['clustering result'] = self.model.labels_
         self.clustering_result = pd.DataFrame(self.model.labels_, columns=['clustering result'])
         print(self.clustering_result)
         save_data(self.clustering_result, f"{self.naming}'s result", DATASET_OUTPUT_PATH)
 
 
 class KMeansClustering(ClusteringWorkflowBase):
+    """The automation workflow of using KMeans algorithm to make insightful products."""
 
     name = "KMeans"
     special_function = ['KMeans Score']
 
-    def __init__(self,
-                 n_clusters=8,
-                 init="k-means++",
-                 n_init=10,
-                 max_iter=300,
-                 tol=1e-4,
-                 verbose=0,
-                 random_state=None,
-                 copy_x=True,
-                 algorithm="auto"
+    def __init__(
+        self,
+        n_clusters=8,
+        init="k-means++",
+        n_init=10,
+        max_iter=300,
+        tol=1e-4,
+        verbose=0,
+        random_state=None,
+        copy_x=True,
+        algorithm="auto"
     ) -> None:
         """
-
         Parameters
         ----------
         n_clusters : int, default=8
             The number of clusters to form as well as the number of
             centroids to generate.
 
         init : {'k-means++', 'random'}, callable or array-like of shape \
@@ -126,72 +133,81 @@
             (n_samples, n_clusters).
 
             For now "auto" (kept for backward compatibility) chooses "elkan" but it
             might change in the future for a better heuristic.
 
         References
         ----------------------------------------
-        Read more in the :ref:`User Guide <k_means>`.
-        https://scikit-learn.org/stable/modules/clustering.html#k-means
+        Scikit-learn API: sklearn.cluster.KMeans
+        https://scikit-learn.org/stable/modules/generated/sklearn.cluster.KMeans.html
         """
 
         super().__init__()
         self.n_clusters = n_clusters
         self.init = init
         self.max_iter = max_iter
         self.tol = tol
         self.n_init = n_init
         self.verbose = verbose
         self.random_state = random_state
         self.copy_x = copy_x
         self.algorithm = algorithm
-        self.model = KMeans(n_clusters=self.n_clusters,
-                            init=self.init,
-                            n_init=self.n_init,
-                            max_iter=self.max_iter,
-                            tol=self.tol,
-                            verbose=self.verbose,
-                            random_state=self.random_state,
-                            copy_x=self.copy_x,
-                            algorithm=self.algorithm)
+
+        self.model = KMeans(
+            n_clusters=self.n_clusters,
+            init=self.init,
+            n_init=self.n_init,
+            max_iter=self.max_iter,
+            tol=self.tol,
+            verbose=self.verbose,
+            random_state=self.random_state,
+            copy_x=self.copy_x,
+            algorithm=self.algorithm
+        )
 
         self.naming = KMeansClustering.name
 
+    @classmethod
+    def manual_hyper_parameters(cls) -> Dict:
+        """Manual hyper-parameters specification."""
+        print(f"-*-*- {cls.name} - Hyper-parameters Specification -*-*-")
+        hyper_parameters = kmeans_manual_hyper_parameters()
+        return hyper_parameters
+
     def _get_scores(self):
+        """Get the scores of the clustering result."""
         print("-----* KMeans Scores *-----")
         print("Inertia Score: ", self.model.inertia_)
         print("Calinski Harabasz Score: ", metrics.calinski_harabasz_score(self.X, self.model.labels_))
         print("Silhouette Score: ", metrics.silhouette_score(self.X, self.model.labels_))
 
     @staticmethod
     def _plot_silhouette_diagram(data: pd.DataFrame, cluster_labels: pd.DataFrame, cluster_centers_: np.ndarray,
                                  n_clusters: int, algorithm_name: str, store_path: str) -> None:
+        """Plot the silhouette diagram of the clustering result."""
         print("-----* Silhouette Diagram *-----")
         plot_silhouette_diagram(data, cluster_labels, cluster_centers_, n_clusters, algorithm_name)
         save_fig(f"Silhouette Diagram - {algorithm_name}", store_path)
 
     @staticmethod
     def _scatter2d(data: pd.DataFrame, cluster_labels: pd.DataFrame, algorithm_name: str, store_path: str) -> None:
+        """Plot the two-dimensional diagram of the clustering result."""
         print("-----* Cluster Two-Dimensional Diagram *-----")
         scatter2d(data, cluster_labels, algorithm_name)
         save_fig(f"Cluster Two-Dimensional Diagram - {algorithm_name}", store_path)
 
     @staticmethod
     def _scatter3d(data: pd.DataFrame, cluster_labels: pd.DataFrame, algorithm_name: str, store_path: str) -> None:
+        """Plot the three-dimensional diagram of the clustering result."""
         print("-----* Cluster Three-Dimensional Diagram *-----")
         scatter3d(data, cluster_labels, algorithm_name)
         save_fig(f"Cluster Three-Dimensional Diagram - {algorithm_name}", store_path)
 
     def special_components(self, **kwargs: Union[Dict, np.ndarray, int]) -> None:
-        """
-            The components_num Represents the dimension of the data.
-            We subtract 1 because the label takes up a column.
-        """
-        # data_dimension = self.X.shape[1] - 1
-
+        """Invoke all special application functions for this algorithms by Scikit-learn framework."""
         self._get_scores()
         self._plot_silhouette_diagram(data=self.X, cluster_labels=self.clustering_result['clustering result'],
                                       cluster_centers_=self.get_cluster_centers(), n_clusters=self.n_clusters,
                                       algorithm_name=self.naming, store_path=MODEL_OUTPUT_IMAGE_PATH)
         # Draw graphs when the number of principal components > 3
         if self.X.shape[1] >= 3:
             # choose two of dimensions to draw
@@ -216,28 +232,30 @@
             self._scatter2d(data=self.X, cluster_labels=self.clustering_result['clustering result'], algorithm_name=self.naming,
                             store_path=MODEL_OUTPUT_IMAGE_PATH)
         else:
             pass
 
 
 class DBSCANClustering(ClusteringWorkflowBase):
+    """The automation workflow of using DBSCAN algorithm to make insightful products."""
 
     name = "DBSCAN"
-    special_function = ['Virtualization of result in 2D graph']
+    special_function = ['Virtualization of Result in 2D Graph']
 
-    def __init__(self,
-                 eps=0.5,
-                 min_samples=5,
-                 metric="euclidean",
-                 metric_params=None,
-                 algorithm="auto",
-                 leaf_size=30,
-                 p=None,
-                 n_jobs=None,
-                 ):
+    def __init__(
+        self,
+        eps=0.5,
+        min_samples=5,
+        metric="euclidean",
+        metric_params=None,
+        algorithm="auto",
+        leaf_size=30,
+        p=None,
+        n_jobs=None,
+    ) -> None:
         """
         Parameters
         ----------
         eps : float, default=0.5
         The maximum distance between two samples for one to be considered as in the neighborhood of the other. This is not a maximum bound on the distances of points within a cluster. This is the most important DBSCAN parameter to choose appropriately for your data set and distance function.
 
         min_samples : int, default=5
@@ -263,45 +281,58 @@
         The power of the Minkowski metric to be used to calculate distance between points. If None, then p=2 (equivalent to the Euclidean distance).
 
         n_jobs : int, default=None
         The number of parallel jobs to run. None means 1 unless in a joblib.parallel_backend context. -1 means using all processors. See Glossary for more details.
 
         References
         ----------------------------------------
-        Read more in the :ref:`User Guide <dbscan>`.
-        https://scikit-learn.org/stable/modules/clustering.html#dbscan
+        Scikit-learn API: sklearn.cluster.DBSCAN
+        https://scikit-learn.org/stable/modules/generated/sklearn.cluster.DBSCAN.html
         """
 
         super().__init__()
         self.eps = eps
         self.min_samples = min_samples
         self.metric = metric
         self.metric_params = metric_params
         self.algorithm = algorithm
         self.leaf_size = leaf_size
         self.p = p
         self.n_jobs = n_jobs
-        self.model = DBSCAN(eps=self.eps,
-                            min_samples=self.min_samples,
-                            metric=self.metric,
-                            metric_params=self.metric_params,
-                            algorithm=self.algorithm,
-                            leaf_size=self.leaf_size,
-                            p=self.p,
-                            n_jobs=self.n_jobs)
+
+        self.model = DBSCAN(
+            eps=self.eps,
+            min_samples=self.min_samples,
+            metric=self.metric,
+            metric_params=self.metric_params,
+            algorithm=self.algorithm,
+            leaf_size=self.leaf_size,
+            p=self.p,
+            n_jobs=self.n_jobs
+        )
+
         self.naming = DBSCANClustering.name
 
+    @classmethod
+    def manual_hyper_parameters(cls) -> Dict:
+        """Manual hyper-parameters specification."""
+        print(f"-*-*- {cls.name} - Hyper-parameters Specification -*-*-")
+        hyper_parameters = dbscan_manual_hyper_parameters()
+        return hyper_parameters
+
     @staticmethod
-    def clustering_result_plot(X: pd.DataFrame, trained_model: any, algorithm_name: str, imag_config: dict, store_path: str) -> None:
-        print("-------** dbscan_clustering_result_2d_plot **----------")
+    def _clustering_result_plot(X: pd.DataFrame, trained_model: any, algorithm_name: str, imag_config: dict, store_path: str) -> None:
+        """Plot the clustering result in 2D graph."""
+        print("-------** DBSCAN Clustering Result 2D Plot **----------")
         dbscan_result_plot(X, trained_model, imag_config, algorithm_name)
         save_fig(f'Plot - {algorithm_name} - 2D', store_path)
 
     def special_components(self, **kwargs: Union[Dict, np.ndarray, int]) -> None:
-        self.clustering_result_plot(X=self.X, trained_model=self.model, algorithm_name=self.naming, imag_config=self.image_config, store_path=MODEL_OUTPUT_IMAGE_PATH)
+        """Invoke all special application functions for this algorithms by Scikit-learn framework."""
+        self._clustering_result_plot(X=self.X, trained_model=self.model, algorithm_name=self.naming, imag_config=self.image_config, store_path=MODEL_OUTPUT_IMAGE_PATH)
 
 
 class AffinityPropagationClustering(ClusteringWorkflowBase):
     name = "AffinityPropagation"
 
     def __init__(self,
                  *,
```

### Comparing `geochemistrypi-0.1.0/geochemistrypi/data_mining/model/decomposition.py` & `geochemistrypi-0.2.0/geochemistrypi/data_mining/model/decomposition.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # -*- coding: utf-8 -*-
 import pandas as pd
 from sklearn.decomposition import PCA
 import numpy as np
-from ..global_variable import MODEL_OUTPUT_IMAGE_PATH
 from typing import Optional, Union, Dict
+
 from ._base import WorkflowBase
-from .func.algo_decomposition._pca import biplot, triplot
+from .func.algo_decomposition._pca import biplot, triplot, pca_manual_hyper_parameters
 from ..utils.base import save_fig
+from ..global_variable import MODEL_OUTPUT_IMAGE_PATH
 
 
 class DecompositionWorkflowBase(WorkflowBase):
     """The base workflow class of decomposition algorithms."""
 
     common_function = [#'Decomposition Result',
                        'Model Persistence']
@@ -25,14 +26,19 @@
         """Fit the model."""
         self.model.fit(X)
 
     def transform(self, X: pd.DataFrame) -> pd.DataFrame:
         """Apply dimensionality reduction to X."""
         return self.model.transform(X)
 
+    @classmethod
+    def manual_hyper_parameters(cls) -> Dict:
+        """Manual hyper-parameters specification."""
+        return dict()
+
     def _reduced_data2pd(self, reduced_data: np.ndarray, components_num: int) -> None:
         """Transform reduced data into the format of pd.DataFrame.
 
         Parameters
         ----------
         reduced_data : np.ndarray
             The data X after dimension reduction.
@@ -157,72 +163,87 @@
             for reproducible results across multiple function calls.
             See :term:`Glossary <random_state>`.
 
             .. versionadded:: 0.18.0
 
         References
         ----------
-        scikit API: sklearn.decomposition.PCA
+        Scikit-learn API: sklearn.decomposition.PCA
         https://scikit-learn.org/stable/modules/generated/sklearn.decomposition.PCA.html
         """
         super().__init__()
         self.n_components = n_components
         self.copy = copy
         self.whiten = whiten
         self.svd_solver = svd_solver
         self.tol = tol
         self.iterated_power = iterated_power
         # self.n_oversamples = n_oversamples
         # self.power_iteration_normalizer = power_iteration_normalizer
         self.random_state = random_state
 
-        self.model = PCA(n_components=self.n_components,
-                         copy=self.copy,
-                         whiten=self.whiten,
-                         svd_solver=self.svd_solver,
-                         tol=self.tol,
-                         iterated_power=self.iterated_power,
-                         # n_oversamples=self.n_oversamples,
-                         # power_iteration_normalizer=self.power_iteration_normalizer,
-                         random_state=self.random_state)
+        self.model = PCA(
+            n_components=self.n_components,
+            copy=self.copy,
+            whiten=self.whiten,
+            svd_solver=self.svd_solver,
+            tol=self.tol,
+            iterated_power=self.iterated_power,
+            # n_oversamples=self.n_oversamples,
+            # power_iteration_normalizer=self.power_iteration_normalizer,
+            random_state=self.random_state
+        )
+        
         self.naming = PCADecomposition.name
 
         # special attributes
         self.pc_data = None
 
+    @classmethod
+    def manual_hyper_parameters(cls) -> Dict:
+        """Manual hyper-parameters specification."""
+        print(f"-*-*- {cls.name} - Hyper-parameters Specification -*-*-")
+        hyper_parameters = pca_manual_hyper_parameters()
+        return hyper_parameters
+
     def _get_principal_components(self) -> None:
+        """Get principal components."""
         print("-----* Principal Components *-----")
         print("Every column represents one principal component respectively.")
         print("Every row represents how much that row feature contributes to each principal component respectively.")
         print("The tabular data looks like in format: 'rows x columns = 'features x principal components'.")
         pc_name = []
         for i in range(self.n_components):
             pc_name.append(f'PC{i+1}')
         self.pc_data = pd.DataFrame(self.model.components_.T)
         self.pc_data.columns = pc_name
         self.pc_data.set_index(DecompositionWorkflowBase.X.columns, inplace=True)
         print(self.pc_data)
 
     def _get_explained_variance_ratio(self) -> None:
+        """Get explained variance ratio."""
         print("-----* Explained Variance Ratio *-----")
         print(self.model.explained_variance_ratio_)
 
     @staticmethod
     def _biplot(reduced_data: pd.DataFrame, pc_data: pd.DataFrame, algorithm_name: str, store_path: str) -> None:
+        """Draw bi-plot."""
         print("-----* Compositional Bi-plot *-----")
         biplot(reduced_data, pc_data, algorithm_name)
         save_fig(f"Compositional Bi-plot - {algorithm_name}", store_path)
 
     @staticmethod
     def _triplot(reduced_data: pd.DataFrame, pc_data: pd.DataFrame, algorithm_name: str, store_path: str) -> None:
+        """Draw tri-plot."""
         print("-----* Compositional Tri-plot *-----")
         triplot(reduced_data, pc_data, algorithm_name)
         save_fig(f"Compositional Tri-plot - {algorithm_name}", store_path)
 
     def special_components(self, **kwargs: Union[Dict, np.ndarray, int]) -> None:
+        """Invoke all special application functions for this algorithms by Scikit-learn framework."""
         self._reduced_data2pd(kwargs['reduced_data'], kwargs['components_num'])
         self._get_principal_components()
         self._get_explained_variance_ratio()
 
         # Draw graphs when the number of principal components > 3
         if kwargs['components_num'] > 3:
             # choose two of dimensions to draw
```

### Comparing `geochemistrypi-0.1.0/geochemistrypi/data_mining/model/regression.py` & `geochemistrypi-0.2.0/geochemistrypi/data_mining/model/regression.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 # -*- coding: utf-8 -*-
-from ..global_variable import MODEL_OUTPUT_IMAGE_PATH, RAY_FLAML
-from ..utils.base import save_fig
 from sklearn.linear_model import LinearRegression
 from sklearn.preprocessing import PolynomialFeatures
 from sklearn.tree import DecisionTreeRegressor, plot_tree
 from sklearn.ensemble import ExtraTreesRegressor, RandomForestRegressor
 from sklearn.svm import SVR
 from sklearn.neural_network import MLPRegressor
 from typing import Union, Optional, List, Dict, Callable, Tuple, Any
 from typing import Sequence
 import numpy as np
 import pandas as pd
 import xgboost
 from multipledispatch import dispatch
 from flaml import AutoML
+
+from ..global_variable import MODEL_OUTPUT_IMAGE_PATH, RAY_FLAML
+from ..utils.base import save_fig
 from ._base import WorkflowBase
 from .func.algo_regression._common import plot_predicted_value_evaluation, plot_true_vs_predicted, score, cross_validation
-from .func.algo_regression._polynomial import show_formula
-from .func.algo_regression._rf import feature_importance__, box_plot
-from .func.algo_regression._xgboost import feature_importance, histograms_feature_weights, permutation_importance_
-from .func.algo_regression._linear import show_formula, plot_2d_graph, plot_3d_graph
-from .func.algo_regression._extra_tree import feature_importances
-from .func.algo_regression._decision_tree import decision_tree_plot
+from .func.algo_regression._polynomial_regression import show_formula, polynomial_regression_manual_hyper_parameters
+from .func.algo_regression._rf import feature_importance__, box_plot, random_forest_manual_hyper_parameters
+from .func.algo_regression._xgboost import feature_importance, histograms_feature_weights, permutation_importance_, xgboost_manual_hyper_parameters
+from .func.algo_regression._linear_regression import show_formula, plot_2d_graph, plot_3d_graph, linear_regression_manual_hyper_parameters
+from .func.algo_regression._extra_tree import feature_importances, extra_trees_manual_hyper_parameters
+from .func.algo_regression._svr import plot_2d_decision_boundary, svr_manual_hyper_parameters
+from .func.algo_regression._decision_tree import decision_tree_plot, decision_tree_manual_hyper_parameters
+from .func.algo_regression._deep_neural_network import deep_neural_network_manual_hyper_parameters
 
 
 class RegressionWorkflowBase(WorkflowBase):
     """The base workflow class of regression algorithms."""
 
     common_function = ['Model Score', 'Cross Validation', 'Model Prediction', 'Model Persistence']
 
@@ -89,34 +92,43 @@
     def customization(self) -> object:
         """The customized model of FLAML framework."""
         return object
 
     def ray_tune(self, X_train, X_test, y_train, y_test) -> object:
         """The customized model of FLAML framework and RAY framework."""
         return object
+    
+    @classmethod
+    def manual_hyper_parameters(cls) -> Dict:
+        """Manual hyper-parameters specification."""
+        return dict()
 
     @staticmethod
     def _plot_predicted_value_evaluation(y_test: pd.DataFrame, y_test_predict: pd.DataFrame, algorithm_name: str, store_path: str) -> None:
+        """Plot the predicted value evaluation."""
         print("-----* Predicted Value Evaluation *-----")
         plot_predicted_value_evaluation(y_test, y_test_predict)
         save_fig(f'Predicted Value Evaluation - {algorithm_name}', store_path)
 
     @staticmethod
     def _plot_true_vs_predicted(y_test_predict: pd.DataFrame, y_test: pd.DataFrame, algorithm_name: str, store_path: str) -> None:
+        """Plot the true value vs. predicted value."""
         print("-----* True Value vs. Predicted Value *-----")
         plot_true_vs_predicted(y_test_predict, y_test, algorithm_name)
         save_fig(f'True Value vs. Predicted Value - {algorithm_name}', store_path)
 
     @staticmethod
     def _score(y_true: pd.DataFrame, y_predict: pd.DataFrame) -> None:
+        """Calculate the score of the model."""
         print("-----* Model Score *-----")
         score(y_true, y_predict)
 
     @staticmethod
     def _cross_validation(trained_model: object, X_train: pd.DataFrame, y_train: pd.DataFrame, cv_num: int = 10) -> None:
+        """Cross validation."""
         print("-----* Cross Validation *-----")
         print(f"K-Folds: {cv_num}")
         cross_validation(trained_model, X_train, y_train, cv_num=cv_num)
 
     # TODO(Sany sanyhew1097618435@163.com): How to prevent overfitting
     def is_overfitting(self):
         pass
@@ -141,65 +153,80 @@
                                               self.naming, MODEL_OUTPUT_IMAGE_PATH)
         self._plot_true_vs_predicted(y_test_predict=RegressionWorkflowBase.y_test_predict,
                                      y_test=RegressionWorkflowBase.y_test, algorithm_name=self.naming,
                                      store_path=MODEL_OUTPUT_IMAGE_PATH)
 
 
 class PolynomialRegression(RegressionWorkflowBase):
+    """The automation workflow of using Polynomial Regression algorithm to make insightful products."""
 
     name = "Polynomial Regression"
     special_function = ["Polynomial Regression Formula"]
 
-    def __init__(self,
-                 degree: int = 2,
-                 interaction_only: bool = False,
-                 is_include_bias: bool = False,
-                 order: str = 'C',
-                 fit_intercept: bool = True,
-                 normalize: bool = False,
-                 copy_X: bool = True,
-                 n_jobs: Optional[int] = None) -> None:
+    def __init__(
+        self,
+        degree: int = 2,
+        interaction_only: bool = False,
+        include_bias: bool = False,
+        order: str = 'C',
+        fit_intercept: bool = True,
+        normalize: bool = False,
+        copy_X: bool = True,
+        n_jobs: Optional[int] = None
+    ) -> None:
 
         super().__init__()
         self.degree = degree
-        self.is_include_bias = is_include_bias
+        self.include_bias = include_bias
         self.interaction_only = interaction_only
         self.order = order
         self.fit_intercept = fit_intercept
         self.normalize = normalize
         self.copy_X = copy_X
         self.n_jobs = n_jobs
 
-        self.model = LinearRegression(fit_intercept=self.fit_intercept,
-                                      copy_X=self.copy_X,
-                                      n_jobs=self.n_jobs)
+        self.model = LinearRegression(
+            fit_intercept=self.fit_intercept,
+            copy_X=self.copy_X,
+            n_jobs=self.n_jobs
+        )
 
         self._features_name = None
         self.naming = PolynomialRegression.name
 
-    def poly(self, X_train, X_test):
+    def poly(self, X_train: pd.DataFrame, X_test: pd.DataFrame) -> Tuple[pd.DataFrame, pd.DataFrame]:
+        """Polynomial features."""
         poly_features = PolynomialFeatures(degree=self.degree,
-                                           include_bias=self.is_include_bias,
+                                           include_bias=self.include_bias,
                                            interaction_only=self.interaction_only,
                                            order=self.order)
         X_train_poly = poly_features.fit_transform(X_train)
         X_test_poly = poly_features.fit_transform(X_test)
         try:
             # scikit-learn >= 1.0
             self._features_name = poly_features.get_feature_names_out()
         except AttributeError:
             self._features_name = poly_features.get_feature_names()
         return X_train_poly, X_test_poly
 
+    @classmethod
+    def manual_hyper_parameters(cls) -> Dict:
+        """Manual hyper-parameters specification."""
+        print(f"-*-*- {cls.name} - Hyper-parameters Specification -*-*-")
+        hyper_parameters = polynomial_regression_manual_hyper_parameters()
+        return hyper_parameters
+
     @staticmethod
-    def _show_formula(coef, intercept, features_name):
+    def _show_formula(coef: np.ndarray, intercept: np.ndarray, features_name: List) -> None:
+        """Show the formula of the polynomial regression."""
         print("-----* Polynomial Regression Formula *-----")
         show_formula(coef, intercept, features_name)
 
-    def special_components(self, **kwargs):
+    def special_components(self, **kwargs) -> None:
+        """Invoke all special application functions for this algorithms by Scikit-learn framework."""
         self._show_formula(coef=self.model.coef_, intercept=self.model.intercept_, features_name=self._features_name)
 
 
 class XgboostRegression(RegressionWorkflowBase):
     """The automation workflow of using Xgboost algorithm to make insightful products."""
 
     name = "Xgboost"
@@ -211,47 +238,48 @@
         Union[
             str, Callable[[np.ndarray, np.ndarray], Tuple[np.ndarray, np.ndarray]]
         ]
     ]
 
     # TODO: find out the attributes importance_type effect
     def __init__(
-                self,
-                max_depth: Optional[int] = 6,
-                learning_rate: Optional[float] = 0.3,
-                n_estimators: int = 100,
-                verbosity: Optional[int] = 1,
-                objective: _SklObjective = None,
-                booster: Optional[str] = None,
-                tree_method: Optional[str] = 'auto',
-                n_jobs: Optional[int] = None,
-                gamma: Optional[float] = 0,
-                min_child_weight: Optional[float] = None,
-                max_delta_step: Optional[float] = 0,
-                subsample: Optional[float] = 1,
-                colsample_bytree: Optional[float] = 1,
-                colsample_bylevel: Optional[float] = 1,
-                colsample_bynode: Optional[float] = 1,
-                reg_alpha: Optional[float] = 0,
-                reg_lambda: Optional[float] = 1,
-                scale_pos_weight: Optional[float] = 1,
-                base_score: Optional[float] = None,
-                random_state: Optional[Union[np.random.RandomState, int]] = None,
-                missing: float = np.nan,
-                num_parallel_tree: Optional[int] = 1,
-                monotone_constraints: Optional[Union[Dict[str, int], str]] = None,
-                interaction_constraints: Optional[Union[str, Sequence[Sequence[str]]]] = None,
-                importance_type: Optional[str] = 'gain',
-                gpu_id: Optional[int] = None,
-                validate_parameters: Optional[bool] = None,
-                predictor: Optional[str] = None,
-                #enable_categorical: bool = False,
-                eval_metric: Optional[Union[str, List[str], Callable]] = None,
-                early_stopping_rounds: Optional[int] = None,
-                **kwargs: Any) -> None:
+        self,
+        max_depth: Optional[int] = 6,
+        learning_rate: Optional[float] = 0.3,
+        n_estimators: int = 100,
+        verbosity: Optional[int] = 1,
+        objective: _SklObjective = None,
+        booster: Optional[str] = None,
+        tree_method: Optional[str] = 'auto',
+        n_jobs: Optional[int] = None,
+        gamma: Optional[float] = 0,
+        min_child_weight: Optional[float] = None,
+        max_delta_step: Optional[float] = 0,
+        subsample: Optional[float] = 1,
+        colsample_bytree: Optional[float] = 1,
+        colsample_bylevel: Optional[float] = 1,
+        colsample_bynode: Optional[float] = 1,
+        reg_alpha: Optional[float] = 0,
+        reg_lambda: Optional[float] = 1,
+        scale_pos_weight: Optional[float] = 1,
+        base_score: Optional[float] = None,
+        random_state: Optional[Union[np.random.RandomState, int]] = None,
+        missing: float = np.nan,
+        num_parallel_tree: Optional[int] = 1,
+        monotone_constraints: Optional[Union[Dict[str, int], str]] = None,
+        interaction_constraints: Optional[Union[str, Sequence[Sequence[str]]]] = None,
+        importance_type: Optional[str] = 'gain',
+        gpu_id: Optional[int] = None,
+        validate_parameters: Optional[bool] = None,
+        predictor: Optional[str] = None,
+        #enable_categorical: bool = False,
+        eval_metric: Optional[Union[str, List[str], Callable]] = None,
+        early_stopping_rounds: Optional[int] = None,
+        **kwargs: Any
+    ) -> None:
         """
         Parameters
         ----------
         max_depth [default=6]
             Maximum depth of a tree. Increasing this value will make the model more complex and more likely to overfit.
             0 indicates no limit on depth. Beware that XGBoost aggressively consumes memory when training a deep tree.
             exact tree method requires non-zero value.
@@ -262,16 +290,14 @@
             After each boosting step, we can directly get the weights of new features,
             and eta shrinks the feature weights to make the boosting process more conservative.
             range: [0,1]
 
         n_estimators : int
         Number of gradient boosted trees.  Equivalent to number of boosting rounds.
 
-
-
         objective : {SklObjective}
             Specify the learning task and the corresponding learning objective or
             a custom objective function to be used (see note below).
 
         verbosity [default=1]
             Verbosity of printing messages. Valid values are 0 (silent), 1 (warning), 2 (info), 3 (debug).
             Sometimes XGBoost tries to change configurations based on heuristics,
@@ -407,15 +433,16 @@
 
         eval_metric : Optional[Union[str, List[str], Callable]]
 
         early_stopping_rounds : Optional[int]
 
         References
         ----------
-        [1] https://xgboost.readthedocs.io/en/stable/parameter.html#
+        [1] Xgboost Python API Reference - Scikit-Learn API
+            https://xgboost.readthedocs.io/en/latest/python/python_api.html#module-xgboost.sklearn
 
         [2] Xgboost API for the scikit-learn wrapper:
             https://github.com/dmlc/xgboost/blob/master/python-package/xgboost/sklearn.py
         """
 
         super().__init__()
         self.n_estimators = n_estimators
@@ -448,45 +475,48 @@
         self.predictor = predictor
         #self.enable_categorical = enable_categorical
         self.eval_metric = eval_metric
         self.early_stopping_rounds = early_stopping_rounds
         if kwargs:
             self.kwargs = kwargs
 
-        self.model = xgboost.XGBRegressor(n_estimators=self.n_estimators,
-                                          objective=self.objective,
-                                          max_depth=self.max_depth,
-                                          learning_rate=self.learning_rate,
-                                          verbosity=self.verbosity,
-                                          booster=self.booster,
-                                          tree_method=self.tree_method,
-                                          gamma=self.gamma,
-                                          min_child_weight=self.min_child_weight,
-                                          max_delta_step=self.max_delta_step,
-                                          subsample=self.subsample,
-                                          colsample_bytree=self.colsample_bytree,
-                                          colsample_bylevel=self.colsample_bylevel,
-                                          colsample_bynode=self.colsample_bynode,
-                                          reg_alpha=self.reg_alpha,
-                                          reg_lambda=self.reg_lambda,
-                                          scale_pos_weight=self.scale_pos_weight,
-                                          base_score=self.base_score,
-                                          missing=self.missing,
-                                          num_parallel_tree=self.num_parallel_tree,
-                                          random_state=self.random_state,
-                                          n_jobs=self.n_jobs,
-                                          monotone_constraints=self.monotone_constraints,
-                                          interaction_constraints=self.interaction_constraints,
-                                          importance_type=self.importance_type,
-                                          gpu_id=self.gpu_id,
-                                          validate_parameters=self.validate_parameters,
-                                          predictor=self.predictor,
-                                          # enable_categorical=self.enable_categorical,
-                                          eval_metric=self.eval_metric,
-                                          early_stopping_rounds=self.early_stopping_rounds)
+        self.model = xgboost.XGBRegressor(
+            n_estimators=self.n_estimators,
+            objective=self.objective,
+            max_depth=self.max_depth,
+            learning_rate=self.learning_rate,
+            verbosity=self.verbosity,
+            booster=self.booster,
+            tree_method=self.tree_method,
+            gamma=self.gamma,
+            min_child_weight=self.min_child_weight,
+            max_delta_step=self.max_delta_step,
+            subsample=self.subsample,
+            colsample_bytree=self.colsample_bytree,
+            colsample_bylevel=self.colsample_bylevel,
+            colsample_bynode=self.colsample_bynode,
+            reg_alpha=self.reg_alpha,
+            reg_lambda=self.reg_lambda,
+            scale_pos_weight=self.scale_pos_weight,
+            base_score=self.base_score,
+            missing=self.missing,
+            num_parallel_tree=self.num_parallel_tree,
+            random_state=self.random_state,
+            n_jobs=self.n_jobs,
+            monotone_constraints=self.monotone_constraints,
+            interaction_constraints=self.interaction_constraints,
+            importance_type=self.importance_type,
+            gpu_id=self.gpu_id,
+            validate_parameters=self.validate_parameters,
+            predictor=self.predictor,
+            # enable_categorical=self.enable_categorical,
+            eval_metric=self.eval_metric,
+            early_stopping_rounds=self.early_stopping_rounds
+        )
+
         self.naming = XgboostRegression.name
 
     @property
     def settings(self) -> Dict:
         """The configuration to implement AutoML by FLAML framework."""
         configuration = {
             "time_budget": 10,  # total running time in seconds
@@ -494,28 +524,38 @@
             "estimator_list": ['xgboost'],  # list of ML learners
             "task": 'regression',  # task type
             # "log_file_name": f'{self.naming} - automl.log',  # flaml log file
             # "log_training_metric": True,  # whether to log training metric
         }
         return configuration
 
+    @classmethod
+    def manual_hyper_parameters(cls) -> Dict:
+        """Manual hyper-parameters specification."""
+        print(f"-*-*- {cls.name} - Hyper-parameters Specification -*-*-")
+        hyper_parameters = xgboost_manual_hyper_parameters()
+        return hyper_parameters
+
     @staticmethod
     def _feature_importance(X: pd.DataFrame, trained_model: object, image_config: dict, algorithm_name: str, store_path: str) -> None:
+        """Feature importance plot."""
         print("-----* Feature Importance *-----")
         feature_importance(X, trained_model, image_config)
         save_fig(f"Feature Importance - {algorithm_name}", store_path)
 
     @staticmethod
     def _histograms_feature_weights(X: pd.DataFrame, trained_model: object, image_config: dict, algorithm_name: str, store_path: str) -> None:
+        """Histograms of feature weights plot."""
         histograms_feature_weights(X, trained_model,image_config)
         save_fig(f"Regression - {algorithm_name} - Feature Importance Score", store_path)
 
     @staticmethod
     def _permutation_importance(X: pd.DataFrame, X_test: pd.DataFrame, y_test: pd.DataFrame, trained_model: object,
                                 image_config: dict, algorithm_name: str, store_path: str) -> None:
+        """Permutation importance plot."""
         permutation_importance_(X, X_test, y_test, trained_model, image_config)
         save_fig(f"Regression - {algorithm_name} - Xgboost Feature Importance", store_path)
 
     @dispatch()
     def special_components(self, **kwargs) -> None:
         """Invoke all special application functions for this algorithms by Scikit-learn framework."""
         self._feature_importance(XgboostRegression.X, self.model, self.image_config, self.naming, MODEL_OUTPUT_IMAGE_PATH)
@@ -529,31 +569,32 @@
         self._feature_importance(XgboostRegression.X, self.auto_model, self.image_config, self.naming, MODEL_OUTPUT_IMAGE_PATH)
         self._histograms_feature_weights(XgboostRegression.X, self.auto_model, self.image_config, self.naming, MODEL_OUTPUT_IMAGE_PATH)
         self._permutation_importance(XgboostRegression.X, XgboostRegression.X_test, XgboostRegression.y_test,
                                      self.auto_model, self.image_config, self.naming, MODEL_OUTPUT_IMAGE_PATH)
 
 
 class DecisionTreeRegression(RegressionWorkflowBase):
-    """The automation workflow of using Extra Tree algorithm to make insightful products."""
+    """The automation workflow of using Decision Tree algorithm to make insightful products."""
 
     name = "Decision Tree"
     special_function = ["Decision Tree Plot"]
 
-    def __init__(self,
-                 criterion: str = 'squared_error',
-                 splitter: str = 'best',
-                 max_depth: Optional[int] = None,
-                 min_samples_split: Union[int, float] = 2,
-                 min_samples_leaf: Union[int, float] = 1,
-                 min_weight_fraction_leaf: float = 0.0,
-                 max_features: Union[int, float, str, None] = None,
-                 random_state: Optional[int] = None,
-                 max_leaf_nodes: Optional[int] = None,
-                 min_impurity_decrease: float = 0.0,
-                 ccp_alpha: float = 0.0
+    def __init__(
+        self,
+        criterion: str = 'squared_error',
+        splitter: str = 'best',
+        max_depth: Optional[int] = None,
+        min_samples_split: Union[int, float] = 2,
+        min_samples_leaf: Union[int, float] = 1,
+        min_weight_fraction_leaf: float = 0.0,
+        max_features: Union[int, float, str, None] = None,
+        random_state: Optional[int] = None,
+        max_leaf_nodes: Optional[int] = None,
+        min_impurity_decrease: float = 0.0,
+        ccp_alpha: float = 0.0
     ) -> None:
         """
         Parameters
         ----------
         criterion : {"squared_error", "friedman_mse", "absolute_error", \
                 "poisson"}, default="squared_error"
             The function to measure the quality of a split. Supported criteria
@@ -668,21 +709,16 @@
             subtree with the largest cost complexity that is smaller than
             ``ccp_alpha`` will be chosen. By default, no pruning is performed. See
             :ref:`minimal_cost_complexity_pruning` for details.
             .. versionadded:: 0.22
 
         References
         ----------
-        [1] https://en.wikipedia.org/wiki/Decision_tree_learning
-        [2] L. Breiman, J. Friedman, R. Olshen, and C. Stone, "Classification
-               and Regression Trees", Wadsworth, Belmont, CA, 1984.
-        [3] T. Hastie, R. Tibshirani and J. Friedman. "Elements of Statistical
-               Learning", Springer, 2009.
-        [4] L. Breiman, and A. Cutler, "Random Forests",
-               https://www.stat.berkeley.edu/~breiman/RandomForests/cc_home.htm
+        Scikit-learn API: sklearn.tree.DecisionTreeClassifier
+        https://scikit-learn.org/stable/modules/generated/sklearn.tree.DecisionTreeClassifier.html#sklearn.tree.DecisionTreeClassifier
         """
 
         super().__init__()
         self.criterion = criterion,
         self.splitter = splitter,
         # FIXME (Sany sanyhew1097618435@163.com): figure out why data type changes after assignment.
         # print("max_depth before: ", max_depth)
@@ -696,27 +732,84 @@
         self.max_features = max_features,
         self.random_state = random_state,
         self.max_leaf_nodes = max_leaf_nodes,
         self.min_impurity_decrease = min_impurity_decrease,
         self.ccp_alpha = ccp_alpha
 
         self.model = DecisionTreeRegressor(
-                                           criterion=self.criterion[0],
-                                           splitter=self.splitter[0],
-                                           max_depth=self.max_depth[0],
-                                           min_samples_split=self.min_samples_split[0],
-                                           min_samples_leaf=self.min_samples_leaf[0],
-                                           min_weight_fraction_leaf=self.min_weight_fraction_leaf[0],
-                                           max_features=self.max_features[0],
-                                           random_state=self.random_state[0],
-                                           max_leaf_nodes=self.max_leaf_nodes[0],
-                                           min_impurity_decrease=self.min_impurity_decrease[0],
-                                           ccp_alpha=self.ccp_alpha
+            criterion=self.criterion[0],
+            splitter=self.splitter[0],
+            max_depth=self.max_depth[0],
+            min_samples_split=self.min_samples_split[0],
+            min_samples_leaf=self.min_samples_leaf[0],
+            min_weight_fraction_leaf=self.min_weight_fraction_leaf[0],
+            max_features=self.max_features[0],
+            random_state=self.random_state[0],
+            max_leaf_nodes=self.max_leaf_nodes[0],
+            min_impurity_decrease=self.min_impurity_decrease[0],
+            ccp_alpha=self.ccp_alpha
         )
         self.naming = DecisionTreeRegression.name
+        self.customized = True
+        self.customized_name = 'Decision Tree'
+
+    @property
+    def settings(self) -> Dict:
+        """The configuration of Decision Tree to implement AutoML by FLAML framework."""
+        configuration = {
+            "time_budget": 10,  # total running time in seconds
+            "metric": 'r2',
+            "estimator_list": [self.customized_name],  # list of ML learners
+            "task": 'regression',  # task type
+            # "log_file_name": f'{self.naming} - automl.log',  # flaml log file
+            # "log_training_metric": True,  # whether to log training metric
+        }
+        return configuration
+    
+    @property
+    def customization(self) -> object:
+        """The customized Decision Tree of FLAML framework."""
+        from flaml.model import SKLearnEstimator
+        from flaml import tune
+        from flaml.data import REGRESSION
+        from sklearn.tree import DecisionTreeRegressor
+
+        class MyDTRegression(SKLearnEstimator):
+            def __init__(self, task='regression', n_jobs=None, **config):
+                super().__init__(task, **config)
+                if task in REGRESSION:
+                    self.estimator_class = DecisionTreeRegressor
+
+            @classmethod
+            def search_space(cls, data_size, task):
+                space = {
+                    'criterion': {'domain': tune.choice(["squared_error", "friedman_mse", "absolute_error", "poisson"])},
+                    'max_depth': {'domain': tune.randint(lower=2, upper=20),
+                                  'init_value': 1,
+                                  'low_cost_init_value': 1},
+                    'min_samples_split': {'domain': tune.randint(lower=2, upper=10),
+                                          'init_value': 2,
+                                          'low_cost_init_value': 2},
+                    'min_samples_leaf': {'domain': tune.randint(lower=1, upper=10),
+                                         'init_value': 1,
+                                         'low_cost_init_value': 1},
+                    'max_features': {'domain': tune.randint(lower=1, upper=10),
+                                     'init_value': 1,
+                                     'low_cost_init_value': 1},
+                }
+                return space
+
+        return MyDTRegression
+
+    @classmethod
+    def manual_hyper_parameters(cls) -> Dict:
+        """Manual hyper-parameters specification."""
+        print(f"-*-*- {cls.name} - Hyper-parameters Specification -*-*-")
+        hyper_parameters = decision_tree_manual_hyper_parameters()
+        return hyper_parameters
 
     def _plot_tree_function(self, trained_model: object, image_config: dict, algorithm_name: str, store_path: str) -> None:
         """Drawing decision tree diagrams."""
         print("-----* Decision Tree Plot *-----")
         decision_tree_plot(trained_model, image_config)
         save_fig(f"Regression - {algorithm_name} - Tree Graph", store_path)
 
@@ -725,30 +818,43 @@
         """Invoke all special application functions for this algorithms by Scikit-learn framework."""
         self._plot_tree_function(self.model, self.image_config, self.naming, MODEL_OUTPUT_IMAGE_PATH)
         
 
     @dispatch(bool)
     def special_components(self, is_automl: bool = False, **kwargs) -> None:
         """Invoke all special application functions for this algorithms by FLAML framework."""
-        self._plot_tree_function(self.model, self.image_config, self.naming, MODEL_OUTPUT_IMAGE_PATH)
+        self._plot_tree_function(self.auto_model, self.image_config, self.naming, MODEL_OUTPUT_IMAGE_PATH)
         
 
-class ExtraTreeRegression(RegressionWorkflowBase):
-    """The automation workflow of using Extra Tree algorithm to make insightful products."""
+class ExtraTreesRegression(RegressionWorkflowBase):
+    """The automation workflow of using Extra-Trees algorithm to make insightful products."""
     
     name = "Extra-Trees"
     special_function = ["Feature Importance"]
 
-    def __init__(self,
-                 n_estimator: int = 500,
-                 bootstrap: bool = False,
-                 oob_score: bool = False,
-                 max_leaf_nodes: int = 20,
-                 random_state: int = 42,
-                 n_jobs: int = -1
+    def __init__(
+        self,
+        n_estimators: int = 100,
+        criterion: str = "mse",
+        max_depth: Optional[int] = None,
+        min_samples_split: Union[int, float] = 2,
+        min_samples_leaf: Union[int, float] = 1,
+        min_weight_fraction_leaf: float = 0.,
+        max_features: Union[int, float, str] = "auto",
+        max_leaf_nodes: int = None,
+        min_impurity_decrease: float = 0.,
+    #  min_impurity_split=None,
+        bootstrap=False,
+        oob_score=False,
+        n_jobs=None,
+        random_state=None,
+        verbose=0,
+        warm_start=False,
+        ccp_alpha: float = 0.0,
+        max_samples=None
     ) -> None:
         """
         Parameters
         ----------
         n_estimators : int, default=100
             The number of trees in the forest.
 
@@ -899,77 +1005,125 @@
             - If float, then draw `max_samples * X.shape[0]` samples. Thus,
               `max_samples` should be in the interval `(0.0, 1.0]`.
 
             .. versionadded:: 0.22
 
         References
         ----------
-        scikit API: sklearn.ensemble.ExtraTreesRegressor
+        Scikit-learn API: sklearn.ensemble.ExtraTreesRegressor
         https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.ExtraTreesRegressor.html?highlight=extratreesregressor#sklearn.ensemble.ExtraTreesRegressor
         """
         
         super().__init__()
-        self.n_estimators = n_estimator
+        self.n_estimators = n_estimators
+        self.criterion = criterion
+        self.max_depth = max_depth
+        self.min_samples_split = min_samples_split
+        self.min_samples_leaf = min_samples_leaf
+        self.min_weight_fraction_leaf = min_weight_fraction_leaf
+        self.max_features = max_features
+        self.max_leaf_nodes = max_leaf_nodes
+        self.min_impurity_decrease = min_impurity_decrease
+        # self.min_impurity_split = min_impurity_split
         self.bootstrap = bootstrap
         self.oob_score = oob_score
-        self.max_leaf_nodes = max_leaf_nodes
-        self.random_state = random_state
         self.n_jobs = n_jobs
+        self.random_state = random_state
+        self.verbose = verbose
+        self.warm_start = warm_start
+        self.ccp_alpha = ccp_alpha
+        self.max_samples = max_samples
+
+        self.model = ExtraTreesRegressor(
+            n_estimators=self.n_estimators,
+            criterion=self.criterion,
+            max_depth=self.max_depth,
+            min_samples_split=self.min_samples_split,
+            min_samples_leaf=self.min_samples_leaf,
+            min_weight_fraction_leaf=self.min_weight_fraction_leaf,
+            max_features=self.max_features,
+            max_leaf_nodes=self.max_leaf_nodes,
+            min_impurity_decrease=self.min_impurity_decrease,
+            # min_impurity_split=self.min_impurity_split,
+            bootstrap=self.bootstrap,
+            oob_score=self.oob_score,
+            n_jobs=self.n_jobs,
+            random_state=self.random_state,
+            verbose=self.verbose,
+            warm_start=self.warm_start,
+            ccp_alpha=self.ccp_alpha,
+            max_samples=self.max_samples,
+        )
 
-        self.model = ExtraTreesRegressor(n_estimators=self.n_estimators,
-                                         bootstrap=self.bootstrap,
-                                         oob_score=self.oob_score,
-                                         max_leaf_nodes=self.max_leaf_nodes,
-                                         random_state=self.random_state,
-                                         n_jobs=self.n_jobs)
-        self.naming = ExtraTreeRegression.name
+        self.naming = ExtraTreesRegression.name
 
     @property
     def settings(self) -> Dict:
         """The configuration to implement AutoML by FLAML framework."""
         configuration = {
             "time_budget": 10,  # total running time in seconds
             "metric": 'r2',
             "estimator_list": ['extra_tree'],  # list of ML learners
             "task": 'regression',  # task type
             # "log_file_name": f'{self.naming} - automl.log',  # flaml log file
             # "log_training_metric": True,  # whether to log training metric
         }
         return configuration
 
+    @classmethod
+    def manual_hyper_parameters(cls) -> Dict:
+        """Manual hyper-parameters specification."""
+        print(f"-*-*- {cls.name} - Hyper-parameters Specification -*-*-")
+        hyper_parameters = extra_trees_manual_hyper_parameters()
+        return hyper_parameters
+
     @staticmethod
     def _feature_importances(X_train: pd.DataFrame, trained_model: object,  image_config: dict, algorithm_name: str, store_path: str) -> None:
         """Draw the feature importance bar diagram."""
         print("-----* Feature Importance *-----")
         feature_importances(X_train, trained_model, image_config)
         save_fig(f"Regression - {algorithm_name} - Feature Importance Plot", store_path)
 
     @dispatch()
     def special_components(self, **kwargs) -> None:
         """Invoke all special application functions for this algorithms by Scikit-learn framework."""
-        self._feature_importances(ExtraTreeRegression.X_train, self.model,  self.image_config, self.naming, MODEL_OUTPUT_IMAGE_PATH)
+        self._feature_importances(ExtraTreesRegression.X_train, self.model,  self.image_config, self.naming, MODEL_OUTPUT_IMAGE_PATH)
 
     @dispatch(bool)
     def special_components(self, is_automl: bool = False, **kwargs) -> None:
         """Invoke all special application functions for this algorithms by FLAML framework."""
-        self._feature_importances(ExtraTreeRegression.X_train, self.auto_model, self.image_config, self.naming, MODEL_OUTPUT_IMAGE_PATH)
+        self._feature_importances(ExtraTreesRegression.X_train, self.auto_model, self.image_config, self.naming, MODEL_OUTPUT_IMAGE_PATH)
 
 
 class RandomForestRegression(RegressionWorkflowBase):
     """The automation workflow of using Random Forest algorithm to make insightful products."""
 
     name = "Random Forest"
     special_function = ["Feature Importance"]
 
-    def __init__(self,
-                 n_estimators: int = 500,
-                 oob_score: bool = True,
-                 max_leaf_nodes: int = 15,
-                 n_jobs: int = -1,
-                 random_state: int = 42
+    def __init__(   
+        self,
+        n_estimators=100,
+        criterion="mse",
+        max_depth=None,
+        min_samples_split=2,
+        min_samples_leaf=1,
+        min_weight_fraction_leaf=0.0,
+        max_features="sqrt",
+        max_leaf_nodes=None,
+        min_impurity_decrease=0.0,
+        bootstrap=True,
+        oob_score=False,
+        n_jobs=None,
+        random_state=None,
+        verbose=0,
+        warm_start=False,
+        # class_weight=None,
+        ccp_alpha=0.0,
+        max_samples=None,
     ) -> None:
         """
         Parameters
         ----------
         n_estimators : int, default=100
             The number of trees in the forest.
 
@@ -1123,30 +1277,58 @@
             - If float, then draw `max_samples * X.shape[0]` samples. Thus,
               `max_samples` should be in the interval `(0.0, 1.0]`.
 
             .. versionadded:: 0.22
 
         References
         ----------
-        scikit API: sklearn.ensemble.RandomForestRegressor
+        Scikit-learn API: sklearn.ensemble.RandomForestRegressor
         https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestRegressor.html?highlight=randomforestregressor#sklearn.ensemble.RandomForestRegressor
         """
         
         super().__init__()
         self.n_estimators = n_estimators
-        self.oob_score = oob_score
+        self.criterion = criterion
+        self.max_depth = max_depth
+        self.min_samples_split = min_samples_split
+        self.min_samples_leaf = min_samples_leaf
+        self.min_weight_fraction_leaf = min_weight_fraction_leaf
+        self.max_features = max_features
         self.max_leaf_nodes = max_leaf_nodes
+        self.min_impurity_decrease = min_impurity_decrease
+        self.bootstrap = bootstrap
+        self.oob_score = oob_score
         self.n_jobs = n_jobs
         self.random_state = random_state
+        self.verbose = verbose
+        self.warm_start = warm_start
+        # self.class_weight = class_weight
+        self.ccp_alpha = ccp_alpha
+        self.max_samples=max_samples
 
-        self.model = RandomForestRegressor(n_estimators=self.n_estimators,
-                                           oob_score=self.oob_score,
-                                           max_leaf_nodes=self.max_leaf_nodes,
-                                           n_jobs=self.n_jobs,
-                                           random_state=self.random_state)
+        self.model = RandomForestRegressor(
+            n_estimators=self.n_estimators,
+            criterion=self.criterion,
+            max_depth=self.max_depth,
+            min_samples_split=self.min_samples_split,
+            min_samples_leaf=self.min_samples_leaf,
+            min_weight_fraction_leaf=self.min_weight_fraction_leaf,
+            max_features=self.max_features,
+            max_leaf_nodes=self.max_leaf_nodes,
+            min_impurity_decrease=self.min_impurity_decrease,
+            bootstrap=self.bootstrap,
+            oob_score=self.oob_score,
+            n_jobs=self.n_jobs,
+            random_state=self.random_state,
+            verbose=self.verbose,
+            warm_start=self.warm_start,
+            # class_weight=self.class_weight,
+            ccp_alpha=self.ccp_alpha,
+            max_samples=self.max_samples,
+        )
         self.naming = RandomForestRegression.name
 
     @property
     def settings(self) -> Dict:
         """The configuration to implement AutoML by FLAML framework."""
         configuration = {
             "time_budget": 10,  # total running time in seconds
@@ -1154,24 +1336,33 @@
             "estimator_list": ['rf'],  # list of ML learners
             "task": 'regression',  # task type
             # "log_file_name": f'{self.naming} - automl.log',  # flaml log file
             # "log_training_metric": True,  # whether to log training metric
         }
         return configuration
 
+    @classmethod
+    def manual_hyper_parameters(cls) -> Dict:
+        """Manual hyper-parameters specification."""
+        print(f"-*-*- {cls.name} - Hyper-parameters Specification -*-*-")
+        hyper_parameters = random_forest_manual_hyper_parameters()
+        return hyper_parameters
+
     @staticmethod
     def _feature_importances(X: pd.DataFrame, X_test: pd.DataFrame, y_test: pd.DataFrame,
                              trained_model: object,  image_config: dict, algorithm_name: str, store_path: str) -> None:
+        """Feature importance plot."""
         print("-----* Feature Importance *-----")
         feature_importance__(X, X_test, y_test, trained_model, image_config)
         save_fig(f"Regression - {algorithm_name} - Feature Importance", store_path)
 
     @staticmethod
     def _box_plot(X: pd.DataFrame, X_test: pd.DataFrame, y_test: pd.DataFrame,
                  trained_model: object,  image_config: dict, algorithm_name: str, store_path: str) -> None:
+        """Box plot."""
         print("-----* Box Plot *-----")
         box_plot(X, X_test, y_test, trained_model, image_config)
         save_fig(f"Regression - {algorithm_name} - Box Plot", store_path)
 
     @dispatch()
     def special_components(self, **kwargs) -> None:
         """Invoke all special application functions for this algorithms by Scikit-learn framework."""
@@ -1193,22 +1384,22 @@
                                   MODEL_OUTPUT_IMAGE_PATH)
 
 
 class SVMRegression(RegressionWorkflowBase):
     """The automation workflow of using SVR algorithm to make insightful products."""
 
     name = "Support Vector Machine"
-    special_function = []
+    special_function = ['Two-dimensional Decision Boundary Diagram']
 
     def __init__(
         self,
-        kernel='rbf',
+        kernel: str = 'rbf',
         degree: int = 3,
-        gamma='scale',
-        coef0: float = 0.0,
+        gamma: Union[str, float] = 'scale',
+        # coef0: float = 0.0,
         tol: float = 1e-3,
         C: float = 1.0,
         epsilon: float = 0.1,
         shrinking: bool = True,
         cache_size: float = 200,
         verbose: bool = False,
         max_iter: int = -1,
@@ -1264,46 +1455,44 @@
             properly in a multithreaded context.
 
         max_iter : int, default=-1
             Hard limit on iterations within solver, or -1 for no limit.
 
         References
         ----------
-        .. [1] `LIBSVM: A Library for Support Vector Machines
-            <http://www.csie.ntu.edu.tw/~cjlin/papers/libsvm.pdf>`_
-          
-        .. [2] `Platt, John (1999). "Probabilistic outputs for support vector
-            machines and comparison to regularizedlikelihood methods."
-            <http://citeseer.ist.psu.edu/viewdoc/summary?doi=10.1.1.41.1639>`_
+        Scikit-learn API: sklearn.svm.SVR
+        https://scikit-learn.org/stable/modules/generated/sklearn.svm.SVR.html
         """
         
         super().__init__()
         self.kernel = kernel
         self.degree = degree
         self.gamma = gamma
-        self.coef0 = coef0
+        # self.coef0 = coef0
         self.tol = tol
         self.C = C
         self.epsilon = epsilon
         self.shrinking = shrinking
         self.cache_size = cache_size
         self.verbose = verbose
         self.max_iter = max_iter
 
-        self.model = SVR(kernel=self.kernel,
-                        degree=self.degree,
-                        gamma=self.gamma,
-                        coef0=self.coef0,
-                        tol=self.tol,
-                        C=self.C,
-                        epsilon=self.epsilon,
-                        shrinking=self.shrinking,
-                        cache_size=self.cache_size,
-                        verbose=self.verbose,
-                        max_iter=self.max_iter)
+        self.model = SVR(
+            kernel=self.kernel,
+            degree=self.degree,
+            gamma=self.gamma,
+            # coef0=self.coef0,
+            tol=self.tol,
+            C=self.C,
+            epsilon=self.epsilon,
+            shrinking=self.shrinking,
+            cache_size=self.cache_size,
+            verbose=self.verbose,
+            max_iter=self.max_iter
+        )
 
         self.naming = SVMRegression.name
         self.customized = True
         self.customized_name = 'SVR'
 
     @property
     def settings(self) -> Dict:
@@ -1331,62 +1520,104 @@
                 super().__init__(task, **config)
                 if task in REGRESSION:
                     self.estimator_class = SVR
 
             @classmethod
             def search_space(cls, data_size, task):
                 space = {
-                    'C': {'domain': tune.uniform(lower=1, upper=data_size[0]),
-                          'init_value': 1,
-                          'low_cost_init_value': 1}
+                    'C': {
+                        'domain': tune.uniform(lower=1, upper=data_size[0]),
+                        'init_value': 1,
+                        'low_cost_init_value': 1
+                    },
+                    'kernel': {'domain': tune.choice(['poly', 'rbf', 'sigmoid'])},
+                    'gamma': {
+                        'domain': tune.uniform(lower=1e-5, upper=10),
+                        'init_value': 1e-1,
+                        'low_cost_init_value': 1e-1
+                    },
+                    'degree': {
+                        'domain': tune.quniform(lower=1, upper=5, q=1),
+                        'init_value': 3,
+                        'low_cost_init_value': 3
+                    },
+                    'coef0': {
+                        'domain': tune.uniform(lower=0, upper=1),
+                        'init_value': 0,
+                        'low_cost_init_value': 0
+                    },
+                    'shrinking': {'domain': tune.choice([True, False])},
                 }
                 return space
 
         return MySVMRegression
 
+    @classmethod
+    def manual_hyper_parameters(cls) -> Dict:
+        """Manual hyper-parameters specification."""
+        print(f"-*-*- {cls.name} - Hyper-parameters Specification -*-*-")
+        hyper_parameters = svr_manual_hyper_parameters()
+        return hyper_parameters
+
+    @staticmethod
+    def _plot_2d_decision_boundary(X: pd.DataFrame, X_test: pd.DataFrame, y_test: pd.DataFrame, trained_model: Any,
+                                   image_config: dict, algorithm_name: str, store_path: str,
+                                   contour_data: Optional[List[np.ndarray]] = None,
+                                   labels: Optional[np.ndarray] = None) -> None:
+        """Plot the decision boundary of the trained model with the testing data set below."""
+        print("-----* Two-dimensional Decision Boundary Diagram *-----")
+        plot_2d_decision_boundary(X, X_test, y_test, trained_model, image_config, algorithm_name)
+        save_fig(f'Regression - {algorithm_name} - Decision Boundary', store_path)
+
     @dispatch()
     def special_components(self, **kwargs):
         """Invoke all special application functions for this algorithms by Scikit-learn framework."""
-        pass
+
+        if SVMRegression.X.shape[1] == 2:
+            self._plot_2d_decision_boundary(SVMRegression.X, SVMRegression.X_test, SVMRegression.y_test,
+                                            self.model, self.image_config, self.naming, MODEL_OUTPUT_IMAGE_PATH)
 
     @dispatch(bool)
     def special_components(self, is_automl: bool, **kwargs) -> None:
         """Invoke all special application functions for this algorithms by FLAML framework."""
-        pass
+
+        if SVMRegression.X.shape[1] == 2:
+            self._plot_2d_decision_boundary(SVMRegression.X, SVMRegression.X_test, SVMRegression.y_test,
+                                            self.auto_model, self.image_config, self.naming, MODEL_OUTPUT_IMAGE_PATH)
+
 
 
 class DNNRegression(RegressionWorkflowBase):
+    """The automation workflow of using Deep Neural Network algorithm to make insightful products."""
 
-    name = "Deep Neural Networks"
+    name = "Deep Neural Network"
     special_function = ["Loss Record"]
 
     def __init__(
-            self,
-            hidden_layer_sizes: tuple = (50, 25, 5),
-            activation: List[str] = 'relu',
-            solver: List[str] ='adam',
-            alpha: float = 0.0001,
-            batch_size: Union[int, str] ='auto',
-            learning_rate: List[str] = 'constant',
-            learning_rate_init: float = 0.001,
-            max_iter: int = 200,
-            shuffle: bool = True,
-            random_state: int = None,
-            tol: float = 1e-4,
-            verbose: bool = False,
-            warm_start: bool = False,
-            early_stopping: bool = False,
-            validation_fraction: float = 0.1,
-            beta_1: float = 0.9,
-            beta_2: float = 0.999,
-            epsilon: float = 1e-8,
-            n_iter_no_change: int = 10,
+        self,
+        hidden_layer_sizes: tuple = (50, 25, 5),
+        activation: str = 'relu',
+        solver: str ='adam',
+        alpha: float = 0.0001,
+        batch_size: Union[int, str] = 'auto',
+        learning_rate: str = 'constant',
+        learning_rate_init: float = 0.001,
+        max_iter: int = 200,
+        shuffle: bool = True,
+        random_state: Optional[int] = None,
+        tol: float = 1e-4,
+        verbose: bool = False,
+        warm_start: bool = False,
+        early_stopping: bool = False,
+        validation_fraction: float = 0.1,
+        beta_1: float = 0.9,
+        beta_2: float = 0.999,
+        epsilon: float = 1e-8,
+        n_iter_no_change: int = 10,
     ):
-
-
         """
         Parameters
         ----------
         hidden_layer_sizes : tuple, length = n_layers - 2, default=(100,)
             The ith element represents the number of neurons in the ith
             hidden layer.
 
@@ -1521,24 +1752,17 @@
             of iterations reaches max_iter, or this number of function calls.
             Note that number of function calls will be greater than or equal to
             the number of iterations for the MLPRegressor.
 
             .. versionadded:: 0.22
 
         References
-        ----------------------------------------
-        Hinton, Geoffrey E. "Connectionist learning procedures."
-        Artificial intelligence 40.1 (1989): 185-234.
-        Glorot, Xavier, and Yoshua Bengio.
-        "Understanding the difficulty of training deep feedforward neural networks."
-        International Conference on Artificial Intelligence and Statistics. 2010.
-        :arxiv:`He, Kaiming, et al (2015). "Delving deep into rectifiers:
-        Surpassing human-level performance on imagenet classification." <1502.01852>`
-        :arxiv:`Kingma, Diederik, and Jimmy Ba (2014)
-        "Adam: A method for stochastic optimization." <1412.6980>`
+        ----------
+        Scikit-learn API: sklearn.neural_network.MLPRegressor
+        https://scikit-learn.org/stable/modules/generated/sklearn.neural_network.MLPRegressor.html
         """
         super().__init__()
         self.hidden_layer_sizes = hidden_layer_sizes
         self.activation = activation
         self.solver = solver
         self.alpha = alpha
         self.batch_size = batch_size
@@ -1553,33 +1777,35 @@
         self.early_stopping = early_stopping
         self.validation_fraction = validation_fraction
         self.beta_1 = beta_1
         self.beta_2 = beta_2
         self.epsilon = epsilon
         self.n_iter_no_change = n_iter_no_change
 
-        self.model = MLPRegressor(hidden_layer_sizes=self.hidden_layer_sizes,
-                                   activation=self.activation,
-                                   solver=self.solver,
-                                   alpha=self.alpha,
-                                   batch_size=self.batch_size,
-                                   learning_rate=self.learning_rate,
-                                   learning_rate_init=self.learning_rate_init,
-                                   max_iter=self.max_iter,
-                                   shuffle=self.shuffle,
-                                   random_state=self.random_state,
-                                   tol=self.tol,
-                                   verbose=self.verbose,
-                                   warm_start=self.warm_start,
-                                   early_stopping=self.early_stopping,
-                                   validation_fraction=self.validation_fraction,
-                                   beta_1=self.beta_1,
-                                   beta_2=self.beta_2,
-                                   epsilon=self.epsilon,
-                                   n_iter_no_change=self.n_iter_no_change)
+        self.model = MLPRegressor(
+            hidden_layer_sizes=self.hidden_layer_sizes,
+            activation=self.activation,
+            solver=self.solver,
+            alpha=self.alpha,
+            batch_size=self.batch_size,
+            learning_rate=self.learning_rate,
+            learning_rate_init=self.learning_rate_init,
+            max_iter=self.max_iter,
+            shuffle=self.shuffle,
+            random_state=self.random_state,
+            tol=self.tol,
+            verbose=self.verbose,
+            warm_start=self.warm_start,
+            early_stopping=self.early_stopping,
+            validation_fraction=self.validation_fraction,
+            beta_1=self.beta_1,
+            beta_2=self.beta_2,
+            epsilon=self.epsilon,
+            n_iter_no_change=self.n_iter_no_change
+        )
 
         self.naming = DNNRegression.name
 
     def ray_tune(self, X_train: pd.DataFrame, X_test: pd.DataFrame, y_train: pd.DataFrame, y_test: pd.DataFrame) -> None:
         """The customized DNN of the combinations of Ray, FLAML and Scikit-learn framework."""
 
         from ray import tune
@@ -1644,16 +1870,24 @@
         results = tuner.fit()
 
         # The hyper-parameters found to minimize the mean loss of the defined objective and the corresponding model.
         best_result = results.get_best_result(metric='mean_loss', mode='min')
         self.ray_best_model = customized_model(best_result.config['l1'], best_result.config['l2'],
                                                best_result.config['l3'], best_result.config['batch'])
 
+    @classmethod
+    def manual_hyper_parameters(cls) -> Dict:
+        """Manual hyper-parameters specification."""
+        print(f"-*-*- {cls.name} - Hyper-parameters Specification -*-*-")
+        hyper_parameters = deep_neural_network_manual_hyper_parameters()
+        return hyper_parameters
+
     @staticmethod
     def _plot_learning_curve(trained_model: object, algorithm_name: str, store_path) -> None:
+        """Plot the learning curve of the trained model."""
         print("-----* Loss Record *-----")
         pd.DataFrame(trained_model.loss_curve_).plot(title="Loss")
         save_fig(f'Loss Record - {algorithm_name}', store_path)
 
     @dispatch()
     def special_components(self, **kwargs) -> None:
         """Invoke all special application functions for this algorithms by Scikit-learn framework."""
@@ -1662,93 +1896,112 @@
     @dispatch(bool)
     def special_components(self, is_automl: bool, **kwargs) -> None:
         """Invoke all special application functions for this algorithms by FLAML framework."""
         self._plot_learning_curve(self.auto_model, self.naming, MODEL_OUTPUT_IMAGE_PATH)
 
 
 class LinearRegression2(RegressionWorkflowBase):
+    """The automation workflow of using Linear Regression algorithm to make insightful products."""
 
     name = "Linear Regression"
     special_function = ["Linear Regression Formula", "Two/Three-dimensional Linear Regression Image"]
 
     def __init__(
-            self,
-            fit_intercept: bool = True,
-            normalize: bool = False,
-            copy_X: bool = True,
-            n_jobs: Optional[int] = None
+        self,
+        fit_intercept: bool = True,
+        normalize: bool = False,
+        copy_X: bool = True,
+        n_jobs: Optional[int] = None
     ) -> None:
         """
         Parameters
         ----------
         fit_intercept : bool, default=True
             Whether to calculate the intercept for this model. If set
             to False, no intercept will be used in calculations
             (i.e. data is expected to be centered).
+
         normalize : bool, default=False
             This parameter is ignored when ``fit_intercept`` is set to False.
             If True, the regressors X will be normalized before regression by
             subtracting the mean and dividing by the l2-norm.
             If you wish to standardize, please use
                             :class:`~sklearn.preprocessing.StandardScaler` before calling ``fit``
             on an estimator with ``normalize=False``.
             .. deprecated:: 1.0
                `normalize` was deprecated in version 1.0 and will be
                removed in 1.2.
+        
         copy_X : bool, default=True
                         If True, X will be copied; else, it may be overwritten.
+        
         n_jobs : int, default=None
             The number of jobs to use for the computation. This will only provide
             speedup in case of sufficiently large problems, that is if firstly
                             `n_targets > 1` and secondly `X` is sparse or if `positive` is set
             to `True`. ``None`` means 1 unless in a
             :obj:`joblib.parallel_backend` context. ``-1`` means using all
             processors. See :term:`Glossary <n_jobs>` for more details.
+        
         positive : bool, default=False
                         When set to ``True``, forces the coefficients to be positive. This
             option is only supported for dense arrays.
             .. versionadded:: 0.24
 
         References
         ----------
-        scikit API: sklearn.linear_model.LinearRegression
+        Scikit-learn API: sklearn.linear_model.LinearRegression
         https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LinearRegression.html?highlight=linearregression
         """
         super().__init__()
         self.fit_intercept = fit_intercept
         self.normalize = normalize
         self.copy_X = copy_X
         self.n_jobs = n_jobs
 
-        self.model = LinearRegression(fit_intercept=self.fit_intercept,
-                                      copy_X=self.copy_X,
-                                      normalize=self.normalize,
-                                      n_jobs=self.n_jobs)
+        self.model = LinearRegression(
+            fit_intercept=self.fit_intercept,
+            copy_X=self.copy_X,
+            normalize=self.normalize,
+            n_jobs=self.n_jobs
+        )
+
         self.naming = LinearRegression2.name
 
+    @classmethod
+    def manual_hyper_parameters(cls) -> Dict:
+        """Manual hyper-parameters specification."""
+        print(f"-*-*- {cls.name} - Hyper-parameters Specification -*-*-")
+        hyper_parameters = linear_regression_manual_hyper_parameters()
+        return hyper_parameters
+
     @staticmethod
     def _show_formula(coef, intercept, columns_name):
+        """Show the formula of the linear regression model."""
         print("-----* Linear Regression Formula *-----")
         show_formula(coef, intercept, columns_name)
 
     @staticmethod
     def _plot_2d_graph(feature_data: pd.DataFrame, target_data: pd.DataFrame, algorithm_name: str,
                        store_path: str):
+        """Plot the 2D graph of the linear regression model."""
         print("-----* Plot 2D Graph *-----")
         plot_2d_graph(feature_data, target_data)
         save_fig(f"2D Scatter Graph - {algorithm_name}", store_path)
 
     @staticmethod
     def _plot_3d_graph(feature_data: pd.DataFrame, target_data: pd.DataFrame, algorithm_name: str,
                        store_path: str):
+        """Plot the 3D graph of the linear regression model."""
         print("-----* Plot 3D Graph *-----")
         plot_3d_graph(feature_data, target_data)
         save_fig(f"3D Scatter Graph - {algorithm_name}", store_path)
 
     def special_components(self, **kwargs):
+        """Invoke all special application functions for this algorithms by Scikit-learn framework."""
         self._show_formula(coef=self.model.coef_, intercept=self.model.intercept_,
                            columns_name=LinearRegression2.X.columns)
 
         columns_num = LinearRegression2.X.shape[1]
         if columns_num > 2:
             # choose two of dimensions to draw
             three_dimen_axis_index, three_dimen_data = self.choose_dimension_data(LinearRegression2.X, 2)
```

### Comparing `geochemistrypi-0.1.0/geochemistrypi/data_mining/model/func/algo_classification/_common.py` & `geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_classification/_common.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.1.0/geochemistrypi/data_mining/model/func/algo_classification/_xgboost.py` & `geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_regression/_decision_tree.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,138 +1,88 @@
 import matplotlib.pyplot as plt
-import xgboost
-import pandas as pd
+from sklearn.tree import plot_tree
+from typing import Dict
+from ....data.data_readiness import num_input, str_input
+from ....global_variable import SECTION
+
+
+def decision_tree_manual_hyper_parameters() -> Dict:
+    """Manually set hyperparameters.
+
+    Returns
+    -------
+    hype_parameters : dict
+    """
+    print("Criterion: The function to measure the quality of a split. Supported criteria are “squared_error” for the mean squared error, which is equal to variance reduction as feature selection criterion and minimizes the L2 loss using the mean of each terminal node, “friedman_mse”, which uses mean squared error with Friedman’s improvement score for potential splits, “absolute_error” for the mean absolute error, which minimizes the L1 loss using the median of each terminal node, and “poisson” which uses reduction in Poisson deviance to find splits.")
+    print("The default value is 'squared_error'. Optional criterions are 'friedman_mse', 'absolute_error' and 'poisson'.")
+    criterions = ["squared_error", "friedman_mse", "absolute_error", "poisson"]
+    criterion = str_input(criterions, SECTION[2])
+    print("Max Depth: The maximum depth of the tree. If None, then nodes are expanded until all leaves are pure or until all leaves contain less than min_samples_split samples.")
+    print("Please specify the maximum depth of the tree. A good starting range could be between 3 and 15, such as 4.")
+    max_depth = num_input(SECTION[2], "@Max Depth: ")
+    print("Min Samples Split: The minimum number of samples required to split an internal node.")
+    print("Please specify the minimum number of samples required to split an internal node. A good starting range could be between 2 and 10, such as 3.")
+    min_samples_split = num_input(SECTION[2], "@Min Samples Split: ")
+    print("Min Samples Leaf: The minimum number of samples required to be at a leaf node.")
+    print("Please specify the minimum number of samples required to be at a leaf node. A good starting range could be between 1 and 10, such as 2.")
+    min_samples_leaf = num_input(SECTION[2], "@Min Samples Leaf: ")
+    print("Max Features: The number of features to consider when looking for the best split.")
+    print("Please specify the number of features to consider when looking for the best split. A good starting range could be between 1 and the total number of features in the dataset.")
+    max_features = num_input(SECTION[2], "@Max Features: ")
+    hyper_parameters = {'criterion': criterion, 'max_depth': max_depth, 'min_samples_split': min_samples_split, 'min_samples_leaf': min_samples_leaf, 'max_features': max_features}
+    return hyper_parameters
 
 
-def feature_importance_value(data: pd.DataFrame, trained_model: any) -> None:
-    """
-    Draw the feature importance value orderly for analysis.
-
-    Parameters
-    ----------
-    data: pd.DataFrame (n_samples, n_components)
-        Data for silhouette.
-
-    trained_model: any
-        The algorithm which to be used
-
-    algorithm_name : str
-        the name of the algorithm
-
-    References
-    ----------
-    XGBoost is an optimized distributed gradient boosting library designed to be highly efficient, f
-    lexible and portable. It implements machine learning algorithms under the Gradient Boosting fram
-    ework. XGBoost provides a parallel tree boosting (also known as GBDT, GBM) that solve many data
-    science problems in a fast and accurate way.
-
-    https://xgboost.readthedocs.io/en/stable/
-    """
-    columns_name = data.columns
-    for feature_name, score in zip(list(columns_name), trained_model.feature_importances_):
-        print(feature_name, ":", score)
-
-
-def feature_weights_histograms(trained_model: any, image_config: dict, algorithm_name: str) -> None:
-    """
-    Draw the histograms of feature weights for XGBoost predictions.
+def decision_tree_plot(trained_model: object, image_config: dict) -> None:
+    """Drawing decision tree diagrams.
 
     Parameters
     ----------
-    data: pd.DataFrame (n_samples, n_components)
-        Data for silhouette.
-
-    trained_model: any
-        The algorithm which to be used
-
-    algorithm_name : str
-        the name of the algorithm
-
-    References
-    ----------
-    XGBoost is an optimized distributed gradient boosting library designed to be highly efficient, f
-    lexible and portable. It implements machine learning algorithms under the Gradient Boosting fram
-    ework. XGBoost provides a parallel tree boosting (also known as GBDT, GBM) that solve many data
-    science problems in a fast and accurate way.
-
-    https://xgboost.readthedocs.io/en/stable/
-    """
-
-    # create drawing canvas
-    fig, ax = plt.subplots(figsize=(image_config['width'], image_config['height']), dpi=image_config['dpi'])
-
-    ax.bar(image_config['bar_x'], trained_model.feature_importances_, tick_label=image_config['bar_label'], width=image_config['bar_width'], bottom=image_config['bottom'])
-
-    # automatically optimize picture layout structure
-    fig.tight_layout()
-    xmin, xmax = ax.get_xlim()
-    ymin, ymax = ax.get_ylim()
-    x_adjustment = (xmax - xmin) * 0.1
-    y_adjustment = (ymax - ymin) * 0.1
-    ax.axis([xmin - x_adjustment, xmax + x_adjustment, ymin - y_adjustment, ymax + y_adjustment])
-
-    # convert the font of the axes
-    plt.tick_params(labelsize=image_config['labelsize'])  # adjust the font size of the axis label
-    # plt.setp(ax.get_xticklabels(), rotation=image_config['xrotation'], ha=image_config['xha'],
-    #          rotation_mode="anchor")  # axis label rotation Angle
-    # plt.setp(ax.get_yticklabels(), rotation=image_config['rot'], ha=image_config['yha'],
-    #          rotation_mode="anchor")  # axis label rotation Angle
-    x1_label = ax.get_xticklabels()  # adjust the axis label font
-    [x1_label_temp.set_fontname(image_config['axislabelfont']) for x1_label_temp in x1_label]
-    y1_label = ax.get_yticklabels()
-    [y1_label_temp.set_fontname(image_config['axislabelfont']) for y1_label_temp in y1_label]
+    trained_model : sklearn algorithm model
+        The sklearn algorithm model trained with X_train data.
 
-    ax.set_title(label=algorithm_name, fontdict={"size": image_config['title_size'], "color": image_config['title_color'],
-                "family": image_config['title_font']}, loc=image_config['title_location'],
-                pad=image_config['title_pad'])
-
-
-def feature_importance_map(trained_model: any, image_config: dict, algorithm_name: str) -> None:
+    image_config : dict
+        Image Configuration
     """
-    Draw the diagram of feature importance map ranked by importance for analysis.
-
-    Parameters
-    ----------
-    trained_model: any
-        The algorithm which to be used
-
-    algorithm_name : str
-        the name of the algorithm
 
-    References
-    ----------
-    XGBoost is an optimized distributed gradient boosting library designed to be highly efficient, f
-    lexible and portable. It implements machine learning algorithms under the Gradient Boosting fram
-    ework. XGBoost provides a parallel tree boosting (also known as GBDT, GBM) that solve many data
-    science problems in a fast and accurate way.
-
-    https://xgboost.readthedocs.io/en/stable/
-    """
     # create drawing canvas
     fig, ax = plt.subplots(figsize=(image_config['width'], image_config['height']), dpi=image_config['dpi'])
 
     # draw the main content
-    xgboost.plot_importance(booster=trained_model, ax=image_config['ax'], height=image_config['bar_width'])
+    plot_tree(trained_model,
+              max_depth=image_config['max_depth'],
+              feature_names=image_config['feature_names'],
+              class_names=image_config['class_names'],
+              label=image_config['label'],
+              filled=image_config['filled'],
+              impurity=image_config['impurity'],
+              node_ids=image_config['node_ids'],
+              proportion=image_config['proportion'],
+              rounded=image_config['rounded'],
+              precision=image_config['precision'],
+              ax=image_config['ax'],
+              fontsize=image_config['fontsize']
+              )
 
     # automatically optimize picture layout structure
     fig.tight_layout()
     xmin, xmax = ax.get_xlim()
     ymin, ymax = ax.get_ylim()
-    x_adjustment = (xmax - xmin) * 0.1
-    y_adjustment = (ymax - ymin) * 0.1
+    x_adjustment = (xmax - xmin) * 0.01
+    y_adjustment = (ymax - ymin) * 0.01
     ax.axis([xmin - x_adjustment, xmax + x_adjustment, ymin - y_adjustment, ymax + y_adjustment])
 
     # convert the font of the axes
-    plt.tick_params(labelsize=image_config['labelsize'])  # adjust the font size of the axis label
+    # plt.tick_params(labelsize=image_config['labelsize'])  # adjust the font size of the axis label
     # plt.setp(ax.get_xticklabels(), rotation=image_config['xrotation'], ha=image_config['xha'],
     #          rotation_mode="anchor")  # axis label rotation Angle
     # plt.setp(ax.get_yticklabels(), rotation=image_config['rot'], ha=image_config['yha'],
     #          rotation_mode="anchor")  # axis label rotation Angle
     x1_label = ax.get_xticklabels()  # adjust the axis label font
     [x1_label_temp.set_fontname(image_config['axislabelfont']) for x1_label_temp in x1_label]
     y1_label = ax.get_yticklabels()
     [y1_label_temp.set_fontname(image_config['axislabelfont']) for y1_label_temp in y1_label]
 
-    ax.set_title(label=algorithm_name,
+    ax.set_title(label=image_config['title_label'],
                  fontdict={"size": image_config['title_size'], "color": image_config['title_color'],
                            "family": image_config['title_font']}, loc=image_config['title_location'],
                  pad=image_config['title_pad'])
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `geochemistrypi-0.1.0/geochemistrypi/data_mining/model/func/algo_clustering/_kmeans.py` & `geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_clustering/_kmeans.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,44 @@
 from sklearn.metrics import silhouette_samples, silhouette_score
 import matplotlib.pyplot as plt
 import matplotlib.cm as cm
 import numpy as np
 import pandas as pd
+from typing import Dict
+from ....data.data_readiness import float_input, num_input, str_input
+from ....global_variable import SECTION
+
+
+def kmeans_manual_hyper_parameters() -> Dict:
+    """Manually set hyperparameters.
+
+    Returns
+    -------
+    hyper_parameters : dict
+    """
+    print("N Clusters: The number of clusters to form as well as the number of centroids to generate.")
+    print("Please specify the number of clusters for KMeans. A good starting range could be between 2 and 10, such as 4.")
+    n_clusters = num_input(SECTION[2], "N Clusters: ")
+    print("Init: Method for initialization of centroids. The centroids represent the center points of the clusters in the dataset.")
+    print("Please specify the method for initialization of centroids. It is generally recommended to leave it set to k-means++.")
+    inits = ["k-means++", "random"]
+    init = str_input(inits, SECTION[2])
+    print("Max Iter: Maximum number of iterations of the k-means algorithm for a single run.")
+    print("Please specify the maximum number of iterations of the k-means algorithm for a single run. A good starting range could be between 100 and 500, such as 300.")
+    max_iters = num_input(SECTION[2], "Max Iter: ")
+    print("Tolerance: Relative tolerance with regards to inertia to declare convergence.")
+    print("Please specify the relative tolerance with regards to inertia to declare convergence. A good starting range could be between 0.0001 and 0.001, such as 0.0005.")
+    tol = float_input(0.0005, SECTION[2], "Tolerance: ")
+    print("Algorithm: The algorithm to use for the computation.")
+    print("Please specify the algorithm to use for the computation. It is generally recommended to leave it set to auto.")
+    print("Auto: selects 'elkan' for dense data and 'full' for sparse data. 'elkan' is generally faster on data with lower dimensionality, while 'full' is faster on data with higher dimensionality")
+    algorithms = ["auto", "full", "elkan"]
+    algorithm = str_input(algorithms, SECTION[2])
+    hyper_parameters = {"n_clusters": n_clusters, "init": init, "max_iter": max_iters, "tol": tol, "algorithm": algorithm}
+    return hyper_parameters
 
 
 def plot_silhouette_diagram(data: pd.DataFrame, cluster_labels: pd.DataFrame,
                             cluster_centers_: np.ndarray, n_clusters: int, algorithm_name: str) -> None:
     """
     Draw the silhouette diagram for analysis.
```

### Comparing `geochemistrypi-0.1.0/geochemistrypi/data_mining/model/func/algo_decomposition/_pca.py` & `geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_decomposition/_pca.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,32 @@
 # -*- coding: utf-8 -*-
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
-from typing import Optional, List
+from typing import Optional, List, Dict
+from ....data.data_readiness import num_input, str_input
+from ....global_variable import SECTION
+
+
+def pca_manual_hyper_parameters() -> Dict:
+    """Manually set hyperparameters.
+
+    Returns
+    -------
+    hyper_parameters : dict
+    """
+    print("N Components: This parameter specifies the number of components to retain after dimensionality reduction.")
+    print("Please specify the number of components to retain. A good starting range could be between 2 and 10, such as 4.")
+    n_components = num_input(SECTION[2], "N Components: ")
+    print("SVD Solver: This parameter specifies the algorithm used to perform the singular value decomposition.")
+    print("Please specify the algorithm. It is generally recommended to leave it set to auto.")
+    svd_solvers = ["auto", "full", "arpack", "randomized"]
+    svd_solver = str_input(svd_solvers, SECTION[2])
+    hyper_parameters = {"n_components": n_components, "svd_solver": svd_solver}
+    return hyper_parameters
 
 
 def biplot(reduced_data: pd.DataFrame, pc: pd.DataFrame, algorithm_name: str,
            labels: Optional[List[str]] = None) -> None:
     """Plot a compositional bi-plot for two principal components.
 
     Parameters
```

### Comparing `geochemistrypi-0.1.0/geochemistrypi/data_mining/model/func/algo_regression/_common.py` & `geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_regression/_common.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.1.0/geochemistrypi/data_mining/plot/geochemistry_plot.py` & `geochemistrypi-0.2.0/geochemistrypi/data_mining/plot/geochemistry_plot.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.1.0/geochemistrypi/data_mining/plot/statistic_plot.py` & `geochemistrypi-0.2.0/geochemistrypi/data_mining/plot/statistic_plot.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.1.0/geochemistrypi/data_mining/process/decompose.py` & `geochemistrypi-0.2.0/geochemistrypi/data_mining/process/decompose.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,35 +8,33 @@
 
 class DecompositionModelSelection(object):
     """Simulate the normal way of invoking scikit-learn decomposition algorithms."""
 
     def __init__(self, model: str) -> None:
         self.model = model
         self.dcp_workflow = DecompositionWorkflowBase()
-        self.components_num = None
 
     def activate(self, X: pd.DataFrame, y: Optional[pd.DataFrame] = None, X_train: Optional[pd.DataFrame] = None,
                  X_test: Optional[pd.DataFrame] = None, y_train: Optional[pd.DataFrame] = None,
                  y_test: Optional[pd.DataFrame] = None) -> None:
         """Train by Scikit-learn framework."""
 
         self.dcp_workflow.data_upload(X=X, y=y, X_train=X_train, X_test=X_test, y_train=y_train, y_test=y_test)
+        
         if self.model == "Principal Component Analysis":
-            print("-*-*- Hyper-parameters Specification -*-*-")
-            print("Decide the component numbers to keep:")
-            self.components_num = num_input(SECTION[2])
-            self.dcp_workflow = PCADecomposition(n_components=self.components_num)
+            hyper_parameters = PCADecomposition.manual_hyper_parameters()
+            self.dcp_workflow = PCADecomposition(n_components=hyper_parameters["n_components"], svd_solver=hyper_parameters["svd_solver"])
 
         # common components for every decomposition algorithm
         self.dcp_workflow.show_info()
         self.dcp_workflow.fit(X)
         X_reduced = self.dcp_workflow.transform(X)
         self.dcp_workflow.data_upload(X=X)
 
         # special components of different algorithms
-        self.dcp_workflow.special_components(components_num=self.components_num, reduced_data=X_reduced)
+        self.dcp_workflow.special_components(components_num=hyper_parameters["n_components"], reduced_data=X_reduced)
 
         # Save decomposition result
         # self.dcp_workflow.data_save(X_reduced, "X reduced", DATASET_OUTPUT_PATH, "Decomposition Result")
 
         # Save the trained model
         self.dcp_workflow.save_model()
```

### Comparing `geochemistrypi-0.1.0/geochemistrypi/data_mining/tests/test_data/test_data_readiness.py` & `geochemistrypi-0.2.0/geochemistrypi/data_mining/tests/test_data/test_data_readiness.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.1.0/geochemistrypi/data_mining/utils/base.py` & `geochemistrypi-0.2.0/geochemistrypi/data_mining/utils/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,15 +32,25 @@
         Automatically adjust subplot parameters to give specified padding.
     """
     # TODO: seperate the stored path outside
     path = os.path.join(image_path, fig_name + ".png")
     print(f"Save figure '{fig_name}' in {image_path}.")
     if tight_layout:
         plt.tight_layout()
+
+
+    # Check that the original file exists,
+    # and if it does, add a number after the filename to distinguish
+    i = 1
+    dir = path[:-4]
+    while os.path.isfile(path):
+        path = dir + str(i) + ".png"
+        i = i + 1
     plt.savefig(path, format='png', dpi=300)
+    plt.close()
 
 
 def save_data(df: pd.DataFrame, df_name: str, path: str) -> None:
     """Save the dataset.
 
     Parameters
     ----------
```

### Comparing `geochemistrypi-0.1.0/LICENSE` & `geochemistrypi-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.1.0/README.md` & `geochemistrypi-0.2.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,29 @@
-<img src="./docs/Geochemistry π.png" width="50%"/>
+<p>
+<img src="./docs/Geochemistry π.png" class="center"/>
+</p>
+<p align="center">
+<img src="https://img.shields.io/github/actions/workflow/status/ZJUEarthData/geochemistrypi/geochemistrypy.yml?logo=github">
+<img src="https://img.shields.io/github/license/ZJUEarthData/geochemistrypi">
+<img src="https://img.shields.io/github/v/release/ZJUEarthData/geochemistrypi?include_prereleases">
+<img src="https://static.pepy.tech/personalized-badge/geochemistrypi?period=total&units=international_system&left_color=grey&right_color=green&left_text=Downloads">
+</p>
 
-Geochemistry π is **a Python framework** for data-driven geochemistry discovery. It provides an extendable tool and
-one-stop shop for **geochemical data analysis** on tabular data. The goal of the Geochemistry π is to create
-a series of user-friendly and extensible products of high automation for the full cycle of geochemistry research.  
+
+Geochemistry π is **a Python framework** for data-driven geochemistry discovery. It provides an extendable tool and one-stop shop for **geochemical data analysis** on tabular data. 
+
+The goal of the Geochemistry π is to create a series of user-friendly and extensible products of high automation for the full cycle of geochemistry research.  
+
+Key features are:
++ **Easy to use:** The automation of data mining process provides the users with simple number options to choose.
++ **Extensible:** It allows appending new algorithms through Scikit-learn with augmented AutoML functionality by FLAML and Ray.
+
+Official Website: https://geochemistrypy.readthedocs.io/en/latest/Introduction/Introduction.html
+
+Latest Update: follow up by clicking `Starred` and  `Watch` on our [GitHub repository](https://github.com/ZJUEarthData/geochemistrypi), then get email notifications of the newest features automatically.
 
 ## Quick Installation
 
 One instruction to download on command line, such as Terminal on macOS, CMD on Windows.  
 ```
 pip install geochemistrypi
 ```
@@ -24,17 +41,20 @@
 
 ### Case 2: Run with your own data set
 ```
 geochemistrypi data-mining --data your_own_data_set.xlsx
 ```
 **Note**: Currently, only `.xlsx` file is supported. Please specify the path your data file exists. 
 
-For more details: Please to refer to 
-+ [Manual for Geochemistry π - Beta (International - Google drive)](https://drive.google.com/file/d/1ZQqmi6nkTZUaODAWzmXLvnaQ1bajEjYp/view?usp=sharing)
-+ [Manual for Geochemistry π - Beta (China - Tencent Docs)](https://docs.qq.com/pdf/DQ1llWXRiTHp1Y0lj?&u=6868f96d4a384b309036e04e637e367a)
+For more details: Please refer to 
++ [Manual v1.1.0 for Geochemistry π - Beta (International - Google drive)](https://drive.google.com/file/d/1yryykCyWKM-Sj88fOYbOba6QkB_fu2ws/view?usp=sharing)
++ [Manual v1.1.0 for Geochemistry π - Beta (China - Tencent Docs)](https://docs.qq.com/pdf/DQ0l5d2xVd2VwcnVW?&u=6868f96d4a384b309036e04e637e367a)
++ [Geochemistry π - Download and Run the Beta Version (International - Youtube)](https://www.youtube.com/watch?v=EeVaJ3H7_AU&list=PLy8hNsI55lvh1UHjhVhqNUj3xPdV9sEiM&index=9)
++ [Geochemistry π - Download and Run the Beta Version (China - Bilibili)](https://www.bilibili.com/video/BV1UM4y1Q7Ju/?spm_id_from=333.999.0.0&vd_source=27944ab3b73a78970c1a52a5dcbb9140)
+
 
 ## First Phase
 It works as a **software application** with a command-line interface (CLI) to automate **data mining** process with
 frequently-used **machine learning algorithms** and **statistical analysis methods**, which would further lower the
 threshold for the geochemists.
 
 The highlight is that through choosing **simple number options**, the users are able to implement a completed cycle of data
@@ -60,29 +80,32 @@
 
 ## Team Info
 **Leader:**
 + Can He (Sany, National University of Singapore, Singapore)    
   Email: sanyhew1097618435@163.com
 
 **Core Developers:**
-+ Jianhao Sun (Jin, China University of Geosciences，Wuhan, China)
++ Jianhao Sun (Jin, China University of Geosciences, Wuhan, China)
 + Jianming Zhao (Jamie, Jilin University, Changchun, China)
 + Yang Lyu (Daisy, Zhejiang University, China)
 + Shengxin Wang (Samson, Lanzhou University, China)
++ Wenyu Zhao (Molly, Zhejiang University, China)
 
 **Members**:
-+ Wenyu Zhao (Molly, Zhejiang University, China)
 + Fang Li (liv, Shenzhen University, China)
 + Ting Liu (Kira, Sun Yat-sen University, China)
 + Kaixin Zheng (Hayne, Sun Yat-sen University, China)
 + Aixiwake·Janganuer (Ayshuak, Sun Yat-sen University, China)
-+ Parnanjan Dutta (Presidency University, Kolkata, India)
-+ Bailun Jiang (EPSI / Lille University, France)
-+ Yongkang Chang (Kill-virus, Langzhou University, China)
 + Xirui Zhu (Rae, University of York, United Kingdom)
++ Jianing Wang (National University of Singapore, Singapore)
++ Yongkang Chang (Kill-virus, Langzhou University, China)
++ Bailun Jiang (EPSI / Lille University, France)
++ Yucheng Yan (Andy, University of Sydney)
++ Keran Li (Kirk, Chengdu University of Technology)
+
 
 ## Join Us :)
 **The recruitment of research interns is ongoing !!!**
 
 **Key Point: All things are done online, remote work (\*^▽^\*)**
 
 **What can you learn?**
@@ -127,19 +150,20 @@
 8. [Cycle Report - Geochemistry π (China - Tencent Docs)](https://docs.qq.com/pdf/DQ25VSGNlbGx4UkFZ?&u=6868f96d4a384b309036e04e637e367a)
 
 ## In-house Videos
 Technical record videos are on Bilibili and Youtube synchronously while other meeting videos are internal materials.
 More Videos will be recorded soon.
 1. [ZJU_Earth_Data Introduction (Geochemical Data, Python, Geochemistry π) - Prof. Zhang](https://www.bilibili.com/video/BV1Lf4y1w7EK?spm_id_from=333.999.0.0)
 2. [How to Collaborate and Provide Bug Report on Geochemistry π Through GitHub - Can He (Sany)](https://www.youtube.com/watch?v=1DWoEsqsfvQ&list=PLy8hNsI55lvh1UHjhVhqNUj3xPdV9sEiM&index=3)
-3. [How to Run Geochemistry π v1.0.0-alpha - Can He (Sany)](https://www.bilibili.com/video/BV1i541117dd?spm_id_from=333.999.0.0)
+3. [Geochemistry π - Download and Run the Beta Version](https://www.youtube.com/watch?v=EeVaJ3H7_AU&list=PLy8hNsI55lvh1UHjhVhqNUj3xPdV9sEiM&index=9)
 4. [How to Create and Use Virtual Environment on Geochemistry π - Can He (Sany)](https://www.youtube.com/watch?v=4KFi7OXxD-c&list=PLy8hNsI55lvh1UHjhVhqNUj3xPdV9sEiM&index=4)
 5. [How to use Github-Desktop in conflict resolution - Qiuhao Zhao (Brad)](https://www.youtube.com/watch?v=KT1g5JpuUVI&list=PLy8hNsI55lvh1UHjhVhqNUj3xPdV9sEiM)
 6. [Virtual Environment & Packages On Windows - Jianming Zhao (Jamie)](https://www.youtube.com/watch?v=e4VqSBuNp_o&list=PLy8hNsI55lvh1UHjhVhqNUj3xPdV9sEiM&index=2)
 7. [Git Workflow & Coordinating Synchronization - Jianming Zhao (Jamie)](https://www.bilibili.com/video/BV1Sa4y1f74k?spm_id_from=333.999.0.0&vd_source=9adcf2c5fdeffe1d11c89d441ef598ba)
 
 
 ## Contributors
 + Qiuhao Zhao (Brad, Zhejiang University, China)
 + Anzhou Li (Andrian, Zhejiang University, China) 
++ Dan Hu (Notre Dame University, United States)
 + Xunxin Liu (Tante, China University of Geosciences, Wuhan, China)
 + Xin Li (The University of Manchester, United Kingdom)
```

### Comparing `geochemistrypi-0.1.0/pyproject.toml` & `geochemistrypi-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "geochemistrypi"
-version = "0.1.0"
+version = "0.2.0"
 authors = [
   { name="Can He", email="sanyhew1097618435@163.com" },
 ]
 maintainers = [] 
 description = "A Python framework for data-driven geochemistry discovery"
 readme = "README.md"
 license = { file="LICENSE" }
-requires-python = ">=3.7"
+requires-python = "~=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
@@ -30,17 +30,18 @@
     "statsmodels==0.13.2",
     "scipy",
     "openpyxl==3.0.10",
     "pandas==1.5.2",
     "joblib==1.2.0",
     "flaml==1.0.14",         # required to run Xgboost + FLMAL
     "numpy==1.21.6",         # required to run Xgboost + FLMAL
-    "xgboost==1.3.1",        # required to run Xgboost + FLAML
+    "xgboost==1.6.2",        # required to run Xgboost + FLAML and be compatible with M2 chip on Mac
     "pyogrio==0.4.2",        # required to draw world map
     "geopandas==0.10.2",     # required to draw world map
+    "Fiona==1.8.19",         # required to draw world map
     "threadpoolctl==3.1.0",  # required to draw 3d plot for KMeans
     "matplotlib==3.5.2"      # required to draw 3d plot for KMeans
 ]
 
 [project.optional-dependencies]
 test = [
     "pytest"
```

### Comparing `geochemistrypi-0.1.0/PKG-INFO` & `geochemistrypi-0.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geochemistrypi
-Version: 0.1.0
+Version: 0.2.0
 Summary: A Python framework for data-driven geochemistry discovery
 Project-URL: Homepage, https://github.com/ZJUEarthData/geochemistrypi
 Project-URL: Bug Tracker, https://github.com/ZJUEarthData/geochemistrypi/issues
 Author-email: Can He <sanyhew1097618435@163.com>
 License: MIT License
         
         Copyright (c) 2021 ZJUEarthData
@@ -26,15 +26,16 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Requires-Python: ~=3.9
+Requires-Dist: fiona==1.8.19
 Requires-Dist: flaml==1.0.14
 Requires-Dist: geopandas==0.10.2
 Requires-Dist: joblib==1.2.0
 Requires-Dist: matplotlib==3.5.2
 Requires-Dist: multipledispatch==0.6.0
 Requires-Dist: numpy==1.21.6
 Requires-Dist: openpyxl==3.0.10
@@ -45,24 +46,41 @@
 Requires-Dist: ray[tune]
 Requires-Dist: scikit-learn==1.1.3
 Requires-Dist: scipy
 Requires-Dist: seaborn==0.11.0
 Requires-Dist: statsmodels==0.13.2
 Requires-Dist: threadpoolctl==3.1.0
 Requires-Dist: typer==0.7.0
-Requires-Dist: xgboost==1.3.1
+Requires-Dist: xgboost==1.6.2
 Provides-Extra: test
 Requires-Dist: pytest; extra == 'test'
 Description-Content-Type: text/markdown
 
-<img src="./docs/Geochemistry π.png" width="50%"/>
+<p>
+<img src="./docs/Geochemistry π.png" class="center"/>
+</p>
+<p align="center">
+<img src="https://img.shields.io/github/actions/workflow/status/ZJUEarthData/geochemistrypi/geochemistrypy.yml?logo=github">
+<img src="https://img.shields.io/github/license/ZJUEarthData/geochemistrypi">
+<img src="https://img.shields.io/github/v/release/ZJUEarthData/geochemistrypi?include_prereleases">
+<img src="https://static.pepy.tech/personalized-badge/geochemistrypi?period=total&units=international_system&left_color=grey&right_color=green&left_text=Downloads">
+</p>
 
-Geochemistry π is **a Python framework** for data-driven geochemistry discovery. It provides an extendable tool and
-one-stop shop for **geochemical data analysis** on tabular data. The goal of the Geochemistry π is to create
-a series of user-friendly and extensible products of high automation for the full cycle of geochemistry research.  
+
+Geochemistry π is **a Python framework** for data-driven geochemistry discovery. It provides an extendable tool and one-stop shop for **geochemical data analysis** on tabular data. 
+
+The goal of the Geochemistry π is to create a series of user-friendly and extensible products of high automation for the full cycle of geochemistry research.  
+
+Key features are:
++ **Easy to use:** The automation of data mining process provides the users with simple number options to choose.
++ **Extensible:** It allows appending new algorithms through Scikit-learn with augmented AutoML functionality by FLAML and Ray.
+
+Official Website: https://geochemistrypy.readthedocs.io/en/latest/Introduction/Introduction.html
+
+Latest Update: follow up by clicking `Starred` and  `Watch` on our [GitHub repository](https://github.com/ZJUEarthData/geochemistrypi), then get email notifications of the newest features automatically.
 
 ## Quick Installation
 
 One instruction to download on command line, such as Terminal on macOS, CMD on Windows.  
 ```
 pip install geochemistrypi
 ```
@@ -80,17 +98,20 @@
 
 ### Case 2: Run with your own data set
 ```
 geochemistrypi data-mining --data your_own_data_set.xlsx
 ```
 **Note**: Currently, only `.xlsx` file is supported. Please specify the path your data file exists. 
 
-For more details: Please to refer to 
-+ [Manual for Geochemistry π - Beta (International - Google drive)](https://drive.google.com/file/d/1ZQqmi6nkTZUaODAWzmXLvnaQ1bajEjYp/view?usp=sharing)
-+ [Manual for Geochemistry π - Beta (China - Tencent Docs)](https://docs.qq.com/pdf/DQ1llWXRiTHp1Y0lj?&u=6868f96d4a384b309036e04e637e367a)
+For more details: Please refer to 
++ [Manual v1.1.0 for Geochemistry π - Beta (International - Google drive)](https://drive.google.com/file/d/1yryykCyWKM-Sj88fOYbOba6QkB_fu2ws/view?usp=sharing)
++ [Manual v1.1.0 for Geochemistry π - Beta (China - Tencent Docs)](https://docs.qq.com/pdf/DQ0l5d2xVd2VwcnVW?&u=6868f96d4a384b309036e04e637e367a)
++ [Geochemistry π - Download and Run the Beta Version (International - Youtube)](https://www.youtube.com/watch?v=EeVaJ3H7_AU&list=PLy8hNsI55lvh1UHjhVhqNUj3xPdV9sEiM&index=9)
++ [Geochemistry π - Download and Run the Beta Version (China - Bilibili)](https://www.bilibili.com/video/BV1UM4y1Q7Ju/?spm_id_from=333.999.0.0&vd_source=27944ab3b73a78970c1a52a5dcbb9140)
+
 
 ## First Phase
 It works as a **software application** with a command-line interface (CLI) to automate **data mining** process with
 frequently-used **machine learning algorithms** and **statistical analysis methods**, which would further lower the
 threshold for the geochemists.
 
 The highlight is that through choosing **simple number options**, the users are able to implement a completed cycle of data
@@ -116,29 +137,32 @@
 
 ## Team Info
 **Leader:**
 + Can He (Sany, National University of Singapore, Singapore)    
   Email: sanyhew1097618435@163.com
 
 **Core Developers:**
-+ Jianhao Sun (Jin, China University of Geosciences，Wuhan, China)
++ Jianhao Sun (Jin, China University of Geosciences, Wuhan, China)
 + Jianming Zhao (Jamie, Jilin University, Changchun, China)
 + Yang Lyu (Daisy, Zhejiang University, China)
 + Shengxin Wang (Samson, Lanzhou University, China)
++ Wenyu Zhao (Molly, Zhejiang University, China)
 
 **Members**:
-+ Wenyu Zhao (Molly, Zhejiang University, China)
 + Fang Li (liv, Shenzhen University, China)
 + Ting Liu (Kira, Sun Yat-sen University, China)
 + Kaixin Zheng (Hayne, Sun Yat-sen University, China)
 + Aixiwake·Janganuer (Ayshuak, Sun Yat-sen University, China)
-+ Parnanjan Dutta (Presidency University, Kolkata, India)
-+ Bailun Jiang (EPSI / Lille University, France)
-+ Yongkang Chang (Kill-virus, Langzhou University, China)
 + Xirui Zhu (Rae, University of York, United Kingdom)
++ Jianing Wang (National University of Singapore, Singapore)
++ Yongkang Chang (Kill-virus, Langzhou University, China)
++ Bailun Jiang (EPSI / Lille University, France)
++ Yucheng Yan (Andy, University of Sydney)
++ Keran Li (Kirk, Chengdu University of Technology)
+
 
 ## Join Us :)
 **The recruitment of research interns is ongoing !!!**
 
 **Key Point: All things are done online, remote work (\*^▽^\*)**
 
 **What can you learn?**
@@ -183,19 +207,20 @@
 8. [Cycle Report - Geochemistry π (China - Tencent Docs)](https://docs.qq.com/pdf/DQ25VSGNlbGx4UkFZ?&u=6868f96d4a384b309036e04e637e367a)
 
 ## In-house Videos
 Technical record videos are on Bilibili and Youtube synchronously while other meeting videos are internal materials.
 More Videos will be recorded soon.
 1. [ZJU_Earth_Data Introduction (Geochemical Data, Python, Geochemistry π) - Prof. Zhang](https://www.bilibili.com/video/BV1Lf4y1w7EK?spm_id_from=333.999.0.0)
 2. [How to Collaborate and Provide Bug Report on Geochemistry π Through GitHub - Can He (Sany)](https://www.youtube.com/watch?v=1DWoEsqsfvQ&list=PLy8hNsI55lvh1UHjhVhqNUj3xPdV9sEiM&index=3)
-3. [How to Run Geochemistry π v1.0.0-alpha - Can He (Sany)](https://www.bilibili.com/video/BV1i541117dd?spm_id_from=333.999.0.0)
+3. [Geochemistry π - Download and Run the Beta Version](https://www.youtube.com/watch?v=EeVaJ3H7_AU&list=PLy8hNsI55lvh1UHjhVhqNUj3xPdV9sEiM&index=9)
 4. [How to Create and Use Virtual Environment on Geochemistry π - Can He (Sany)](https://www.youtube.com/watch?v=4KFi7OXxD-c&list=PLy8hNsI55lvh1UHjhVhqNUj3xPdV9sEiM&index=4)
 5. [How to use Github-Desktop in conflict resolution - Qiuhao Zhao (Brad)](https://www.youtube.com/watch?v=KT1g5JpuUVI&list=PLy8hNsI55lvh1UHjhVhqNUj3xPdV9sEiM)
 6. [Virtual Environment & Packages On Windows - Jianming Zhao (Jamie)](https://www.youtube.com/watch?v=e4VqSBuNp_o&list=PLy8hNsI55lvh1UHjhVhqNUj3xPdV9sEiM&index=2)
 7. [Git Workflow & Coordinating Synchronization - Jianming Zhao (Jamie)](https://www.bilibili.com/video/BV1Sa4y1f74k?spm_id_from=333.999.0.0&vd_source=9adcf2c5fdeffe1d11c89d441ef598ba)
 
 
 ## Contributors
 + Qiuhao Zhao (Brad, Zhejiang University, China)
 + Anzhou Li (Andrian, Zhejiang University, China) 
++ Dan Hu (Notre Dame University, United States)
 + Xunxin Liu (Tante, China University of Geosciences, Wuhan, China)
 + Xin Li (The University of Manchester, United Kingdom)
```

