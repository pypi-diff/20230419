# Comparing `tmp/graph_attention_student-0.7.0.tar.gz` & `tmp/graph_attention_student-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graph_attention_student-0.7.0.tar", max compression
+gzip compressed data, was "graph_attention_student-0.7.1.tar", max compression
```

## Comparing `graph_attention_student-0.7.0.tar` & `graph_attention_student-0.7.1.tar`

### file list

```diff
@@ -1,64 +1,67 @@
--rwxr-xr-x   0        0        0     8961 2022-12-29 07:58:42.522987 graph_attention_student-0.7.0/README.rst
--rwxr-xr-x   0        0        0        5 2023-03-27 10:44:22.879852 graph_attention_student-0.7.0/graph_attention_student/VERSION
--rwxr-xr-x   0        0        0       90 2022-12-29 07:58:42.522987 graph_attention_student-0.7.0/graph_attention_student/__init__.py
--rwxr-xr-x   0        0        0    84242 2023-03-19 09:18:21.518826 graph_attention_student-0.7.0/graph_attention_student/_models.py
--rwxr-xr-x   0        0        0     1131 2022-12-29 07:58:42.522987 graph_attention_student-0.7.0/graph_attention_student/cli.py
--rwxr-xr-x   0        0        0    54483 2023-01-17 14:13:51.169936 graph_attention_student-0.7.0/graph_attention_student/data.py
--rwxr-xr-x   0        0        0        0 2022-12-29 07:58:42.522987 graph_attention_student-0.7.0/graph_attention_student/examples/__init__.py
--rw-r--r--   0        0        0     9670 2023-01-20 11:45:50.758439 graph_attention_student-0.7.0/graph_attention_student/examples/__pycache__/vgd_multitask_gnn.cpython-310.pyc
--rw-r--r--   0        0        0    12164 2023-01-20 09:12:31.703590 graph_attention_student-0.7.0/graph_attention_student/examples/__pycache__/vgd_multitask_megan.cpython-310.pyc
--rwxr-xr-x   0        0        0    11582 2022-12-29 07:58:42.522987 graph_attention_student-0.7.0/graph_attention_student/examples/gnes_example.py
--rwxr-xr-x   0        0        0    11569 2022-12-29 07:58:42.522987 graph_attention_student-0.7.0/graph_attention_student/examples/gnnx_example.py
--rwxr-xr-x   0        0        0    18745 2022-12-29 07:58:42.522987 graph_attention_student-0.7.0/graph_attention_student/examples/smiles_example.py
--rw-r--r--   0        0        0    14585 2023-01-20 12:59:31.279402 graph_attention_student-0.7.0/graph_attention_student/examples/vgd_multitask_gnn.py
--rw-r--r--   0        0        0     5503 2023-01-20 11:59:55.452453 graph_attention_student-0.7.0/graph_attention_student/examples/vgd_multitask_gnn_gatv2.py
--rw-r--r--   0        0        0     4809 2023-01-20 11:39:35.159855 graph_attention_student-0.7.0/graph_attention_student/examples/vgd_multitask_gnn_gin.py
--rwxr-xr-x   0        0        0    20103 2023-01-20 10:32:00.863590 graph_attention_student-0.7.0/graph_attention_student/examples/vgd_multitask_megan.py
--rw-r--r--   0        0        0     1272 2023-01-20 09:42:42.629614 graph_attention_student-0.7.0/graph_attention_student/examples/vgd_multitask_megan_tadf.py
--rwxr-xr-x   0        0        0      726 2022-12-29 07:58:42.522987 graph_attention_student-0.7.0/graph_attention_student/experiments/README.rst
--rwxr-xr-x   0        0        0        0 2022-12-29 07:58:42.522987 graph_attention_student-0.7.0/graph_attention_student/experiments/__init__.py
--rw-r--r--   0        0        0    15106 2023-03-20 09:39:48.984068 graph_attention_student-0.7.0/graph_attention_student/experiments/__pycache__/vgd_regression_supervised.cpython-310.pyc
--rw-r--r--   0        0        0    10282 2023-01-24 14:34:57.947757 graph_attention_student-0.7.0/graph_attention_student/experiments/__pycache__/vgd_single.cpython-310.pyc
--rw-r--r--   0        0        0     6258 2023-01-24 12:19:49.929234 graph_attention_student-0.7.0/graph_attention_student/experiments/__pycache__/vgd_single_gnnx.cpython-310.pyc
--rw-r--r--   0        0        0     1373 2023-01-24 14:25:26.991807 graph_attention_student-0.7.0/graph_attention_student/experiments/__pycache__/vgd_single_gnnx_aqsoldb.cpython-310.pyc
--rw-r--r--   0        0        0     4349 2023-01-24 12:39:05.178403 graph_attention_student-0.7.0/graph_attention_student/experiments/__pycache__/vgd_single_megan.cpython-310.pyc
--rw-r--r--   0        0        0     1345 2023-01-24 12:56:57.478326 graph_attention_student-0.7.0/graph_attention_student/experiments/__pycache__/vgd_single_megan_aqsoldb.cpython-310.pyc
--rwxr-xr-x   0        0        0     9205 2022-12-29 07:58:42.522987 graph_attention_student-0.7.0/graph_attention_student/experiments/process_aqsoldb.py
--rwxr-xr-x   0        0        0    31932 2022-12-29 07:58:42.522987 graph_attention_student-0.7.0/graph_attention_student/experiments/rb_motifs_multi.py
--rwxr-xr-x   0        0        0    34843 2022-12-29 07:58:42.522987 graph_attention_student-0.7.0/graph_attention_student/experiments/rb_motifs_single.py
--rw-r--r--   0        0        0      459 2023-01-24 12:36:03.337029 graph_attention_student-0.7.0/graph_attention_student/experiments/template_sub_experiment.py
--rw-r--r--   0        0        0    18717 2023-03-19 08:35:02.980618 graph_attention_student-0.7.0/graph_attention_student/experiments/vgd_regression_posthoc.py
--rw-r--r--   0        0        0    24342 2023-03-20 09:39:47.552048 graph_attention_student-0.7.0/graph_attention_student/experiments/vgd_regression_supervised.py
--rw-r--r--   0        0        0     5567 2023-03-20 09:39:47.564048 graph_attention_student-0.7.0/graph_attention_student/experiments/vgd_regression_supervised_multi.py
--rw-r--r--   0        0        0     5788 2023-03-20 07:08:16.190877 graph_attention_student-0.7.0/graph_attention_student/experiments/vgd_regression_supervised_single.py
--rw-r--r--   0        0        0    16880 2023-01-24 14:34:55.699741 graph_attention_student-0.7.0/graph_attention_student/experiments/vgd_single.py
--rw-r--r--   0        0        0     8128 2023-01-24 12:19:49.761232 graph_attention_student-0.7.0/graph_attention_student/experiments/vgd_single_gnnx.py
--rw-r--r--   0        0        0     1038 2023-01-24 14:25:25.831799 graph_attention_student-0.7.0/graph_attention_student/experiments/vgd_single_gnnx_aqsoldb.py
--rw-r--r--   0        0        0     5506 2023-01-24 13:54:11.870993 graph_attention_student-0.7.0/graph_attention_student/experiments/vgd_single_gnnx_aqsoldb_dmpnn.py
--rw-r--r--   0        0        0     3581 2023-01-24 14:26:38.996305 graph_attention_student-0.7.0/graph_attention_student/experiments/vgd_single_gnnx_aqsoldb_gatv2.py
--rw-r--r--   0        0        0     5234 2023-01-24 13:19:46.309473 graph_attention_student-0.7.0/graph_attention_student/experiments/vgd_single_gnnx_aqsoldb_painn.py
--rw-r--r--   0        0        0     7532 2023-01-24 12:14:49.719109 graph_attention_student-0.7.0/graph_attention_student/experiments/vgd_single_megan.py
--rw-r--r--   0        0        0     1023 2023-01-24 14:34:42.335649 graph_attention_student-0.7.0/graph_attention_student/experiments/vgd_single_megan_aqsoldb.py
--rw-r--r--   0        0        0      695 2023-02-27 13:28:58.309313 graph_attention_student-0.7.0/graph_attention_student/keras.py
--rwxr-xr-x   0        0        0    20274 2023-02-23 19:42:55.562555 graph_attention_student-0.7.0/graph_attention_student/layers.py
--rw-r--r--   0        0        0      205 2023-03-19 09:12:41.525356 graph_attention_student-0.7.0/graph_attention_student/models/__init__.py
--rw-r--r--   0        0        0      380 2023-03-19 09:15:50.038102 graph_attention_student-0.7.0/graph_attention_student/models/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3314 2023-03-19 09:15:50.054102 graph_attention_student-0.7.0/graph_attention_student/models/__pycache__/gnes.cpython-310.pyc
--rw-r--r--   0        0        0     1950 2023-03-19 09:15:50.054102 graph_attention_student-0.7.0/graph_attention_student/models/__pycache__/gnnx.cpython-310.pyc
--rw-r--r--   0        0        0     9148 2023-03-19 09:15:50.050102 graph_attention_student-0.7.0/graph_attention_student/models/__pycache__/gradient.cpython-310.pyc
--rw-r--r--   0        0        0    15000 2023-03-19 09:15:50.042102 graph_attention_student-0.7.0/graph_attention_student/models/__pycache__/megan.cpython-310.pyc
--rw-r--r--   0        0        0     3406 2023-03-19 09:12:41.537356 graph_attention_student-0.7.0/graph_attention_student/models/gnes.py
--rw-r--r--   0        0        0     2590 2023-03-19 09:15:48.990097 graph_attention_student-0.7.0/graph_attention_student/models/gnnx.py
--rw-r--r--   0        0        0    12180 2023-03-19 09:10:38.508809 graph_attention_student-0.7.0/graph_attention_student/models/gradient.py
--rw-r--r--   0        0        0    28472 2023-03-19 09:07:02.503170 graph_attention_student-0.7.0/graph_attention_student/models/megan.py
--rwxr-xr-x   0        0        0     1040 2023-01-18 09:06:23.993806 graph_attention_student-0.7.0/graph_attention_student/templates/article.tex.j2
--rw-r--r--   0        0        0      375 2023-01-24 12:08:49.160527 graph_attention_student-0.7.0/graph_attention_student/templates/table.tex.j2
--rw-r--r--   0        0        0      151 2023-01-17 16:58:58.659355 graph_attention_student-0.7.0/graph_attention_student/templates/table_content.tex.j2
--rw-r--r--   0        0        0       76 2023-01-17 17:10:30.475776 graph_attention_student-0.7.0/graph_attention_student/templates/table_element_mean.tex.j2
--rwxr-xr-x   0        0        0     9821 2023-03-18 15:02:20.950207 graph_attention_student-0.7.0/graph_attention_student/training.py
--rwxr-xr-x   0        0        0     3753 2022-12-29 07:58:42.522987 graph_attention_student-0.7.0/graph_attention_student/typing.py
--rwxr-xr-x   0        0        0    15021 2023-01-18 08:39:58.301379 graph_attention_student-0.7.0/graph_attention_student/util.py
--rwxr-xr-x   0        0        0    16147 2023-03-27 10:44:14.975799 graph_attention_student-0.7.0/graph_attention_student/visualization.py
--rwxr-xr-x   0        0        0     1397 2023-03-27 10:44:22.871852 graph_attention_student-0.7.0/pyproject.toml
--rw-r--r--   0        0        0    10441 1970-01-01 00:00:00.000000 graph_attention_student-0.7.0/setup.py
--rw-r--r--   0        0        0    10052 1970-01-01 00:00:00.000000 graph_attention_student-0.7.0/PKG-INFO
+-rwxr-xr-x   0        0        0     8961 2022-12-29 07:58:42.522987 graph_attention_student-0.7.1/README.rst
+-rwxr-xr-x   0        0        0        5 2023-04-19 13:30:28.447135 graph_attention_student-0.7.1/graph_attention_student/VERSION
+-rwxr-xr-x   0        0        0       90 2022-12-29 07:58:42.522987 graph_attention_student-0.7.1/graph_attention_student/__init__.py
+-rwxr-xr-x   0        0        0    84242 2023-03-19 09:18:21.518826 graph_attention_student-0.7.1/graph_attention_student/_models.py
+-rwxr-xr-x   0        0        0     1131 2022-12-29 07:58:42.522987 graph_attention_student-0.7.1/graph_attention_student/cli.py
+-rwxr-xr-x   0        0        0    54483 2023-01-17 14:13:51.169936 graph_attention_student-0.7.1/graph_attention_student/data.py
+-rwxr-xr-x   0        0        0        0 2022-12-29 07:58:42.522987 graph_attention_student-0.7.1/graph_attention_student/examples/__init__.py
+-rw-r--r--   0        0        0     9670 2023-01-20 11:45:50.758439 graph_attention_student-0.7.1/graph_attention_student/examples/__pycache__/vgd_multitask_gnn.cpython-310.pyc
+-rw-r--r--   0        0        0    12164 2023-01-20 09:12:31.703590 graph_attention_student-0.7.1/graph_attention_student/examples/__pycache__/vgd_multitask_megan.cpython-310.pyc
+-rwxr-xr-x   0        0        0    11582 2022-12-29 07:58:42.522987 graph_attention_student-0.7.1/graph_attention_student/examples/gnes_example.py
+-rwxr-xr-x   0        0        0    11569 2022-12-29 07:58:42.522987 graph_attention_student-0.7.1/graph_attention_student/examples/gnnx_example.py
+-rwxr-xr-x   0        0        0    18745 2022-12-29 07:58:42.522987 graph_attention_student-0.7.1/graph_attention_student/examples/smiles_example.py
+-rw-r--r--   0        0        0    14585 2023-01-20 12:59:31.279402 graph_attention_student-0.7.1/graph_attention_student/examples/vgd_multitask_gnn.py
+-rw-r--r--   0        0        0     5503 2023-01-20 11:59:55.452453 graph_attention_student-0.7.1/graph_attention_student/examples/vgd_multitask_gnn_gatv2.py
+-rw-r--r--   0        0        0     4809 2023-01-20 11:39:35.159855 graph_attention_student-0.7.1/graph_attention_student/examples/vgd_multitask_gnn_gin.py
+-rwxr-xr-x   0        0        0    20103 2023-01-20 10:32:00.863590 graph_attention_student-0.7.1/graph_attention_student/examples/vgd_multitask_megan.py
+-rw-r--r--   0        0        0     1272 2023-01-20 09:42:42.629614 graph_attention_student-0.7.1/graph_attention_student/examples/vgd_multitask_megan_tadf.py
+-rwxr-xr-x   0        0        0      726 2022-12-29 07:58:42.522987 graph_attention_student-0.7.1/graph_attention_student/experiments/README.rst
+-rwxr-xr-x   0        0        0        0 2022-12-29 07:58:42.522987 graph_attention_student-0.7.1/graph_attention_student/experiments/__init__.py
+-rw-r--r--   0        0        0    10604 2023-03-28 09:55:24.672691 graph_attention_student-0.7.1/graph_attention_student/experiments/__pycache__/vgd_classification.cpython-310.pyc
+-rw-r--r--   0        0        0    15106 2023-03-20 09:39:48.984068 graph_attention_student-0.7.1/graph_attention_student/experiments/__pycache__/vgd_regression_supervised.cpython-310.pyc
+-rw-r--r--   0        0        0    10324 2023-04-19 12:44:07.919515 graph_attention_student-0.7.1/graph_attention_student/experiments/__pycache__/vgd_single.cpython-310.pyc
+-rw-r--r--   0        0        0     6258 2023-01-24 12:19:49.929234 graph_attention_student-0.7.1/graph_attention_student/experiments/__pycache__/vgd_single_gnnx.cpython-310.pyc
+-rw-r--r--   0        0        0     1373 2023-01-24 14:25:26.991807 graph_attention_student-0.7.1/graph_attention_student/experiments/__pycache__/vgd_single_gnnx_aqsoldb.cpython-310.pyc
+-rw-r--r--   0        0        0     4729 2023-04-19 12:44:06.195491 graph_attention_student-0.7.1/graph_attention_student/experiments/__pycache__/vgd_single_megan.cpython-310.pyc
+-rw-r--r--   0        0        0     1345 2023-01-24 12:56:57.478326 graph_attention_student-0.7.1/graph_attention_student/experiments/__pycache__/vgd_single_megan_aqsoldb.cpython-310.pyc
+-rwxr-xr-x   0        0        0     9205 2022-12-29 07:58:42.522987 graph_attention_student-0.7.1/graph_attention_student/experiments/process_aqsoldb.py
+-rwxr-xr-x   0        0        0    31932 2022-12-29 07:58:42.522987 graph_attention_student-0.7.1/graph_attention_student/experiments/rb_motifs_multi.py
+-rwxr-xr-x   0        0        0    34843 2022-12-29 07:58:42.522987 graph_attention_student-0.7.1/graph_attention_student/experiments/rb_motifs_single.py
+-rw-r--r--   0        0        0      459 2023-01-24 12:36:03.337029 graph_attention_student-0.7.1/graph_attention_student/experiments/template_sub_experiment.py
+-rw-r--r--   0        0        0    18495 2023-03-28 09:55:23.204678 graph_attention_student-0.7.1/graph_attention_student/experiments/vgd_classification.py
+-rw-r--r--   0        0        0     5029 2023-03-29 07:00:40.799553 graph_attention_student-0.7.1/graph_attention_student/experiments/vgd_classification_megan.py
+-rw-r--r--   0        0        0    18717 2023-03-19 08:35:02.980618 graph_attention_student-0.7.1/graph_attention_student/experiments/vgd_regression_posthoc.py
+-rw-r--r--   0        0        0    24342 2023-03-20 09:39:47.552048 graph_attention_student-0.7.1/graph_attention_student/experiments/vgd_regression_supervised.py
+-rw-r--r--   0        0        0     5567 2023-03-20 09:39:47.564048 graph_attention_student-0.7.1/graph_attention_student/experiments/vgd_regression_supervised_multi.py
+-rw-r--r--   0        0        0     5788 2023-03-20 07:08:16.190877 graph_attention_student-0.7.1/graph_attention_student/experiments/vgd_regression_supervised_single.py
+-rw-r--r--   0        0        0    17117 2023-04-19 12:42:45.170288 graph_attention_student-0.7.1/graph_attention_student/experiments/vgd_single.py
+-rw-r--r--   0        0        0     8128 2023-01-24 12:19:49.761232 graph_attention_student-0.7.1/graph_attention_student/experiments/vgd_single_gnnx.py
+-rw-r--r--   0        0        0     1038 2023-01-24 14:25:25.831799 graph_attention_student-0.7.1/graph_attention_student/experiments/vgd_single_gnnx_aqsoldb.py
+-rw-r--r--   0        0        0     5506 2023-01-24 13:54:11.870993 graph_attention_student-0.7.1/graph_attention_student/experiments/vgd_single_gnnx_aqsoldb_dmpnn.py
+-rw-r--r--   0        0        0     3581 2023-01-24 14:26:38.996305 graph_attention_student-0.7.1/graph_attention_student/experiments/vgd_single_gnnx_aqsoldb_gatv2.py
+-rw-r--r--   0        0        0     5234 2023-01-24 13:19:46.309473 graph_attention_student-0.7.1/graph_attention_student/experiments/vgd_single_gnnx_aqsoldb_painn.py
+-rw-r--r--   0        0        0     7948 2023-04-19 12:44:06.007488 graph_attention_student-0.7.1/graph_attention_student/experiments/vgd_single_megan.py
+-rw-r--r--   0        0        0     1034 2023-04-19 12:46:43.177610 graph_attention_student-0.7.1/graph_attention_student/experiments/vgd_single_megan_aqsoldb.py
+-rw-r--r--   0        0        0      695 2023-02-27 13:28:58.309313 graph_attention_student-0.7.1/graph_attention_student/keras.py
+-rwxr-xr-x   0        0        0    20274 2023-02-23 19:42:55.562555 graph_attention_student-0.7.1/graph_attention_student/layers.py
+-rw-r--r--   0        0        0      205 2023-03-19 09:12:41.525356 graph_attention_student-0.7.1/graph_attention_student/models/__init__.py
+-rw-r--r--   0        0        0      380 2023-03-19 09:15:50.038102 graph_attention_student-0.7.1/graph_attention_student/models/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3314 2023-04-01 14:29:59.234990 graph_attention_student-0.7.1/graph_attention_student/models/__pycache__/gnes.cpython-310.pyc
+-rw-r--r--   0        0        0     1950 2023-03-19 09:15:50.054102 graph_attention_student-0.7.1/graph_attention_student/models/__pycache__/gnnx.cpython-310.pyc
+-rw-r--r--   0        0        0     9247 2023-04-01 10:01:31.663992 graph_attention_student-0.7.1/graph_attention_student/models/__pycache__/gradient.cpython-310.pyc
+-rw-r--r--   0        0        0    15003 2023-03-28 11:59:53.838597 graph_attention_student-0.7.1/graph_attention_student/models/__pycache__/megan.cpython-310.pyc
+-rw-r--r--   0        0        0     3406 2023-04-01 14:29:47.290900 graph_attention_student-0.7.1/graph_attention_student/models/gnes.py
+-rw-r--r--   0        0        0     2590 2023-03-19 09:15:48.990097 graph_attention_student-0.7.1/graph_attention_student/models/gnnx.py
+-rw-r--r--   0        0        0    12361 2023-04-01 10:01:20.259917 graph_attention_student-0.7.1/graph_attention_student/models/gradient.py
+-rw-r--r--   0        0        0    28462 2023-03-28 11:59:52.766589 graph_attention_student-0.7.1/graph_attention_student/models/megan.py
+-rwxr-xr-x   0        0        0     1040 2023-01-18 09:06:23.993806 graph_attention_student-0.7.1/graph_attention_student/templates/article.tex.j2
+-rw-r--r--   0        0        0      375 2023-01-24 12:08:49.160527 graph_attention_student-0.7.1/graph_attention_student/templates/table.tex.j2
+-rw-r--r--   0        0        0      151 2023-01-17 16:58:58.659355 graph_attention_student-0.7.1/graph_attention_student/templates/table_content.tex.j2
+-rw-r--r--   0        0        0       76 2023-01-17 17:10:30.475776 graph_attention_student-0.7.1/graph_attention_student/templates/table_element_mean.tex.j2
+-rwxr-xr-x   0        0        0    13166 2023-04-01 11:27:51.694228 graph_attention_student-0.7.1/graph_attention_student/training.py
+-rwxr-xr-x   0        0        0     3753 2022-12-29 07:58:42.522987 graph_attention_student-0.7.1/graph_attention_student/typing.py
+-rwxr-xr-x   0        0        0    15021 2023-01-18 08:39:58.301379 graph_attention_student-0.7.1/graph_attention_student/util.py
+-rwxr-xr-x   0        0        0    16147 2023-03-27 10:44:14.975799 graph_attention_student-0.7.1/graph_attention_student/visualization.py
+-rwxr-xr-x   0        0        0     1397 2023-04-19 13:30:28.439135 graph_attention_student-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0    10441 1970-01-01 00:00:00.000000 graph_attention_student-0.7.1/setup.py
+-rw-r--r--   0        0        0    10052 1970-01-01 00:00:00.000000 graph_attention_student-0.7.1/PKG-INFO
```

### Comparing `graph_attention_student-0.7.0/README.rst` & `graph_attention_student-0.7.1/README.rst`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.0/graph_attention_student/_models.py` & `graph_attention_student-0.7.1/graph_attention_student/_models.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.0/graph_attention_student/cli.py` & `graph_attention_student-0.7.1/graph_attention_student/cli.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.0/graph_attention_student/data.py` & `graph_attention_student-0.7.1/graph_attention_student/data.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.0/graph_attention_student/examples/__pycache__/vgd_multitask_gnn.cpython-310.pyc` & `graph_attention_student-0.7.1/graph_attention_student/examples/__pycache__/vgd_multitask_gnn.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.0/graph_attention_student/examples/__pycache__/vgd_multitask_megan.cpython-310.pyc` & `graph_attention_student-0.7.1/graph_attention_student/examples/__pycache__/vgd_multitask_megan.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.0/graph_attention_student/examples/gnes_example.py` & `graph_attention_student-0.7.1/graph_attention_student/examples/gnes_example.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.0/graph_attention_student/examples/gnnx_example.py` & `graph_attention_student-0.7.1/graph_attention_student/examples/gnnx_example.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.0/graph_attention_student/examples/smiles_example.py` & `graph_attention_student-0.7.1/graph_attention_student/examples/smiles_example.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.0/graph_attention_student/examples/vgd_multitask_gnn.py` & `graph_attention_student-0.7.1/graph_attention_student/examples/vgd_multitask_gnn.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.0/graph_attention_student/examples/vgd_multitask_gnn_gatv2.py` & `graph_attention_student-0.7.1/graph_attention_student/examples/vgd_multitask_gnn_gatv2.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.0/graph_attention_student/examples/vgd_multitask_gnn_gin.py` & `graph_attention_student-0.7.1/graph_attention_student/examples/vgd_multitask_gnn_gin.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.0/graph_attention_student/examples/vgd_multitask_megan.py` & `graph_attention_student-0.7.1/graph_attention_student/examples/vgd_multitask_megan.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.0/graph_attention_student/examples/vgd_multitask_megan_tadf.py` & `graph_attention_student-0.7.1/graph_attention_student/examples/vgd_multitask_megan_tadf.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.0/graph_attention_student/experiments/README.rst` & `graph_attention_student-0.7.1/graph_attention_student/experiments/README.rst`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.0/graph_attention_student/experiments/__pycache__/vgd_regression_supervised.cpython-310.pyc` & `graph_attention_student-0.7.1/graph_attention_student/experiments/__pycache__/vgd_regression_supervised.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.0/graph_attention_student/experiments/__pycache__/vgd_single.cpython-310.pyc` & `graph_attention_student-0.7.1/graph_attention_student/experiments/__pycache__/vgd_single.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jan 24 14:34:55 2023 UTC, .py size: 16880 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 19% similar despite different names*

```diff
@@ -1,643 +1,646 @@
-00000000: 6f0d 0d0a 0000 0000 8fec cf63 f041 0000  o..........c.A..
+00000000: 6f0d 0d0a 0000 0000 c5e1 3f64 dd42 0000  o.........?d.B..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0019 0000 0040 0000 0073 360c 0000 5500  .....@...s6...U.
-00000030: 6400 6401 6c00 5a00 6400 6401 6c01 5a01  d.d.l.Z.d.d.l.Z.
-00000040: 6400 6401 6c02 5a02 6400 6401 6c03 5a03  d.d.l.Z.d.d.l.Z.
-00000050: 6400 6401 6c04 5a05 6400 6402 6c06 6d07  d.d.l.Z.d.d.l.m.
-00000060: 5a07 0100 6400 6401 6c08 5a09 6400 6401  Z...d.d.l.Z.d.d.
-00000070: 6c0a 6d0b 5a0c 0100 6400 6401 6c0d 5a0e  l.m.Z...d.d.l.Z.
-00000080: 6400 6401 6c0f 6d10 5a11 0100 6400 6403  d.d.l.m.Z...d.d.
-00000090: 6c12 6d13 5a13 0100 6400 6404 6c12 6d14  l.m.Z...d.d.l.m.
-000000a0: 5a14 0100 6400 6405 6c12 6d15 5a15 0100  Z...d.d.l.m.Z...
-000000b0: 6400 6406 6c12 6d16 5a16 0100 6400 6407  d.d.l.m.Z...d.d.
-000000c0: 6c17 6d18 5a18 0100 6400 6408 6c19 6d1a  l.m.Z...d.d.l.m.
-000000d0: 5a1a 0100 6400 6409 6c1b 6d1c 5a1c 0100  Z...d.d.l.m.Z...
-000000e0: 6400 640a 6c1d 6d1e 5a1e 0100 6400 640b  d.d.l.m.Z...d.d.
-000000f0: 6c1f 6d20 5a20 0100 6400 6401 6c21 6d04  l.m Z ..d.d.l!m.
-00000100: 5a22 0100 6400 640c 6c23 6d24 5a24 0100  Z"..d.d.l#m$Z$..
-00000110: 6400 640d 6c25 6d26 5a26 6d27 5a27 0100  d.d.l%m&Z&m'Z'..
-00000120: 6400 640e 6c25 6d28 5a28 6d29 5a29 0100  d.d.l%m(Z(m)Z)..
-00000130: 6400 640f 6c25 6d2a 5a2a 0100 6500 6a2b  d.d.l%m*Z*..e.j+
-00000140: a02c 6410 a101 5a2d 652e 652f 6411 3c00  .,d...Z-e.e/d.<.
-00000150: 6401 5a30 6505 6a31 6532 1900 652f 6412  d.Z0e.j1e2..e/d.
-00000160: 3c00 6413 5a33 6534 652f 6414 3c00 6415  <.d.Z3e4e/d.<.d.
-00000170: 5a35 6532 652f 6416 3c00 6700 5a36 6505  Z5e2e/d.<.g.Z6e.
-00000180: 6a37 6532 1900 652f 6417 3c00 6418 5a38  j7e2..e/d.<.d.Z8
-00000190: 6419 5a39 6505 6a31 652e 1900 652f 641a  d.Z9e.j1e...e/d.
-000001a0: 3c00 641b 5a3a 6505 6a31 652e 1900 652f  <.d.Z:e.j1e...e/
-000001b0: 641c 3c00 641d 5a3b 653c 652f 641e 3c00  d.<.d.Z;e<e/d.<.
-000001c0: 641f 5a3d 653c 652f 6420 3c00 641d 5a3e  d.Z=e<e/d <.d.Z>
-000001d0: 653c 652f 6421 3c00 6422 5a3f 652e 652f  e<e/d!<.d"Z?e.e/
-000001e0: 6423 3c00 6418 5a40 6532 652f 6424 3c00  d#<.d.Z@e2e/d$<.
-000001f0: 6425 6426 8400 5a41 6427 5a42 6532 652f  d%d&..ZAd'ZBe2e/
-00000200: 6428 3c00 6429 5a43 6532 652f 642a 3c00  d(<.d)ZCe2e/d*<.
-00000210: 642b 5a44 652e 652f 642c 3c00 6415 5a45  d+ZDe.e/d,<.d.ZE
-00000220: 6532 652f 642d 3c00 6427 5a46 6532 652f  e2e/d-<.d'ZFe2e/
-00000230: 642e 3c00 642f 6701 5a47 6500 a048 a100  d.<.d/g.ZGe..H..
-00000240: 5a49 6430 5a4a 641f 5a4b 6518 8300 9004  ZId0ZJd.ZKe.....
-00000250: 8f1b 0100 651a 6549 654a 654c 8300 8303  ....e.eIeJeL....
-00000260: 0400 5a4d 9004 8f00 0100 6500 6a2b a04e  ..ZM......e.j+.N
-00000270: 652d a101 5a4f 654d a050 6431 654f 9b00  e-..ZOeM.Pd1eO..
-00000280: 6432 9d03 a101 0100 651c 652d 654d 6a51  d2......e.e-eMjQ
-00000290: 6545 641f 6433 8d04 5c02 5a52 5a53 6554  eEd.d3..\.ZRZSeT
-000002a0: 6555 6553 a056 a100 8301 8301 5a57 6558  eUeS.V......ZWeX
-000002b0: 6557 8301 5a59 655a 6553 8301 5a5b 6700  eW..ZYeZeS..Z[g.
-000002c0: 5a5c 6505 6a37 6522 6a5d 1900 652f 6434  Z\e.j7e"j]..e/d4
-000002d0: 3c00 6557 4400 5d7b 5a5e 6553 655e 1900  <.eWD.]{Z^eSe^..
-000002e0: 5a5f 655f 6435 1900 6436 1900 5a60 6539  Z_e_d5..d6..Z`e9
-000002f0: 6401 7501 9001 726c 6560 6539 1900 6560  d.u...rle`e9..e`
-00000300: 6437 3c00 6e0e 650e 6a61 655a 6560 6438  d7<.n.e.jaeZe`d8
-00000310: 1900 8301 6538 6602 6439 8d01 6560 6437  ....e8f.d9..e`d7
-00000320: 3c00 653a 6401 7501 9001 7286 6560 653a  <.e:d.u...r.e`e:
-00000330: 1900 6560 643a 3c00 6e0e 650e 6a61 655a  ..e`d:<.n.e.jaeZ
-00000340: 6560 643b 1900 8301 6538 6602 6439 8d01  e`d;....e8f.d9..
-00000350: 6560 643a 3c00 653b 9001 72a5 650e a062  e`d:<.e;..r.e..b
-00000360: 643c 643d 8400 6560 6438 1900 4400 8301  d<d=..e`d8..D...
-00000370: a101 6560 643e 3c00 653e 9001 72b8 650e  ..e`d><.e>..r.e.
-00000380: a062 643f 643d 8400 6563 6560 643b 1900  .bd?d=..ece`d;..
-00000390: 8301 4400 8301 a101 6560 6440 3c00 653d  ..D.....e`d@<.e=
-000003a0: 9001 73c9 650e 6a64 655a 6560 643b 1900  ..s.e.jdeZe`d;..
-000003b0: 8301 6418 6602 6439 8d01 6560 6440 3c00  ..d.f.d9..e`d@<.
-000003c0: 655c a065 6560 a101 0100 9001 7154 654d  e\.ee`......qTeM
-000003d0: a050 6441 655a 655c 8301 9b00 6442 9d03  .PdAeZe\....dB..
-000003e0: a101 0100 654d 6a66 6443 641f 6444 8d02  ....eMjfdCd.dD..
-000003f0: 6445 6443 8400 8301 5a67 6568 6540 8301  dEdC....Zgehe@..
-00000400: 4400 9003 5d2a 5a69 654d a050 6446 6569  D...]*ZieM.PdFei
-00000410: 6418 1700 9b00 6447 6540 9b00 6448 9d05  d.....dGe@..dH..
-00000420: a101 0100 6569 654d 6449 3c00 6509 a06a  ....eieMdI<.e..j
-00000430: 6544 a101 9003 8f06 0100 6530 6401 7501  eD........e0d.u.
-00000440: 9002 7223 654d a050 644a a101 0100 644b  ..r#eM.PdJ....dK
-00000450: 643d 8400 6553 a06b a100 4400 8301 5a6c  d=..eS.k..D...Zl
-00000460: 644c 643d 8400 6553 a06b a100 4400 8301  dLd=..eS.k..D...
-00000470: 5a6d 6e1d 654d a050 644d a101 0100 6503  Zmn.eM.PdM....e.
-00000480: 6a6e 6557 6532 6533 655b 1400 8301 644e  jneWe2e3e[....dN
-00000490: 8d02 5a6c 6558 656c 8301 5a6f 6559 a070  ..ZleXel..ZoeY.p
-000004a0: 656f a101 5a71 6554 6571 8301 5a6d 6558  eo..ZqeTeq..ZmeX
-000004b0: 656d 8301 6558 6536 8301 4200 5a71 6554  em..eXe6..B.ZqeT
-000004c0: 6571 8301 5a6d 654d a050 644f 655a 656c  eq..ZmeM.PdOeZel
-000004d0: 8301 9b00 6450 655a 656d 8301 9b00 6451  ....dPeZem....dQ
-000004e0: 9d05 a101 0100 656c 654d 6452 6569 9b00  ......eleMdRei..
-000004f0: 9d02 3c00 656d 654d 6453 6569 9b00 9d02  ..<.emeMdSei....
-00000500: 3c00 6572 6535 655a 656d 8301 8302 655a  <.ere5eZem....eZ
-00000510: 6536 8301 1800 5a73 6536 6554 6503 6a6e  e6....Zse6eTe.jn
-00000520: 656d 6573 644e 8d02 8301 1700 5a74 654d  emesdN......ZteM
-00000530: a050 644f 655a 6574 8301 9b00 6454 9d03  .PdOeZet....dT..
-00000540: a101 0100 6574 654d 6455 6569 9b00 9d02  ....eteMdUei....
-00000550: 3c00 654d a050 6456 a101 0100 654d 6a75  <.eM.PdV....eMju
-00000560: 6443 655c 656c 656d 6457 8d04 5c04 5a76  dCe\elemdW..\.Zv
-00000570: 5a77 5a78 5a79 654d a050 6458 a101 0100  ZwZxZyeM.PdX....
-00000580: 654d a075 6459 a101 5a7a 650c 6a7b 6a7c  eM.udY..Zze.j{j|
-00000590: 652f 645a 3c00 654d a050 645b a101 0100  e/dZ<.eM.Pd[....
-000005a0: 654d 6a75 645c 657a 6576 6577 6578 6579  eMjud\ezevewexey
-000005b0: 645d 8d06 5a7d 657e 652f 645e 3c00 657d  d]..Z}e~e/d^<.e}
-000005c0: 654d 645f 6569 9b00 9d02 3c00 6554 6568  eMd_ei....<.eTeh
-000005d0: 6543 8301 8301 654d 6460 6569 9b00 9d02  eC....eMd`ei....
-000005e0: 3c00 654d a050 6461 a101 0100 654d 6a75  <.eM.Pda....eMju
-000005f0: 6462 657a 6578 6579 641f 6463 8d05 5c03  dbezexeyd.dc..\.
-00000600: 5a7f 5a80 5a81 650e a062 657f a00d a100  Z.Z.Z.e..be.....
-00000610: a101 5a7f 650e a062 6580 a00d a100 a101  ..Z.e..be.......
-00000620: 5a80 650e a062 6581 a00d a100 a101 5a81  Z.e..be.......Z.
-00000630: 650e a062 6579 6400 1900 a101 5a82 650e  e..beyd.....Z.e.
-00000640: a062 6579 6418 1900 a00d a100 a101 5a83  .beyd.........Z.
-00000650: 650e a062 6579 6464 1900 a00d a100 a101  e..beydd........
-00000660: 5a84 654d a050 6465 a101 0100 6514 657f  Z.eM.Pde....e.e.
-00000670: 6582 8302 5a85 650e a086 6585 a101 5a87  e...Z.e...e...Z.
-00000680: 6515 657f 6582 8302 5a88 6513 657f 6582  e.e.e...Z.e.e.e.
-00000690: 8302 5a89 6585 654d 6466 6569 9b00 9d02  ..Z.e.eMdfei....
-000006a0: 3c00 6587 654d 6467 6569 9b00 9d02 3c00  <.e.eMdgei....<.
-000006b0: 6588 654d 6468 6569 9b00 9d02 3c00 6589  e.eMdhei....<.e.
-000006c0: 654d 6469 6569 9b00 9d02 3c00 654d a050  eMdiei....<.eM.P
-000006d0: 646a a101 0100 654d 6a75 646b 657a 656d  dj....eMjudkezem
-000006e0: 6578 6579 657f 6580 6581 646c 8d08 5a8a  exeye.e.e.dl..Z.
-000006f0: 658b 656d 658a 8302 4400 5d0f 5c02 5a5e  e.eme...D.].\.Z^
-00000700: 5a8c 658c 654d 646d 6569 9b00 6447 655e  Z.e.eMdmei..dGe^
-00000710: 9b00 9d04 3c00 9003 7166 654d a050 646e  ....<...qfeM.Pdn
-00000720: a101 0100 6700 5a8d 6700 5a8e 6700 5a8f  ....g.Z.g.Z.g.Z.
-00000730: 6700 5a90 6563 656d 8301 4400 5d9d 5c02  g.Z.ecem..D.].\.
-00000740: 5a91 5a5e 6553 655e 1900 6435 1900 6436  Z.Z^eSe^..d5..d6
-00000750: 1900 5a60 6526 6580 6591 1900 8301 5a92  ..Z`e&e.e.....Z.
-00000760: 6526 6581 6591 1900 8301 5a93 6534 6560  e&e.e.....Z.e4e`
-00000770: 646f 1900 6400 1900 8301 654d 6470 6569  do..d.....eMdpei
-00000780: 9b00 6447 655e 9b00 9d04 3c00 6534 657f  ..dGe^....<.e4e.
-00000790: 6591 1900 6400 1900 8301 654d 6471 6569  e...d.....eMdqei
-000007a0: 9b00 6447 655e 9b00 9d04 3c00 6592 654d  ..dGe^....<.e.eM
-000007b0: 6472 6569 9b00 6447 655e 9b00 9d04 3c00  drei..dGe^....<.
-000007c0: 6593 654d 6473 6569 9b00 6447 655e 9b00  e.eMdsei..dGe^..
-000007d0: 9d04 3c00 658d 6580 6591 1900 a094 a100  ..<.e.e.e.......
-000007e0: a095 a100 3700 5a8d 658e 6581 6591 1900  ....7.Z.e.e.e...
-000007f0: a094 a100 a095 a100 3700 5a8e 658f 6583  ........7.Z.e.e.
-00000800: 6591 1900 a094 a100 a095 a100 3700 5a8f  e...........7.Z.
-00000810: 6590 6584 6591 1900 a094 a100 a095 a100  e.e.e...........
-00000820: 3700 5a90 6534 650e a096 6527 6592 6474  7.Z.e4e...e'e.dt
-00000830: 8302 a101 8301 5a97 6534 650e a096 6527  ......Z.e4e...e'
-00000840: 6593 6474 8302 a101 8301 5a98 6597 654d  e.dt......Z.e.eM
-00000850: 6475 6569 9b00 6447 655e 9b00 9d04 3c00  duei..dGe^....<.
-00000860: 6598 654d 6476 6569 9b00 6447 655e 9b00  e.eMdvei..dGe^..
-00000870: 9d04 3c00 9003 7187 650e a096 6554 654d  ..<...q.e...eTeM
-00000880: 646d 6569 9b00 9d02 1900 a099 a100 8301  dmei............
-00000890: a101 5a9a 650e a096 6554 654d 6475 6569  ..Z.e...eTeMduei
-000008a0: 9b00 9d02 1900 a099 a100 8301 a101 5a9b  ..............Z.
-000008b0: 650e a096 6554 654d 6476 6569 9b00 9d02  e...eTeMdvei....
-000008c0: 1900 a099 a100 8301 a101 5a9c 7a0c 6516  ..........Z.z.e.
-000008d0: 658f 658d 8302 5a9d 6516 6590 658e 8302  e.e...Z.e.e.e...
-000008e0: 5a9e 5700 6e0e 0400 659f 9004 7969 0100  Z.W.n...e...yi..
-000008f0: 0100 0100 6474 5a9d 6474 5a9e 5900 6e01  ....dtZ.dtZ.Y.n.
-00000900: 7700 659d 654d 6477 6569 9b00 9d02 3c00  w.e.eMdwei....<.
-00000910: 659e 654d 6478 6569 9b00 9d02 3c00 654d  e.eMdxei....<.eM
-00000920: a050 6479 6585 647a 9b04 647b 6587 647a  .Pdye.dz..d{e.dz
-00000930: 9b04 647c 6588 647a 9b04 647d 6589 647a  ..d|e.dz..d}e.dz
-00000940: 9b04 647e 659a 647a 9b04 647f 659b 647a  ..d~e.dz..d.e.dz
-00000950: 9b04 6480 659c 647a 9b04 6481 659d 647a  ..d.e.dz..d.e.dz
-00000960: 9b04 6482 659e 647a 9b04 9d12 a101 0100  ..d.e.dz........
-00000970: 654d a050 6483 a101 0100 6700 5aa0 6700  eM.Pd.....g.Z.g.
-00000980: 5aa1 6574 4400 5d1d 5a5e 65a0 a065 654d  Z.etD.].Z^e..eeM
-00000990: 6472 6569 9b00 6447 655e 9b00 9d04 1900  drei..dGe^......
-000009a0: a101 0100 65a1 a065 654d 6473 6569 9b00  ....e..eeMdsei..
-000009b0: 6447 655e 9b00 9d04 1900 a101 0100 9004  dGe^............
-000009c0: 71ac 6500 6a2b a0a2 654d 6a2b 6484 6569  q.e.j+..eMj+d.ei
-000009d0: 6485 9b04 6486 9d03 a102 5aa3 6487 643d  d...d.....Z.d.d=
-000009e0: 8400 6574 4400 8301 5aa4 6488 643d 8400  ..etD...Z.d.d=..
-000009f0: 6574 4400 8301 5aa5 6489 643d 8400 65a4  etD...Z.d.d=..e.
-00000a00: 4400 8301 5aa6 651e 65a4 65a5 65a6 645a  D...Z.e.e.e.e.dZ
-00000a10: 65a0 65a1 6602 6901 65a3 6547 648a 643d  e.e.f.i.e.eGd.d=
-00000a20: 8400 6574 4400 8301 648b 8d07 0100 654d  ..etD...d.....eM
-00000a30: a0a7 a100 0100 5700 6401 0400 0400 8303  ......W.d.......
-00000a40: 0100 6e09 3100 9005 730f 7701 0100 0100  ..n.1...s.w.....
-00000a50: 0100 5900 0100 9001 71ea 5700 6401 0400  ..Y.....q.W.d...
-00000a60: 0400 8303 0100 6e09 3100 9005 7321 7701  ......n.1...s!w.
-00000a70: 0100 0100 0100 5900 0100 5700 6401 0400  ......Y...W.d...
-00000a80: 0400 8303 0100 6e09 3100 9005 7331 7701  ......n.1...s1w.
-00000a90: 0100 0100 0100 5900 0100 6518 8300 8fd7  ......Y...e.....
-00000aa0: 0100 654d 6aa8 8fba 0100 654d a050 648c  ..eMj.....eM.Pd.
-00000ab0: a101 0100 6700 648d a201 5aa9 6700 5aaa  ....g.d...Z.g.Z.
-00000ac0: 6700 5aab 65ab a065 648e a101 0100 65ab  g.Z.e..ed.....e.
-00000ad0: a065 648f 643d 8400 6568 6540 8301 4400  .ed.d=..ehe@..D.
-00000ae0: 8301 a101 0100 65ab a065 6490 643d 8400  ......e..ed.d=..
-00000af0: 6568 6540 8301 4400 8301 a101 0100 65ab  ehe@..D.......e.
-00000b00: a065 6491 643d 8400 6568 6540 8301 4400  .ed.d=..ehe@..D.
-00000b10: 8301 a101 0100 65ab a065 6492 643d 8400  ......e..ed.d=..
-00000b20: 6568 6540 8301 4400 8301 a101 0100 65ab  ehe@..D.......e.
-00000b30: a065 6493 643d 8400 6568 6540 8301 4400  .ed.d=..ehe@..D.
-00000b40: 8301 a101 0100 65ab a065 6494 643d 8400  ......e..ed.d=..
-00000b50: 6568 6540 8301 4400 8301 a101 0100 65ab  ehe@..D.......e.
-00000b60: a065 6495 643d 8400 6568 6540 8301 4400  .ed.d=..ehe@..D.
-00000b70: 8301 a101 0100 65ab a065 6496 643d 8400  ......e..ed.d=..
-00000b80: 6568 6540 8301 4400 8301 a101 0100 65ab  ehe@..D.......e.
-00000b90: a065 6497 643d 8400 6568 6540 8301 4400  .ed.d=..ehe@..D.
-00000ba0: 8301 a101 0100 65aa a065 65ab a101 0100  ......e..ee.....
-00000bb0: 6528 65a9 65aa 6529 6498 6540 9b00 6499  e(e.e.e)d.e@..d.
-00000bc0: 9d03 649a 1700 653f 1700 649b 1700 649c  ..d...e?..d...d.
-00000bd0: 8d04 5c02 5aac 5aad 654d a0ae 649d 65ad  ..\.Z.Z.eM..d.e.
-00000be0: a102 0100 6500 6a2b a0a2 654d 6a2b 649e  ....e.j+..eMj+d.
-00000bf0: a102 5aa3 652a 649f 65ad 6901 65a3 64a0  ..Z.e*d.e.i.e.d.
-00000c00: 8d02 0100 654d a050 64a1 a101 0100 5700  ....eM.Pd.....W.
-00000c10: 6401 0400 0400 8303 0100 6e11 3100 9005  d.........n.1...
-00000c20: 73fb 7701 0100 0100 0100 5900 0100 5700  s.w.......Y...W.
-00000c30: 6401 0400 0400 8303 0100 6401 5300 5700  d.........d.S.W.
-00000c40: 6401 0400 0400 8303 0100 6401 5300 3100  d.........d.S.1.
-00000c50: 9006 7314 7701 0100 0100 0100 5900 0100  ..s.w.......Y...
-00000c60: 6401 5300 29a2 e900 0000 004e 2901 da07  d.S.)......N)...
-00000c70: 436f 756e 7465 7229 01da 0872 325f 7363  Counter)...r2_sc
-00000c80: 6f72 6529 01da 126d 6561 6e5f 7371 7561  ore)...mean_squa
-00000c90: 7265 645f 6572 726f 7229 01da 136d 6561  red_error)...mea
-00000ca0: 6e5f 6162 736f 6c75 7465 5f65 7272 6f72  n_absolute_error
-00000cb0: 2901 da0d 726f 635f 6175 635f 7363 6f72  )...roc_auc_scor
-00000cc0: 6529 01da 0953 6b69 7070 6162 6c65 2901  e)...Skippable).
-00000cd0: da0a 4578 7065 7269 6d65 6e74 2901 da19  ..Experiment)...
-00000ce0: 6c6f 6164 5f76 6973 7561 6c5f 6772 6170  load_visual_grap
-00000cf0: 685f 6461 7461 7365 7429 01da 1663 7265  h_dataset)...cre
-00000d00: 6174 655f 696d 706f 7274 616e 6365 735f  ate_importances_
-00000d10: 7064 6629 01da 1f72 6167 6765 645f 7465  pdf)...ragged_te
-00000d20: 6e73 6f72 5f66 726f 6d5f 6e65 7374 6564  nsor_from_nested
-00000d30: 5f6e 756d 7079 a901 da15 7072 6f63 6573  _numpy....proces
-00000d40: 735f 6772 6170 685f 6461 7461 7365 7429  s_graph_dataset)
-00000d50: 02da 0f61 7272 6179 5f6e 6f72 6d61 6c69  ...array_normali
-00000d60: 7a65 da10 6269 6e61 7279 5f74 6872 6573  ze..binary_thres
-00000d70: 686f 6c64 2902 da0b 6c61 7465 785f 7461  hold)...latex_ta
-00000d80: 626c 65da 186c 6174 6578 5f74 6162 6c65  ble..latex_table
-00000d90: 5f65 6c65 6d65 6e74 5f6d 6561 6e29 01da  _element_mean)..
-00000da0: 0c72 656e 6465 725f 6c61 7465 787a 307e  .render_latexz0~
-00000db0: 2f2e 7669 7375 616c 5f67 7261 7068 5f64  /.visual_graph_d
-00000dc0: 6174 6173 6574 732f 6461 7461 7365 7473  atasets/datasets
-00000dd0: 2f72 625f 6475 616c 5f6d 6f74 6966 73da  /rb_dual_motifs.
-00000de0: 1956 4953 5541 4c5f 4752 4150 485f 4441  .VISUAL_GRAPH_DA
-00000df0: 5441 5345 545f 5041 5448 da11 5553 455f  TASET_PATH..USE_
-00000e00: 4441 5441 5345 545f 5350 4c49 5467 9a99  DATASET_SPLITg..
-00000e10: 9999 9999 e93f da0b 5452 4149 4e5f 5241  .....?..TRAIN_RA
-00000e20: 5449 4fe9 6400 0000 da0c 4e55 4d5f 4558  TIO.d.....NUM_EX
-00000e30: 414d 504c 4553 da0f 4558 414d 504c 455f  AMPLES..EXAMPLE_
-00000e40: 494e 4449 4345 53e9 0100 0000 da12 6e6f  INDICES.......no
-00000e50: 6465 5f69 6d70 6f72 7461 6e63 6573 5f31  de_importances_1
-00000e60: da14 4e4f 4445 5f49 4d50 4f52 5441 4e43  ..NODE_IMPORTANC
-00000e70: 4553 5f4b 4559 da12 6564 6765 5f69 6d70  ES_KEY..edge_imp
-00000e80: 6f72 7461 6e63 6573 5f31 da14 4544 4745  ortances_1..EDGE
-00000e90: 5f49 4d50 4f52 5441 4e43 4553 5f4b 4559  _IMPORTANCES_KEY
-00000ea0: 46da 1455 5345 5f4e 4f44 455f 434f 4f52  F..USE_NODE_COOR
-00000eb0: 4449 4e41 5445 5354 da13 5553 455f 4544  DINATEST..USE_ED
-00000ec0: 4745 5f41 5454 5249 4255 5445 53da 1055  GE_ATTRIBUTES..U
-00000ed0: 5345 5f45 4447 455f 4c45 4e47 5448 53da  SE_EDGE_LENGTHS.
-00000ee0: 044d 4f43 4bda 0a4d 4f44 454c 5f4e 414d  .MOCK..MODEL_NAM
-00000ef0: 45da 0b52 4550 4554 4954 494f 4e53 6300  E..REPETITIONSc.
-00000f00: 0000 0000 0000 0000 0000 0000 0000 0003  ................
-00000f10: 0000 0043 0000 0073 0e00 0000 7400 6a01  ...C...s....t.j.
-00000f20: 6a02 6401 6402 8d01 5300 2903 4e67 7b14  j.d.d...S.).Ng{.
-00000f30: ae47 e17a 843f 2901 da0d 6c65 6172 6e69  .G.z.?)...learni
-00000f40: 6e67 5f72 6174 6529 03da 026b 73da 0a6f  ng_rate)...ks..o
-00000f50: 7074 696d 697a 6572 73da 054e 6164 616d  ptimizers..Nadam
-00000f60: a900 7228 0000 0072 2800 0000 fa5d 2f68  ..r(...r(....]/h
-00000f70: 6f6d 652f 6a6f 6e61 732f 5072 6976 6174  ome/jonas/Privat
-00000f80: 652f 6772 6170 685f 6174 7465 6e74 696f  e/graph_attentio
-00000f90: 6e5f 7374 7564 656e 742f 6772 6170 685f  n_student/graph_
-00000fa0: 6174 7465 6e74 696f 6e5f 7374 7564 656e  attention_studen
-00000fb0: 742f 6578 7065 7269 6d65 6e74 732f 7667  t/experiments/vg
-00000fc0: 645f 7369 6e67 6c65 2e70 79da 083c 6c61  d_single.py..<la
-00000fd0: 6d62 6461 3e50 0000 0073 0200 0000 0e00  mbda>P...s......
-00000fe0: 722a 0000 00e9 0001 0000 da0a 4241 5443  r*..........BATC
-00000ff0: 485f 5349 5a45 e9c8 0000 00da 0645 504f  H_SIZE.......EPO
-00001000: 4348 537a 0567 7075 3a30 da06 4445 5649  CHSz.gpu:0..DEVI
-00001010: 4345 da0d 4c4f 475f 5354 4550 5f45 5641  CE..LOG_STEP_EVA
-00001020: 4cda 0f42 4154 4348 5f53 495a 455f 4556  L..BATCH_SIZE_EV
-00001030: 414c da09 7072 6564 6963 7465 647a 1272  AL..predictedz.r
-00001040: 6573 756c 7473 2f76 6764 5f73 696e 676c  esults/vgd_singl
-00001050: 657a 2553 7461 7274 696e 6720 746f 2074  ez%Starting to t
-00001060: 7261 696e 2047 4e4e 5820 6d6f 6465 6c20  rain GNNX model 
-00001070: 6f6e 2076 6764 2022 fa01 2229 03da 066c  on vgd "..")...l
-00001080: 6f67 6765 72da 086c 6f67 5f73 7465 70da  ogger..log_step.
-00001090: 176d 6574 6164 6174 615f 636f 6e74 6169  .metadata_contai
-000010a0: 6e73 5f69 6e64 6578 da07 6461 7461 7365  ns_index..datase
-000010b0: 74da 086d 6574 6164 6174 61da 0567 7261  t..metadata..gra
-000010c0: 7068 da10 6e6f 6465 5f69 6d70 6f72 7461  ph..node_importa
-000010d0: 6e63 6573 da0c 6e6f 6465 5f69 6e64 6963  nces..node_indic
-000010e0: 6573 2901 da05 7368 6170 65da 1065 6467  es)...shape..edg
-000010f0: 655f 696d 706f 7274 616e 6365 73da 0c65  e_importances..e
-00001100: 6467 655f 696e 6469 6365 7363 0100 0000  dge_indicesc....
-00001110: 0000 0000 0000 0000 0200 0000 0500 0000  ................
-00001120: 4300 0000 732c 0000 0067 007c 005d 127d  C...s,...g.|.].}
-00001130: 0174 0064 0019 007c 0119 00a0 01a1 0074  .t.d...|.......t
-00001140: 0064 0119 007c 0119 00a0 01a1 0017 0091  .d...|..........
-00001150: 0271 0253 0029 02da 0f6e 6f64 655f 6174  .q.S.)...node_at
-00001160: 7472 6962 7574 6573 da10 6e6f 6465 5f63  tributes..node_c
-00001170: 6f6f 7264 696e 6174 6573 a902 da01 67da  oordinates....g.
-00001180: 0674 6f6c 6973 74a9 02da 022e 30da 0169  .tolist.....0..i
-00001190: 7228 0000 0072 2800 0000 7229 0000 00da  r(...r(...r)....
-000011a0: 0a3c 6c69 7374 636f 6d70 3e8a 0000 0073  .<listcomp>....s
-000011b0: 0600 0000 0600 0201 24ff 7247 0000 0072  ........$.rG...r
-000011c0: 3f00 0000 6301 0000 0000 0000 0000 0000  ?...c...........
-000011d0: 0003 0000 0005 0000 0043 0000 0073 2e00  .........C...s..
-000011e0: 0000 6700 7c00 5d13 5c02 7d01 7d02 7400  ..g.|.].\.}.}.t.
-000011f0: 6400 1900 7c01 1900 a001 a100 7400 6401  d...|.......t.d.
-00001200: 1900 7c01 1900 6701 1700 9102 7102 5300  ..|...g.....q.S.
-00001210: 2902 da0f 6564 6765 5f61 7474 7269 6275  )...edge_attribu
-00001220: 7465 73da 0c65 6467 655f 6c65 6e67 7468  tes..edge_length
-00001230: 7372 4100 0000 2903 7245 0000 0072 4600  srA...).rE...rF.
-00001240: 0000 da01 5f72 2800 0000 7228 0000 0072  ...._r(...r(...r
-00001250: 2900 0000 7247 0000 008e 0000 0073 0600  )...rG.......s..
-00001260: 0000 0600 0601 22ff 7248 0000 007a 146c  ......".rH...z.l
-00001270: 6f61 6465 6420 6461 7461 7365 7420 7769  oaded dataset wi
-00001280: 7468 207a 0920 656c 656d 656e 7473 da0f  th z. elements..
-00001290: 7072 6f63 6573 735f 6461 7461 7365 7429  process_dataset)
-000012a0: 01da 0764 6566 6175 6c74 6304 0000 0000  ...defaultc.....
-000012b0: 0000 0000 0000 0008 0000 0005 0000 0043  ...............C
-000012c0: 0000 0073 2200 0000 7400 7c01 7c02 7c03  ...s"...t.|.|.|.
-000012d0: 6401 8d03 5c04 7d04 7d05 7d06 7d07 7c04  d...\.}.}.}.}.|.
-000012e0: 7c05 7c06 7c07 6604 5300 2902 4e29 02da  |.|.|.f.S.).N)..
-000012f0: 0d74 7261 696e 5f69 6e64 6963 6573 da0c  .train_indices..
-00001300: 7465 7374 5f69 6e64 6963 6573 720c 0000  test_indicesr...
-00001310: 0029 08da 025f 6572 3700 0000 724d 0000  .)..._er7...rM..
-00001320: 0072 4e00 0000 da07 785f 7472 6169 6eda  .rN.....x_train.
-00001330: 0779 5f74 7261 696e da06 785f 7465 7374  .y_train..x_test
-00001340: da06 795f 7465 7374 7228 0000 0072 2800  ..y_testr(...r(.
-00001350: 0000 7229 0000 0072 4b00 0000 9a00 0000  ..r)...rK.......
-00001360: 730c 0000 0002 0202 0102 0102 010e fd0c  s...............
-00001370: 057a 0c52 4550 4554 4954 494f 4e20 28fa  .z.REPETITION (.
-00001380: 012f fa01 29da 0372 6570 7a29 6372 6561  ./..)..repz)crea
-00001390: 7469 6e67 2074 7261 696e 2074 6573 7420  ting train test 
-000013a0: 7370 6c69 7420 6672 6f6d 2064 6174 6173  split from datas
-000013b0: 6574 2e2e 2e63 0100 0000 0000 0000 0000  et...c..........
-000013c0: 0000 0300 0000 0500 0000 4300 0000 f324  ..........C....$
-000013d0: 0000 0067 007c 005d 0e5c 027d 017d 0274  ...g.|.].\.}.}.t
-000013e0: 007c 0264 0019 0064 0119 0076 0072 027c  .|.d...d...v.r.|
-000013f0: 0191 0271 0253 0029 0272 3800 0000 724d  ...q.S.).r8...rM
-00001400: 0000 00a9 0172 1400 0000 a903 7245 0000  .....r......rE..
-00001410: 00da 0569 6e64 6578 da04 6461 7461 7228  ...index..datar(
-00001420: 0000 0072 2800 0000 7229 0000 0072 4700  ...r(...r)...rG.
-00001430: 0000 ac00 0000 f306 0000 000c 000e 010a  ................
-00001440: ff63 0100 0000 0000 0000 0000 0000 0300  .c..............
-00001450: 0000 0500 0000 4300 0000 7257 0000 0029  ......C...rW...)
-00001460: 0272 3800 0000 724e 0000 0072 5800 0000  .r8...rN...rX...
-00001470: 7259 0000 0072 2800 0000 7228 0000 0072  rY...r(...r(...r
-00001480: 2900 0000 7247 0000 00ae 0000 0072 5c00  )...rG.......r\.
-00001490: 0000 7a23 6372 6561 7469 6e67 2072 616e  ..z#creating ran
-000014a0: 646f 6d20 7472 6169 6e20 7465 7374 2073  dom train test s
-000014b0: 706c 6974 2e2e 2e29 01da 016b 7a06 7573  plit...)...kz.us
-000014c0: 696e 6720 7a17 2074 7261 696e 696e 6720  ing z. training 
-000014d0: 656c 656d 656e 7473 2061 6e64 207a 0e20  elements and z. 
-000014e0: 7465 7374 2065 6c65 6d65 6e74 737a 0e74  test elementsz.t
-000014f0: 7261 696e 5f69 6e64 6963 6573 2ffa 0d74  rain_indices/..t
-00001500: 6573 745f 696e 6469 6365 732f 7a0c 2061  est_indices/z. a
-00001510: 7320 6578 616d 706c 6573 7a10 6578 616d  s examplesz.exam
-00001520: 706c 655f 696e 6469 6365 732f 7a36 636f  ple_indices/z6co
-00001530: 6e76 6572 7469 6e67 2064 6174 6173 6574  nverting dataset
-00001540: 2069 6e74 6f20 7261 6767 6564 2074 656e   into ragged ten
-00001550: 736f 7273 2066 6f72 2074 7261 696e 696e  sors for trainin
-00001560: 672e 2e2e 2903 7237 0000 0072 4d00 0000  g...).r7...rM...
-00001570: 724e 0000 007a 1563 7265 6174 696e 6720  rN...z.creating 
-00001580: 7468 6520 6d6f 6465 6c2e 2e2e da0c 6372  the model.....cr
-00001590: 6561 7465 5f6d 6f64 656c da05 6d6f 6465  eate_model..mode
-000015a0: 6c7a 1466 6974 7469 6e67 2074 6865 206d  lz.fitting the m
-000015b0: 6f64 656c 2e2e 2eda 0966 6974 5f6d 6f64  odel.....fit_mod
-000015c0: 656c 2905 7260 0000 0072 5000 0000 7251  el).r`...rP...rQ
-000015d0: 0000 0072 5200 0000 7253 0000 00da 0768  ...rR...rS.....h
-000015e0: 6973 746f 7279 7a08 6869 7374 6f72 792f  istoryz.history/
-000015f0: 7a07 6570 6f63 6873 2f7a 1665 7661 6c75  z.epochs/z.evalu
-00001600: 6174 696e 6720 7465 7374 2073 6574 2e2e  ating test set..
-00001610: 2eda 0b71 7565 7279 5f6d 6f64 656c 2904  ...query_model).
-00001620: 7260 0000 00da 0178 da01 79da 1369 6e63  r`.....x..y..inc
-00001630: 6c75 6465 5f69 6d70 6f72 7461 6e63 6573  lude_importances
-00001640: e902 0000 007a 2163 616c 6375 6c61 7469  .....z!calculati
-00001650: 6e67 2070 7265 6469 6374 696f 6e20 6d65  ng prediction me
-00001660: 7472 6963 732e 2e2e fa04 6d73 652f fa05  trics.....mse/..
-00001670: 726d 7365 2ffa 046d 6165 2ffa 0372 322f  rmse/..mae/..r2/
-00001680: 7a17 6361 6c63 756c 6174 696e 6720 6669  z.calculating fi
-00001690: 6465 6c69 7479 2e2e 2eda 1263 616c 6375  delity.....calcu
-000016a0: 6c61 7465 5f66 6964 656c 6974 7929 0772  late_fidelity).r
-000016b0: 6000 0000 da0c 696e 6469 6365 735f 7472  `.....indices_tr
-000016c0: 7565 da06 785f 7472 7565 da06 795f 7472  ue..x_true..y_tr
-000016d0: 7565 da08 6f75 745f 7072 6564 da07 6e69  ue..out_pred..ni
-000016e0: 5f70 7265 64da 0765 695f 7072 6564 fa09  _pred..ei_pred..
-000016f0: 6669 6465 6c69 7479 2f7a 2263 616c 6375  fidelity/z"calcu
-00001700: 6c61 7469 6e67 2065 7870 6c61 6e61 7469  lating explanati
-00001710: 6f6e 206d 6574 7269 6373 2e2e 2eda 0c67  on metrics.....g
-00001720: 7261 7068 5f6c 6162 656c 737a 096f 7574  raph_labelsz.out
-00001730: 2f74 7275 652f 7a09 6f75 742f 7072 6564  /true/z.out/pred
-00001740: 2f7a 086e 692f 7072 6564 2f7a 0865 692f  /z.ni/pred/z.ei/
-00001750: 7072 6564 2f67 0000 0000 0000 e03f fa0e  pred/g.......?..
-00001760: 6e6f 6465 5f73 7061 7273 6974 792f fa0e  node_sparsity/..
-00001770: 6564 6765 5f73 7061 7273 6974 792f fa09  edge_sparsity/..
-00001780: 6e6f 6465 5f61 7563 2ffa 0965 6467 655f  node_auc/..edge_
-00001790: 6175 632f 7a08 203d 206d 7365 3a20 7a03  auc/z. = mse: z.
-000017a0: 2e32 667a 0920 2d20 726d 7365 3a20 7a08  .2fz. - rmse: z.
-000017b0: 202d 206d 6165 3a20 7a07 202d 2072 323a   - mae: z. - r2:
-000017c0: 207a 1220 2d20 6d65 616e 2066 6964 656c   z. - mean fidel
-000017d0: 6974 793a 207a 1720 2d20 6d65 616e 206e  ity: z. - mean n
-000017e0: 6f64 6520 7370 6172 7369 7479 3a20 7a17  ode sparsity: z.
-000017f0: 202d 206d 6561 6e20 6564 6765 2073 7061   - mean edge spa
-00001800: 7273 6974 793a 207a 0d20 2d20 6e6f 6465  rsity: z. - node
-00001810: 2061 7563 3a20 7a0d 202d 2065 6467 6520   auc: z. - edge 
-00001820: 6175 633a 207a 2164 7261 7769 6e67 2065  auc: z!drawing e
-00001830: 7861 6d70 6c65 2076 6973 7561 6c69 7a61  xample visualiza
-00001840: 7469 6f6e 732e 2e2e da09 6578 616d 706c  tions.....exampl
-00001850: 6573 5fda 0330 3264 7a04 2e70 6466 6301  es_..02dz..pdfc.
-00001860: 0000 0000 0000 0000 0000 0002 0000 0004  ................
-00001870: 0000 0043 0000 00f3 1c00 0000 6700 7c00  ...C........g.|.
-00001880: 5d0a 7d01 7400 7c01 1900 6400 1900 6401  ].}.t.|...d...d.
-00001890: 1900 9102 7102 5300 2902 7238 0000 0072  ....q.S.).r8...r
-000018a0: 3900 0000 a901 da0e 696e 6465 785f 6461  9.......index_da
-000018b0: 7461 5f6d 6170 7244 0000 0072 2800 0000  ta_maprD...r(...
-000018c0: 7228 0000 0072 2900 0000 7247 0000 004e  r(...r)...rG...N
-000018d0: 0100 00f3 0200 0000 1c00 6301 0000 0000  ..........c.....
-000018e0: 0000 0000 0000 0002 0000 0004 0000 0043  ...............C
-000018f0: 0000 0073 1800 0000 6700 7c00 5d08 7d01  ...s....g.|.].}.
-00001900: 7400 7c01 1900 6400 1900 9102 7102 5300  t.|...d.....q.S.
-00001910: 2901 da0a 696d 6167 655f 7061 7468 727c  )...image_pathr|
-00001920: 0000 0072 4400 0000 7228 0000 0072 2800  ...rD...r(...r(.
-00001930: 0000 7229 0000 0072 4700 0000 4f01 0000  ..r)...rG...O...
-00001940: 7302 0000 0018 0063 0100 0000 0000 0000  s......c........
-00001950: 0000 0000 0200 0000 0400 0000 4300 0000  ............C...
-00001960: 7314 0000 0067 007c 005d 067d 017c 0164  s....g.|.].}.|.d
-00001970: 0019 0091 0271 0253 0029 01da 0e6e 6f64  .....q.S.)...nod
-00001980: 655f 706f 7369 7469 6f6e 7372 2800 0000  e_positionsr(...
-00001990: 2902 7245 0000 0072 4200 0000 7228 0000  ).rE...rB...r(..
-000019a0: 0072 2800 0000 7229 0000 0072 4700 0000  .r(...r)...rG...
-000019b0: 5001 0000 7302 0000 0014 0063 0100 0000  P...s......c....
-000019c0: 0000 0000 0000 0000 0200 0000 0400 0000  ................
-000019d0: 4300 0000 727b 0000 0029 0272 3800 0000  C...r{...).r8...
-000019e0: da04 6e61 6d65 727c 0000 0072 4400 0000  ..namer|...rD...
-000019f0: 7228 0000 0072 2800 0000 7229 0000 0072  r(...r(...r)...r
-00001a00: 4700 0000 5a01 0000 727e 0000 0029 07da  G...Z...r~...)..
-00001a10: 0a67 7261 7068 5f6c 6973 74da 0f69 6d61  .graph_list..ima
-00001a20: 6765 5f70 6174 685f 6c69 7374 da13 6e6f  ge_path_list..no
-00001a30: 6465 5f70 6f73 6974 696f 6e73 5f6c 6973  de_positions_lis
-00001a40: 74da 0f69 6d70 6f72 7461 6e63 6573 5f6d  t..importances_m
-00001a50: 6170 da0b 6f75 7470 7574 5f70 6174 68da  ap..output_path.
-00001a60: 1969 6d70 6f72 7461 6e63 655f 6368 616e  .importance_chan
-00001a70: 6e65 6c5f 6c61 6265 6c73 da0b 6c61 6265  nel_labels..labe
-00001a80: 6c73 5f6c 6973 747a 1872 656e 6465 7269  ls_listz.renderi
-00001a90: 6e67 206c 6174 6578 2074 6162 6c65 2e2e  ng latex table..
-00001aa0: 2e29 0a7a 0b54 6172 6765 7420 4e61 6d65  .).z.Target Name
-00001ab0: 7a18 245c 7465 7874 7b4d 5345 7d20 5c64  z.$\text{MSE} \d
-00001ac0: 6f77 6e61 7272 6f77 2024 7a19 245c 7465  ownarrow $z.$\te
-00001ad0: 7874 7b52 4d53 457d 205c 646f 776e 6172  xt{RMSE} \downar
-00001ae0: 726f 7720 247a 1824 5c74 6578 747b 4d41  row $z.$\text{MA
-00001af0: 457d 205c 646f 776e 6172 726f 7720 247a  E} \downarrow $z
-00001b00: 0f24 525e 3220 5c75 7061 7272 6f77 2024  .$R^2 \uparrow $
-00001b10: 7a1a 245c 7465 7874 7b46 6964 656c 6974  z.$\text{Fidelit
-00001b20: 797d 205c 7570 6172 726f 7724 7a21 245c  y} \uparrow$z!$\
-00001b30: 7465 7874 7b4e 6f64 6520 5370 6172 7369  text{Node Sparsi
-00001b40: 7479 7d20 5c64 6f77 6e61 7272 6f77 247a  ty} \downarrow$z
-00001b50: 2124 5c74 6578 747b 4564 6765 2053 7061  !$\text{Edge Spa
-00001b60: 7273 6974 797d 205c 646f 776e 6172 726f  rsity} \downarro
-00001b70: 7724 7a1a 245c 7465 7874 7b4e 6f64 6520  w$z.$\text{Node 
-00001b80: 4155 437d 205c 7570 6172 726f 7724 7a1a  AUC} \uparrow$z.
-00001b90: 245c 7465 7874 7b45 6467 6520 4155 437d  $\text{Edge AUC}
-00001ba0: 205c 7570 6172 726f 7724 fa01 2d63 0100   \uparrow$..-c..
-00001bb0: 0000 0000 0000 0000 0000 0200 0000 0500  ................
-00001bc0: 0000 4300 0000 f31a 0000 0067 007c 005d  ..C........g.|.]
-00001bd0: 097d 0174 0064 007c 019b 009d 0219 0091  .}.t.d.|........
-00001be0: 0271 0253 0029 0172 6800 0000 a901 da01  .q.S.).rh.......
-00001bf0: 65a9 0272 4500 0000 7256 0000 0072 2800  e..rE...rV...r(.
-00001c00: 0000 7228 0000 0072 2900 0000 7247 0000  ..r(...r)...rG..
-00001c10: 0074 0100 00f3 0200 0000 1a00 6301 0000  .t..........c...
-00001c20: 0000 0000 0000 0000 0002 0000 0005 0000  ................
-00001c30: 0043 0000 0072 8a00 0000 2901 7269 0000  .C...r....).ri..
-00001c40: 0072 8b00 0000 728d 0000 0072 2800 0000  .r....r....r(...
-00001c50: 7228 0000 0072 2900 0000 7247 0000 0075  r(...r)...rG...u
-00001c60: 0100 0072 8e00 0000 6301 0000 0000 0000  ...r....c.......
-00001c70: 0000 0000 0002 0000 0005 0000 0043 0000  .............C..
-00001c80: 0072 8a00 0000 2901 726a 0000 0072 8b00  .r....).rj...r..
-00001c90: 0000 728d 0000 0072 2800 0000 7228 0000  ..r....r(...r(..
-00001ca0: 0072 2900 0000 7247 0000 0076 0100 0072  .r)...rG...v...r
-00001cb0: 8e00 0000 6301 0000 0000 0000 0000 0000  ....c...........
-00001cc0: 0002 0000 0005 0000 0043 0000 0072 8a00  .........C...r..
-00001cd0: 0000 2901 726b 0000 0072 8b00 0000 728d  ..).rk...r....r.
-00001ce0: 0000 0072 2800 0000 7228 0000 0072 2900  ...r(...r(...r).
-00001cf0: 0000 7247 0000 0077 0100 0072 8e00 0000  ..rG...w...r....
-00001d00: 6301 0000 0000 0000 0000 0000 0003 0000  c...............
-00001d10: 0008 0000 0043 0000 00f3 3400 0000 6700  .....C....4...g.
-00001d20: 7c00 5d16 7d01 7400 6400 7c01 9b00 9d02  |.].}.t.d.|.....
-00001d30: 1900 4400 5d0c 7d02 7400 6401 7c01 9b00  ..D.].}.t.d.|...
-00001d40: 6402 7c02 9b00 9d04 1900 9103 710b 7102  d.|.........q.q.
-00001d50: 5300 2903 725e 0000 0072 7300 0000 7254  S.).r^...rs...rT
-00001d60: 0000 0072 8b00 0000 a903 7245 0000 0072  ...r......rE...r
-00001d70: 5600 0000 725a 0000 0072 2800 0000 7228  V...rZ...r(...r(
-00001d80: 0000 0072 2900 0000 7247 0000 0078 0100  ...r)...rG...x..
-00001d90: 00f3 0c00 0000 0600 0201 0c01 04fe 0202  ................
-00001da0: 1afe 6301 0000 0000 0000 0000 0000 0003  ..c.............
-00001db0: 0000 0008 0000 0043 0000 0072 8f00 0000  .......C...r....
-00001dc0: 2903 725e 0000 0072 7500 0000 7254 0000  ).r^...ru...rT..
-00001dd0: 0072 8b00 0000 7290 0000 0072 2800 0000  .r....r....r(...
-00001de0: 7228 0000 0072 2900 0000 7247 0000 007b  r(...r)...rG...{
-00001df0: 0100 0072 9100 0000 6301 0000 0000 0000  ...r....c.......
-00001e00: 0000 0000 0003 0000 0008 0000 0043 0000  .............C..
-00001e10: 0072 8f00 0000 2903 725e 0000 0072 7600  .r....).r^...rv.
-00001e20: 0000 7254 0000 0072 8b00 0000 7290 0000  ..rT...r....r...
-00001e30: 0072 2800 0000 7228 0000 0072 2900 0000  .r(...r(...r)...
-00001e40: 7247 0000 007e 0100 0072 9100 0000 6301  rG...~...r....c.
-00001e50: 0000 0000 0000 0000 0000 0002 0000 0005  ................
-00001e60: 0000 0043 0000 0072 8a00 0000 2901 7277  ...C...r....).rw
-00001e70: 0000 0072 8b00 0000 728d 0000 0072 2800  ...r....r....r(.
-00001e80: 0000 7228 0000 0072 2900 0000 7247 0000  ..r(...r)...rG..
-00001e90: 0081 0100 0072 8e00 0000 6301 0000 0000  .....r....c.....
-00001ea0: 0000 0000 0000 0002 0000 0005 0000 0043  ...............C
-00001eb0: 0000 0072 8a00 0000 2901 7278 0000 0072  ...r....).rx...r
-00001ec0: 8b00 0000 728d 0000 0072 2800 0000 7228  ....r....r(...r(
-00001ed0: 0000 0072 2900 0000 7247 0000 0082 0100  ...r)...rG......
-00001ee0: 0072 8e00 0000 7a0b 5265 7375 6c74 7320  .r....z.Results 
-00001ef0: 6f66 207a 1220 7265 7065 7469 7469 6f6e  of z. repetition
-00001f00: 2873 2920 6f66 207a 085c 7465 7874 6266  (s) of z.\textbf
-00001f10: 7bda 017d 2904 da0c 636f 6c75 6d6e 5f6e  {..})...column_n
-00001f20: 616d 6573 da04 726f 7773 da0f 6c69 7374  ames..rows..list
-00001f30: 5f65 6c65 6d65 6e74 5f63 62da 0763 6170  _element_cb..cap
-00001f40: 7469 6f6e 7a09 7461 626c 652e 7465 787a  tionz.table.texz
-00001f50: 0974 6162 6c65 2e70 6466 da07 636f 6e74  .table.pdf..cont
-00001f60: 656e 7429 0172 8600 0000 7a14 7265 6e64  ent).r....z.rend
-00001f70: 6572 6564 206c 6174 6578 2074 6162 6c65  ered latex table
-00001f80: 29af da02 6f73 da03 7379 73da 0770 6174  )...os..sys..pat
-00001f90: 686c 6962 da06 7261 6e64 6f6d da06 7479  hlib..random..ty
-00001fa0: 7069 6e67 da01 74da 0b63 6f6c 6c65 6374  ping..t..collect
-00001fb0: 696f 6e73 7202 0000 00da 0a74 656e 736f  ionsr......tenso
-00001fc0: 7266 6c6f 77da 0274 66da 1074 656e 736f  rflow..tf..tenso
-00001fd0: 7266 6c6f 772e 6b65 7261 73da 056b 6572  rflow.keras..ker
-00001fe0: 6173 7225 0000 00da 056e 756d 7079 da02  asr%.....numpy..
-00001ff0: 6e70 da11 6d61 7470 6c6f 746c 6962 2e70  np..matplotlib.p
-00002000: 7970 6c6f 74da 0670 7970 6c6f 74da 0370  yplot..pyplot..p
-00002010: 6c74 da0f 736b 6c65 6172 6e2e 6d65 7472  lt..sklearn.metr
-00002020: 6963 7372 0300 0000 7204 0000 0072 0500  icsr....r....r..
-00002030: 0000 7206 0000 00da 0c70 7963 6f6d 6578  ..r......pycomex
-00002040: 2e75 7469 6c72 0700 0000 da12 7079 636f  .utilr......pyco
-00002050: 6d65 782e 6578 7065 7269 6d65 6e74 7208  mex.experimentr.
-00002060: 0000 00da 1a76 6973 7561 6c5f 6772 6170  .....visual_grap
-00002070: 685f 6461 7461 7365 7473 2e64 6174 6172  h_datasets.datar
-00002080: 0900 0000 da2f 7669 7375 616c 5f67 7261  ...../visual_gra
-00002090: 7068 5f64 6174 6173 6574 732e 7669 7375  ph_datasets.visu
-000020a0: 616c 697a 6174 696f 6e2e 696d 706f 7274  alization.import
-000020b0: 616e 6365 7372 0a00 0000 da10 6b67 636e  ancesr......kgcn
-000020c0: 6e2e 6461 7461 2e75 7469 6c73 720b 0000  n.data.utilsr...
-000020d0: 00da 1e67 7261 7068 5f61 7474 656e 7469  ...graph_attenti
-000020e0: 6f6e 5f73 7475 6465 6e74 2e74 7970 696e  on_student.typin
-000020f0: 67da 0274 63da 1c67 7261 7068 5f61 7474  g..tc..graph_att
-00002100: 656e 7469 6f6e 5f73 7475 6465 6e74 2e64  ention_student.d
-00002110: 6174 6172 0d00 0000 da1c 6772 6170 685f  atar......graph_
-00002120: 6174 7465 6e74 696f 6e5f 7374 7564 656e  attention_studen
-00002130: 742e 7574 696c 720e 0000 0072 0f00 0000  t.utilr....r....
-00002140: 7210 0000 0072 1100 0000 7212 0000 00da  r....r....r.....
-00002150: 0470 6174 68da 0a65 7870 616e 6475 7365  .path..expanduse
-00002160: 7272 1300 0000 da03 7374 72da 0f5f 5f61  rr......str..__a
-00002170: 6e6e 6f74 6174 696f 6e73 5f5f 7214 0000  nnotations__r...
-00002180: 00da 084f 7074 696f 6e61 6cda 0369 6e74  ...Optional..int
-00002190: 7215 0000 00da 0566 6c6f 6174 7217 0000  r......floatr...
-000021a0: 0072 1800 0000 da04 4c69 7374 da13 494d  .r......List..IM
-000021b0: 504f 5254 414e 4345 5f43 4841 4e4e 454c  PORTANCE_CHANNEL
-000021c0: 5372 1b00 0000 721d 0000 0072 1e00 0000  Sr....r....r....
-000021d0: da04 626f 6f6c 721f 0000 0072 2000 0000  ..boolr....r ...
-000021e0: 7222 0000 0072 2300 0000 da0c 4f50 5449  r"...r#.....OPTI
-000021f0: 4d49 5a45 525f 4342 722c 0000 0072 2e00  MIZER_CBr,...r..
-00002200: 0000 722f 0000 0072 3000 0000 7231 0000  ..r/...r0...r1..
-00002210: 00da 1949 4d50 4f52 5441 4e43 455f 4348  ...IMPORTANCE_CH
-00002220: 414e 4e45 4c5f 4c41 4245 4c53 da06 6765  ANNEL_LABELS..ge
-00002230: 7463 7764 da09 4241 5345 5f50 4154 48da  tcwd..BASE_PATH.
-00002240: 094e 414d 4553 5041 4345 da05 4445 4255  .NAMESPACE..DEBU
-00002250: 47da 0767 6c6f 6261 6c73 728c 0000 00da  G..globalsr.....
-00002260: 0862 6173 656e 616d 65da 0876 6764 5f6e  .basename..vgd_n
-00002270: 616d 65da 0469 6e66 6f72 3400 0000 da0c  ame..infor4.....
-00002280: 6d65 7461 6461 7461 5f6d 6170 727d 0000  metadata_mapr}..
-00002290: 00da 046c 6973 74da 0673 6f72 7465 64da  ...list..sorted.
-000022a0: 046b 6579 73da 0f64 6174 6173 6574 5f69  .keys..dataset_i
-000022b0: 6e64 6963 6573 da03 7365 74da 1364 6174  ndices..set..dat
-000022c0: 6173 6574 5f69 6e64 6963 6573 5f73 6574  aset_indices_set
-000022d0: da03 6c65 6eda 0e64 6174 6173 6574 5f6c  ..len..dataset_l
-000022e0: 656e 6774 6872 3700 0000 da09 4772 6170  engthr7.....Grap
-000022f0: 6844 6963 7472 5a00 0000 725b 0000 0072  hDictrZ...r[...r
-00002300: 4200 0000 da05 7a65 726f 73da 0561 7272  B.....zeros..arr
-00002310: 6179 da09 656e 756d 6572 6174 65da 046f  ay..enumerate..o
-00002320: 6e65 73da 0661 7070 656e 64da 0468 6f6f  nes..append..hoo
-00002330: 6b72 4b00 0000 da05 7261 6e67 6572 5600  krK.....rangerV.
-00002340: 0000 da06 6465 7669 6365 da05 6974 656d  ....device..item
-00002350: 7372 4d00 0000 724e 0000 00da 0673 616d  srM...rN.....sam
-00002360: 706c 65da 1174 7261 696e 5f69 6e64 6963  ple..train_indic
-00002370: 6573 5f73 6574 da0a 6469 6666 6572 656e  es_set..differen
-00002380: 6365 da10 7465 7374 5f69 6e64 6963 6573  ce..test_indices
-00002390: 5f73 6574 da03 6d69 6eda 0c6e 756d 5f65  _set..min..num_e
-000023a0: 7861 6d70 6c65 73da 0f65 7861 6d70 6c65  xamples..example
-000023b0: 5f69 6e64 6963 6573 da0a 6170 706c 795f  _indices..apply_
-000023c0: 686f 6f6b 7250 0000 0072 5100 0000 7252  hookrP...rQ...rR
-000023d0: 0000 0072 5300 0000 7260 0000 00da 066d  ...rS...r`.....m
-000023e0: 6f64 656c 73da 054d 6f64 656c 7262 0000  odels..Modelrb..
-000023f0: 00da 0464 6963 7472 7000 0000 7271 0000  ...dictrp...rq..
-00002400: 0072 7200 0000 da08 6f75 745f 7472 7565  .rr.....out_true
-00002410: da07 6e69 5f74 7275 65da 0765 695f 7472  ..ni_true..ei_tr
-00002420: 7565 da09 6d73 655f 7661 6c75 65da 0473  ue..mse_value..s
-00002430: 7172 74da 0a72 6d73 655f 7661 6c75 65da  qrt..rmse_value.
-00002440: 096d 6165 5f76 616c 7565 da08 7232 5f76  .mae_value..r2_v
-00002450: 616c 7565 da0a 6669 6465 6c69 7469 6573  alue..fidelities
-00002460: da03 7a69 70da 0866 6964 656c 6974 79da  ..zip..fidelity.
-00002470: 1570 7265 645f 6e6f 6465 5f69 6d70 6f72  .pred_node_impor
-00002480: 7461 6e63 6573 da15 7072 6564 5f65 6467  tances..pred_edg
-00002490: 655f 696d 706f 7274 616e 6365 73da 1574  e_importances..t
-000024a0: 7275 655f 6e6f 6465 5f69 6d70 6f72 7461  rue_node_importa
-000024b0: 6e63 6573 da15 7472 7565 5f65 6467 655f  nces..true_edge_
-000024c0: 696d 706f 7274 616e 6365 73da 0163 da02  importances..c..
-000024d0: 6e69 da02 6569 da07 666c 6174 7465 6e72  ni..ei..flattenr
-000024e0: 4300 0000 da04 6d65 616e da0d 6e6f 6465  C.....mean..node
-000024f0: 5f73 7061 7273 6974 79da 0d65 6467 655f  _sparsity..edge_
-00002500: 7370 6172 7369 7479 da06 7661 6c75 6573  sparsity..values
-00002510: da0d 6d65 616e 5f66 6964 656c 6974 79da  ..mean_fidelity.
-00002520: 126d 6561 6e5f 6e6f 6465 5f73 7061 7273  .mean_node_spars
-00002530: 6974 79da 126d 6561 6e5f 6564 6765 5f73  ity..mean_edge_s
-00002540: 7061 7273 6974 79da 086e 6f64 655f 6175  parsity..node_au
-00002550: 63da 0865 6467 655f 6175 63da 0a56 616c  c..edge_auc..Val
-00002560: 7565 4572 726f 72da 0f6e 695f 6578 616d  ueError..ni_exam
-00002570: 706c 655f 7072 6564 da0f 6569 5f65 7861  ple_pred..ei_exa
-00002580: 6d70 6c65 5f70 7265 64da 046a 6f69 6eda  mple_pred..join.
-00002590: 0870 6466 5f70 6174 6872 8200 0000 7283  .pdf_pathr....r.
-000025a0: 0000 0072 8400 0000 da06 7374 6174 7573  ...r......status
-000025b0: da08 616e 616c 7973 6973 7293 0000 0072  ..analysisr....r
-000025c0: 9400 0000 da03 726f 7772 9700 0000 da05  ......rowr......
-000025d0: 7461 626c 65da 0a63 6f6d 6d69 745f 7261  table..commit_ra
-000025e0: 7772 2800 0000 7228 0000 0072 2800 0000  wr(...r(...r(...
-000025f0: 7229 0000 00da 083c 6d6f 6475 6c65 3e01  r).....<module>.
-00002600: 0000 0073 2202 0000 0a00 0801 0801 0801  ...s"...........
-00002610: 0801 0c01 0802 0c01 0801 0c01 0c01 0c01  ................
-00002620: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c02  ................
-00002630: 0c01 1001 1001 0c01 1407 1205 0c03 0c04  ................
-00002640: 1203 0402 1204 1202 0c03 0c04 0c03 0c05  ................
-00002650: 0c07 0802 0c01 0c01 0c01 0c06 0c02 0604  ................
-00002660: 0803 0401 0401 2001 0c02 1201 0204 0201  ...... .........
-00002670: 0401 0201 0201 0afc 1008 0801 0801 1404  ................
-00002680: 0801 0801 0c01 0a02 0e01 1c02 0a02 0e01  ................
-00002690: 1c02 0602 0a01 0601 0cff 0603 0a01 0a01  ................
-000026a0: 0cff 0603 1c01 0e02 1602 0c04 0a01 0e09  ................
-000026b0: 1c01 0801 0e02 0a02 0a01 1201 1402 0a04  ................
-000026c0: 1601 0801 0a01 0801 1002 0801 2001 0e01  ............ ...
-000026d0: 0e01 1602 1601 1601 0e01 0a02 0401 0201  ................
-000026e0: 0201 0201 0201 0efc 0a07 1601 0a02 0401  ................
-000026f0: 0201 0201 0201 0201 0201 0201 0efa 0e08  ................
-00002700: 1601 0a03 0401 0201 0201 0201 0201 0201  ................
-00002710: 0cfb 0e07 0e01 0e01 0e02 1201 1201 0a03  ................
-00002720: 0a01 0a01 0a01 0a01 0e01 0e01 0e01 0e01  ................
-00002730: 0a02 0401 0201 0201 0201 0201 0201 0201  ................
-00002740: 0201 0201 06f8 120a 1801 0a03 0402 0401  ................
-00002750: 0402 0401 1002 1001 0c01 0c01 2002 2001  ............ . .
-00002760: 1402 1401 1402 1401 1402 1401 1403 1401  ................
-00002770: 1401 1801 1c02 1c01 1c01 0206 0a01 0e01  ................
-00002780: 0e01 0401 0801 02fe 0e04 0e01 0e02 0401  ................
-00002790: 04ff 0402 04fe 0403 04fd 0404 04fc 0405  ................
-000027a0: 04fb 0406 04fa 0407 04f9 0408 08f8 0a0d  ................
-000027b0: 0402 0401 0801 1a01 1e01 1a04 0e01 0e01  ................
-000027c0: 0e01 0201 0201 0201 0201 0802 02ff 0203  ................
-000027d0: 0201 0c01 06f7 0a0c 0081 1eca 0480 02fc  ................
-000027e0: 1ec1 0280 1e00 007f 107c 0a02 0801 040c  .........|......
-000027f0: 0402 0a02 1801 1801 1801 1801 0a01 0601  ................
-00002800: 08ff 0a03 0601 08ff 0a03 0601 08ff 1803  ................
-00002810: 1801 0a02 0202 0201 0201 0201 1601 0afc  ................
-00002820: 0c06 1001 1001 0c01 54d1                 ........T.
+00000020: 0019 0000 0040 0000 0073 4c0c 0000 5500  .....@...sL...U.
+00000030: 6400 5a00 6401 6402 6c01 5a01 6401 6402  d.Z.d.d.l.Z.d.d.
+00000040: 6c02 5a02 6401 6402 6c03 5a03 6401 6402  l.Z.d.d.l.Z.d.d.
+00000050: 6c04 5a04 6401 6402 6c05 5a06 6401 6403  l.Z.d.d.l.Z.d.d.
+00000060: 6c07 6d08 5a08 0100 6401 6402 6c09 5a0a  l.m.Z...d.d.l.Z.
+00000070: 6401 6402 6c0b 6d0c 5a0d 0100 6401 6402  d.d.l.m.Z...d.d.
+00000080: 6c0e 5a0f 6401 6402 6c10 6d11 5a12 0100  l.Z.d.d.l.m.Z...
+00000090: 6401 6404 6c13 6d14 5a14 0100 6401 6405  d.d.l.m.Z...d.d.
+000000a0: 6c13 6d15 5a15 0100 6401 6406 6c13 6d16  l.m.Z...d.d.l.m.
+000000b0: 5a16 0100 6401 6407 6c13 6d17 5a17 0100  Z...d.d.l.m.Z...
+000000c0: 6401 6408 6c18 6d19 5a19 0100 6401 6409  d.d.l.m.Z...d.d.
+000000d0: 6c1a 6d1b 5a1b 0100 6401 640a 6c1c 6d1d  l.m.Z...d.d.l.m.
+000000e0: 5a1d 0100 6401 640b 6c1e 6d1f 5a1f 0100  Z...d.d.l.m.Z...
+000000f0: 6401 640c 6c20 6d21 5a21 0100 6401 6402  d.d.l m!Z!..d.d.
+00000100: 6c22 6d05 5a23 0100 6401 640d 6c24 6d25  l"m.Z#..d.d.l$m%
+00000110: 5a25 0100 6401 640e 6c26 6d27 5a27 6d28  Z%..d.d.l&m'Z'm(
+00000120: 5a28 0100 6401 640f 6c26 6d29 5a29 6d2a  Z(..d.d.l&m)Z)m*
+00000130: 5a2a 0100 6401 6410 6c26 6d2b 5a2b 0100  Z*..d.d.l&m+Z+..
+00000140: 6501 6a2c a02d 6411 a101 5a2e 652f 6530  e.j,.-d...Z.e/e0
+00000150: 6412 3c00 6402 5a31 6506 6a32 6533 1900  d.<.d.Z1e.j2e3..
+00000160: 6530 6413 3c00 6414 5a34 6535 6530 6415  e0d.<.d.Z4e5e0d.
+00000170: 3c00 6416 5a36 6533 6530 6417 3c00 6700  <.d.Z6e3e0d.<.g.
+00000180: 5a37 6506 6a38 6533 1900 6530 6418 3c00  Z7e.j8e3..e0d.<.
+00000190: 6419 5a39 641a 5a3a 6506 6a32 652f 1900  d.Z9d.Z:e.j2e/..
+000001a0: 6530 641b 3c00 641c 5a3b 6506 6a32 652f  e0d.<.d.Z;e.j2e/
+000001b0: 1900 6530 641d 3c00 641e 5a3c 653d 6530  ..e0d.<.d.Z<e=e0
+000001c0: 641f 3c00 6420 5a3e 653d 6530 6421 3c00  d.<.d Z>e=e0d!<.
+000001d0: 641e 5a3f 653d 6530 6422 3c00 6423 5a40  d.Z?e=e0d"<.d#Z@
+000001e0: 652f 6530 6424 3c00 6419 5a41 6533 6530  e/e0d$<.d.ZAe3e0
+000001f0: 6425 3c00 6426 6427 8400 5a42 6428 5a43  d%<.d&d'..ZBd(ZC
+00000200: 6533 6530 6429 3c00 642a 5a44 6533 6530  e3e0d)<.d*ZDe3e0
+00000210: 642b 3c00 642c 5a45 652f 6530 642d 3c00  d+<.d,ZEe/e0d-<.
+00000220: 6416 5a46 6533 6530 642e 3c00 6428 5a47  d.ZFe3e0d.<.d(ZG
+00000230: 6533 6530 642f 3c00 6430 6701 5a48 6501  e3e0d/<.d0g.ZHe.
+00000240: a049 a100 5a4a 6431 5a4b 6420 5a4c 6519  .I..ZJd1ZKd ZLe.
+00000250: 8300 9004 8f24 0100 651b 654a 654b 654d  .....$..e.eJeKeM
+00000260: 8300 8303 0400 5a4e 9004 8f09 0100 6501  ......ZN......e.
+00000270: 6a2c a04f 652e a101 5a50 654e a051 6432  j,.Oe...ZPeN.Qd2
+00000280: 6550 9b00 6433 9d03 a101 0100 651d 652e  eP..d3......e.e.
+00000290: 654e 6a52 6546 6420 6434 8d04 5c02 5a53  eNjReFd d4..\.ZS
+000002a0: 5a54 6555 6556 6554 a057 a100 8301 8301  ZTeUeVeT.W......
+000002b0: 5a58 6559 6558 8301 5a5a 655b 6554 8301  ZXeYeX..ZZe[eT..
+000002c0: 5a5c 6700 5a5d 6506 6a38 6523 6a5e 1900  Z\g.Z]e.j8e#j^..
+000002d0: 6530 6435 3c00 6558 4400 5d7b 5a5f 6554  e0d5<.eXD.]{Z_eT
+000002e0: 655f 1900 5a60 6560 6436 1900 6437 1900  e_..Z`e`d6..d7..
+000002f0: 5a61 653a 6402 7501 9001 726e 6561 653a  Zae:d.u...rneae:
+00000300: 1900 6561 6438 3c00 6e0e 650f 6a62 655b  ..ead8<.n.e.jbe[
+00000310: 6561 6439 1900 8301 6539 6602 643a 8d01  ead9....e9f.d:..
+00000320: 6561 6438 3c00 653b 6402 7501 9001 7288  ead8<.e;d.u...r.
+00000330: 6561 653b 1900 6561 643b 3c00 6e0e 650f  eae;..ead;<.n.e.
+00000340: 6a62 655b 6561 643c 1900 8301 6539 6602  jbe[ead<....e9f.
+00000350: 643a 8d01 6561 643b 3c00 653c 9001 72a7  d:..ead;<.e<..r.
+00000360: 650f a063 643d 643e 8400 6561 6439 1900  e..cd=d>..ead9..
+00000370: 4400 8301 a101 6561 643f 3c00 653f 9001  D.....ead?<.e?..
+00000380: 72ba 650f a063 6440 643e 8400 6564 6561  r.e..cd@d>..edea
+00000390: 643c 1900 8301 4400 8301 a101 6561 6441  d<....D.....eadA
+000003a0: 3c00 653e 9001 73cb 650f 6a65 655b 6561  <.e>..s.e.jee[ea
+000003b0: 643c 1900 8301 6419 6602 643a 8d01 6561  d<....d.f.d:..ea
+000003c0: 6441 3c00 655d a066 6561 a101 0100 9001  dA<.e].fea......
+000003d0: 7156 654e a051 6442 655b 655d 8301 9b00  qVeN.QdBe[e]....
+000003e0: 6443 9d03 a101 0100 654e 6a67 6444 6420  dC......eNjgdDd 
+000003f0: 6445 8d02 6446 6444 8400 8301 5a68 6569  dE..dFdD....Zhei
+00000400: 6541 8301 4400 9003 5d33 5a6a 654e a051  eA..D...]3ZjeN.Q
+00000410: 6447 656a 6419 1700 9b00 6448 6541 9b00  dGejd.....dHeA..
+00000420: 6449 9d05 a101 0100 656a 654e 644a 3c00  dI......ejeNdJ<.
+00000430: 650a a06b 6545 a101 9003 8f0f 0100 6531  e..keE........e1
+00000440: 6402 7501 9002 7225 654e a051 644b a101  d.u...r%eN.QdK..
+00000450: 0100 644c 643e 8400 6554 a06c a100 4400  ..dLd>..eT.l..D.
+00000460: 8301 5a6d 644d 643e 8400 6554 a06c a100  ..ZmdMd>..eT.l..
+00000470: 4400 8301 5a6e 6e1d 654e a051 644e a101  D...Znn.eN.QdN..
+00000480: 0100 6504 6a6f 6558 6533 6534 655c 1400  ..e.joeXe3e4e\..
+00000490: 8301 644f 8d02 5a6d 6559 656d 8301 5a70  ..dO..ZmeYem..Zp
+000004a0: 655a a071 6570 a101 5a72 6555 6572 8301  eZ.qep..ZreUer..
+000004b0: 5a6e 6559 656e 8301 6559 6537 8301 4200  ZneYen..eYe7..B.
+000004c0: 5a72 6555 6572 8301 5a6e 654e a051 6450  ZreUer..ZneN.QdP
+000004d0: 655b 656d 8301 9b00 6451 655b 656e 8301  e[em....dQe[en..
+000004e0: 9b00 6452 9d05 a101 0100 656d 654e 6453  ..dR......emeNdS
+000004f0: 656a 9b00 9d02 3c00 656e 654e 6454 656a  ej....<.eneNdTej
+00000500: 9b00 9d02 3c00 6573 6536 655b 656e 8301  ....<.ese6e[en..
+00000510: 8302 655b 6537 8301 1800 5a74 6537 6555  ..e[e7....Zte7eU
+00000520: 6504 6a6f 656e 6574 644f 8d02 8301 1700  e.joenetdO......
+00000530: 5a75 654e a051 6450 655b 6575 8301 9b00  ZueN.QdPe[eu....
+00000540: 6455 9d03 a101 0100 6575 654e 6456 656a  dU......eueNdVej
+00000550: 9b00 9d02 3c00 654e a051 6457 a101 0100  ....<.eN.QdW....
+00000560: 654e 6a76 6444 655d 656d 656e 6458 8d04  eNjvdDe]emendX..
+00000570: 5c04 5a77 5a78 5a79 5a7a 654e a051 6459  \.ZwZxZyZzeN.QdY
+00000580: a101 0100 654e a076 645a a101 5a7b 650d  ....eN.vdZ..Z{e.
+00000590: 6a7c 6a7d 6530 645b 3c00 654e a051 645c  j|j}e0d[<.eN.Qd\
+000005a0: a101 0100 654e 6a76 645d 657b 6577 6578  ....eNjvd]e{ewex
+000005b0: 6579 657a 645e 8d06 5a7e 657f 6530 645f  eyezd^..Z~e.e0d_
+000005c0: 3c00 657e 654e 6460 656a 9b00 9d02 3c00  <.e~eNd`ej....<.
+000005d0: 6555 6569 6544 8301 8301 654e 6461 656a  eUeieD....eNdaej
+000005e0: 9b00 9d02 3c00 654e a051 6462 a101 0100  ....<.eN.Qdb....
+000005f0: 654e 6a76 6463 657b 6579 657a 6420 6464  eNjvdce{eyezd dd
+00000600: 8d05 5c03 5a80 5a81 5a82 650f a063 6580  ..\.Z.Z.Z.e..ce.
+00000610: a00e a100 a101 5a80 650f a063 6581 a00e  ......Z.e..ce...
+00000620: a100 a101 5a81 650f a063 6582 a00e a100  ....Z.e..ce.....
+00000630: a101 5a82 650f a063 657a 6401 1900 a101  ..Z.e..cezd.....
+00000640: 5a83 650f a063 657a 6419 1900 a00e a100  Z.e..cezd.......
+00000650: a101 5a84 650f a063 657a 6465 1900 a00e  ..Z.e..cezde....
+00000660: a100 a101 5a85 654e a051 6466 a101 0100  ....Z.eN.Qdf....
+00000670: 6515 6580 6583 8302 5a86 650f a087 6586  e.e.e...Z.e...e.
+00000680: a101 5a88 6516 6580 6583 8302 5a89 6514  ..Z.e.e.e...Z.e.
+00000690: 6580 6583 8302 5a8a 6586 654e 6467 656a  e.e...Z.e.eNdgej
+000006a0: 9b00 9d02 3c00 6588 654e 6468 656a 9b00  ....<.e.eNdhej..
+000006b0: 9d02 3c00 6589 654e 6469 656a 9b00 9d02  ..<.e.eNdiej....
+000006c0: 3c00 658a 654e 646a 656a 9b00 9d02 3c00  <.e.eNdjej....<.
+000006d0: 654e a051 646b a101 0100 654e 6a76 646c  eN.Qdk....eNjvdl
+000006e0: 657b 656e 6579 657a 6580 6581 6582 646d  e{eneyeze.e.e.dm
+000006f0: 8d08 5a8b 658b 9003 727b 658c 656e 658b  ..Z.e...r{e.ene.
+00000700: 8302 4400 5d0f 5c02 5a5f 5a8d 658d 654e  ..D.].\.Z_Z.e.eN
+00000710: 646e 656a 9b00 6448 655f 9b00 9d04 3c00  dnej..dHe_....<.
+00000720: 9003 716b 654e a051 646f a101 0100 6700  ..qkeN.Qdo....g.
+00000730: 5a8e 6700 5a8f 6700 5a90 6700 5a91 6564  Z.g.Z.g.Z.g.Z.ed
+00000740: 656e 8301 4400 5d9d 5c02 5a92 5a5f 6554  en..D.].\.Z.Z_eT
+00000750: 655f 1900 6436 1900 6437 1900 5a61 6527  e_..d6..d7..Zae'
+00000760: 6581 6592 1900 8301 5a93 6527 6582 6592  e.e.....Z.e'e.e.
+00000770: 1900 8301 5a94 6535 6561 6470 1900 6401  ....Z.e5eadp..d.
+00000780: 1900 8301 654e 6471 656a 9b00 6448 655f  ....eNdqej..dHe_
+00000790: 9b00 9d04 3c00 6535 6580 6592 1900 6401  ....<.e5e.e...d.
+000007a0: 1900 8301 654e 6472 656a 9b00 6448 655f  ....eNdrej..dHe_
+000007b0: 9b00 9d04 3c00 6593 654e 6473 656a 9b00  ....<.e.eNdsej..
+000007c0: 6448 655f 9b00 9d04 3c00 6594 654e 6474  dHe_....<.e.eNdt
+000007d0: 656a 9b00 6448 655f 9b00 9d04 3c00 658e  ej..dHe_....<.e.
+000007e0: 6581 6592 1900 a095 a100 a096 a100 3700  e.e...........7.
+000007f0: 5a8e 658f 6582 6592 1900 a095 a100 a096  Z.e.e.e.........
+00000800: a100 3700 5a8f 6590 6584 6592 1900 a095  ..7.Z.e.e.e.....
+00000810: a100 a096 a100 3700 5a90 6591 6585 6592  ......7.Z.e.e.e.
+00000820: 1900 a095 a100 a096 a100 3700 5a91 6535  ..........7.Z.e5
+00000830: 650f a097 6528 6593 6475 8302 a101 8301  e...e(e.du......
+00000840: 5a98 6535 650f a097 6528 6594 6475 8302  Z.e5e...e(e.du..
+00000850: a101 8301 5a99 6598 654e 6476 656a 9b00  ....Z.e.eNdvej..
+00000860: 6448 655f 9b00 9d04 3c00 6599 654e 6477  dHe_....<.e.eNdw
+00000870: 656a 9b00 6448 655f 9b00 9d04 3c00 9003  ej..dHe_....<...
+00000880: 718c 650f a097 6555 654e 646e 656a 9b00  q.e...eUeNdnej..
+00000890: 9d02 1900 a09a a100 8301 a101 5a9b 650f  ............Z.e.
+000008a0: a097 6555 654e 6476 656a 9b00 9d02 1900  ..eUeNdvej......
+000008b0: a09a a100 8301 a101 5a9c 650f a097 6555  ........Z.e...eU
+000008c0: 654e 6477 656a 9b00 9d02 1900 a09a a100  eNdwej..........
+000008d0: 8301 a101 5a9d 7a0c 6517 6590 658e 8302  ....Z.z.e.e.e...
+000008e0: 5a9e 6517 6591 658f 8302 5a9f 5700 6e0e  Z.e.e.e...Z.W.n.
+000008f0: 0400 65a0 9004 796e 0100 0100 0100 6475  ..e...yn......du
+00000900: 5a9e 6475 5a9f 5900 6e01 7700 659e 654e  Z.duZ.Y.n.w.e.eN
+00000910: 6478 656a 9b00 9d02 3c00 659f 654e 6479  dxej....<.e.eNdy
+00000920: 656a 9b00 9d02 3c00 654e a051 647a 6586  ej....<.eN.Qdze.
+00000930: 647b 9b04 647c 6588 647b 9b04 647d 6589  d{..d|e.d{..d}e.
+00000940: 647b 9b04 647e 658a 647b 9b04 647f 659b  d{..d~e.d{..d.e.
+00000950: 647b 9b04 6480 659c 647b 9b04 6481 659d  d{..d.e.d{..d.e.
+00000960: 647b 9b04 6482 659e 647b 9b04 6483 659f  d{..d.e.d{..d.e.
+00000970: 647b 9b04 9d12 a101 0100 654e a051 6484  d{........eN.Qd.
+00000980: a101 0100 6700 5aa1 6700 5aa2 6575 4400  ....g.Z.g.Z.euD.
+00000990: 5d1d 5a5f 65a1 a066 654e 6473 656a 9b00  ].Z_e..feNdsej..
+000009a0: 6448 655f 9b00 9d04 1900 a101 0100 65a2  dHe_..........e.
+000009b0: a066 654e 6474 656a 9b00 6448 655f 9b00  .feNdtej..dHe_..
+000009c0: 9d04 1900 a101 0100 9004 71b1 6501 6a2c  ..........q.e.j,
+000009d0: a0a3 654e 6a2c 6485 656a 6486 9b04 6487  ..eNj,d.ejd...d.
+000009e0: 9d03 a102 5aa4 6488 643e 8400 6575 4400  ....Z.d.d>..euD.
+000009f0: 8301 5aa5 6489 643e 8400 6575 4400 8301  ..Z.d.d>..euD...
+00000a00: 5aa6 648a 643e 8400 65a5 4400 8301 5aa7  Z.d.d>..e.D...Z.
+00000a10: 651f 65a5 65a6 65a7 645b 65a1 65a2 6602  e.e.e.e.d[e.e.f.
+00000a20: 6901 65a4 648b 643e 8400 6575 4400 8301  i.e.d.d>..euD...
+00000a30: 648c 8d06 0100 654e 6a76 648d 657b 648e  d.....eNjvd.e{d.
+00000a40: 8d02 0100 654e a0a8 a100 0100 5700 6402  ....eN......W.d.
+00000a50: 0400 0400 8303 0100 6e09 3100 9005 731a  ........n.1...s.
+00000a60: 7701 0100 0100 0100 5900 0100 9001 71ec  w.......Y.....q.
+00000a70: 5700 6402 0400 0400 8303 0100 6e09 3100  W.d.........n.1.
+00000a80: 9005 732c 7701 0100 0100 0100 5900 0100  ..s,w.......Y...
+00000a90: 5700 6402 0400 0400 8303 0100 6e09 3100  W.d.........n.1.
+00000aa0: 9005 733c 7701 0100 0100 0100 5900 0100  ..s<w.......Y...
+00000ab0: 6519 8300 8fd7 0100 654e 6aa9 8fba 0100  e.......eNj.....
+00000ac0: 654e a051 648f a101 0100 6700 6490 a201  eN.Qd.....g.d...
+00000ad0: 5aaa 6700 5aab 6700 5aac 65ac a066 6491  Z.g.Z.g.Z.e..fd.
+00000ae0: a101 0100 65ac a066 6492 643e 8400 6569  ....e..fd.d>..ei
+00000af0: 6541 8301 4400 8301 a101 0100 65ac a066  eA..D.......e..f
+00000b00: 6493 643e 8400 6569 6541 8301 4400 8301  d.d>..eieA..D...
+00000b10: a101 0100 65ac a066 6494 643e 8400 6569  ....e..fd.d>..ei
+00000b20: 6541 8301 4400 8301 a101 0100 65ac a066  eA..D.......e..f
+00000b30: 6495 643e 8400 6569 6541 8301 4400 8301  d.d>..eieA..D...
+00000b40: a101 0100 65ac a066 6496 643e 8400 6569  ....e..fd.d>..ei
+00000b50: 6541 8301 4400 8301 a101 0100 65ac a066  eA..D.......e..f
+00000b60: 6497 643e 8400 6569 6541 8301 4400 8301  d.d>..eieA..D...
+00000b70: a101 0100 65ac a066 6498 643e 8400 6569  ....e..fd.d>..ei
+00000b80: 6541 8301 4400 8301 a101 0100 65ac a066  eA..D.......e..f
+00000b90: 6499 643e 8400 6569 6541 8301 4400 8301  d.d>..eieA..D...
+00000ba0: a101 0100 65ac a066 649a 643e 8400 6569  ....e..fd.d>..ei
+00000bb0: 6541 8301 4400 8301 a101 0100 65ab a066  eA..D.......e..f
+00000bc0: 65ac a101 0100 6529 65aa 65ab 652a 649b  e.....e)e.e.e*d.
+00000bd0: 6541 9b00 649c 9d03 649d 1700 6540 1700  eA..d...d...e@..
+00000be0: 649e 1700 649f 8d04 5c02 5aad 5aae 654e  d...d...\.Z.Z.eN
+00000bf0: a0af 64a0 65ae a102 0100 6501 6a2c a0a3  ..d.e.....e.j,..
+00000c00: 654e 6a2c 64a1 a102 5aa4 652b 64a2 65ae  eNj,d...Z.e+d.e.
+00000c10: 6901 65a4 64a3 8d02 0100 654e a051 64a4  i.e.d.....eN.Qd.
+00000c20: a101 0100 5700 6402 0400 0400 8303 0100  ....W.d.........
+00000c30: 6e11 3100 9006 7306 7701 0100 0100 0100  n.1...s.w.......
+00000c40: 5900 0100 5700 6402 0400 0400 8303 0100  Y...W.d.........
+00000c50: 6402 5300 5700 6402 0400 0400 8303 0100  d.S.W.d.........
+00000c60: 6402 5300 3100 9006 731f 7701 0100 0100  d.S.1...s.w.....
+00000c70: 0100 5900 0100 6402 5300 29a5 7a02 0a0a  ..Y...d.S.).z...
+00000c80: e900 0000 004e 2901 da07 436f 756e 7465  .....N)...Counte
+00000c90: 7229 01da 0872 325f 7363 6f72 6529 01da  r)...r2_score)..
+00000ca0: 126d 6561 6e5f 7371 7561 7265 645f 6572  .mean_squared_er
+00000cb0: 726f 7229 01da 136d 6561 6e5f 6162 736f  ror)...mean_abso
+00000cc0: 6c75 7465 5f65 7272 6f72 2901 da0d 726f  lute_error)...ro
+00000cd0: 635f 6175 635f 7363 6f72 6529 01da 0953  c_auc_score)...S
+00000ce0: 6b69 7070 6162 6c65 2901 da0a 4578 7065  kippable)...Expe
+00000cf0: 7269 6d65 6e74 2901 da19 6c6f 6164 5f76  riment)...load_v
+00000d00: 6973 7561 6c5f 6772 6170 685f 6461 7461  isual_graph_data
+00000d10: 7365 7429 01da 1663 7265 6174 655f 696d  set)...create_im
+00000d20: 706f 7274 616e 6365 735f 7064 6629 01da  portances_pdf)..
+00000d30: 1f72 6167 6765 645f 7465 6e73 6f72 5f66  .ragged_tensor_f
+00000d40: 726f 6d5f 6e65 7374 6564 5f6e 756d 7079  rom_nested_numpy
+00000d50: a901 da15 7072 6f63 6573 735f 6772 6170  ....process_grap
+00000d60: 685f 6461 7461 7365 7429 02da 0f61 7272  h_dataset)...arr
+00000d70: 6179 5f6e 6f72 6d61 6c69 7a65 da10 6269  ay_normalize..bi
+00000d80: 6e61 7279 5f74 6872 6573 686f 6c64 2902  nary_threshold).
+00000d90: da0b 6c61 7465 785f 7461 626c 65da 186c  ..latex_table..l
+00000da0: 6174 6578 5f74 6162 6c65 5f65 6c65 6d65  atex_table_eleme
+00000db0: 6e74 5f6d 6561 6e29 01da 0c72 656e 6465  nt_mean)...rende
+00000dc0: 725f 6c61 7465 787a 307e 2f2e 7669 7375  r_latexz0~/.visu
+00000dd0: 616c 5f67 7261 7068 5f64 6174 6173 6574  al_graph_dataset
+00000de0: 732f 6461 7461 7365 7473 2f72 625f 6475  s/datasets/rb_du
+00000df0: 616c 5f6d 6f74 6966 73da 1956 4953 5541  al_motifs..VISUA
+00000e00: 4c5f 4752 4150 485f 4441 5441 5345 545f  L_GRAPH_DATASET_
+00000e10: 5041 5448 da11 5553 455f 4441 5441 5345  PATH..USE_DATASE
+00000e20: 545f 5350 4c49 5467 9a99 9999 9999 e93f  T_SPLITg.......?
+00000e30: da0b 5452 4149 4e5f 5241 5449 4fe9 6400  ..TRAIN_RATIO.d.
+00000e40: 0000 da0c 4e55 4d5f 4558 414d 504c 4553  ....NUM_EXAMPLES
+00000e50: da0f 4558 414d 504c 455f 494e 4449 4345  ..EXAMPLE_INDICE
+00000e60: 53e9 0100 0000 da12 6e6f 6465 5f69 6d70  S.......node_imp
+00000e70: 6f72 7461 6e63 6573 5f31 da14 4e4f 4445  ortances_1..NODE
+00000e80: 5f49 4d50 4f52 5441 4e43 4553 5f4b 4559  _IMPORTANCES_KEY
+00000e90: da12 6564 6765 5f69 6d70 6f72 7461 6e63  ..edge_importanc
+00000ea0: 6573 5f31 da14 4544 4745 5f49 4d50 4f52  es_1..EDGE_IMPOR
+00000eb0: 5441 4e43 4553 5f4b 4559 46da 1455 5345  TANCES_KEYF..USE
+00000ec0: 5f4e 4f44 455f 434f 4f52 4449 4e41 5445  _NODE_COORDINATE
+00000ed0: 5354 da13 5553 455f 4544 4745 5f41 5454  ST..USE_EDGE_ATT
+00000ee0: 5249 4255 5445 53da 1055 5345 5f45 4447  RIBUTES..USE_EDG
+00000ef0: 455f 4c45 4e47 5448 53da 044d 4f43 4bda  E_LENGTHS..MOCK.
+00000f00: 0a4d 4f44 454c 5f4e 414d 45da 0b52 4550  .MODEL_NAME..REP
+00000f10: 4554 4954 494f 4e53 6300 0000 0000 0000  ETITIONSc.......
+00000f20: 0000 0000 0000 0000 0003 0000 0043 0000  .............C..
+00000f30: 0073 0e00 0000 7400 6a01 6a02 6401 6402  .s....t.j.j.d.d.
+00000f40: 8d01 5300 2903 4e67 7b14 ae47 e17a 843f  ..S.).Ng{..G.z.?
+00000f50: 2901 da0d 6c65 6172 6e69 6e67 5f72 6174  )...learning_rat
+00000f60: 6529 03da 026b 73da 0a6f 7074 696d 697a  e)...ks..optimiz
+00000f70: 6572 73da 054e 6164 616d a900 7228 0000  ers..Nadam..r(..
+00000f80: 0072 2800 0000 fa60 2f6d 6564 6961 2f73  .r(....`/media/s
+00000f90: 7364 2f50 726f 6772 616d 6d69 6e67 2f67  sd/Programming/g
+00000fa0: 7261 7068 5f61 7474 656e 7469 6f6e 5f73  raph_attention_s
+00000fb0: 7475 6465 6e74 2f67 7261 7068 5f61 7474  tudent/graph_att
+00000fc0: 656e 7469 6f6e 5f73 7475 6465 6e74 2f65  ention_student/e
+00000fd0: 7870 6572 696d 656e 7473 2f76 6764 5f73  xperiments/vgd_s
+00000fe0: 696e 676c 652e 7079 da08 3c6c 616d 6264  ingle.py..<lambd
+00000ff0: 613e 5300 0000 7302 0000 000e 0072 2a00  a>S...s......r*.
+00001000: 0000 e900 0100 00da 0a42 4154 4348 5f53  .........BATCH_S
+00001010: 495a 45e9 c800 0000 da06 4550 4f43 4853  IZE.......EPOCHS
+00001020: 7a05 6770 753a 30da 0644 4556 4943 45da  z.gpu:0..DEVICE.
+00001030: 0d4c 4f47 5f53 5445 505f 4556 414c da0f  .LOG_STEP_EVAL..
+00001040: 4241 5443 485f 5349 5a45 5f45 5641 4cda  BATCH_SIZE_EVAL.
+00001050: 0970 7265 6469 6374 6564 7a12 7265 7375  .predictedz.resu
+00001060: 6c74 732f 7667 645f 7369 6e67 6c65 7a25  lts/vgd_singlez%
+00001070: 5374 6172 7469 6e67 2074 6f20 7472 6169  Starting to trai
+00001080: 6e20 474e 4e58 206d 6f64 656c 206f 6e20  n GNNX model on 
+00001090: 7667 6420 22fa 0122 2903 da06 6c6f 6767  vgd "..")...logg
+000010a0: 6572 da08 6c6f 675f 7374 6570 da17 6d65  er..log_step..me
+000010b0: 7461 6461 7461 5f63 6f6e 7461 696e 735f  tadata_contains_
+000010c0: 696e 6465 78da 0764 6174 6173 6574 da08  index..dataset..
+000010d0: 6d65 7461 6461 7461 da05 6772 6170 68da  metadata..graph.
+000010e0: 106e 6f64 655f 696d 706f 7274 616e 6365  .node_importance
+000010f0: 73da 0c6e 6f64 655f 696e 6469 6365 7329  s..node_indices)
+00001100: 01da 0573 6861 7065 da10 6564 6765 5f69  ...shape..edge_i
+00001110: 6d70 6f72 7461 6e63 6573 da0c 6564 6765  mportances..edge
+00001120: 5f69 6e64 6963 6573 6301 0000 0000 0000  _indicesc.......
+00001130: 0000 0000 0002 0000 0005 0000 0043 0000  .............C..
+00001140: 0073 2c00 0000 6700 7c00 5d12 7d01 7400  .s,...g.|.].}.t.
+00001150: 6400 1900 7c01 1900 a001 a100 7400 6401  d...|.......t.d.
+00001160: 1900 7c01 1900 a001 a100 1700 9102 7102  ..|...........q.
+00001170: 5300 2902 da0f 6e6f 6465 5f61 7474 7269  S.)...node_attri
+00001180: 6275 7465 73da 106e 6f64 655f 636f 6f72  butes..node_coor
+00001190: 6469 6e61 7465 73a9 02da 0167 da06 746f  dinates....g..to
+000011a0: 6c69 7374 a902 da02 2e30 da01 6972 2800  list.....0..ir(.
+000011b0: 0000 7228 0000 0072 2900 0000 da0a 3c6c  ..r(...r).....<l
+000011c0: 6973 7463 6f6d 703e 8d00 0000 7306 0000  istcomp>....s...
+000011d0: 0006 0002 0124 ff72 4700 0000 723f 0000  .....$.rG...r?..
+000011e0: 0063 0100 0000 0000 0000 0000 0000 0300  .c..............
+000011f0: 0000 0500 0000 4300 0000 732e 0000 0067  ......C...s....g
+00001200: 007c 005d 135c 027d 017d 0274 0064 0019  .|.].\.}.}.t.d..
+00001210: 007c 0119 00a0 01a1 0074 0064 0119 007c  .|.......t.d...|
+00001220: 0119 0067 0117 0091 0271 0253 0029 02da  ...g.....q.S.)..
+00001230: 0f65 6467 655f 6174 7472 6962 7574 6573  .edge_attributes
+00001240: da0c 6564 6765 5f6c 656e 6774 6873 7241  ..edge_lengthsrA
+00001250: 0000 0029 0372 4500 0000 7246 0000 00da  ...).rE...rF....
+00001260: 015f 7228 0000 0072 2800 0000 7229 0000  ._r(...r(...r)..
+00001270: 0072 4700 0000 9100 0000 7306 0000 0006  .rG.......s.....
+00001280: 0006 0122 ff72 4800 0000 7a14 6c6f 6164  ...".rH...z.load
+00001290: 6564 2064 6174 6173 6574 2077 6974 6820  ed dataset with 
+000012a0: 7a09 2065 6c65 6d65 6e74 73da 0f70 726f  z. elements..pro
+000012b0: 6365 7373 5f64 6174 6173 6574 2901 da07  cess_dataset)...
+000012c0: 6465 6661 756c 7463 0400 0000 0000 0000  defaultc........
+000012d0: 0000 0000 0800 0000 0500 0000 4300 0000  ............C...
+000012e0: 7322 0000 0074 007c 017c 027c 0364 018d  s"...t.|.|.|.d..
+000012f0: 035c 047d 047d 057d 067d 077c 047c 057c  .\.}.}.}.}.|.|.|
+00001300: 067c 0766 0453 0029 024e 2902 da0d 7472  .|.f.S.).N)...tr
+00001310: 6169 6e5f 696e 6469 6365 73da 0c74 6573  ain_indices..tes
+00001320: 745f 696e 6469 6365 7372 0c00 0000 2908  t_indicesr....).
+00001330: da02 5f65 7237 0000 0072 4d00 0000 724e  .._er7...rM...rN
+00001340: 0000 00da 0778 5f74 7261 696e da07 795f  .....x_train..y_
+00001350: 7472 6169 6eda 0678 5f74 6573 74da 0679  train..x_test..y
+00001360: 5f74 6573 7472 2800 0000 7228 0000 0072  _testr(...r(...r
+00001370: 2900 0000 724b 0000 009d 0000 0073 0c00  )...rK.......s..
+00001380: 0000 0202 0201 0201 0201 0efd 0c05 7a0c  ..............z.
+00001390: 5245 5045 5449 5449 4f4e 2028 fa01 2ffa  REPETITION (../.
+000013a0: 0129 da03 7265 707a 2963 7265 6174 696e  .)..repz)creatin
+000013b0: 6720 7472 6169 6e20 7465 7374 2073 706c  g train test spl
+000013c0: 6974 2066 726f 6d20 6461 7461 7365 742e  it from dataset.
+000013d0: 2e2e 6301 0000 0000 0000 0000 0000 0003  ..c.............
+000013e0: 0000 0005 0000 0043 0000 00f3 2400 0000  .......C....$...
+000013f0: 6700 7c00 5d0e 5c02 7d01 7d02 7400 7c02  g.|.].\.}.}.t.|.
+00001400: 6400 1900 6401 1900 7600 7202 7c01 9102  d...d...v.r.|...
+00001410: 7102 5300 2902 7238 0000 0072 4d00 0000  q.S.).r8...rM...
+00001420: a901 7214 0000 00a9 0372 4500 0000 da05  ..r......rE.....
+00001430: 696e 6465 78da 0464 6174 6172 2800 0000  index..datar(...
+00001440: 7228 0000 0072 2900 0000 7247 0000 00af  r(...r)...rG....
+00001450: 0000 00f3 0600 0000 0c00 0e01 0aff 6301  ..............c.
+00001460: 0000 0000 0000 0000 0000 0003 0000 0005  ................
+00001470: 0000 0043 0000 0072 5700 0000 2902 7238  ...C...rW...).r8
+00001480: 0000 0072 4e00 0000 7258 0000 0072 5900  ...rN...rX...rY.
+00001490: 0000 7228 0000 0072 2800 0000 7229 0000  ..r(...r(...r)..
+000014a0: 0072 4700 0000 b100 0000 725c 0000 007a  .rG.......r\...z
+000014b0: 2363 7265 6174 696e 6720 7261 6e64 6f6d  #creating random
+000014c0: 2074 7261 696e 2074 6573 7420 7370 6c69   train test spli
+000014d0: 742e 2e2e 2901 da01 6b7a 0675 7369 6e67  t...)...kz.using
+000014e0: 207a 1720 7472 6169 6e69 6e67 2065 6c65   z. training ele
+000014f0: 6d65 6e74 7320 616e 6420 7a0e 2074 6573  ments and z. tes
+00001500: 7420 656c 656d 656e 7473 7a0e 7472 6169  t elementsz.trai
+00001510: 6e5f 696e 6469 6365 732f fa0d 7465 7374  n_indices/..test
+00001520: 5f69 6e64 6963 6573 2f7a 0c20 6173 2065  _indices/z. as e
+00001530: 7861 6d70 6c65 737a 1065 7861 6d70 6c65  xamplesz.example
+00001540: 5f69 6e64 6963 6573 2f7a 3663 6f6e 7665  _indices/z6conve
+00001550: 7274 696e 6720 6461 7461 7365 7420 696e  rting dataset in
+00001560: 746f 2072 6167 6765 6420 7465 6e73 6f72  to ragged tensor
+00001570: 7320 666f 7220 7472 6169 6e69 6e67 2e2e  s for training..
+00001580: 2e29 0372 3700 0000 724d 0000 0072 4e00  .).r7...rM...rN.
+00001590: 0000 7a15 6372 6561 7469 6e67 2074 6865  ..z.creating the
+000015a0: 206d 6f64 656c 2e2e 2eda 0c63 7265 6174   model.....creat
+000015b0: 655f 6d6f 6465 6cda 056d 6f64 656c 7a14  e_model..modelz.
+000015c0: 6669 7474 696e 6720 7468 6520 6d6f 6465  fitting the mode
+000015d0: 6c2e 2e2e da09 6669 745f 6d6f 6465 6c29  l.....fit_model)
+000015e0: 0572 6000 0000 7250 0000 0072 5100 0000  .r`...rP...rQ...
+000015f0: 7252 0000 0072 5300 0000 da07 6869 7374  rR...rS.....hist
+00001600: 6f72 797a 0868 6973 746f 7279 2f7a 0765  oryz.history/z.e
+00001610: 706f 6368 732f 7a16 6576 616c 7561 7469  pochs/z.evaluati
+00001620: 6e67 2074 6573 7420 7365 742e 2e2e da0b  ng test set.....
+00001630: 7175 6572 795f 6d6f 6465 6c29 0472 6000  query_model).r`.
+00001640: 0000 da01 78da 0179 da13 696e 636c 7564  ....x..y..includ
+00001650: 655f 696d 706f 7274 616e 6365 73e9 0200  e_importances...
+00001660: 0000 7a21 6361 6c63 756c 6174 696e 6720  ..z!calculating 
+00001670: 7072 6564 6963 7469 6f6e 206d 6574 7269  prediction metri
+00001680: 6373 2e2e 2efa 046d 7365 2ffa 0572 6d73  cs.....mse/..rms
+00001690: 652f fa04 6d61 652f fa03 7232 2f7a 1763  e/..mae/..r2/z.c
+000016a0: 616c 6375 6c61 7469 6e67 2066 6964 656c  alculating fidel
+000016b0: 6974 792e 2e2e da12 6361 6c63 756c 6174  ity.....calculat
+000016c0: 655f 6669 6465 6c69 7479 2907 7260 0000  e_fidelity).r`..
+000016d0: 00da 0c69 6e64 6963 6573 5f74 7275 65da  ...indices_true.
+000016e0: 0678 5f74 7275 65da 0679 5f74 7275 65da  .x_true..y_true.
+000016f0: 086f 7574 5f70 7265 64da 076e 695f 7072  .out_pred..ni_pr
+00001700: 6564 da07 6569 5f70 7265 64fa 0966 6964  ed..ei_pred..fid
+00001710: 656c 6974 792f 7a22 6361 6c63 756c 6174  elity/z"calculat
+00001720: 696e 6720 6578 706c 616e 6174 696f 6e20  ing explanation 
+00001730: 6d65 7472 6963 732e 2e2e da0c 6772 6170  metrics.....grap
+00001740: 685f 6c61 6265 6c73 7a09 6f75 742f 7472  h_labelsz.out/tr
+00001750: 7565 2f7a 096f 7574 2f70 7265 642f 7a08  ue/z.out/pred/z.
+00001760: 6e69 2f70 7265 642f 7a08 6569 2f70 7265  ni/pred/z.ei/pre
+00001770: 642f 6700 0000 0000 00e0 3ffa 0e6e 6f64  d/g.......?..nod
+00001780: 655f 7370 6172 7369 7479 2ffa 0e65 6467  e_sparsity/..edg
+00001790: 655f 7370 6172 7369 7479 2ffa 096e 6f64  e_sparsity/..nod
+000017a0: 655f 6175 632f fa09 6564 6765 5f61 7563  e_auc/..edge_auc
+000017b0: 2f7a 0820 3d20 6d73 653a 207a 032e 3266  /z. = mse: z..2f
+000017c0: 7a09 202d 2072 6d73 653a 207a 0820 2d20  z. - rmse: z. - 
+000017d0: 6d61 653a 207a 0720 2d20 7232 3a20 7a12  mae: z. - r2: z.
+000017e0: 202d 206d 6561 6e20 6669 6465 6c69 7479   - mean fidelity
+000017f0: 3a20 7a17 202d 206d 6561 6e20 6e6f 6465  : z. - mean node
+00001800: 2073 7061 7273 6974 793a 207a 1720 2d20   sparsity: z. - 
+00001810: 6d65 616e 2065 6467 6520 7370 6172 7369  mean edge sparsi
+00001820: 7479 3a20 7a0d 202d 206e 6f64 6520 6175  ty: z. - node au
+00001830: 633a 207a 0d20 2d20 6564 6765 2061 7563  c: z. - edge auc
+00001840: 3a20 7a21 6472 6177 696e 6720 6578 616d  : z!drawing exam
+00001850: 706c 6520 7669 7375 616c 697a 6174 696f  ple visualizatio
+00001860: 6e73 2e2e 2eda 0965 7861 6d70 6c65 735f  ns.....examples_
+00001870: da03 3032 647a 042e 7064 6663 0100 0000  ..02dz..pdfc....
+00001880: 0000 0000 0000 0000 0200 0000 0400 0000  ................
+00001890: 4300 0000 f31c 0000 0067 007c 005d 0a7d  C........g.|.].}
+000018a0: 0174 007c 0119 0064 0019 0064 0119 0091  .t.|...d...d....
+000018b0: 0271 0253 0029 0272 3800 0000 7239 0000  .q.S.).r8...r9..
+000018c0: 00a9 01da 0e69 6e64 6578 5f64 6174 615f  .....index_data_
+000018d0: 6d61 7072 4400 0000 7228 0000 0072 2800  maprD...r(...r(.
+000018e0: 0000 7229 0000 0072 4700 0000 5201 0000  ..r)...rG...R...
+000018f0: f302 0000 001c 0063 0100 0000 0000 0000  .......c........
+00001900: 0000 0000 0200 0000 0400 0000 4300 0000  ............C...
+00001910: 7318 0000 0067 007c 005d 087d 0174 007c  s....g.|.].}.t.|
+00001920: 0119 0064 0019 0091 0271 0253 0029 01da  ...d.....q.S.)..
+00001930: 0a69 6d61 6765 5f70 6174 6872 7c00 0000  .image_pathr|...
+00001940: 7244 0000 0072 2800 0000 7228 0000 0072  rD...r(...r(...r
+00001950: 2900 0000 7247 0000 0053 0100 0073 0200  )...rG...S...s..
+00001960: 0000 1800 6301 0000 0000 0000 0000 0000  ....c...........
+00001970: 0002 0000 0004 0000 0043 0000 0073 1400  .........C...s..
+00001980: 0000 6700 7c00 5d06 7d01 7c01 6400 1900  ..g.|.].}.|.d...
+00001990: 9102 7102 5300 2901 da0e 6e6f 6465 5f70  ..q.S.)...node_p
+000019a0: 6f73 6974 696f 6e73 7228 0000 0029 0272  ositionsr(...).r
+000019b0: 4500 0000 7242 0000 0072 2800 0000 7228  E...rB...r(...r(
+000019c0: 0000 0072 2900 0000 7247 0000 0054 0100  ...r)...rG...T..
+000019d0: 0073 0200 0000 1400 6301 0000 0000 0000  .s......c.......
+000019e0: 0000 0000 0002 0000 0004 0000 0043 0000  .............C..
+000019f0: 0072 7b00 0000 2902 7238 0000 00da 046e  .r{...).r8.....n
+00001a00: 616d 6572 7c00 0000 7244 0000 0072 2800  amer|...rD...r(.
+00001a10: 0000 7228 0000 0072 2900 0000 7247 0000  ..r(...r)...rG..
+00001a20: 005e 0100 0072 7e00 0000 2906 da0a 6772  .^...r~...)...gr
+00001a30: 6170 685f 6c69 7374 da0f 696d 6167 655f  aph_list..image_
+00001a40: 7061 7468 5f6c 6973 74da 136e 6f64 655f  path_list..node_
+00001a50: 706f 7369 7469 6f6e 735f 6c69 7374 da0f  positions_list..
+00001a60: 696d 706f 7274 616e 6365 735f 6d61 70da  importances_map.
+00001a70: 0b6f 7574 7075 745f 7061 7468 da0b 6c61  .output_path..la
+00001a80: 6265 6c73 5f6c 6973 74da 0a73 6176 655f  bels_list..save_
+00001a90: 6d6f 6465 6c29 0172 6000 0000 7a18 7265  model).r`...z.re
+00001aa0: 6e64 6572 696e 6720 6c61 7465 7820 7461  ndering latex ta
+00001ab0: 626c 652e 2e2e 290a 7a0b 5461 7267 6574  ble...).z.Target
+00001ac0: 204e 616d 657a 1824 5c74 6578 747b 4d53   Namez.$\text{MS
+00001ad0: 457d 205c 646f 776e 6172 726f 7720 247a  E} \downarrow $z
+00001ae0: 1924 5c74 6578 747b 524d 5345 7d20 5c64  .$\text{RMSE} \d
+00001af0: 6f77 6e61 7272 6f77 2024 7a18 245c 7465  ownarrow $z.$\te
+00001b00: 7874 7b4d 4145 7d20 5c64 6f77 6e61 7272  xt{MAE} \downarr
+00001b10: 6f77 2024 7a0f 2452 5e32 205c 7570 6172  ow $z.$R^2 \upar
+00001b20: 726f 7720 247a 1a24 5c74 6578 747b 4669  row $z.$\text{Fi
+00001b30: 6465 6c69 7479 7d20 5c75 7061 7272 6f77  delity} \uparrow
+00001b40: 247a 2124 5c74 6578 747b 4e6f 6465 2053  $z!$\text{Node S
+00001b50: 7061 7273 6974 797d 205c 646f 776e 6172  parsity} \downar
+00001b60: 726f 7724 7a21 245c 7465 7874 7b45 6467  row$z!$\text{Edg
+00001b70: 6520 5370 6172 7369 7479 7d20 5c64 6f77  e Sparsity} \dow
+00001b80: 6e61 7272 6f77 247a 1a24 5c74 6578 747b  narrow$z.$\text{
+00001b90: 4e6f 6465 2041 5543 7d20 5c75 7061 7272  Node AUC} \uparr
+00001ba0: 6f77 247a 1a24 5c74 6578 747b 4564 6765  ow$z.$\text{Edge
+00001bb0: 2041 5543 7d20 5c75 7061 7272 6f77 24fa   AUC} \uparrow$.
+00001bc0: 012d 6301 0000 0000 0000 0000 0000 0002  .-c.............
+00001bd0: 0000 0005 0000 0043 0000 00f3 1a00 0000  .......C........
+00001be0: 6700 7c00 5d09 7d01 7400 6400 7c01 9b00  g.|.].}.t.d.|...
+00001bf0: 9d02 1900 9102 7102 5300 2901 7268 0000  ......q.S.).rh..
+00001c00: 00a9 01da 0165 a902 7245 0000 0072 5600  .....e..rE...rV.
+00001c10: 0000 7228 0000 0072 2800 0000 7229 0000  ..r(...r(...r)..
+00001c20: 0072 4700 0000 7e01 0000 f302 0000 001a  .rG...~.........
+00001c30: 0063 0100 0000 0000 0000 0000 0000 0200  .c..............
+00001c40: 0000 0500 0000 4300 0000 728a 0000 0029  ......C...r....)
+00001c50: 0172 6900 0000 728b 0000 0072 8d00 0000  .ri...r....r....
+00001c60: 7228 0000 0072 2800 0000 7229 0000 0072  r(...r(...r)...r
+00001c70: 4700 0000 7f01 0000 728e 0000 0063 0100  G.......r....c..
+00001c80: 0000 0000 0000 0000 0000 0200 0000 0500  ................
+00001c90: 0000 4300 0000 728a 0000 0029 0172 6a00  ..C...r....).rj.
+00001ca0: 0000 728b 0000 0072 8d00 0000 7228 0000  ..r....r....r(..
+00001cb0: 0072 2800 0000 7229 0000 0072 4700 0000  .r(...r)...rG...
+00001cc0: 8001 0000 728e 0000 0063 0100 0000 0000  ....r....c......
+00001cd0: 0000 0000 0000 0200 0000 0500 0000 4300  ..............C.
+00001ce0: 0000 728a 0000 0029 0172 6b00 0000 728b  ..r....).rk...r.
+00001cf0: 0000 0072 8d00 0000 7228 0000 0072 2800  ...r....r(...r(.
+00001d00: 0000 7229 0000 0072 4700 0000 8101 0000  ..r)...rG.......
+00001d10: 728e 0000 0063 0100 0000 0000 0000 0000  r....c..........
+00001d20: 0000 0300 0000 0800 0000 4300 0000 f334  ..........C....4
+00001d30: 0000 0067 007c 005d 167d 0174 0064 007c  ...g.|.].}.t.d.|
+00001d40: 019b 009d 0219 0044 005d 0c7d 0274 0064  .......D.].}.t.d
+00001d50: 017c 019b 0064 027c 029b 009d 0419 0091  .|...d.|........
+00001d60: 0371 0b71 0253 0029 0372 5e00 0000 7273  .q.q.S.).r^...rs
+00001d70: 0000 0072 5400 0000 728b 0000 00a9 0372  ...rT...r......r
+00001d80: 4500 0000 7256 0000 0072 5a00 0000 7228  E...rV...rZ...r(
+00001d90: 0000 0072 2800 0000 7229 0000 0072 4700  ...r(...r)...rG.
+00001da0: 0000 8201 0000 f30c 0000 0006 0002 010c  ................
+00001db0: 0104 fe02 021a fe63 0100 0000 0000 0000  .......c........
+00001dc0: 0000 0000 0300 0000 0800 0000 4300 0000  ............C...
+00001dd0: 728f 0000 0029 0372 5e00 0000 7275 0000  r....).r^...ru..
+00001de0: 0072 5400 0000 728b 0000 0072 9000 0000  .rT...r....r....
+00001df0: 7228 0000 0072 2800 0000 7229 0000 0072  r(...r(...r)...r
+00001e00: 4700 0000 8501 0000 7291 0000 0063 0100  G.......r....c..
+00001e10: 0000 0000 0000 0000 0000 0300 0000 0800  ................
+00001e20: 0000 4300 0000 728f 0000 0029 0372 5e00  ..C...r....).r^.
+00001e30: 0000 7276 0000 0072 5400 0000 728b 0000  ..rv...rT...r...
+00001e40: 0072 9000 0000 7228 0000 0072 2800 0000  .r....r(...r(...
+00001e50: 7229 0000 0072 4700 0000 8801 0000 7291  r)...rG.......r.
+00001e60: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
+00001e70: 0200 0000 0500 0000 4300 0000 728a 0000  ........C...r...
+00001e80: 0029 0172 7700 0000 728b 0000 0072 8d00  .).rw...r....r..
+00001e90: 0000 7228 0000 0072 2800 0000 7229 0000  ..r(...r(...r)..
+00001ea0: 0072 4700 0000 8b01 0000 728e 0000 0063  .rG.......r....c
+00001eb0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00001ec0: 0500 0000 4300 0000 728a 0000 0029 0172  ....C...r....).r
+00001ed0: 7800 0000 728b 0000 0072 8d00 0000 7228  x...r....r....r(
+00001ee0: 0000 0072 2800 0000 7229 0000 0072 4700  ...r(...r)...rG.
+00001ef0: 0000 8c01 0000 728e 0000 007a 0b52 6573  ......r....z.Res
+00001f00: 756c 7473 206f 6620 7a12 2072 6570 6574  ults of z. repet
+00001f10: 6974 696f 6e28 7329 206f 6620 7a08 5c74  ition(s) of z.\t
+00001f20: 6578 7462 667b da01 7d29 04da 0c63 6f6c  extbf{..})...col
+00001f30: 756d 6e5f 6e61 6d65 73da 0472 6f77 73da  umn_names..rows.
+00001f40: 0f6c 6973 745f 656c 656d 656e 745f 6362  .list_element_cb
+00001f50: da07 6361 7074 696f 6e7a 0974 6162 6c65  ..captionz.table
+00001f60: 2e74 6578 7a09 7461 626c 652e 7064 66da  .texz.table.pdf.
+00001f70: 0763 6f6e 7465 6e74 2901 7286 0000 007a  .content).r....z
+00001f80: 1472 656e 6465 7265 6420 6c61 7465 7820  .rendered latex 
+00001f90: 7461 626c 6529 b0da 075f 5f64 6f63 5f5f  table)...__doc__
+00001fa0: da02 6f73 da03 7379 73da 0770 6174 686c  ..os..sys..pathl
+00001fb0: 6962 da06 7261 6e64 6f6d da06 7479 7069  ib..random..typi
+00001fc0: 6e67 da01 74da 0b63 6f6c 6c65 6374 696f  ng..t..collectio
+00001fd0: 6e73 7202 0000 00da 0a74 656e 736f 7266  nsr......tensorf
+00001fe0: 6c6f 77da 0274 66da 1074 656e 736f 7266  low..tf..tensorf
+00001ff0: 6c6f 772e 6b65 7261 73da 056b 6572 6173  low.keras..keras
+00002000: 7225 0000 00da 056e 756d 7079 da02 6e70  r%.....numpy..np
+00002010: da11 6d61 7470 6c6f 746c 6962 2e70 7970  ..matplotlib.pyp
+00002020: 6c6f 74da 0670 7970 6c6f 74da 0370 6c74  lot..pyplot..plt
+00002030: da0f 736b 6c65 6172 6e2e 6d65 7472 6963  ..sklearn.metric
+00002040: 7372 0300 0000 7204 0000 0072 0500 0000  sr....r....r....
+00002050: 7206 0000 00da 0c70 7963 6f6d 6578 2e75  r......pycomex.u
+00002060: 7469 6c72 0700 0000 da12 7079 636f 6d65  tilr......pycome
+00002070: 782e 6578 7065 7269 6d65 6e74 7208 0000  x.experimentr...
+00002080: 00da 1a76 6973 7561 6c5f 6772 6170 685f  ...visual_graph_
+00002090: 6461 7461 7365 7473 2e64 6174 6172 0900  datasets.datar..
+000020a0: 0000 da2f 7669 7375 616c 5f67 7261 7068  .../visual_graph
+000020b0: 5f64 6174 6173 6574 732e 7669 7375 616c  _datasets.visual
+000020c0: 697a 6174 696f 6e2e 696d 706f 7274 616e  ization.importan
+000020d0: 6365 7372 0a00 0000 da10 6b67 636e 6e2e  cesr......kgcnn.
+000020e0: 6461 7461 2e75 7469 6c73 720b 0000 00da  data.utilsr.....
+000020f0: 1e67 7261 7068 5f61 7474 656e 7469 6f6e  .graph_attention
+00002100: 5f73 7475 6465 6e74 2e74 7970 696e 67da  _student.typing.
+00002110: 0274 63da 1c67 7261 7068 5f61 7474 656e  .tc..graph_atten
+00002120: 7469 6f6e 5f73 7475 6465 6e74 2e64 6174  tion_student.dat
+00002130: 6172 0d00 0000 da1c 6772 6170 685f 6174  ar......graph_at
+00002140: 7465 6e74 696f 6e5f 7374 7564 656e 742e  tention_student.
+00002150: 7574 696c 720e 0000 0072 0f00 0000 7210  utilr....r....r.
+00002160: 0000 0072 1100 0000 7212 0000 00da 0470  ...r....r......p
+00002170: 6174 68da 0a65 7870 616e 6475 7365 7272  ath..expanduserr
+00002180: 1300 0000 da03 7374 72da 0f5f 5f61 6e6e  ......str..__ann
+00002190: 6f74 6174 696f 6e73 5f5f 7214 0000 00da  otations__r.....
+000021a0: 084f 7074 696f 6e61 6cda 0369 6e74 7215  .Optional..intr.
+000021b0: 0000 00da 0566 6c6f 6174 7217 0000 0072  .....floatr....r
+000021c0: 1800 0000 da04 4c69 7374 da13 494d 504f  ......List..IMPO
+000021d0: 5254 414e 4345 5f43 4841 4e4e 454c 5372  RTANCE_CHANNELSr
+000021e0: 1b00 0000 721d 0000 0072 1e00 0000 da04  ....r....r......
+000021f0: 626f 6f6c 721f 0000 0072 2000 0000 7222  boolr....r ...r"
+00002200: 0000 0072 2300 0000 da0c 4f50 5449 4d49  ...r#.....OPTIMI
+00002210: 5a45 525f 4342 722c 0000 0072 2e00 0000  ZER_CBr,...r....
+00002220: 722f 0000 0072 3000 0000 7231 0000 00da  r/...r0...r1....
+00002230: 1949 4d50 4f52 5441 4e43 455f 4348 414e  .IMPORTANCE_CHAN
+00002240: 4e45 4c5f 4c41 4245 4c53 da06 6765 7463  NEL_LABELS..getc
+00002250: 7764 da09 4241 5345 5f50 4154 48da 094e  wd..BASE_PATH..N
+00002260: 414d 4553 5041 4345 da05 4445 4255 47da  AMESPACE..DEBUG.
+00002270: 0767 6c6f 6261 6c73 728c 0000 00da 0862  .globalsr......b
+00002280: 6173 656e 616d 65da 0876 6764 5f6e 616d  asename..vgd_nam
+00002290: 65da 0469 6e66 6f72 3400 0000 da0c 6d65  e..infor4.....me
+000022a0: 7461 6461 7461 5f6d 6170 727d 0000 00da  tadata_mapr}....
+000022b0: 046c 6973 74da 0673 6f72 7465 64da 046b  .list..sorted..k
+000022c0: 6579 73da 0f64 6174 6173 6574 5f69 6e64  eys..dataset_ind
+000022d0: 6963 6573 da03 7365 74da 1364 6174 6173  ices..set..datas
+000022e0: 6574 5f69 6e64 6963 6573 5f73 6574 da03  et_indices_set..
+000022f0: 6c65 6eda 0e64 6174 6173 6574 5f6c 656e  len..dataset_len
+00002300: 6774 6872 3700 0000 da09 4772 6170 6844  gthr7.....GraphD
+00002310: 6963 7472 5a00 0000 725b 0000 0072 4200  ictrZ...r[...rB.
+00002320: 0000 da05 7a65 726f 73da 0561 7272 6179  ....zeros..array
+00002330: da09 656e 756d 6572 6174 65da 046f 6e65  ..enumerate..one
+00002340: 73da 0661 7070 656e 64da 0468 6f6f 6b72  s..append..hookr
+00002350: 4b00 0000 da05 7261 6e67 6572 5600 0000  K.....rangerV...
+00002360: da06 6465 7669 6365 da05 6974 656d 7372  ..device..itemsr
+00002370: 4d00 0000 724e 0000 00da 0673 616d 706c  M...rN.....sampl
+00002380: 65da 1174 7261 696e 5f69 6e64 6963 6573  e..train_indices
+00002390: 5f73 6574 da0a 6469 6666 6572 656e 6365  _set..difference
+000023a0: da10 7465 7374 5f69 6e64 6963 6573 5f73  ..test_indices_s
+000023b0: 6574 da03 6d69 6eda 0c6e 756d 5f65 7861  et..min..num_exa
+000023c0: 6d70 6c65 73da 0f65 7861 6d70 6c65 5f69  mples..example_i
+000023d0: 6e64 6963 6573 da0a 6170 706c 795f 686f  ndices..apply_ho
+000023e0: 6f6b 7250 0000 0072 5100 0000 7252 0000  okrP...rQ...rR..
+000023f0: 0072 5300 0000 7260 0000 00da 066d 6f64  .rS...r`.....mod
+00002400: 656c 73da 054d 6f64 656c 7262 0000 00da  els..Modelrb....
+00002410: 0464 6963 7472 7000 0000 7271 0000 0072  .dictrp...rq...r
+00002420: 7200 0000 da08 6f75 745f 7472 7565 da07  r.....out_true..
+00002430: 6e69 5f74 7275 65da 0765 695f 7472 7565  ni_true..ei_true
+00002440: da09 6d73 655f 7661 6c75 65da 0473 7172  ..mse_value..sqr
+00002450: 74da 0a72 6d73 655f 7661 6c75 65da 096d  t..rmse_value..m
+00002460: 6165 5f76 616c 7565 da08 7232 5f76 616c  ae_value..r2_val
+00002470: 7565 da0a 6669 6465 6c69 7469 6573 da03  ue..fidelities..
+00002480: 7a69 70da 0866 6964 656c 6974 79da 1570  zip..fidelity..p
+00002490: 7265 645f 6e6f 6465 5f69 6d70 6f72 7461  red_node_importa
+000024a0: 6e63 6573 da15 7072 6564 5f65 6467 655f  nces..pred_edge_
+000024b0: 696d 706f 7274 616e 6365 73da 1574 7275  importances..tru
+000024c0: 655f 6e6f 6465 5f69 6d70 6f72 7461 6e63  e_node_importanc
+000024d0: 6573 da15 7472 7565 5f65 6467 655f 696d  es..true_edge_im
+000024e0: 706f 7274 616e 6365 73da 0163 da02 6e69  portances..c..ni
+000024f0: da02 6569 da07 666c 6174 7465 6e72 4300  ..ei..flattenrC.
+00002500: 0000 da04 6d65 616e da0d 6e6f 6465 5f73  ....mean..node_s
+00002510: 7061 7273 6974 79da 0d65 6467 655f 7370  parsity..edge_sp
+00002520: 6172 7369 7479 da06 7661 6c75 6573 da0d  arsity..values..
+00002530: 6d65 616e 5f66 6964 656c 6974 79da 126d  mean_fidelity..m
+00002540: 6561 6e5f 6e6f 6465 5f73 7061 7273 6974  ean_node_sparsit
+00002550: 79da 126d 6561 6e5f 6564 6765 5f73 7061  y..mean_edge_spa
+00002560: 7273 6974 79da 086e 6f64 655f 6175 63da  rsity..node_auc.
+00002570: 0865 6467 655f 6175 63da 0a56 616c 7565  .edge_auc..Value
+00002580: 4572 726f 72da 0f6e 695f 6578 616d 706c  Error..ni_exampl
+00002590: 655f 7072 6564 da0f 6569 5f65 7861 6d70  e_pred..ei_examp
+000025a0: 6c65 5f70 7265 64da 046a 6f69 6eda 0870  le_pred..join..p
+000025b0: 6466 5f70 6174 6872 8200 0000 7283 0000  df_pathr....r...
+000025c0: 0072 8400 0000 da06 7374 6174 7573 da08  .r......status..
+000025d0: 616e 616c 7973 6973 7293 0000 0072 9400  analysisr....r..
+000025e0: 0000 da03 726f 7772 9700 0000 da05 7461  ....rowr......ta
+000025f0: 626c 65da 0a63 6f6d 6d69 745f 7261 7772  ble..commit_rawr
+00002600: 2800 0000 7228 0000 0072 2800 0000 7229  (...r(...r(...r)
+00002610: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
+00002620: 0073 2e02 0000 0600 0803 0801 0801 0801  .s..............
+00002630: 0801 0c01 0802 0c01 0801 0c01 0c01 0c01  ................
+00002640: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c02  ................
+00002650: 0c01 1001 1001 0c01 1407 1205 0c03 0c04  ................
+00002660: 1203 0402 1204 1202 0c03 0c04 0c03 0c05  ................
+00002670: 0c07 0802 0c01 0c01 0c01 0c06 0c02 0604  ................
+00002680: 0803 0401 0401 2001 0c02 1201 0204 0201  ...... .........
+00002690: 0401 0201 0201 0afc 1008 0801 0801 1404  ................
+000026a0: 0801 0801 0c01 0a02 0e01 1c02 0a02 0e01  ................
+000026b0: 1c02 0602 0a01 0601 0cff 0603 0a01 0a01  ................
+000026c0: 0cff 0603 1c01 0e02 1602 0c04 0a01 0e09  ................
+000026d0: 1c01 0801 0e02 0a02 0a01 1201 1402 0a04  ................
+000026e0: 1601 0801 0a01 0801 1002 0801 2001 0e01  ............ ...
+000026f0: 0e01 1602 1601 1601 0e01 0a02 0401 0201  ................
+00002700: 0201 0201 0201 0efc 0a07 1601 0a02 0401  ................
+00002710: 0201 0201 0201 0201 0201 0201 0efa 0e08  ................
+00002720: 1601 0a03 0401 0201 0201 0201 0201 0201  ................
+00002730: 0cfb 0e07 0e01 0e01 0e02 1201 1201 0a03  ................
+00002740: 0a01 0a01 0a01 0a01 0e01 0e01 0e01 0e01  ................
+00002750: 0a02 0401 0201 0201 0201 0201 0201 0201  ................
+00002760: 0201 0201 06f8 060a 1201 1801 0a03 0402  ................
+00002770: 0401 0402 0401 1002 1001 0c01 0c01 2002  .............. .
+00002780: 2001 1402 1401 1402 1401 1402 1401 1403   ...............
+00002790: 1401 1401 1801 1c02 1c01 1c01 0206 0a01  ................
+000027a0: 0e01 0e01 0401 0801 02fe 0e04 0e01 0e02  ................
+000027b0: 0401 04ff 0402 04fe 0403 04fd 0404 04fc  ................
+000027c0: 0405 04fb 0406 04fa 0407 04f9 0408 08f8  ................
+000027d0: 0a0d 0402 0401 0801 1a01 1e01 1a04 0e01  ................
+000027e0: 0e01 0e01 0201 0201 0201 0201 0802 02ff  ................
+000027f0: 0203 0c02 06f7 040d 0201 0201 06fe 0a05  ................
+00002800: 0081 1ec3 0480 02fc 1ec1 0280 1e00 007f  ................
+00002810: 007f 1004 0a02 0801 040c 0402 0a02 1801  ................
+00002820: 1801 1801 1801 0a01 0601 08ff 0a03 0601  ................
+00002830: 08ff 0a03 0601 08ff 1803 1801 0a02 0202  ................
+00002840: 0201 0201 0201 1601 0afc 0c06 1001 1001  ................
+00002850: 0c01 54d1                                ..T.
```

### Comparing `graph_attention_student-0.7.0/graph_attention_student/experiments/__pycache__/vgd_single_gnnx.cpython-310.pyc` & `graph_attention_student-0.7.1/graph_attention_student/experiments/__pycache__/vgd_single_gnnx.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.0/graph_attention_student/experiments/__pycache__/vgd_single_gnnx_aqsoldb.cpython-310.pyc` & `graph_attention_student-0.7.1/graph_attention_student/experiments/__pycache__/vgd_single_gnnx_aqsoldb.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.0/graph_attention_student/experiments/__pycache__/vgd_single_megan.cpython-310.pyc` & `graph_attention_student-0.7.1/graph_attention_student/experiments/__pycache__/vgd_single_megan.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jan 24 12:14:49 2023 UTC, .py size: 7532 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,272 +1,296 @@
-00000000: 6f0d 0d0a 0000 0000 b9cb cf63 6c1d 0000  o..........cl...
+00000000: 6f0d 0d0a 0000 0000 16e2 3f64 0c1f 0000  o.........?d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0009 0000 0040 0000 0073 3402 0000 5500  .....@...s4...U.
-00000030: 6400 6401 6c00 5a00 6400 6401 6c01 5a01  d.d.l.Z.d.d.l.Z.
-00000040: 6400 6401 6c02 5a03 6400 6401 6c04 5a05  d.d.l.Z.d.d.l.Z.
-00000050: 6400 6401 6c06 6d07 5a08 0100 6400 6401  d.d.l.m.Z...d.d.
-00000060: 6c09 5a0a 6400 6402 6c0b 6d0c 5a0c 0100  l.Z.d.d.l.m.Z...
-00000070: 6400 6403 6c0d 6d0e 5a0e 0100 6400 6404  d.d.l.m.Z...d.d.
-00000080: 6c0f 6d10 5a10 0100 6400 6405 6c11 6d12  l.m.Z...d.d.l.m.
-00000090: 5a12 0100 6400 6406 6c13 6d14 5a14 6d15  Z...d.d.l.m.Z.m.
-000000a0: 5a15 0100 6400 6407 6c13 6d16 5a16 0100  Z...d.d.l.m.Z...
-000000b0: 6408 5a17 6503 6a18 6519 1900 651a 6409  d.Z.e.j.e...e.d.
-000000c0: 3c00 640a 5a1b 6503 6a18 6519 1900 651a  <.d.Z.e.j.e...e.
-000000d0: 640b 3c00 640c 5a1c 6519 651a 640d 3c00  d.<.d.Z.e.e.d.<.
-000000e0: 6700 640e a201 5a1d 6503 6a1e 651f 1900  g.d...Z.e.j.e...
-000000f0: 651a 640f 3c00 6410 5a20 6521 651a 6411  e.d.<.d.Z e!e.d.
-00000100: 3c00 6412 5a22 6521 651a 6413 3c00 6414  <.d.Z"e!e.d.<.d.
-00000110: 5a23 6521 651a 6415 3c00 6416 5a24 651f  Z#e!e.d.<.d.Z$e.
-00000120: 651a 6417 3c00 6418 5a25 6521 651a 6419  e.d.<.d.Z%e!e.d.
-00000130: 3c00 641a 5a26 6527 651a 641b 3c00 6400  <.d.Z&e'e.d.<.d.
-00000140: 5a28 641c 641d 6702 6701 5a29 641e 641f  Z(d.d.g.g.Z)d.d.
-00000150: 6420 9c02 5a2a 6700 6421 a201 5a2b 6410  d ..Z*g.d!..Z+d.
-00000160: 5a2c 6422 5a2d 6423 6424 8400 5a2e 6425  Z,d"Z-d#d$..Z.d%
-00000170: 6426 6702 5a2f 6501 a030 6531 a101 6a32  d&g.Z/e..0e1..j2
-00000180: a033 a100 5a34 6500 6a35 a036 6534 6427  .3..Z4e.j5.6e4d'
-00000190: a102 5a37 6534 5a38 6428 5a39 6429 5a3a  ..Z7e4Z8d(Z9d)Z:
-000001a0: 650c 8300 8f53 0100 650e 6537 6538 6539  e....S..e.e7e8e9
-000001b0: 653b 8300 8304 0400 5a3c 8f30 0100 653c  e;......Z<.0..e<
-000001c0: a03d 642a a101 642b 642a 8400 8301 5a3e  .=d*..d+d*....Z>
-000001d0: 653c a03d 642c a101 642d 642c 8400 8301  e<.=d,..d-d,....
-000001e0: 5a3f 653c a03d 642e a101 6433 642f 6527  Z?e<.=d...d3d/e'
-000001f0: 6602 6430 642e 8405 8301 5a40 653c a03d  f.d0d.....Z@e<.=
-00000200: 6431 a101 6432 6431 8400 8301 5a41 5700  d1..d2d1....ZAW.
-00000210: 6401 0400 0400 8303 0100 6e10 3100 73fa  d.........n.1.s.
-00000220: 7701 0100 0100 0100 5900 0100 5700 6401  w.......Y...W.d.
-00000230: 0400 0400 8303 0100 6401 5300 5700 6401  ........d.S.W.d.
-00000240: 0400 0400 8303 0100 6401 5300 3100 9001  ........d.S.1...
-00000250: 7313 7701 0100 0100 0100 5900 0100 6401  s.w.......Y...d.
-00000260: 5300 2934 e900 0000 004e 2901 da09 536b  S.)4.....N)...Sk
-00000270: 6970 7061 626c 6529 01da 0d53 7562 4578  ippable)...SubEx
-00000280: 7065 7269 6d65 6e74 2901 da1f 7261 6767  periment)...ragg
-00000290: 6564 5f74 656e 736f 725f 6672 6f6d 5f6e  ed_tensor_from_n
-000002a0: 6573 7465 645f 6e75 6d70 7929 01da 054d  ested_numpy)...M
-000002b0: 6567 616e 2902 da06 4e6f 4c6f 7373 da03  egan)...NoLoss..
-000002c0: 6d73 6529 01da 134c 6f67 5072 6f67 7265  mse)...LogProgre
-000002d0: 7373 4361 6c6c 6261 636b da12 6e6f 6465  ssCallback..node
-000002e0: 5f69 6d70 6f72 7461 6e63 6573 5f32 da14  _importances_2..
-000002f0: 4e4f 4445 5f49 4d50 4f52 5441 4e43 4553  NODE_IMPORTANCES
-00000300: 5f4b 4559 da12 6564 6765 5f69 6d70 6f72  _KEY..edge_impor
-00000310: 7461 6e63 6573 5f32 da14 4544 4745 5f49  tances_2..EDGE_I
-00000320: 4d50 4f52 5441 4e43 4553 5f4b 4559 da05  MPORTANCES_KEY..
-00000330: 4d45 4741 4eda 0a4d 4f44 454c 5f4e 414d  MEGAN..MODEL_NAM
-00000340: 4529 03e9 2000 0000 720f 0000 0072 0f00  E).. ...r....r..
-00000350: 0000 da05 554e 4954 5367 0000 0000 0000  ....UNITSg......
-00000360: 0000 da0c 4452 4f50 4f55 545f 5241 5445  ....DROPOUT_RATE
-00000370: 6700 0000 0000 00f0 3fda 1149 4d50 4f52  g.......?..IMPOR
-00000380: 5441 4e43 455f 4641 4354 4f52 e905 0000  TANCE_FACTOR....
-00000390: 00da 1549 4d50 4f52 5441 4e43 455f 4d55  ...IMPORTANCE_MU
-000003a0: 4c54 4950 4c49 4552 e902 0000 00da 1349  LTIPLIER.......I
-000003b0: 4d50 4f52 5441 4e43 455f 4348 414e 4e45  MPORTANCE_CHANNE
-000003c0: 4c53 6700 0000 0000 0014 40da 0f53 5041  LSg.......@..SPA
-000003d0: 5253 4954 595f 4641 4354 4f52 46da 0c43  RSITY_FACTORF..C
-000003e0: 4f4e 4341 545f 4845 4144 53e9 fdff ffff  ONCAT_HEADS.....
-000003f0: e903 0000 00e9 ffff ffff e901 0000 0029  ...............)
-00000400: 0272 0100 0000 721c 0000 0029 03e9 3c00  .r....r....)..<.
-00000410: 0000 e914 0000 0072 1c00 0000 e9fa 0000  .......r........
-00000420: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-00000430: 0000 0300 0000 4300 0000 730e 0000 0074  ......C...s....t
-00000440: 006a 016a 0264 0164 028d 0153 0029 034e  .j.j.d.d...S.).N
-00000450: 677b 14ae 47e1 7a84 3f29 01da 0d6c 6561  g{..G.z.?)...lea
-00000460: 726e 696e 675f 7261 7465 2903 da02 6b73  rning_rate)...ks
-00000470: da0a 6f70 7469 6d69 7a65 7273 da05 4e61  ..optimizers..Na
-00000480: 6461 6da9 0072 2400 0000 7224 0000 00fa  dam..r$...r$....
-00000490: 632f 686f 6d65 2f6a 6f6e 6173 2f50 7269  c/home/jonas/Pri
-000004a0: 7661 7465 2f67 7261 7068 5f61 7474 656e  vate/graph_atten
-000004b0: 7469 6f6e 5f73 7475 6465 6e74 2f67 7261  tion_student/gra
-000004c0: 7068 5f61 7474 656e 7469 6f6e 5f73 7475  ph_attention_stu
-000004d0: 6465 6e74 2f65 7870 6572 696d 656e 7473  dent/experiments
-000004e0: 2f76 6764 5f73 696e 676c 655f 6d65 6761  /vgd_single_mega
-000004f0: 6e2e 7079 da08 3c6c 616d 6264 613e 5200  n.py..<lambda>R.
-00000500: 0000 7302 0000 000e 0072 2600 0000 da08  ..s......r&.....
-00000510: 6e65 6761 7469 7665 da08 706f 7369 7469  negative..positi
-00000520: 7665 7a0d 7667 645f 7369 6e67 6c65 2e70  vez.vgd_single.p
-00000530: 797a 1872 6573 756c 7473 2f76 6764 5f73  yz.results/vgd_s
-00000540: 696e 676c 655f 6d65 6761 6e54 da0c 6372  ingle_meganT..cr
-00000550: 6561 7465 5f6d 6f64 656c 6301 0000 0000  eate_modelc.....
-00000560: 0000 0000 0000 0002 0000 000f 0000 0043  ...............C
-00000570: 0000 0073 9e00 0000 7c00 a000 6401 a101  ...s....|...d...
-00000580: 0100 7401 7c00 6a02 6402 1900 7c00 6a02  ..t.|.j.d...|.j.
-00000590: 6403 1900 7c00 6a02 6404 1900 7c00 6a02  d...|.j.d...|.j.
-000005a0: 6405 1900 7c00 6a02 6406 1900 7c00 6a02  d...|.j.d...|.j.
-000005b0: 6407 1900 7c00 6a02 6408 1900 7c00 6a02  d...|.j.d...|.j.
-000005c0: 6409 1900 7c00 6a02 640a 1900 7c00 6a02  d...|.j.d...|.j.
-000005d0: 640b 1900 640c 640d 7c00 6a02 640e 1900  d...d.d.|.j.d...
-000005e0: 640f 8d0d 7d01 7c01 6a03 7404 7405 8300  d...}.|.j.t.t...
-000005f0: 7405 8300 6703 6700 6410 a201 7404 6701  t...g.g.d...t.g.
-00000600: 7c00 6a02 6411 1900 8300 640c 6412 8d05  |.j.d.....d.d...
-00000610: 0100 7c01 5300 2913 4e72 0d00 0000 7210  ..|.S.).Nr....r.
-00000620: 0000 0072 1100 0000 7212 0000 0072 1400  ...r....r....r..
-00000630: 0000 7216 0000 0072 1700 0000 da14 5245  ..r....r......RE
-00000640: 4752 4553 5349 4f4e 5f52 4546 4552 454e  GRESSION_REFEREN
-00000650: 4345 da11 5245 4752 4553 5349 4f4e 5f4c  CE..REGRESSION_L
-00000660: 494d 4954 53da 0b46 494e 414c 5f55 4e49  IMITS..FINAL_UNI
-00000670: 5453 da0d 4649 4e41 4c5f 4452 4f50 4f55  TS..FINAL_DROPOU
-00000680: 5446 5472 1800 0000 290d da05 756e 6974  TFTr....)...unit
-00000690: 73da 0c64 726f 706f 7574 5f72 6174 65da  s..dropout_rate.
-000006a0: 1169 6d70 6f72 7461 6e63 655f 6661 6374  .importance_fact
-000006b0: 6f72 da15 696d 706f 7274 616e 6365 5f6d  or..importance_m
-000006c0: 756c 7469 706c 6965 72da 1369 6d70 6f72  ultiplier..impor
-000006d0: 7461 6e63 655f 6368 616e 6e65 6c73 da0f  tance_channels..
-000006e0: 7370 6172 7369 7479 5f66 6163 746f 72da  sparsity_factor.
-000006f0: 1472 6567 7265 7373 696f 6e5f 7265 6665  .regression_refe
-00000700: 7265 6e63 65da 1172 6567 7265 7373 696f  rence..regressio
-00000710: 6e5f 6c69 6d69 7473 da0b 6669 6e61 6c5f  n_limits..final_
-00000720: 756e 6974 73da 1266 696e 616c 5f64 726f  units..final_dro
-00000730: 706f 7574 5f72 6174 65da 1475 7365 5f67  pout_rate..use_g
-00000740: 7261 7068 5f61 7474 7269 6275 7465 73da  raph_attributes.
-00000750: 1175 7365 5f65 6467 655f 6665 6174 7572  .use_edge_featur
-00000760: 6573 da0c 636f 6e63 6174 5f68 6561 6473  es..concat_heads
-00000770: 2903 721c 0000 0072 0100 0000 7201 0000  ).r....r....r...
-00000780: 00da 0c4f 5054 494d 495a 4552 5f43 4229  ...OPTIMIZER_CB)
-00000790: 05da 046c 6f73 73da 0c6c 6f73 735f 7765  ...loss..loss_we
-000007a0: 6967 6874 73da 076d 6574 7269 6373 da09  ights..metrics..
-000007b0: 6f70 7469 6d69 7a65 72da 0b72 756e 5f65  optimizer..run_e
-000007c0: 6167 6572 6c79 2906 da04 696e 666f 7205  agerly)...infor.
-000007d0: 0000 00da 0a70 6172 616d 6574 6572 73da  .....parameters.
-000007e0: 0763 6f6d 7069 6c65 7207 0000 0072 0600  .compiler....r..
-000007f0: 0000 2902 da01 65da 056d 6f64 656c 7224  ..)...e..modelr$
-00000800: 0000 0072 2400 0000 7225 0000 0072 2900  ...r$...r%...r).
-00000810: 0000 6100 0000 7336 0000 000a 0202 0108  ..a...s6........
-00000820: 0108 0108 0108 0108 0108 0108 0108 0108  ................
-00000830: 0108 0102 0102 0108 0106 f304 0f02 0204  ................
-00000840: 0104 0102 fd06 0504 030a 0102 0106 f504  ................
-00000850: 0dda 0966 6974 5f6d 6f64 656c 6306 0000  ...fit_modelc...
-00000860: 0000 0000 0000 0000 0007 0000 000c 0000  ................
-00000870: 0043 0000 0073 3e00 0000 7c01 6a00 7c02  .C...s>...|.j.|.
-00000880: 7c03 7c00 6a01 6401 1900 7c00 6a01 6402  |.|.j.d...|.j.d.
-00000890: 1900 7c04 7c05 6602 6403 7402 7c00 6a03  ..|.|.f.d.t.|.j.
-000008a0: 6404 6405 6406 8d03 6701 6407 6408 8d08  d.d.d...g.d.d...
-000008b0: 7d06 7c06 6a04 5300 2909 4eda 0a42 4154  }.|.j.S.).N..BAT
-000008c0: 4348 5f53 495a 45da 0645 504f 4348 5372  CH_SIZE..EPOCHSr
-000008d0: 1c00 0000 7213 0000 00da 1f76 616c 5f6f  ....r......val_o
-000008e0: 7574 7075 745f 315f 6d65 616e 5f73 7175  utput_1_mean_squ
-000008f0: 6172 6564 5f65 7272 6f72 2903 da06 6c6f  ared_error)...lo
-00000900: 6767 6572 da0a 6570 6f63 685f 7374 6570  gger..epoch_step
-00000910: da0a 6964 656e 7469 6669 6572 7201 0000  ..identifierr...
-00000920: 0029 06da 0a62 6174 6368 5f73 697a 65da  .)...batch_size.
-00000930: 0665 706f 6368 73da 0f76 616c 6964 6174  .epochs..validat
-00000940: 696f 6e5f 6461 7461 da0f 7661 6c69 6461  ion_data..valida
-00000950: 7469 6f6e 5f66 7265 71da 0963 616c 6c62  tion_freq..callb
-00000960: 6163 6b73 da07 7665 7262 6f73 6529 05da  acks..verbose)..
-00000970: 0366 6974 7242 0000 0072 0800 0000 724a  .fitrB...r....rJ
-00000980: 0000 00da 0768 6973 746f 7279 2907 7244  .....history).rD
-00000990: 0000 0072 4500 0000 da07 785f 7472 6169  ...rE.....x_trai
-000009a0: 6eda 0779 5f74 7261 696e da06 785f 7465  n..y_train..x_te
-000009b0: 7374 da06 795f 7465 7374 7254 0000 0072  st..y_testrT...r
-000009c0: 2400 0000 7224 0000 0072 2500 0000 7246  $...r$...r%...rF
-000009d0: 0000 0082 0000 0073 2000 0000 0402 0201  .......s .......
-000009e0: 0201 0801 0801 0601 0201 0202 0401 0201  ................
-000009f0: 0201 04fd 02ff 0207 06f2 0610 da0b 7175  ..............qu
-00000a00: 6572 795f 6d6f 6465 6cda 1369 6e63 6c75  ery_model..inclu
-00000a10: 6465 5f69 6d70 6f72 7461 6e63 6573 6305  de_importancesc.
-00000a20: 0000 0000 0000 0000 0000 0008 0000 0003  ................
-00000a30: 0000 0043 0000 0073 2a00 0000 7c00 a000  ...C...s*...|...
-00000a40: 6401 a101 0100 7c01 7c02 8301 5c03 7d05  d.....|.|...\.}.
-00000a50: 7d06 7d07 7c04 7213 7c05 7c06 7c07 6603  }.}.|.r.|.|.|.f.
-00000a60: 5300 7c05 5300 2902 4e7a 1571 7565 7279  S.|.S.).Nz.query
-00000a70: 696e 6720 7468 6520 6d6f 6465 6c2e 2e2e  ing the model...
-00000a80: 2901 7241 0000 0029 0872 4400 0000 7245  ).rA...).rD...rE
-00000a90: 0000 00da 0178 da01 7972 5a00 0000 da08  .....x..yrZ.....
-00000aa0: 6f75 745f 7072 6564 da07 6e69 5f70 7265  out_pred..ni_pre
-00000ab0: 64da 0765 695f 7072 6564 7224 0000 0072  d..ei_predr$...r
-00000ac0: 2400 0000 7225 0000 0072 5900 0000 9700  $...r%...rY.....
-00000ad0: 0000 730a 0000 000a 020e 0104 020a 0104  ..s.............
-00000ae0: 02da 1263 616c 6375 6c61 7465 5f66 6964  ...calculate_fid
-00000af0: 656c 6974 7963 0800 0000 0000 0000 0000  elityc..........
-00000b00: 0000 1500 0000 0a00 0000 4300 0000 733a  ..........C...s:
-00000b10: 0100 007c 0064 0119 007d 0874 0074 0183  ...|.d...}.t.t..
-00000b20: 0144 005d 597d 0967 007d 0a7c 0644 005d  .D.]Y}.g.}.|.D.]
-00000b30: 147d 0b74 02a0 037c 0ba1 017d 0c64 027c  .}.t...|...}.d.|
-00000b40: 0c64 0064 0085 027c 0966 023c 007c 0aa0  .d.d...|.f.<.|..
-00000b50: 047c 0ca1 0101 0071 0e74 057c 0a83 017d  .|.....q.t.|...}
-00000b60: 0d64 0364 0484 007c 017c 037c 0d64 058d  .d.d...|.|.|.d..
-00000b70: 0244 0083 015c 037d 0e7d 0f7d 0f74 067c  .D...\.}.}.}.t.|
-00000b80: 0283 0144 005d 275c 027d 107d 1174 077c  ...D.]'\.}.}.t.|
-00000b90: 057c 1019 0064 0219 0083 017c 0064 067c  .|...d.....|.d.|
-00000ba0: 089b 0064 077c 119b 009d 043c 0074 077c  ...d.|.....<.t.|
-00000bb0: 0e7c 1019 0064 0219 0083 017c 0064 087c  .|...d.....|.d.|
-00000bc0: 089b 0064 077c 119b 0064 077c 099b 009d  ...d.|...d.|....
-00000bd0: 063c 0071 3971 0867 007d 127c 0244 005d  .<.q9q.g.}.|.D.]
-00000be0: 347d 1164 027d 1374 0074 0183 0144 005d  4}.d.}.t.t...D.]
-00000bf0: 267d 097c 0064 067c 089b 0064 077c 119b  &}.|.d.|...d.|..
-00000c00: 009d 0419 007d 147c 0064 087c 089b 0064  .....}.|.d.|...d
-00000c10: 077c 119b 0064 077c 099b 009d 0619 007d  .|...d.|.......}
-00000c20: 0e7c 137c 006a 0864 0919 007c 0919 007c  .|.|.j.d...|...|
-00000c30: 147c 0e18 0014 0037 007d 1371 6e7c 12a0  .|.....7.}.qn|..
-00000c40: 047c 13a1 0101 0071 667c 1253 0029 0a4e  .|.....qf|.S.).N
-00000c50: da03 7265 7072 0100 0000 6301 0000 0000  ..repr....c.....
-00000c60: 0000 0000 0000 0002 0000 0004 0000 0053  ...............S
-00000c70: 0000 0073 1400 0000 6700 7c00 5d06 7d01  ...s....g.|.].}.
-00000c80: 7c01 a000 a100 9102 7102 5300 7224 0000  |.......q.S.r$..
-00000c90: 0029 01da 056e 756d 7079 2902 da02 2e30  .)...numpy)....0
-00000ca0: da01 7672 2400 0000 7224 0000 0072 2500  ..vr$...r$...r%.
-00000cb0: 0000 da0a 3c6c 6973 7463 6f6d 703e b400  ....<listcomp>..
-00000cc0: 0000 7302 0000 0014 007a 2663 616c 6375  ..s......z&calcu
-00000cd0: 6c61 7465 5f66 6964 656c 6974 792e 3c6c  late_fidelity.<l
-00000ce0: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
-00000cf0: 3e29 01da 156e 6f64 655f 696d 706f 7274  >)...node_import
-00000d00: 616e 6365 735f 6d61 736b 7a09 6f75 742f  ances_maskz.out/
-00000d10: 7072 6564 2ffa 012f 7a0b 6f75 742f 6d61  pred/../z.out/ma
-00000d20: 736b 6564 2fda 1243 4841 4e4e 454c 5f44  sked/..CHANNEL_D
-00000d30: 4952 4543 5449 4f4e 5329 09da 0572 616e  IRECTIONS)...ran
-00000d40: 6765 7216 0000 00da 026e 70da 096f 6e65  ger......np..one
-00000d50: 735f 6c69 6b65 da06 6170 7065 6e64 7204  s_like..appendr.
-00000d60: 0000 00da 0965 6e75 6d65 7261 7465 da05  .....enumerate..
-00000d70: 666c 6f61 7472 4200 0000 2915 7244 0000  floatrB...).rD..
-00000d80: 0072 4500 0000 da0c 696e 6469 6365 735f  .rE.....indices_
-00000d90: 7472 7565 da06 785f 7472 7565 da06 795f  true..x_true..y_
-00000da0: 7472 7565 725d 0000 0072 5e00 0000 725f  truer]...r^...r_
-00000db0: 0000 0072 6100 0000 da01 6bda 056d 6173  ...ra.....k..mas
-00000dc0: 6b73 da02 6e69 da04 6d61 736b da0c 6d61  ks..ni..mask..ma
-00000dd0: 736b 735f 7465 6e73 6f72 da0a 6f75 745f  sks_tensor..out_
-00000de0: 6d61 736b 6564 da01 5fda 0163 da05 696e  masked.._..c..in
-00000df0: 6465 78da 0a66 6964 656c 6974 6965 73da  dex..fidelities.
-00000e00: 0866 6964 656c 6974 79da 036f 7574 7224  .fidelity..outr$
-00000e10: 0000 0072 2400 0000 7225 0000 0072 6000  ...r$...r%...r`.
-00000e20: 0000 a200 0000 7330 0000 0008 020c 0704  ......s0........
-00000e30: 0208 010a 0110 010c 0108 0206 010a 010c  ................
-00000e40: ff10 0320 0128 0102 fe04 0408 0104 020c  ... .(..........
-00000e50: 0114 011a 011c 010c 0204 0229 0154 2942  ...........).T)B
-00000e60: da02 6f73 da07 7061 7468 6c69 62da 0674  ..os..pathlib..t
-00000e70: 7970 696e 67da 0174 da0a 7465 6e73 6f72  yping..t..tensor
-00000e80: 666c 6f77 da02 7466 da10 7465 6e73 6f72  flow..tf..tensor
-00000e90: 666c 6f77 2e6b 6572 6173 da05 6b65 7261  flow.keras..kera
-00000ea0: 7372 2100 0000 7262 0000 0072 6a00 0000  sr!...rb...rj...
-00000eb0: da0c 7079 636f 6d65 782e 7574 696c 7202  ..pycomex.utilr.
-00000ec0: 0000 00da 1270 7963 6f6d 6578 2e65 7870  .....pycomex.exp
-00000ed0: 6572 696d 656e 7472 0300 0000 da10 6b67  erimentr......kg
-00000ee0: 636e 6e2e 6461 7461 2e75 7469 6c73 7204  cnn.data.utilsr.
-00000ef0: 0000 00da 1e67 7261 7068 5f61 7474 656e  .....graph_atten
-00000f00: 7469 6f6e 5f73 7475 6465 6e74 2e6d 6f64  tion_student.mod
-00000f10: 656c 7372 0500 0000 da20 6772 6170 685f  elsr..... graph_
-00000f20: 6174 7465 6e74 696f 6e5f 7374 7564 656e  attention_studen
-00000f30: 742e 7472 6169 6e69 6e67 7206 0000 0072  t.trainingr....r
-00000f40: 0700 0000 7208 0000 0072 0a00 0000 da08  ....r....r......
-00000f50: 4f70 7469 6f6e 616c da03 7374 72da 0f5f  Optional..str.._
-00000f60: 5f61 6e6e 6f74 6174 696f 6e73 5f5f 720c  _annotations__r.
-00000f70: 0000 0072 0e00 0000 7210 0000 00da 044c  ...r....r......L
-00000f80: 6973 74da 0369 6e74 7211 0000 0072 6e00  ist..intr....rn.
-00000f90: 0000 7212 0000 0072 1400 0000 7216 0000  ..r....r....r...
-00000fa0: 0072 1700 0000 7218 0000 00da 0462 6f6f  .r....r......boo
-00000fb0: 6c72 2a00 0000 722b 0000 0072 6800 0000  lr*...r+...rh...
-00000fc0: 722c 0000 0072 2d00 0000 7248 0000 0072  r,...r-...rH...r
-00000fd0: 3b00 0000 da19 494d 504f 5254 414e 4345  ;.....IMPORTANCE
-00000fe0: 5f43 4841 4e4e 454c 5f4c 4142 454c 53da  _CHANNEL_LABELS.
-00000ff0: 0450 6174 68da 085f 5f66 696c 655f 5fda  .Path..__file__.
-00001000: 0670 6172 656e 74da 0861 6273 6f6c 7574  .parent..absolut
-00001010: 65da 0450 4154 48da 0470 6174 68da 046a  e..PATH..path..j
-00001020: 6f69 6eda 0f45 5850 4552 494d 454e 545f  oin..EXPERIMENT_
-00001030: 5041 5448 da09 4241 5345 5f50 4154 48da  PATH..BASE_PATH.
-00001040: 094e 414d 4553 5041 4345 da05 4445 4255  .NAMESPACE..DEBU
-00001050: 47da 0767 6c6f 6261 6c73 da02 7365 da04  G..globals..se..
-00001060: 686f 6f6b 7229 0000 0072 4600 0000 7259  hookr)...rF...rY
-00001070: 0000 0072 6000 0000 7224 0000 0072 2400  ...r`...r$...r$.
-00001080: 0000 7224 0000 0072 2500 0000 da08 3c6d  ..r$...r%.....<m
-00001090: 6f64 756c 653e 0100 0000 735e 0000 000a  odule>....s^....
-000010a0: 0008 0108 0108 020c 0108 010c 010c 010c  ................
-000010b0: 010c 0210 010c 0112 0612 010c 0616 040c  ................
-000010c0: 040c 050c 030c 060c 040c 0404 060a 0102  ................
-000010d0: 0302 0106 fe08 0904 0304 0308 0108 0410  ................
-000010e0: 040e 0104 0104 0104 011e 0108 020a 0108  ................
-000010f0: 200a 0108 1412 0108 0a0c 0152 bc          ..........R.
+00000020: 0009 0000 0040 0000 0073 4c02 0000 5500  .....@...sL...U.
+00000030: 6400 5a00 6401 6402 6c01 5a01 6401 6402  d.Z.d.d.l.Z.d.d.
+00000040: 6c02 5a02 6401 6402 6c03 5a04 6401 6402  l.Z.d.d.l.Z.d.d.
+00000050: 6c05 5a06 6401 6402 6c07 6d08 5a09 0100  l.Z.d.d.l.m.Z...
+00000060: 6401 6402 6c0a 5a0b 6401 6403 6c0c 6d0d  d.d.l.Z.d.d.l.m.
+00000070: 5a0d 0100 6401 6404 6c0e 6d0f 5a0f 0100  Z...d.d.l.m.Z...
+00000080: 6401 6405 6c10 6d11 5a11 0100 6401 6406  d.d.l.m.Z...d.d.
+00000090: 6c12 6d13 5a13 0100 6401 6407 6c14 6d15  l.m.Z...d.d.l.m.
+000000a0: 5a15 6d16 5a16 0100 6401 6408 6c14 6d17  Z.m.Z...d.d.l.m.
+000000b0: 5a17 0100 6409 5a18 6504 6a19 651a 1900  Z...d.Z.e.j.e...
+000000c0: 651b 640a 3c00 640b 5a1c 6504 6a19 651a  e.d.<.d.Z.e.j.e.
+000000d0: 1900 651b 640c 3c00 640d 5a1d 651a 651b  ..e.d.<.d.Z.e.e.
+000000e0: 640e 3c00 6700 640f a201 5a1e 6504 6a1f  d.<.g.d...Z.e.j.
+000000f0: 6520 1900 651b 6410 3c00 6411 5a21 6522  e ..e.d.<.d.Z!e"
+00000100: 651b 6412 3c00 6413 5a23 6522 651b 6414  e.d.<.d.Z#e"e.d.
+00000110: 3c00 6415 5a24 6522 651b 6416 3c00 6417  <.d.Z$e"e.d.<.d.
+00000120: 5a25 6520 651b 6418 3c00 6419 5a26 6522  Z%e e.d.<.d.Z&e"
+00000130: 651b 641a 3c00 641b 5a27 6528 651b 641c  e.d.<.d.Z'e(e.d.
+00000140: 3c00 6401 5a29 641d 641e 6702 6701 5a2a  <.d.Z)d.d.g.g.Z*
+00000150: 641f 6420 6421 9c02 5a2b 6700 6422 a201  d.d d!..Z+g.d"..
+00000160: 5a2c 6411 5a2d 6423 5a2e 6424 6425 8400  Z,d.Z-d#Z.d$d%..
+00000170: 5a2f 6426 6427 6702 5a30 6502 a031 6532  Z/d&d'g.Z0e..1e2
+00000180: a101 6a33 a034 a100 5a35 6501 6a36 a037  ..j3.4..Z5e.j6.7
+00000190: 6535 6428 a102 5a38 6535 5a39 6429 5a3a  e5d(..Z8e5Z9d)Z:
+000001a0: 642a 5a3b 650d 8300 8f5d 0100 650f 6538  d*Z;e....]..e.e8
+000001b0: 6539 653a 653c 8300 8304 0400 5a3d 8f39  e9e:e<......Z=.9
+000001c0: 0100 653d a03e 642b a101 642c 642b 8400  ..e=.>d+..d,d+..
+000001d0: 8301 5a3f 653d a03e 642d a101 642e 642d  ..Z?e=.>d-..d.d-
+000001e0: 8400 8301 5a40 653d a03e 642f a101 6436  ....Z@e=.>d/..d6
+000001f0: 6430 6528 6602 6431 642f 8405 8301 5a41  d0e(f.d1d/....ZA
+00000200: 653d a03e 6432 a101 6433 6432 8400 8301  e=.>d2..d3d2....
+00000210: 5a42 653d a03e 6434 a101 6435 6434 8400  ZBe=.>d4..d5d4..
+00000220: 8301 5a43 5700 6402 0400 0400 8303 0100  ..ZCW.d.........
+00000230: 6e11 3100 9001 7306 7701 0100 0100 0100  n.1...s.w.......
+00000240: 5900 0100 5700 6402 0400 0400 8303 0100  Y...W.d.........
+00000250: 6402 5300 5700 6402 0400 0400 8303 0100  d.S.W.d.........
+00000260: 6402 5300 3100 9001 731f 7701 0100 0100  d.S.1...s.w.....
+00000270: 0100 5900 0100 6402 5300 2937 7a13 0a0a  ..Y...d.S.)7z...
+00000280: 4348 414e 4745 4c4f 470a 0a30 2e31 2e30  CHANGELOG..0.1.0
+00000290: 0ae9 0000 0000 4e29 01da 0953 6b69 7070  ......N)...Skipp
+000002a0: 6162 6c65 2901 da0d 5375 6245 7870 6572  able)...SubExper
+000002b0: 696d 656e 7429 01da 1f72 6167 6765 645f  iment)...ragged_
+000002c0: 7465 6e73 6f72 5f66 726f 6d5f 6e65 7374  tensor_from_nest
+000002d0: 6564 5f6e 756d 7079 2901 da05 4d65 6761  ed_numpy)...Mega
+000002e0: 6e29 02da 064e 6f4c 6f73 73da 036d 7365  n)...NoLoss..mse
+000002f0: 2901 da13 4c6f 6750 726f 6772 6573 7343  )...LogProgressC
+00000300: 616c 6c62 6163 6bda 126e 6f64 655f 696d  allback..node_im
+00000310: 706f 7274 616e 6365 735f 32da 144e 4f44  portances_2..NOD
+00000320: 455f 494d 504f 5254 414e 4345 535f 4b45  E_IMPORTANCES_KE
+00000330: 59da 1265 6467 655f 696d 706f 7274 616e  Y..edge_importan
+00000340: 6365 735f 32da 1445 4447 455f 494d 504f  ces_2..EDGE_IMPO
+00000350: 5254 414e 4345 535f 4b45 59da 054d 4547  RTANCES_KEY..MEG
+00000360: 414e da0a 4d4f 4445 4c5f 4e41 4d45 2903  AN..MODEL_NAME).
+00000370: e920 0000 0072 0f00 0000 720f 0000 00da  . ...r....r.....
+00000380: 0555 4e49 5453 6700 0000 0000 0000 00da  .UNITSg.........
+00000390: 0c44 524f 504f 5554 5f52 4154 4567 0000  .DROPOUT_RATEg..
+000003a0: 0000 0000 f03f da11 494d 504f 5254 414e  .....?..IMPORTAN
+000003b0: 4345 5f46 4143 544f 52e9 0500 0000 da15  CE_FACTOR.......
+000003c0: 494d 504f 5254 414e 4345 5f4d 554c 5449  IMPORTANCE_MULTI
+000003d0: 504c 4945 52e9 0200 0000 da13 494d 504f  PLIER.......IMPO
+000003e0: 5254 414e 4345 5f43 4841 4e4e 454c 5367  RTANCE_CHANNELSg
+000003f0: 0000 0000 0000 1440 da0f 5350 4152 5349  .......@..SPARSI
+00000400: 5459 5f46 4143 544f 5246 da0c 434f 4e43  TY_FACTORF..CONC
+00000410: 4154 5f48 4541 4453 e9fd ffff ffe9 0300  AT_HEADS........
+00000420: 0000 e9ff ffff ffe9 0100 0000 2902 7201  ............).r.
+00000430: 0000 0072 1c00 0000 2903 e93c 0000 00e9  ...r....)..<....
+00000440: 1400 0000 721c 0000 00e9 fa00 0000 6300  ....r.........c.
+00000450: 0000 0000 0000 0000 0000 0000 0000 0003  ................
+00000460: 0000 0043 0000 0073 0e00 0000 7400 6a01  ...C...s....t.j.
+00000470: 6a02 6401 6402 8d01 5300 2903 4e67 7b14  j.d.d...S.).Ng{.
+00000480: ae47 e17a 843f 2901 da0d 6c65 6172 6e69  .G.z.?)...learni
+00000490: 6e67 5f72 6174 6529 03da 026b 73da 0a6f  ng_rate)...ks..o
+000004a0: 7074 696d 697a 6572 73da 054e 6164 616d  ptimizers..Nadam
+000004b0: a900 7224 0000 0072 2400 0000 fa66 2f6d  ..r$...r$....f/m
+000004c0: 6564 6961 2f73 7364 2f50 726f 6772 616d  edia/ssd/Program
+000004d0: 6d69 6e67 2f67 7261 7068 5f61 7474 656e  ming/graph_atten
+000004e0: 7469 6f6e 5f73 7475 6465 6e74 2f67 7261  tion_student/gra
+000004f0: 7068 5f61 7474 656e 7469 6f6e 5f73 7475  ph_attention_stu
+00000500: 6465 6e74 2f65 7870 6572 696d 656e 7473  dent/experiments
+00000510: 2f76 6764 5f73 696e 676c 655f 6d65 6761  /vgd_single_mega
+00000520: 6e2e 7079 da08 3c6c 616d 6264 613e 5800  n.py..<lambda>X.
+00000530: 0000 7302 0000 000e 0072 2600 0000 da08  ..s......r&.....
+00000540: 6e65 6761 7469 7665 da08 706f 7369 7469  negative..positi
+00000550: 7665 7a0d 7667 645f 7369 6e67 6c65 2e70  vez.vgd_single.p
+00000560: 797a 1872 6573 756c 7473 2f76 6764 5f73  yz.results/vgd_s
+00000570: 696e 676c 655f 6d65 6761 6e54 da0c 6372  ingle_meganT..cr
+00000580: 6561 7465 5f6d 6f64 656c 6301 0000 0000  eate_modelc.....
+00000590: 0000 0000 0000 0002 0000 000f 0000 0043  ...............C
+000005a0: 0000 0073 b400 0000 7c00 a000 6401 a101  ...s....|...d...
+000005b0: 0100 7c00 a000 6402 7c00 6a01 6403 1900  ..|...d.|.j.d...
+000005c0: 9b00 9d02 a101 0100 7402 7c00 6a01 6404  ........t.|.j.d.
+000005d0: 1900 7c00 6a01 6405 1900 7c00 6a01 6406  ..|.j.d...|.j.d.
+000005e0: 1900 7c00 6a01 6407 1900 7c00 6a01 6408  ..|.j.d...|.j.d.
+000005f0: 1900 7c00 6a01 6403 1900 7c00 6a01 6409  ..|.j.d...|.j.d.
+00000600: 1900 7c00 6a01 640a 1900 7c00 6a01 640b  ..|.j.d...|.j.d.
+00000610: 1900 7c00 6a01 640c 1900 640d 640e 7c00  ..|.j.d...d.d.|.
+00000620: 6a01 640f 1900 6410 8d0d 7d01 7c01 6a03  j.d...d...}.|.j.
+00000630: 7404 7405 8300 7405 8300 6703 6700 6411  t.t...t...g.g.d.
+00000640: a201 7404 6701 7c00 6a01 6412 1900 8300  ..t.g.|.j.d.....
+00000650: 640d 6413 8d05 0100 7c01 5300 2914 4e72  d.d.....|.S.).Nr
+00000660: 0d00 0000 7a14 202a 2053 5041 5253 4954  ....z. * SPARSIT
+00000670: 595f 4641 4354 4f52 3a20 7217 0000 0072  Y_FACTOR: r....r
+00000680: 1000 0000 7211 0000 0072 1200 0000 7214  ....r....r....r.
+00000690: 0000 0072 1600 0000 da14 5245 4752 4553  ...r......REGRES
+000006a0: 5349 4f4e 5f52 4546 4552 454e 4345 da11  SION_REFERENCE..
+000006b0: 5245 4752 4553 5349 4f4e 5f4c 494d 4954  REGRESSION_LIMIT
+000006c0: 53da 0b46 494e 414c 5f55 4e49 5453 da0d  S..FINAL_UNITS..
+000006d0: 4649 4e41 4c5f 4452 4f50 4f55 5446 5472  FINAL_DROPOUTFTr
+000006e0: 1800 0000 290d da05 756e 6974 73da 0c64  ....)...units..d
+000006f0: 726f 706f 7574 5f72 6174 65da 1169 6d70  ropout_rate..imp
+00000700: 6f72 7461 6e63 655f 6661 6374 6f72 da15  ortance_factor..
+00000710: 696d 706f 7274 616e 6365 5f6d 756c 7469  importance_multi
+00000720: 706c 6965 72da 1369 6d70 6f72 7461 6e63  plier..importanc
+00000730: 655f 6368 616e 6e65 6c73 da0f 7370 6172  e_channels..spar
+00000740: 7369 7479 5f66 6163 746f 72da 1472 6567  sity_factor..reg
+00000750: 7265 7373 696f 6e5f 7265 6665 7265 6e63  ression_referenc
+00000760: 65da 1172 6567 7265 7373 696f 6e5f 6c69  e..regression_li
+00000770: 6d69 7473 da0b 6669 6e61 6c5f 756e 6974  mits..final_unit
+00000780: 73da 1266 696e 616c 5f64 726f 706f 7574  s..final_dropout
+00000790: 5f72 6174 65da 1475 7365 5f67 7261 7068  _rate..use_graph
+000007a0: 5f61 7474 7269 6275 7465 73da 1175 7365  _attributes..use
+000007b0: 5f65 6467 655f 6665 6174 7572 6573 da0c  _edge_features..
+000007c0: 636f 6e63 6174 5f68 6561 6473 2903 721c  concat_heads).r.
+000007d0: 0000 0072 0100 0000 7201 0000 00da 0c4f  ...r....r......O
+000007e0: 5054 494d 495a 4552 5f43 4229 05da 046c  PTIMIZER_CB)...l
+000007f0: 6f73 73da 0c6c 6f73 735f 7765 6967 6874  oss..loss_weight
+00000800: 73da 076d 6574 7269 6373 da09 6f70 7469  s..metrics..opti
+00000810: 6d69 7a65 72da 0b72 756e 5f65 6167 6572  mizer..run_eager
+00000820: 6c79 2906 da04 696e 666f da0a 7061 7261  ly)...info..para
+00000830: 6d65 7465 7273 7205 0000 00da 0763 6f6d  metersr......com
+00000840: 7069 6c65 7207 0000 0072 0600 0000 2902  piler....r....).
+00000850: da01 65da 056d 6f64 656c 7224 0000 0072  ..e..modelr$...r
+00000860: 2400 0000 7225 0000 0072 2900 0000 6700  $...r%...r)...g.
+00000870: 0000 7338 0000 000a 0216 0102 0108 0108  ..s8............
+00000880: 0108 0108 0108 0108 0108 0108 0108 0108  ................
+00000890: 0102 0102 0108 0106 f304 0f02 0204 0104  ................
+000008a0: 0102 fd06 0504 030a 0102 0106 f504 0dda  ................
+000008b0: 0966 6974 5f6d 6f64 656c 6306 0000 0000  .fit_modelc.....
+000008c0: 0000 0000 0000 0007 0000 000c 0000 0043  ...............C
+000008d0: 0000 0073 3e00 0000 7c01 6a00 7c02 7c03  ...s>...|.j.|.|.
+000008e0: 7c00 6a01 6401 1900 7c00 6a01 6402 1900  |.j.d...|.j.d...
+000008f0: 7c04 7c05 6602 6403 7402 7c00 6a03 6404  |.|.f.d.t.|.j.d.
+00000900: 6405 6406 8d03 6701 6407 6408 8d08 7d06  d.d...g.d.d...}.
+00000910: 7c06 6a04 5300 2909 4eda 0a42 4154 4348  |.j.S.).N..BATCH
+00000920: 5f53 495a 45da 0645 504f 4348 5372 1c00  _SIZE..EPOCHSr..
+00000930: 0000 7213 0000 00da 1f76 616c 5f6f 7574  ..r......val_out
+00000940: 7075 745f 315f 6d65 616e 5f73 7175 6172  put_1_mean_squar
+00000950: 6564 5f65 7272 6f72 2903 da06 6c6f 6767  ed_error)...logg
+00000960: 6572 da0a 6570 6f63 685f 7374 6570 da0a  er..epoch_step..
+00000970: 6964 656e 7469 6669 6572 7201 0000 0029  identifierr....)
+00000980: 06da 0a62 6174 6368 5f73 697a 65da 0665  ...batch_size..e
+00000990: 706f 6368 73da 0f76 616c 6964 6174 696f  pochs..validatio
+000009a0: 6e5f 6461 7461 da0f 7661 6c69 6461 7469  n_data..validati
+000009b0: 6f6e 5f66 7265 71da 0963 616c 6c62 6163  on_freq..callbac
+000009c0: 6b73 da07 7665 7262 6f73 6529 05da 0366  ks..verbose)...f
+000009d0: 6974 7242 0000 0072 0800 0000 724a 0000  itrB...r....rJ..
+000009e0: 00da 0768 6973 746f 7279 2907 7244 0000  ...history).rD..
+000009f0: 0072 4500 0000 da07 785f 7472 6169 6eda  .rE.....x_train.
+00000a00: 0779 5f74 7261 696e da06 785f 7465 7374  .y_train..x_test
+00000a10: da06 795f 7465 7374 7254 0000 0072 2400  ..y_testrT...r$.
+00000a20: 0000 7224 0000 0072 2500 0000 7246 0000  ..r$...r%...rF..
+00000a30: 0089 0000 0073 2000 0000 0402 0201 0201  .....s .........
+00000a40: 0801 0801 0601 0201 0202 0401 0201 0201  ................
+00000a50: 04fd 02ff 0207 06f2 0610 da0b 7175 6572  ............quer
+00000a60: 795f 6d6f 6465 6cda 1369 6e63 6c75 6465  y_model..include
+00000a70: 5f69 6d70 6f72 7461 6e63 6573 6305 0000  _importancesc...
+00000a80: 0000 0000 0000 0000 0008 0000 0003 0000  ................
+00000a90: 0043 0000 0073 2a00 0000 7c00 a000 6401  .C...s*...|...d.
+00000aa0: a101 0100 7c01 7c02 8301 5c03 7d05 7d06  ....|.|...\.}.}.
+00000ab0: 7d07 7c04 7213 7c05 7c06 7c07 6603 5300  }.|.r.|.|.|.f.S.
+00000ac0: 7c05 5300 2902 4e7a 1571 7565 7279 696e  |.S.).Nz.queryin
+00000ad0: 6720 7468 6520 6d6f 6465 6c2e 2e2e 2901  g the model...).
+00000ae0: 7241 0000 0029 0872 4400 0000 7245 0000  rA...).rD...rE..
+00000af0: 00da 0178 da01 7972 5a00 0000 da08 6f75  ...x..yrZ.....ou
+00000b00: 745f 7072 6564 da07 6e69 5f70 7265 64da  t_pred..ni_pred.
+00000b10: 0765 695f 7072 6564 7224 0000 0072 2400  .ei_predr$...r$.
+00000b20: 0000 7225 0000 0072 5900 0000 9e00 0000  ..r%...rY.......
+00000b30: 730a 0000 000a 020e 0104 020a 0104 02da  s...............
+00000b40: 1263 616c 6375 6c61 7465 5f66 6964 656c  .calculate_fidel
+00000b50: 6974 7963 0800 0000 0000 0000 0000 0000  ityc............
+00000b60: 1500 0000 0a00 0000 4300 0000 7358 0100  ........C...sX..
+00000b70: 007c 0064 0119 007d 087c 006a 0064 0219  .|.d...}.|.j.d..
+00000b80: 0074 017c 006a 0064 0319 0083 016b 0372  .t.|.j.d.....k.r
+00000b90: 1364 0467 0153 0074 0274 0383 0144 005d  .d.g.S.t.t...D.]
+00000ba0: 597d 0967 007d 0a7c 0644 005d 147d 0b74  Y}.g.}.|.D.].}.t
+00000bb0: 04a0 057c 0ba1 017d 0c64 047c 0c64 0064  ...|...}.d.|.d.d
+00000bc0: 0085 027c 0966 023c 007c 0aa0 067c 0ca1  ...|.f.<.|...|..
+00000bd0: 0101 0071 1d74 077c 0a83 017d 0d64 0564  ...q.t.|...}.d.d
+00000be0: 0684 007c 017c 037c 0d64 078d 0244 0083  ...|.|.|.d...D..
+00000bf0: 015c 037d 0e7d 0f7d 0f74 087c 0283 0144  .\.}.}.}.t.|...D
+00000c00: 005d 275c 027d 107d 1174 097c 057c 1019  .]'\.}.}.t.|.|..
+00000c10: 0064 0419 0083 017c 0064 087c 089b 0064  .d.....|.d.|...d
+00000c20: 097c 119b 009d 043c 0074 097c 0e7c 1019  .|.....<.t.|.|..
+00000c30: 0064 0419 0083 017c 0064 0a7c 089b 0064  .d.....|.d.|...d
+00000c40: 097c 119b 0064 097c 099b 009d 063c 0071  .|...d.|.....<.q
+00000c50: 4871 1767 007d 127c 0244 005d 347d 1164  Hq.g.}.|.D.]4}.d
+00000c60: 047d 1374 0274 0383 0144 005d 267d 097c  .}.t.t...D.]&}.|
+00000c70: 0064 087c 089b 0064 097c 119b 009d 0419  .d.|...d.|......
+00000c80: 007d 147c 0064 0a7c 089b 0064 097c 119b  .}.|.d.|...d.|..
+00000c90: 0064 097c 099b 009d 0619 007d 0e7c 137c  .d.|.......}.|.|
+00000ca0: 006a 0a64 0319 007c 0919 007c 147c 0e18  .j.d...|...|.|..
+00000cb0: 0014 0037 007d 1371 7d7c 12a0 067c 13a1  ...7.}.q}|...|..
+00000cc0: 0101 0071 757c 1253 0029 0b4e da03 7265  ...qu|.S.).N..re
+00000cd0: 7072 1600 0000 da12 4348 414e 4e45 4c5f  pr......CHANNEL_
+00000ce0: 4449 5245 4354 494f 4e53 7201 0000 0063  DIRECTIONSr....c
+00000cf0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00000d00: 0400 0000 5300 0000 7314 0000 0067 007c  ....S...s....g.|
+00000d10: 005d 067d 017c 01a0 00a1 0091 0271 0253  .].}.|.......q.S
+00000d20: 0072 2400 0000 2901 da05 6e75 6d70 7929  .r$...)...numpy)
+00000d30: 02da 022e 30da 0176 7224 0000 0072 2400  ....0..vr$...r$.
+00000d40: 0000 7225 0000 00da 0a3c 6c69 7374 636f  ..r%.....<listco
+00000d50: 6d70 3ebe 0000 0073 0200 0000 1400 7a26  mp>....s......z&
+00000d60: 6361 6c63 756c 6174 655f 6669 6465 6c69  calculate_fideli
+00000d70: 7479 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973  ty.<locals>.<lis
+00000d80: 7463 6f6d 703e 2901 da15 6e6f 6465 5f69  tcomp>)...node_i
+00000d90: 6d70 6f72 7461 6e63 6573 5f6d 6173 6b7a  mportances_maskz
+00000da0: 096f 7574 2f70 7265 642f fa01 2f7a 0b6f  .out/pred/../z.o
+00000db0: 7574 2f6d 6173 6b65 642f 290b da01 70da  ut/masked/)...p.
+00000dc0: 036c 656e da05 7261 6e67 6572 1600 0000  .len..ranger....
+00000dd0: da02 6e70 da09 6f6e 6573 5f6c 696b 65da  ..np..ones_like.
+00000de0: 0661 7070 656e 6472 0400 0000 da09 656e  .appendr......en
+00000df0: 756d 6572 6174 65da 0566 6c6f 6174 7242  umerate..floatrB
+00000e00: 0000 0029 1572 4400 0000 7245 0000 00da  ...).rD...rE....
+00000e10: 0c69 6e64 6963 6573 5f74 7275 65da 0678  .indices_true..x
+00000e20: 5f74 7275 65da 0679 5f74 7275 6572 5d00  _true..y_truer].
+00000e30: 0000 725e 0000 0072 5f00 0000 7261 0000  ..r^...r_...ra..
+00000e40: 00da 016b da05 6d61 736b 73da 026e 69da  ...k..masks..ni.
+00000e50: 046d 6173 6bda 0c6d 6173 6b73 5f74 656e  .mask..masks_ten
+00000e60: 736f 72da 0a6f 7574 5f6d 6173 6b65 64da  sor..out_masked.
+00000e70: 015f da01 63da 0569 6e64 6578 da0a 6669  ._..c..index..fi
+00000e80: 6465 6c69 7469 6573 da08 6669 6465 6c69  delities..fideli
+00000e90: 7479 da03 6f75 7472 2400 0000 7224 0000  ty..outr$...r$..
+00000ea0: 0072 2500 0000 7260 0000 00a9 0000 0073  .r%...r`.......s
+00000eb0: 3400 0000 0802 1802 0601 0c07 0402 0801  4...............
+00000ec0: 0a01 1001 0c01 0802 0601 0a01 0cff 1003  ................
+00000ed0: 2001 2801 02fe 0404 0801 0402 0c01 1401   .(.............
+00000ee0: 1a01 1c01 0c02 0402 da0a 7361 7665 5f6d  ..........save_m
+00000ef0: 6f64 656c 6302 0000 0000 0000 0000 0000  odelc...........
+00000f00: 0003 0000 0004 0000 0043 0000 0073 3000  .........C...s0.
+00000f10: 0000 7c00 a000 6401 a101 0100 7401 6a02  ..|...d.....t.j.
+00000f20: a003 7c00 6a02 6402 a102 7d02 7c02 7c00  ..|.j.d...}.|.|.
+00000f30: 6403 3c00 7c01 a004 7c02 a101 0100 6400  d.<.|...|.....d.
+00000f40: 5300 2904 4e7a 1973 6176 696e 6720 7468  S.).Nz.saving th
+00000f50: 6520 4d45 4741 4e20 6d6f 6465 6c2e 2e2e  e MEGAN model...
+00000f60: 7245 0000 00da 0a6d 6f64 656c 5f70 6174  rE.....model_pat
+00000f70: 6829 0572 4100 0000 da02 6f73 da04 7061  h).rA.....os..pa
+00000f80: 7468 da04 6a6f 696e da04 7361 7665 2903  th..join..save).
+00000f90: 7244 0000 0072 4500 0000 7281 0000 0072  rD...rE...r....r
+00000fa0: 2400 0000 7224 0000 0072 2500 0000 7280  $...r$...r%...r.
+00000fb0: 0000 00d2 0000 0073 0800 0000 0a02 1001  .......s........
+00000fc0: 0801 0e01 2901 5429 44da 075f 5f64 6f63  ....).T)D..__doc
+00000fd0: 5f5f 7282 0000 00da 0770 6174 686c 6962  __r......pathlib
+00000fe0: da06 7479 7069 6e67 da01 74da 0a74 656e  ..typing..t..ten
+00000ff0: 736f 7266 6c6f 77da 0274 66da 1074 656e  sorflow..tf..ten
+00001000: 736f 7266 6c6f 772e 6b65 7261 73da 056b  sorflow.keras..k
+00001010: 6572 6173 7221 0000 0072 6300 0000 726c  erasr!...rc...rl
+00001020: 0000 00da 0c70 7963 6f6d 6578 2e75 7469  .....pycomex.uti
+00001030: 6c72 0200 0000 da12 7079 636f 6d65 782e  lr......pycomex.
+00001040: 6578 7065 7269 6d65 6e74 7203 0000 00da  experimentr.....
+00001050: 106b 6763 6e6e 2e64 6174 612e 7574 696c  .kgcnn.data.util
+00001060: 7372 0400 0000 da1e 6772 6170 685f 6174  sr......graph_at
+00001070: 7465 6e74 696f 6e5f 7374 7564 656e 742e  tention_student.
+00001080: 6d6f 6465 6c73 7205 0000 00da 2067 7261  modelsr..... gra
+00001090: 7068 5f61 7474 656e 7469 6f6e 5f73 7475  ph_attention_stu
+000010a0: 6465 6e74 2e74 7261 696e 696e 6772 0600  dent.trainingr..
+000010b0: 0000 7207 0000 0072 0800 0000 720a 0000  ..r....r....r...
+000010c0: 00da 084f 7074 696f 6e61 6cda 0373 7472  ...Optional..str
+000010d0: da0f 5f5f 616e 6e6f 7461 7469 6f6e 735f  ..__annotations_
+000010e0: 5f72 0c00 0000 720e 0000 0072 1000 0000  _r....r....r....
+000010f0: da04 4c69 7374 da03 696e 7472 1100 0000  ..List..intr....
+00001100: 7270 0000 0072 1200 0000 7214 0000 0072  rp...r....r....r
+00001110: 1600 0000 7217 0000 0072 1800 0000 da04  ....r....r......
+00001120: 626f 6f6c 722a 0000 0072 2b00 0000 7262  boolr*...r+...rb
+00001130: 0000 0072 2c00 0000 722d 0000 0072 4800  ...r,...r-...rH.
+00001140: 0000 723b 0000 00da 1949 4d50 4f52 5441  ..r;.....IMPORTA
+00001150: 4e43 455f 4348 414e 4e45 4c5f 4c41 4245  NCE_CHANNEL_LABE
+00001160: 4c53 da04 5061 7468 da08 5f5f 6669 6c65  LS..Path..__file
+00001170: 5f5f da06 7061 7265 6e74 da08 6162 736f  __..parent..abso
+00001180: 6c75 7465 da04 5041 5448 7283 0000 0072  lute..PATHr....r
+00001190: 8400 0000 da0f 4558 5045 5249 4d45 4e54  ......EXPERIMENT
+000011a0: 5f50 4154 48da 0942 4153 455f 5041 5448  _PATH..BASE_PATH
+000011b0: da09 4e41 4d45 5350 4143 45da 0544 4542  ..NAMESPACE..DEB
+000011c0: 5547 da07 676c 6f62 616c 73da 0273 65da  UG..globals..se.
+000011d0: 0468 6f6f 6b72 2900 0000 7246 0000 0072  .hookr)...rF...r
+000011e0: 5900 0000 7260 0000 0072 8000 0000 7224  Y...r`...r....r$
+000011f0: 0000 0072 2400 0000 7224 0000 0072 2500  ...r$...r$...r%.
+00001200: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+00001210: 7364 0000 0006 0008 0608 0108 0108 020c  sd..............
+00001220: 0108 010c 010c 010c 010c 0210 010c 0112  ................
+00001230: 0612 010c 0616 040c 040c 050c 030c 060c  ................
+00001240: 040c 0404 060a 0102 0302 0106 fe08 0904  ................
+00001250: 0304 0308 0108 0410 040e 0104 0104 0104  ................
+00001260: 011e 0108 020a 0108 210a 0108 1412 0108  ........!.......
+00001270: 0a0a 0108 280c 0154 92                   ....(..T.
```

### Comparing `graph_attention_student-0.7.0/graph_attention_student/experiments/__pycache__/vgd_single_megan_aqsoldb.cpython-310.pyc` & `graph_attention_student-0.7.1/graph_attention_student/experiments/__pycache__/vgd_single_megan_aqsoldb.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.0/graph_attention_student/experiments/process_aqsoldb.py` & `graph_attention_student-0.7.1/graph_attention_student/experiments/process_aqsoldb.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.0/graph_attention_student/experiments/rb_motifs_multi.py` & `graph_attention_student-0.7.1/graph_attention_student/experiments/rb_motifs_multi.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.0/graph_attention_student/experiments/rb_motifs_single.py` & `graph_attention_student-0.7.1/graph_attention_student/experiments/rb_motifs_single.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.0/graph_attention_student/experiments/vgd_regression_posthoc.py` & `graph_attention_student-0.7.1/graph_attention_student/experiments/vgd_regression_posthoc.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.0/graph_attention_student/experiments/vgd_regression_supervised.py` & `graph_attention_student-0.7.1/graph_attention_student/experiments/vgd_regression_supervised.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.0/graph_attention_student/experiments/vgd_regression_supervised_multi.py` & `graph_attention_student-0.7.1/graph_attention_student/experiments/vgd_regression_supervised_multi.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.0/graph_attention_student/experiments/vgd_regression_supervised_single.py` & `graph_attention_student-0.7.1/graph_attention_student/experiments/vgd_regression_supervised_single.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.0/graph_attention_student/experiments/vgd_single.py` & `graph_attention_student-0.7.1/graph_attention_student/experiments/vgd_single.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+"""
+
+"""
 import os
 import sys
 import pathlib
 import random
 import typing as t
 from collections import Counter
 
@@ -250,16 +253,17 @@
                 indices_true=test_indices,
                 x_true=x_test,
                 y_true=y_test,
                 out_pred=out_pred,
                 ni_pred=ni_pred,
                 ei_pred=ei_pred,
             )
-            for index, fidelity in zip(test_indices, fidelities):
-                e[f'fidelity/{rep}/{index}'] = fidelity
+            if fidelities:
+                for index, fidelity in zip(test_indices, fidelities):
+                    e[f'fidelity/{rep}/{index}'] = fidelity
 
             # ~ calculating explanation metrics
             e.info('calculating explanation metrics...')
 
             pred_node_importances = []
             pred_edge_importances = []
 
@@ -338,18 +342,24 @@
                 graph_list=graph_list,
                 image_path_list=image_path_list,
                 node_positions_list=node_positions_list,
                 importances_map={
                     'model': (ni_example_pred, ei_example_pred)
                 },
                 output_path=pdf_path,
-                importance_channel_labels=IMPORTANCE_CHANNEL_LABELS,
+                # importance_channel_labels=IMPORTANCE_CHANNEL_LABELS,
                 labels_list=[index_data_map[i]['metadata']['name'] for i in example_indices]
             )
 
+            # 19.04.2021 - Saving the model persistently to the disk now as well optionally
+            e.apply_hook(
+                'save_model',
+                model=model
+            )
+
             e.status()
 
 
 with Skippable(), e.analysis:
     # Creating latex code to display the results in a table
     e.info('rendering latex table...')
     column_names = [
```

### Comparing `graph_attention_student-0.7.0/graph_attention_student/experiments/vgd_single_gnnx.py` & `graph_attention_student-0.7.1/graph_attention_student/experiments/vgd_single_gnnx.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.0/graph_attention_student/experiments/vgd_single_gnnx_aqsoldb.py` & `graph_attention_student-0.7.1/graph_attention_student/experiments/vgd_single_gnnx_aqsoldb.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.0/graph_attention_student/experiments/vgd_single_gnnx_aqsoldb_dmpnn.py` & `graph_attention_student-0.7.1/graph_attention_student/experiments/vgd_single_gnnx_aqsoldb_dmpnn.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.0/graph_attention_student/experiments/vgd_single_gnnx_aqsoldb_gatv2.py` & `graph_attention_student-0.7.1/graph_attention_student/experiments/vgd_single_gnnx_aqsoldb_gatv2.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.0/graph_attention_student/experiments/vgd_single_gnnx_aqsoldb_painn.py` & `graph_attention_student-0.7.1/graph_attention_student/experiments/vgd_single_gnnx_aqsoldb_painn.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.0/graph_attention_student/experiments/vgd_single_megan.py` & `graph_attention_student-0.7.1/graph_attention_student/experiments/vgd_single_megan.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+"""
+
+CHANGELOG
+
+0.1.0
+"""
 import os
 import pathlib
 import typing as t
 
 import tensorflow as tf
 import tensorflow.keras as ks
 import numpy as np
@@ -93,14 +99,15 @@
 NAMESPACE = 'results/vgd_single_megan'
 DEBUG = True
 with Skippable(), (se := SubExperiment(EXPERIMENT_PATH, BASE_PATH, NAMESPACE, globals())):
 
     @se.hook('create_model')
     def create_model(e):
         e.info('MEGAN')
+        e.info(f' * SPARSITY_FACTOR: {e.parameters["SPARSITY_FACTOR"]}')
         model = Megan(
             units=e.parameters['UNITS'],
             dropout_rate=e.parameters['DROPOUT_RATE'],
             importance_factor=e.parameters['IMPORTANCE_FACTOR'],
             importance_multiplier=e.parameters['IMPORTANCE_MULTIPLIER'],
             importance_channels=e.parameters['IMPORTANCE_CHANNELS'],
             sparsity_factor=e.parameters['SPARSITY_FACTOR'],
@@ -159,14 +166,17 @@
             return out_pred
 
 
     @se.hook('calculate_fidelity')
     def calculate_fidelity(e, model, indices_true, x_true, y_true, out_pred, ni_pred, ei_pred):
         rep = e['rep']
 
+        if e.p['IMPORTANCE_CHANNELS'] != len(e.p['CHANNEL_DIRECTIONS']):
+            return [0]
+
         # ~ fidelity
         # For each importance channel we construct a mask which only masks out that very channel
         # and then we query the model using that mask, which effectively means that this channel
         # has absolutely no effect on the prediction. We record the outputs generated by these
         # masked predictions and then afterwards calculate the fidelity from that.
         for k in range(IMPORTANCE_CHANNELS):
             # First of all we need to construct the masks
@@ -193,7 +203,13 @@
                 out_masked = e[f"out/masked/{rep}/{index}/{k}"]
                 fidelity += e.parameters['CHANNEL_DIRECTIONS'][k] * (out - out_masked)
 
             fidelities.append(fidelity)
 
         return fidelities
 
+    @se.hook('save_model')
+    def save_model(e, model):
+        e.info('saving the MEGAN model...')
+        model_path = os.path.join(e.path, 'model')
+        e['model_path'] = model_path
+        model.save(model_path)
```

### Comparing `graph_attention_student-0.7.0/graph_attention_student/experiments/vgd_single_megan_aqsoldb.py` & `graph_attention_student-0.7.1/graph_attention_student/experiments/vgd_single_megan_aqsoldb.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,16 +21,17 @@
 # == MODEL PARAMETERS ==
 UNITS = [32, 32, 32]
 FINAL_UNITS = [64, 32, 1]
 REGRESSION_REFERENCE = -3
 REGRESSION_LIMITS = [[-12, 3]]
 
 # == TRAINING PARAMETERS ==
-BATCH_SIZE = 128
-REPETITIONS = 5
+BATCH_SIZE = 32
+EPOCHS = 50
+REPETITIONS = 1
 
 # == EXPERIMENT PARAMETERS ==
 PATH = pathlib.Path(__file__).parent.absolute()
 EXPERIMENT_PATH = os.path.join(PATH, 'vgd_single_megan.py')
 BASE_PATH = PATH
 NAMESPACE = 'results/vgd_single_megan_aqsoldb'
 with Skippable(), (se := SubExperiment(EXPERIMENT_PATH, BASE_PATH, NAMESPACE, globals())):
```

### Comparing `graph_attention_student-0.7.0/graph_attention_student/keras.py` & `graph_attention_student-0.7.1/graph_attention_student/keras.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.0/graph_attention_student/layers.py` & `graph_attention_student-0.7.1/graph_attention_student/layers.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.0/graph_attention_student/models/__pycache__/gnes.cpython-310.pyc` & `graph_attention_student-0.7.1/graph_attention_student/models/__pycache__/gnes.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Mar 19 09:12:41 2023 UTC, .py size: 3406 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 09d2 1664 4e0d 0000  o..........dN...
+00000000: 6f0d 0d0a 0000 0000 db3f 2864 4e0d 0000  o........?(dN...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6c00 0000 6400  .....@...sl...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c04 6d05 5a06 0100 6400 6402 6c07  d.l.m.Z...d.d.l.
 00000050: 6d08 5a08 0100 6400 6403 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6404 6c0b 6d0c 5a0c 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6405 6c0d 6d0e 5a0e 0100 6400 6406 6c0f  d.l.m.Z...d.d.l.
```

### Comparing `graph_attention_student-0.7.0/graph_attention_student/models/__pycache__/gnnx.cpython-310.pyc` & `graph_attention_student-0.7.1/graph_attention_student/models/__pycache__/gnnx.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.0/graph_attention_student/models/__pycache__/gradient.cpython-310.pyc` & `graph_attention_student-0.7.1/graph_attention_student/models/__pycache__/gradient.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Mar 19 09:10:38 2023 UTC, .py size: 12180 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,572 +1,578 @@
-00000000: 6f0d 0d0a 0000 0000 8ed1 1664 942f 0000  o..........d./..
+00000000: 6f0d 0d0a 0000 0000 f000 2864 4930 0000  o.........(dI0..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 000d 0000 0040 0000 0073 ee00 0000 6400  .....@...s....d.
+00000020: 000d 0000 0040 0000 0073 fa00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c04 6d05 5a06 0100 6400 6402 6c07  d.l.m.Z...d.d.l.
 00000050: 6d08 5a08 0100 6400 6403 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6404 6c0b 6d0c 5a0c 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6405 6c0d 6d0e 5a0e 0100 4700 6406 6407  d.l.m.Z...G.d.d.
 00000080: 8400 6407 6506 6a0f 6a10 8303 5a11 4700  ..d.e.j.j...Z.G.
 00000090: 6408 6409 8400 6409 6511 650e 8304 5a12  d.d...d.e.e...Z.
-000000a0: 090a 090a 090a 6416 640b 6501 6a13 6501  ......d.d.e.j.e.
-000000b0: 6a14 6503 6a15 6503 6a15 6602 1900 1900  j.e.j.e.j.f.....
-000000c0: 640c 6516 640d 6516 640e 6516 6608 640f  d.e.d.e.d.e.f.d.
-000000d0: 6410 8405 5a17 090a 090a 090a 0911 090a  d...Z...........
-000000e0: 6417 640b 6501 6a13 6501 6a14 6503 6a15  d.d.e.j.e.j.e.j.
-000000f0: 6503 6a15 6602 1900 1900 6412 6516 640c  e.j.f.....d.e.d.
-00000100: 6516 640d 6516 6413 6518 640e 6516 660c  e.d.e.d.e.d.e.f.
-00000110: 6414 6415 8405 5a19 6401 5300 2918 e900  d.d...Z.d.S.)...
-00000120: 0000 004e a901 da03 4743 4e29 01da 0e44  ...N....GCN)...D
-00000130: 656e 7365 456d 6265 6464 696e 6729 01da  enseEmbedding)..
-00000140: 0c50 6f6f 6c69 6e67 4e6f 6465 7329 01da  .PoolingNodes)..
-00000150: 0c47 4e4e 496e 7465 7266 6163 6563 0000  .GNNInterfacec..
-00000160: 0000 0000 0000 0000 0000 0000 0000 0600  ................
-00000170: 0000 4000 0000 7352 0000 0065 005a 0164  ..@...sR...e.Z.d
-00000180: 005a 0264 015a 0364 0d64 0364 0484 015a  .Z.d.Z.d.d.d...Z
-00000190: 0464 0d64 0564 0684 015a 0564 0765 066a  .d.d.d...Z.d.e.j
-000001a0: 0765 066a 0765 086a 0919 0019 0064 0865  .e.j.e.j.....d.e
-000001b0: 066a 0765 086a 0919 0064 0965 086a 0a66  .j.e.j...d.e.j.f
-000001c0: 0664 0a64 0b84 045a 0b64 0c53 0029 0eda  .d.d...Z.d.S.)..
-000001d0: 1541 6273 7472 6163 7447 7261 6469 656e  .AbstractGradien
-000001e0: 744d 6f64 656c 618c 0100 000a 2020 2020  tModela.....    
-000001f0: 5468 6973 2069 7320 616e 2061 6273 7472  This is an abstr
-00000200: 6163 7420 6261 7365 2063 6c61 7373 2066  act base class f
-00000210: 6f72 206d 6f64 656c 7320 7768 6963 6820  or models which 
-00000220: 7769 6c6c 2070 726f 7669 6465 2074 6865  will provide the
-00000230: 6972 2067 7261 6469 656e 7420 696e 666f  ir gradient info
-00000240: 726d 6174 696f 6e20 666f 7220 6675 7274  rmation for furt
-00000250: 6865 720a 2020 2020 7072 6f63 6573 7369  her.    processi
-00000260: 6e67 2e20 5468 6973 206d 6561 6e73 2074  ng. This means t
-00000270: 6861 7420 6475 7269 6e67 2074 6865 2069  hat during the i
-00000280: 6e66 6572 656e 6365 2063 616c 6c2c 2074  nference call, t
-00000290: 6865 7365 206b 696e 6473 206f 6620 6d6f  hese kinds of mo
-000002a0: 6465 6c73 2068 6176 6520 746f 206d 6169  dels have to mai
-000002b0: 6e74 6169 6e20 7468 6569 720a 2020 2020  ntain their.    
-000002c0: 6f77 6e20 6772 6164 6965 6e74 2074 6170  own gradient tap
-000002d0: 6520 746f 2072 6563 6f72 6420 7468 6520  e to record the 
-000002e0: 6675 6c6c 2069 6e66 6572 656e 6365 2070  full inference p
-000002f0: 726f 6365 7373 2061 6e64 2074 6865 6e20  rocess and then 
-00000300: 7573 6520 7468 6973 2074 6f20 7072 6f76  use this to prov
-00000310: 6964 6520 6772 6164 6965 6e74 7320 6f66  ide gradients of
-00000320: 2074 6865 0a20 2020 2069 6e70 7574 2061   the.    input a
-00000330: 6e64 2069 6e74 6572 6d65 6469 6174 6520  nd intermediate 
-00000340: 6e6f 6465 202f 2065 6467 6520 656d 6265  node / edge embe
-00000350: 6464 696e 6773 2077 6974 6820 7265 7370  ddings with resp
-00000360: 6563 7420 746f 2074 6865 206f 7574 7075  ect to the outpu
-00000370: 742e 0a20 2020 2054 6303 0000 0000 0000  t..    Tc.......
-00000380: 0000 0000 0003 0000 0001 0000 0043 0000  .............C..
-00000390: 0073 0600 0000 7400 8300 8201 2901 61e9  .s....t.....).a.
-000003a0: 0300 000a 2020 2020 2020 2020 2a2a 486f  ....        **Ho
-000003b0: 7720 7468 6520 6c69 7374 206f 6620 6772  w the list of gr
-000003c0: 6164 6965 6e74 7320 7368 6f75 6c64 206c  adients should l
-000003d0: 6f6f 6b20 6c69 6b65 2a2a 0a0a 2020 2020  ook like**..    
-000003e0: 2020 2020 4173 7375 6d69 6e67 206f 7574      Assuming out
-000003f0: 7075 7420 6469 6d65 6e73 696f 6e20 482c  put dimension H,
-00000400: 206e 756d 6265 7220 6f66 206e 6f64 6573   number of nodes
-00000410: 2056 2c20 6e6f 6465 2066 6561 7475 7265   V, node feature
-00000420: 7320 4e20 616e 6420 6261 7463 6820 7369  s N and batch si
-00000430: 7a65 2042 2c20 6173 2077 656c 6c20 6173  ze B, as well as
-00000440: 2074 6865 0a20 2020 2020 2020 206e 756d   the.        num
-00000450: 6265 7220 6f66 2063 6f6e 766f 6c75 7469  ber of convoluti
-00000460: 6f6e 616c 206c 6179 6572 7320 4c20 696e  onal layers L in
-00000470: 2074 6865 206e 6574 776f 726b 2e0a 0a20   the network... 
-00000480: 2020 2020 2020 2054 6865 206c 6973 7420         The list 
-00000490: 7368 6f75 6c64 2063 6f6e 7369 7374 206f  should consist o
-000004a0: 6620 4c2b 3120 656c 656d 656e 7473 2c20  f L+1 elements, 
-000004b0: 7768 6572 6520 7468 6520 6669 7273 7420  where the first 
-000004c0: 656c 656d 656e 7420 6973 2061 6c77 6179  element is alway
-000004d0: 7320 7468 6520 6772 6164 6965 6e74 7320  s the gradients 
-000004e0: 7769 7468 2072 6573 7065 6374 0a20 2020  with respect.   
-000004f0: 2020 2020 2074 6f20 7468 6520 696e 7075       to the inpu
-00000500: 7420 616e 6420 6166 7465 7220 7468 6174  t and after that
-00000510: 2074 6865 2067 7261 6469 656e 7473 206f   the gradients o
-00000520: 6620 7468 6520 696e 7465 726d 6564 6961  f the intermedia
-00000530: 7465 206e 6f64 652f 6564 6765 2065 6d62  te node/edge emb
-00000540: 6564 6469 6e67 732e 0a0a 2020 2020 2020  eddings...      
-00000550: 2020 4561 6368 2065 6c65 6d65 6e74 2073    Each element s
-00000560: 686f 756c 6420 6265 2061 2072 6167 6765  hould be a ragge
-00000570: 6420 7465 6e73 6f72 2077 6974 6820 7468  d tensor with th
-00000580: 6520 6469 6d65 6e73 696f 6e20 285b 425d  e dimension ([B]
-00000590: 2c20 5b56 5d2c 204e 2c20 4829 0a0a 2020  , [V], N, H)..  
-000005a0: 2020 2020 2020 3a72 6574 7572 6e3a 2054        :return: T
-000005b0: 6869 7320 6861 7320 746f 2062 6520 6120  his has to be a 
-000005c0: 7475 706c 6520 6f66 2066 6f75 7220 7661  tuple of four va
-000005d0: 6c75 6573 3a0a 2020 2020 2020 2020 2020  lues:.          
-000005e0: 2020 2d20 5468 6520 6d61 696e 206f 7574    - The main out
-000005f0: 7075 7420 7072 6564 6963 7469 6f6e 2022  put prediction "
-00000600: 7922 206f 6620 7468 6520 6d6f 6465 6c0a  y" of the model.
-00000610: 2020 2020 2020 2020 2020 2020 2d20 4120              - A 
-00000620: 6c69 7374 2063 6f6e 7461 696e 696e 6720  list containing 
-00000630: 7468 6520 6772 6164 6965 6e74 7320 6f66  the gradients of
-00000640: 2074 6865 2069 6e70 7574 2061 7320 7765   the input as we
-00000650: 6c6c 2061 7320 7468 6520 696e 7465 726d  ll as the interm
-00000660: 6564 6961 7465 206e 6f64 6528 2129 2065  ediate node(!) e
-00000670: 6d62 6564 6469 6e67 730a 2020 2020 2020  mbeddings.      
-00000680: 2020 2020 2020 2020 772e 722e 7420 746f          w.r.t to
-00000690: 2074 6865 206f 7574 7075 7420 2279 222e   the output "y".
-000006a0: 0a20 2020 2020 2020 2020 2020 202d 2041  .            - A
-000006b0: 206c 6973 7420 636f 6e74 6169 6e69 6e67   list containing
-000006c0: 2074 6865 2067 7261 6469 656e 7473 206f   the gradients o
-000006d0: 6620 7468 6520 696e 7075 7420 6173 2077  f the input as w
-000006e0: 656c 6c20 6173 2074 6865 2069 6e74 6572  ell as the inter
-000006f0: 6d65 6469 6174 6520 6564 6765 2821 2920  mediate edge(!) 
-00000700: 656d 6265 6464 696e 6773 0a20 2020 2020  embeddings.     
-00000710: 2020 2020 2020 2020 2077 2e72 2e74 2074           w.r.t t
-00000720: 6f20 7468 6520 6f75 7470 7574 2022 7922  o the output "y"
-00000730: 2e0a 2020 2020 2020 2020 2020 2020 2d20  ..            - 
-00000740: 5468 6520 6772 6164 6965 6e74 2074 6170  The gradient tap
-00000750: 6520 7573 6564 2074 6f20 6372 6561 7465  e used to create
-00000760: 2074 6865 2070 7265 7669 6f75 736c 7920   the previously 
-00000770: 6d65 6e74 696f 6e65 6420 6772 6164 6965  mentioned gradie
-00000780: 6e74 730a 2020 2020 2020 2020 2901 da13  nts.        )...
-00000790: 4e6f 7449 6d70 6c65 6d65 6e74 6564 4572  NotImplementedEr
-000007a0: 726f 7229 03da 0473 656c 66da 0669 6e70  ror)...self..inp
-000007b0: 7574 73da 0874 7261 696e 696e 67a9 0072  uts..training..r
-000007c0: 0c00 0000 fa59 2f6d 6564 6961 2f73 7364  .....Y/media/ssd
-000007d0: 2f50 726f 6772 616d 6d69 6e67 2f67 7261  /Programming/gra
-000007e0: 7068 5f61 7474 656e 7469 6f6e 5f73 7475  ph_attention_stu
-000007f0: 6465 6e74 2f67 7261 7068 5f61 7474 656e  dent/graph_atten
-00000800: 7469 6f6e 5f73 7475 6465 6e74 2f6d 6f64  tion_student/mod
-00000810: 656c 732f 6772 6164 6965 6e74 2e70 79da  els/gradient.py.
-00000820: 1363 616c 6c5f 7769 7468 5f67 7261 6469  .call_with_gradi
-00000830: 656e 7473 1300 0000 7302 0000 0006 147a  ents....s......z
-00000840: 2941 6273 7472 6163 7447 7261 6469 656e  )AbstractGradien
-00000850: 744d 6f64 656c 2e63 616c 6c5f 7769 7468  tModel.call_with
-00000860: 5f67 7261 6469 656e 7473 6303 0000 0000  _gradientsc.....
-00000870: 0000 0000 0000 0009 0000 0004 0000 004f  ...............O
-00000880: 0000 0073 2600 0000 7c00 6a00 7c01 7c02  ...s&...|.j.|.|.
-00000890: 6702 7c03 a201 5200 6900 7c04 a401 8e01  g.|...R.i.|.....
-000008a0: 5c04 7d05 7d06 7d07 7d08 7c05 5300 a901  \.}.}.}.}.|.S...
-000008b0: 4ea9 0172 0e00 0000 2909 7209 0000 0072  N..r....).r....r
-000008c0: 0a00 0000 720b 0000 00da 0461 7267 73da  ....r......args.
-000008d0: 066b 7761 7267 73da 0179 da0e 6e6f 6465  .kwargs..y..node
-000008e0: 5f67 7261 6469 656e 7473 da0e 6564 6765  _gradients..edge
-000008f0: 5f67 7261 6469 656e 7473 da04 7461 7065  _gradients..tape
-00000900: 720c 0000 0072 0c00 0000 720d 0000 00da  r....r....r.....
-00000910: 0463 616c 6c29 0000 0073 0400 0000 2201  .call)...s....".
-00000920: 0401 7a1a 4162 7374 7261 6374 4772 6164  ..z.AbstractGrad
-00000930: 6965 6e74 4d6f 6465 6c2e 6361 6c6c da04  ientModel.call..
-00000940: 6f75 7473 da0b 6163 7469 7661 7469 6f6e  outs..activation
-00000950: 7372 1600 0000 6305 0000 0000 0000 0000  sr....c.........
-00000960: 0000 000c 0000 0007 0000 0043 0000 0073  ...........C...s
-00000970: aa00 0000 6700 7d05 7c02 4400 5d4e 7d06  ....g.}.|.D.]N}.
-00000980: 6700 7d07 7400 7c04 8301 4400 5d30 7d08  g.}.t.|...D.]0}.
-00000990: 6700 7d09 7c01 7c08 1900 4400 5d14 7d0a  g.}.|.|...D.].}.
-000009a0: 7c03 a001 7c0a 7c06 a102 7d0b 7402 6a03  |...|.|...}.t.j.
-000009b0: 7c0b 6401 6402 8d02 7d0b 7c09 a004 7c0b  |.d.d...}.|...|.
-000009c0: a101 0100 7114 7402 6a05 7c09 6401 6402  ....q.t.j.|.d.d.
-000009d0: 8d02 7d09 7402 6a03 7c09 6403 6402 8d02  ..}.t.j.|.d.d...
-000009e0: 7d09 7c07 a004 7c09 a101 0100 710c 7402  }.|...|.....q.t.
-000009f0: 6a05 7c07 6403 6402 8d02 7d07 7402 6a06  j.|.d.d...}.t.j.
-00000a00: 7c07 6403 6402 8d02 7d07 7c05 a004 7c06  |.d.d...}.|...|.
-00000a10: 7c07 6602 a101 0100 7104 7c05 5300 2904  |.f.....q.|.S.).
-00000a20: 61ff 0800 000a 2020 2020 2020 2020 5468  a.....        Th
-00000a30: 6973 206d 6574 686f 6420 6973 2061 2062  is method is a b
-00000a40: 6f69 6c65 7270 6c61 7465 2069 6d70 6c65  oilerplate imple
-00000a50: 6d65 6e74 6174 696f 6e20 7468 6174 2077  mentation that w
-00000a60: 696c 6c20 6361 6c63 756c 6174 6520 7468  ill calculate th
-00000a70: 6520 6772 6164 6965 6e74 2069 6e66 6f20  e gradient info 
-00000a80: 6c69 7374 2c20 6769 7665 6e20 6120 6c69  list, given a li
-00000a90: 7374 0a20 2020 2020 2020 206f 6620 6d6f  st.        of mo
-00000aa0: 6465 6c20 6f75 7470 7574 732c 2061 206c  del outputs, a l
-00000ab0: 6973 7420 6f66 206c 6179 6572 2061 6374  ist of layer act
-00000ac0: 6976 6174 696f 6e20 7465 6e73 6f72 732c  ivation tensors,
-00000ad0: 2074 6865 2067 7261 6469 656e 7420 7461   the gradient ta
-00000ae0: 7065 2061 6e64 2074 6865 2062 6174 6368  pe and the batch
-00000af0: 2073 697a 652e 0a0a 2020 2020 2020 2020   size...        
-00000b00: 4173 7375 6d69 6e67 2074 6865 2066 6f6c  Assuming the fol
-00000b10: 6c6f 7769 6e67 2076 6172 6961 626c 6573  lowing variables
-00000b20: 3a0a 2020 2020 2020 2020 2d20 423a 2062  :.        - B: b
-00000b30: 6174 6368 2064 696d 656e 7369 6f6e 0a20  atch dimension. 
-00000b40: 2020 2020 2020 202d 204f 3a20 6f75 7470         - O: outp
-00000b50: 7574 2064 696d 656e 7369 6f6e 0a20 2020  ut dimension.   
-00000b60: 2020 2020 202d 204c 3a20 6e75 6d62 6572       - L: number
-00000b70: 206f 6620 636f 6e76 6f6c 7574 696f 6e61   of convolutiona
-00000b80: 6c20 6c61 7965 7273 202f 206e 756d 6265  l layers / numbe
-00000b90: 7220 6f66 2069 6e74 6572 6d65 6469 6174  r of intermediat
-00000ba0: 6520 656d 6265 6464 696e 6773 2077 2e72  e embeddings w.r
-00000bb0: 2e74 2077 6869 6368 2074 6865 2067 7261  .t which the gra
-00000bc0: 6469 656e 7473 0a20 2020 2020 2020 2020  dients.         
-00000bd0: 2020 2061 7265 2074 6f20 6265 2063 616c     are to be cal
-00000be0: 6375 6c61 7465 640a 2020 2020 2020 2020  culated.        
-00000bf0: 2d20 563a 204e 6f64 6520 6f72 2065 6467  - V: Node or edg
-00000c00: 6520 7368 6170 650a 2020 2020 2020 2020  e shape.        
-00000c10: 2d20 463a 2046 6561 7475 7265 2073 6861  - F: Feature sha
-00000c20: 7065 0a0a 2020 2020 2020 2020 3a70 6172  pe..        :par
-00000c30: 616d 206f 7574 733a 2054 6869 7320 6973  am outs: This is
-00000c40: 2073 7570 706f 7365 6420 746f 2062 6520   supposed to be 
-00000c50: 6120 6c69 7374 206f 6620 6c69 7374 7320  a list of lists 
-00000c60: 6f66 207a 6572 6f20 6469 6d65 6e73 696f  of zero dimensio
-00000c70: 6e61 6c20 7465 6e73 6f72 732e 2047 656e  nal tensors. Gen
-00000c80: 6572 616c 6c79 2c20 7468 650a 2020 2020  erally, the.    
-00000c90: 2020 2020 2020 2020 6f75 7470 7574 206f          output o
-00000ca0: 6620 6120 7265 6772 6573 7369 6f6e 202f  f a regression /
-00000cb0: 2063 6c61 7373 6966 6963 6174 696f 6e20   classification 
-00000cc0: 6e65 7477 6f72 6b20 7769 6c6c 2062 6520  network will be 
-00000cd0: 6120 7665 6374 6f72 206f 6620 7368 6170  a vector of shap
-00000ce0: 6520 285b 425d 2c20 4f29 2e20 5468 6973  e ([B], O). This
-00000cf0: 206c 6973 740a 2020 2020 2020 2020 2020   list.          
-00000d00: 2020 6861 7320 746f 2062 6173 6963 616c    has to basical
-00000d10: 6c79 2062 6520 7468 6973 2074 656e 736f  ly be this tenso
-00000d20: 7220 6f6e 6c79 2069 6e20 6c69 7374 2066  r only in list f
-00000d30: 6f72 6d61 742e 2054 6869 7320 6c69 7374  ormat. This list
-00000d40: 2073 686f 756c 6420 6265 2063 7265 6174   should be creat
-00000d50: 6564 2062 7920 6170 706c 7969 6e67 0a20  ed by applying. 
-00000d60: 2020 2020 2020 2020 2020 2074 6865 2063             the c
-00000d70: 6f72 7265 7370 6f6e 6469 6e67 2069 6e64  orresponding ind
-00000d80: 6578 696e 6720 736c 6963 6573 2074 6f20  exing slices to 
-00000d90: 7468 6520 6f75 7470 7574 2076 6563 746f  the output vecto
-00000da0: 7220 746f 2073 706c 6974 2069 7420 696e  r to split it in
-00000db0: 746f 2074 6865 206e 6573 7465 6420 666f  to the nested fo
-00000dc0: 726d 6174 206f 660a 2020 2020 2020 2020  rmat of.        
-00000dd0: 2020 2020 7a65 726f 2064 696d 656e 7369      zero dimensi
-00000de0: 6f6e 616c 2074 656e 736f 7220 6f62 6a65  onal tensor obje
-00000df0: 6374 732e 204e 6f74 6520 7468 6174 2074  cts. Note that t
-00000e00: 6869 7320 696e 6465 7869 6e67 206f 7065  his indexing ope
-00000e10: 7261 7469 6f6e 2068 6173 2074 6f20 6265  ration has to be
-00000e20: 2064 6f6e 6520 494e 5349 4445 2074 6865   done INSIDE the
-00000e30: 0a20 2020 2020 2020 2020 2020 2067 7261  .            gra
-00000e40: 6469 656e 7420 7461 7065 2063 6f6e 7465  dient tape conte
-00000e50: 7874 2c20 6f74 6865 7277 6973 6520 7468  xt, otherwise th
-00000e60: 6520 6361 6c63 756c 6174 696f 6e20 6f66  e calculation of
-00000e70: 2074 6865 2067 7261 6469 656e 7473 2077   the gradients w
-00000e80: 696c 6c20 6e6f 7420 776f 726b 210a 2020  ill not work!.  
-00000e90: 2020 2020 2020 3a70 6172 616d 2061 6374        :param act
-00000ea0: 6976 6174 696f 6e73 3a20 5468 6973 2069  ivations: This i
-00000eb0: 7320 6120 6c69 7374 2077 6974 6820 4c20  s a list with L 
-00000ec0: 656c 656d 656e 7473 2c20 7768 6572 6520  elements, where 
-00000ed0: 6561 6368 2065 6c65 6d65 6e74 2069 7320  each element is 
-00000ee0: 616e 2069 6e74 6572 6d65 6469 6174 6520  an intermediate 
-00000ef0: 6e6f 6465 202f 0a20 2020 2020 2020 2020  node /.         
-00000f00: 2020 2065 6467 6520 656d 6265 6464 696e     edge embeddin
-00000f10: 6720 7665 6374 6f72 2066 726f 6d20 7468  g vector from th
-00000f20: 6520 6361 6c6c 2070 726f 6365 7373 206f  e call process o
-00000f30: 6620 7468 6520 6e65 7477 6f72 6b2e 2049  f the network. I
-00000f40: 6e20 7468 6973 206d 6574 686f 6420 6f6e  n this method on
-00000f50: 6520 6772 6164 6965 6e74 2076 6563 746f  e gradient vecto
-00000f60: 720a 2020 2020 2020 2020 2020 2020 7769  r.            wi
-00000f70: 6c6c 2062 6520 6372 6561 7465 6420 666f  ll be created fo
-00000f80: 7220 6561 6368 206f 6620 7468 6520 6f75  r each of the ou
-00000f90: 7470 7574 7320 772e 722e 7420 746f 2065  tputs w.r.t to e
-00000fa0: 6163 6820 6f66 2074 6865 7365 2065 6d62  ach of these emb
-00000fb0: 6564 6469 6e67 732e 2054 6865 2072 6573  eddings. The res
-00000fc0: 756c 7469 6e67 0a20 2020 2020 2020 2020  ulting.         
-00000fd0: 2020 2067 7261 6469 656e 7420 7465 6e73     gradient tens
-00000fe0: 6f72 7320 7769 6c6c 2068 6176 6520 7468  ors will have th
-00000ff0: 6520 7361 6d65 2073 6861 7065 2061 7320  e same shape as 
-00001000: 7468 6520 656d 6265 6464 696e 6773 210a  the embeddings!.
-00001010: 2020 2020 2020 2020 3a70 6172 616d 2074          :param t
-00001020: 6170 653a 2054 6865 2047 7261 6469 656e  ape: The Gradien
-00001030: 7454 6170 6520 7768 6963 6820 7761 7320  tTape which was 
-00001040: 7573 6564 2064 7572 696e 6720 7468 6520  used during the 
-00001050: 6361 6c6c 2070 726f 6365 7373 2e0a 2020  call process..  
-00001060: 2020 2020 2020 3a70 6172 616d 2062 6174        :param bat
-00001070: 6368 5f73 697a 653a 2054 6865 2062 6174  ch_size: The bat
-00001080: 6368 2073 697a 6520 4220 7468 6174 2077  ch size B that w
-00001090: 6173 2075 7365 6420 746f 206f 6274 6169  as used to obtai
-000010a0: 6e20 7468 6520 6f75 7470 7574 7320 616e  n the outputs an
-000010b0: 6420 7468 6520 656d 6265 6464 696e 6773  d the embeddings
-000010c0: 2e20 5468 6973 2068 6173 0a20 2020 2020  . This has.     
-000010d0: 2020 2020 2020 2074 6f20 6265 2065 7861         to be exa
-000010e0: 6374 6c79 2063 6f72 7265 6374 210a 2020  ctly correct!.  
-000010f0: 2020 2020 2020 3a72 6574 7572 6e3a 2041        :return: A
-00001100: 206c 6973 7420 6f66 2074 7570 6c65 7320   list of tuples 
-00001110: 7769 7468 2074 6865 206c 656e 6774 6820  with the length 
-00001120: 4c2e 2045 6163 6820 7475 706c 6520 636f  L. Each tuple co
-00001130: 6e74 6169 6e73 2074 776f 2065 6c65 6d65  ntains two eleme
-00001140: 6e74 732e 2054 6865 2066 6972 7374 206f  nts. The first o
-00001150: 6e65 2069 7320 7468 650a 2020 2020 2020  ne is the.      
-00001160: 2020 2020 2020 6578 6163 7420 7361 6d65        exact same
-00001170: 2065 6d62 6564 6469 6e67 2074 656e 736f   embedding tenso
-00001180: 7220 7468 6174 2077 6173 2070 6173 7365  r that was passe
-00001190: 6420 746f 2074 6865 206d 6574 686f 6420  d to the method 
-000011a0: 696e 2074 6865 2022 6163 7469 7661 7469  in the "activati
-000011b0: 6f6e 7322 2070 6172 616d 6574 6572 2e0a  ons" parameter..
-000011c0: 2020 2020 2020 2020 2020 2020 5468 6973              This
-000011d0: 2074 656e 736f 7220 6861 7320 7468 6520   tensor has the 
-000011e0: 7368 6170 6520 285b 425d 2c20 5b56 5d2c  shape ([B], [V],
-000011f0: 2046 292e 2054 6865 2073 6563 6f6e 6420   F). The second 
-00001200: 656c 656d 656e 7420 6973 2074 6865 2063  element is the c
-00001210: 6f72 7265 7370 6f6e 6469 6e67 2067 7261  orresponding gra
-00001220: 6469 656e 740a 2020 2020 2020 2020 2020  dient.          
-00001230: 2020 7465 6e73 6f72 2074 6861 7420 7761    tensor that wa
-00001240: 7320 6372 6561 7465 6420 666f 7220 7468  s created for th
-00001250: 6174 2076 6572 7920 656d 6265 6464 696e  at very embeddin
-00001260: 6720 7769 7468 2074 6865 2073 6861 7065  g with the shape
-00001270: 2028 5b42 5d2c 205b 565d 2c20 462c 204f   ([B], [V], F, O
-00001280: 292e 204e 6f74 6520 7468 6174 2074 6865  ). Note that the
-00001290: 0a20 2020 2020 2020 2020 2020 2067 7261  .            gra
-000012a0: 6469 656e 7420 6861 7320 616e 2061 6464  dient has an add
-000012b0: 6974 696f 6e61 6c20 6469 6d65 6e73 696f  itional dimensio
-000012c0: 6e20 666f 7220 7468 6520 6f75 7470 7574  n for the output
-000012d0: 2073 6861 7065 2e20 5468 6973 2069 7320   shape. This is 
-000012e0: 6265 6361 7573 6520 6772 6164 6965 6e74  because gradient
-000012f0: 7320 6172 650a 2020 2020 2020 2020 2020  s are.          
-00001300: 2020 6372 6561 7465 6420 666f 7220 6576    created for ev
-00001310: 6572 7920 6f75 7470 7574 2e0a 2020 2020  ery output..    
-00001320: 2020 2020 e9fe ffff ffa9 01da 0461 7869      .........axi
-00001330: 73e9 ffff ffff 2907 da05 7261 6e67 65da  s.....)...range.
-00001340: 0867 7261 6469 656e 74da 0274 66da 0b65  .gradient..tf..e
-00001350: 7870 616e 645f 6469 6d73 da06 6170 7065  xpand_dims..appe
-00001360: 6e64 da06 636f 6e63 6174 da0a 7265 6475  nd..concat..redu
-00001370: 6365 5f73 756d 290c 7209 0000 0072 1800  ce_sum).r....r..
-00001380: 0000 7219 0000 0072 1600 0000 da0a 6261  ..r....r......ba
-00001390: 7463 685f 7369 7a65 da0d 6772 6164 6965  tch_size..gradie
-000013a0: 6e74 5f69 6e66 6fda 0a61 6374 6976 6174  nt_info..activat
-000013b0: 696f 6eda 0967 7261 6469 656e 7473 da01  ion..gradients..
-000013c0: 62da 0e67 7261 6469 656e 745f 7374 6163  b..gradient_stac
-000013d0: 6bda 036f 7574 721f 0000 0072 0c00 0000  k..outr....r....
-000013e0: 720c 0000 0072 0d00 0000 da17 6361 6c63  r....r......calc
-000013f0: 756c 6174 655f 6772 6164 6965 6e74 5f69  ulate_gradient_i
-00001400: 6e66 6f2d 0000 0073 2000 0000 0425 0801  nfo-...s ....%..
-00001410: 0401 0c01 0407 0c01 0c08 0e01 0c01 0e05  ................
-00001420: 0e01 0c02 0e03 0e04 1001 0402 7a2d 4162  ............z-Ab
-00001430: 7374 7261 6374 4772 6164 6965 6e74 4d6f  stractGradientMo
-00001440: 6465 6c2e 6361 6c63 756c 6174 655f 6772  del.calculate_gr
-00001450: 6164 6965 6e74 5f69 6e66 6f4e 2901 5429  adient_infoN).T)
-00001460: 0cda 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
-00001470: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
-00001480: 616d 655f 5fda 075f 5f64 6f63 5f5f 720e  ame__..__doc__r.
-00001490: 0000 0072 1700 0000 da01 74da 044c 6973  ...r......t..Lis
-000014a0: 7472 2000 0000 da06 5465 6e73 6f72 da0c  tr .....Tensor..
-000014b0: 4772 6164 6965 6e74 5461 7065 722c 0000  GradientTaper,..
-000014c0: 0072 0c00 0000 720c 0000 0072 0c00 0000  .r....r....r....
-000014d0: 720d 0000 0072 0700 0000 0b00 0000 7316  r....r........s.
-000014e0: 0000 0008 0004 010a 070a 1602 0410 0102  ................
-000014f0: ff0a 0202 fe04 030e fd72 0700 0000 6300  .........r....c.
-00001500: 0000 0000 0000 0000 0000 0000 0000 000d  ................
-00001510: 0000 0040 0000 0073 6400 0000 6500 5a01  ...@...sd...e.Z.
-00001520: 6400 5a02 6401 6402 8400 6403 6404 6603  d.Z.d.d...d.d.f.
-00001530: 6405 6503 6406 6504 6a05 6503 1900 6407  d.e.d.e.j.e...d.
-00001540: 6504 6a05 6503 1900 6408 6504 6a06 6409  e.j.e...d.e.j.d.
-00001550: 6507 640a 6507 660c 640b 640c 8405 5a08  e.d.e.f.d.d...Z.
-00001560: 6414 640f 6410 8401 5a09 090d 090e 090d  d.d.d...Z.......
-00001570: 0911 6415 6412 6413 8401 5a0a 640e 5300  ..d.d.d...Z.d.S.
-00001580: 2916 da10 4763 6e47 7261 6469 656e 744d  )...GcnGradientM
-00001590: 6f64 656c 6301 0000 0000 0000 0000 0000  odelc...........
-000015a0: 0001 0000 0003 0000 0043 0000 0073 0a00  .........C...s..
-000015b0: 0000 7400 7c00 6401 8d01 5300 2902 4ea9  ..t.|.d...S.).N.
-000015c0: 01da 0575 6e69 7473 7202 0000 0072 3600  ...unitsr....r6.
-000015d0: 0000 720c 0000 0072 0c00 0000 720d 0000  ..r....r....r...
-000015e0: 00da 083c 6c61 6d62 6461 3e82 0000 0073  ...<lambda>....s
-000015f0: 0200 0000 0a00 7a19 4763 6e47 7261 6469  ......z.GcnGradi
-00001600: 656e 744d 6f64 656c 2e3c 6c61 6d62 6461  entModel.<lambda
-00001610: 3eda 046d 6561 6eda 066c 696e 6561 7272  >..mean..linearr
-00001620: 2500 0000 7237 0000 00da 0b66 696e 616c  %...r7.....final
-00001630: 5f75 6e69 7473 da08 6c61 7965 725f 6362  _units..layer_cb
-00001640: da0e 706f 6f6c 696e 675f 6d65 7468 6f64  ..pooling_method
-00001650: da10 6669 6e61 6c5f 6163 7469 7661 7469  ..final_activati
-00001660: 6f6e 6307 0000 0000 0000 0000 0000 000a  onc.............
-00001670: 0000 0005 0000 0043 0000 0073 b600 0000  .......C...s....
-00001680: 7400 a001 7c00 a101 0100 7402 a001 7c00  t...|.....t...|.
-00001690: a101 0100 7c01 7c00 5f03 7c02 7c00 5f04  ....|.|._.|.|._.
-000016a0: 7c03 6401 1900 7c00 5f05 6700 7c00 5f06  |.d...|._.g.|._.
-000016b0: 7c00 6a04 4400 5d0c 7d07 7c04 7c07 8301  |.j.D.].}.|.|...
-000016c0: 7d08 7c00 6a06 a007 7c08 a101 0100 711b  }.|.j...|.....q.
-000016d0: 7408 7c05 6402 8d01 7c00 5f09 7c03 7c00  t.|.d...|._.|.|.
-000016e0: 5f0a 6403 6404 8400 7c03 4400 8301 7c00  _.d.d...|.D...|.
-000016f0: 5f0b 7c06 7c00 6a0b 6401 3c00 6700 7c00  _.|.|.j.d.<.g.|.
-00001700: 5f0c 740d 7c00 6a0a 7c00 6a0b 8302 4400  _.t.|.j.|.j...D.
-00001710: 5d10 5c02 7d07 7d09 740e 7c07 7c09 6405  ].\.}.}.t.|.|.d.
-00001720: 8d02 7d08 7c00 6a0c a007 7c08 a101 0100  ..}.|.j...|.....
-00001730: 7148 6400 5300 2906 4e72 1d00 0000 2901  qHd.S.).Nr....).
-00001740: 723d 0000 0063 0100 0000 0000 0000 0000  r=...c..........
-00001750: 0000 0200 0000 0300 0000 5300 0000 7310  ..........S...s.
-00001760: 0000 0067 007c 005d 047d 0164 0091 0271  ...g.|.].}.d...q
-00001770: 0253 0029 017a 106b 6763 6e6e 3e6c 6561  .S.).z.kgcnn>lea
-00001780: 6b79 5f72 656c 7572 0c00 0000 2902 da02  ky_relur....)...
-00001790: 2e30 da01 5f72 0c00 0000 720c 0000 0072  .0.._r....r....r
-000017a0: 0d00 0000 da0a 3c6c 6973 7463 6f6d 703e  ......<listcomp>
-000017b0: 9400 0000 7302 0000 0010 007a 2d47 636e  ....s......z-Gcn
-000017c0: 4772 6164 6965 6e74 4d6f 6465 6c2e 5f5f  GradientModel.__
-000017d0: 696e 6974 5f5f 2e3c 6c6f 6361 6c73 3e2e  init__.<locals>.
-000017e0: 3c6c 6973 7463 6f6d 703e 2902 7237 0000  <listcomp>).r7..
-000017f0: 0072 2700 0000 290f 7207 0000 00da 085f  .r'...).r......_
-00001800: 5f69 6e69 745f 5f72 0600 0000 7225 0000  _init__r....r%..
-00001810: 0072 3700 0000 da0b 6e75 6d5f 6f75 7470  .r7.....num_outp
-00001820: 7574 73da 0b63 6f6e 765f 6c61 7965 7273  uts..conv_layers
-00001830: 7222 0000 0072 0500 0000 da0b 6c61 795f  r"...r......lay_
-00001840: 706f 6f6c 696e 6772 3b00 0000 da0a 6669  poolingr;.....fi
-00001850: 6e61 6c5f 6163 7473 da0c 6669 6e61 6c5f  nal_acts..final_
-00001860: 6c61 7965 7273 da03 7a69 7072 0400 0000  layers..zipr....
-00001870: 290a 7209 0000 0072 2500 0000 7237 0000  ).r....r%...r7..
-00001880: 0072 3b00 0000 723c 0000 0072 3d00 0000  .r;...r<...r=...
-00001890: 723e 0000 00da 016b da03 6c61 79da 0361  r>.....k..lay..a
-000018a0: 6374 720c 0000 0072 0c00 0000 720d 0000  ctr....r....r...
-000018b0: 0072 4200 0000 7e00 0000 7324 0000 000a  .rB...~...s$....
-000018c0: 070a 0106 0206 010a 0106 020a 0108 010e  ................
-000018d0: 010c 0206 0210 010a 0106 0116 010c 010e  ................
-000018e0: 0104 fe7a 1947 636e 4772 6164 6965 6e74  ...z.GcnGradient
-000018f0: 4d6f 6465 6c2e 5f5f 696e 6974 5f5f 544e  Model.__init__TN
-00001900: 6305 0000 0000 0000 0000 0000 0011 0000  c...............
-00001910: 0008 0000 0003 0000 0073 1201 0000 7c04  .........s....|.
-00001920: 6400 7500 7207 8801 6a00 7d04 7c01 5c03  d.u.r...j.}.|.\.
-00001930: 7d05 7d06 7d07 7c05 7d08 7401 6a02 6401  }.}.}.|.}.t.j.d.
-00001940: 6402 8d01 8f50 7d09 7c09 a003 7c05 a101  d....P}.|...|...
-00001950: 0100 7c09 a003 7c06 a101 0100 7c06 6701  ..|...|.....|.g.
-00001960: 7d0a 7c08 6701 7d0b 8801 6a04 4400 5d0e  }.|.g.}...j.D.].
-00001970: 7d0c 7c0c 7c08 7c06 7c07 6703 8301 7d08  }.|.|.|.|.g...}.
-00001980: 7c0b a005 7c08 a101 0100 7128 8801 a006  |...|.....q(....
-00001990: 7c08 a101 8900 8801 6a07 4400 5d06 7d0c  |.......j.D.].}.
-000019a0: 7c0c 8800 8301 8900 713f 8700 6601 6403  |.......q?..f.d.
-000019b0: 6404 8408 7408 7c04 8301 4400 8301 7d0d  d...t.|...D...}.
-000019c0: 8700 8701 6602 6405 6404 8408 7408 7c04  ....f.d.d...t.|.
-000019d0: 8301 4400 8301 7d0e 5700 6400 0400 0400  ..D...}.W.d.....
-000019e0: 8303 0100 6e08 3100 7367 7701 0100 0100  ....n.1.sgw.....
-000019f0: 0100 5900 0100 7c03 727f 8801 a009 7c0e  ..Y...|.r.....|.
-00001a00: 7c0a 7c09 7c04 a104 7d0f 8801 a009 7c0e  |.|.|...}.....|.
-00001a10: 7c0b 7c09 7c04 a104 7d10 6e04 6700 7d10  |.|.|...}.n.g.}.
-00001a20: 6700 7d0f 8800 7c10 7c0f 7c09 6604 5300  g.}...|.|.|.f.S.
-00001a30: 2906 4e54 2901 da0a 7065 7273 6973 7465  ).NT)...persiste
-00001a40: 6e74 6301 0000 0000 0000 0000 0000 0002  ntc.............
-00001a50: 0000 0006 0000 0013 0000 0073 1c00 0000  ...........s....
-00001a60: 6700 7c00 5d0a 7d01 8800 7c01 6400 6400  g.|.].}...|.d.d.
-00001a70: 8502 6602 1900 9102 7102 5300 720f 0000  ..f.....q.S.r...
-00001a80: 0072 0c00 0000 2902 723f 0000 0072 2900  .r....).r?...r).
-00001a90: 0000 2901 722b 0000 0072 0c00 0000 720d  ..).r+...r....r.
-00001aa0: 0000 0072 4100 0000 b100 0000 7302 0000  ...rA.......s...
-00001ab0: 001c 007a 3847 636e 4772 6164 6965 6e74  ...z8GcnGradient
-00001ac0: 4d6f 6465 6c2e 6361 6c6c 5f77 6974 685f  Model.call_with_
-00001ad0: 6772 6164 6965 6e74 732e 3c6c 6f63 616c  gradients.<local
-00001ae0: 733e 2e3c 6c69 7374 636f 6d70 3e63 0100  s>.<listcomp>c..
-00001af0: 0000 0000 0000 0000 0000 0100 0000 0500  ................
-00001b00: 0000 1300 0000 7326 0000 0067 007c 005d  ......s&...g.|.]
-00001b10: 0f89 0087 0087 0166 0264 0064 0184 0874  .......f.d.d...t
-00001b20: 0088 026a 0183 0144 0083 0191 0271 0253  ...j...D.....q.S
-00001b30: 0029 0263 0100 0000 0000 0000 0000 0000  .).c............
-00001b40: 0200 0000 0500 0000 1300 0000 7318 0000  ............s...
-00001b50: 0067 007c 005d 087d 0188 0188 007c 0166  .g.|.].}.....|.f
-00001b60: 0219 0091 0271 0253 0072 0c00 0000 720c  .....q.S.r....r.
-00001b70: 0000 0029 0272 3f00 0000 da01 6f29 0272  ...).r?.....o).r
-00001b80: 2900 0000 722b 0000 0072 0c00 0000 720d  )...r+...r....r.
-00001b90: 0000 0072 4100 0000 b200 0000 7302 0000  ...rA.......s...
-00001ba0: 0018 007a 4347 636e 4772 6164 6965 6e74  ...zCGcnGradient
-00001bb0: 4d6f 6465 6c2e 6361 6c6c 5f77 6974 685f  Model.call_with_
-00001bc0: 6772 6164 6965 6e74 732e 3c6c 6f63 616c  gradients.<local
-00001bd0: 733e 2e3c 6c69 7374 636f 6d70 3e2e 3c6c  s>.<listcomp>.<l
-00001be0: 6973 7463 6f6d 703e 2902 721e 0000 0072  istcomp>).r....r
-00001bf0: 4300 0000 2901 723f 0000 00a9 0272 2b00  C...).r?.....r+.
-00001c00: 0000 7209 0000 0029 0172 2900 0000 720d  ..r....).r)...r.
-00001c10: 0000 0072 4100 0000 b200 0000 7302 0000  ...rA.......s...
-00001c20: 0026 0029 0a72 2500 0000 7220 0000 0072  .&.).r%...r ...r
-00001c30: 3400 0000 da05 7761 7463 6872 4400 0000  4.....watchrD...
-00001c40: 7222 0000 0072 4500 0000 7247 0000 0072  r"...rE...rG...r
-00001c50: 1e00 0000 722c 0000 0029 1172 0900 0000  ....r,...).r....
-00001c60: 720a 0000 0072 0b00 0000 da10 6372 6561  r....r......crea
-00001c70: 7465 5f67 7261 6469 656e 7473 7225 0000  te_gradientsr%..
-00001c80: 00da 0a6e 6f64 655f 696e 7075 74da 0a65  ...node_input..e
-00001c90: 6467 655f 696e 7075 74da 1065 6467 655f  dge_input..edge_
-00001ca0: 696e 6465 785f 696e 7075 74da 0178 7216  index_input..xr.
-00001cb0: 0000 00da 1065 6467 655f 6163 7469 7661  .....edge_activa
-00001cc0: 7469 6f6e 73da 106e 6f64 655f 6163 7469  tions..node_acti
-00001cd0: 7661 7469 6f6e 7372 4a00 0000 7218 0000  vationsrJ...r...
-00001ce0: 00da 0a6f 7574 735f 6d75 6c74 69da 1265  ...outs_multi..e
-00001cf0: 6467 655f 6772 6164 6965 6e74 5f69 6e66  dge_gradient_inf
-00001d00: 6fda 126e 6f64 655f 6772 6164 6965 6e74  o..node_gradient
-00001d10: 5f69 6e66 6f72 0c00 0000 724e 0000 0072  _infor....rN...r
-00001d20: 0d00 0000 720e 0000 009b 0000 0073 3000  ....r........s0.
-00001d30: 0000 0801 0601 0a02 0401 0e02 0a01 0a01  ................
-00001d40: 0602 0601 0a01 0e01 0c01 0a02 0a02 0a01  ................
-00001d50: 1602 1a01 1cf0 0412 1001 1201 0402 0401  ................
-00001d60: 0c02 7a24 4763 6e47 7261 6469 656e 744d  ..z$GcnGradientM
-00001d70: 6f64 656c 2e63 616c 6c5f 7769 7468 5f67  odel.call_with_g
-00001d80: 7261 6469 656e 7473 4663 0600 0000 0000  radientsFc......
-00001d90: 0000 0000 0000 0a00 0000 0600 0000 4300  ..............C.
-00001da0: 0000 732c 0000 007c 006a 007c 017c 027c  ..s,...|.j.|.|.|
-00001db0: 037c 0464 018d 045c 047d 067d 077d 087d  .|.d...\.}.}.}.}
-00001dc0: 097c 0572 147c 067c 077c 0866 0353 007c  .|.r.|.|.|.f.S.|
-00001dd0: 0653 0029 024e 2903 720b 0000 0072 2500  .S.).N).r....r%.
-00001de0: 0000 7250 0000 0072 1000 0000 290a 7209  ..rP...r....).r.
-00001df0: 0000 0072 0a00 0000 720b 0000 0072 2500  ...r....r....r%.
-00001e00: 0000 7250 0000 00da 1072 6574 7572 6e5f  ..rP.....return_
-00001e10: 6772 6164 6965 6e74 7372 1300 0000 da09  gradientsr......
-00001e20: 6e6f 6465 5f69 6e66 6fda 0965 6467 655f  node_info..edge_
-00001e30: 696e 666f 7216 0000 0072 0c00 0000 720c  infor....r....r.
-00001e40: 0000 0072 0d00 0000 7217 0000 00bd 0000  ...r....r.......
-00001e50: 0073 1200 0000 0406 0201 0201 0201 0201  .s..............
-00001e60: 0efc 0407 0a01 0402 7a15 4763 6e47 7261  ........z.GcnGra
-00001e70: 6469 656e 744d 6f64 656c 2e63 616c 6c29  dientModel.call)
-00001e80: 0354 544e 2904 544e 5446 290b 722d 0000  .TTN).TNTF).r-..
-00001e90: 0072 2e00 0000 722f 0000 00da 0369 6e74  .r....r/.....int
-00001ea0: 7231 0000 0072 3200 0000 da08 4361 6c6c  r1...r2.....Call
-00001eb0: 6162 6c65 da03 7374 7272 4200 0000 720e  able..strrB...r.
-00001ec0: 0000 0072 1700 0000 720c 0000 0072 0c00  ...r....r....r..
-00001ed0: 0000 720c 0000 0072 0d00 0000 7235 0000  ..r....r....r5..
-00001ee0: 007c 0000 0073 2e00 0000 0800 0606 0201  .|...s..........
-00001ef0: 0201 04fa 0201 02ff 0802 02fe 0803 02fd  ................
-00001f00: 0404 02fc 0205 02fb 0206 0afa 0a1d 0224  ...............$
-00001f10: 0201 0201 0201 0efb 7235 0000 0046 7226  ........r5...Fr&
-00001f20: 0000 00da 0875 7365 5f72 656c 75da 0c75  .....use_relu..u
-00001f30: 7365 5f61 6273 6f6c 7574 65da 086b 6565  se_absolute..kee
-00001f40: 7064 696d 7363 0400 0000 0000 0000 0000  pdimsc..........
-00001f50: 0000 0700 0000 0600 0000 4300 0000 734c  ..........C...sL
-00001f60: 0000 007c 0064 0119 005c 027d 047d 0574  ...|.d...\.}.}.t
-00001f70: 006a 017c 0574 006a 027c 0464 0264 038d  .j.|.t.j.|.d.d..
-00001f80: 0214 0064 047c 0364 058d 037d 067c 0172  ...d.|.d...}.|.r
-00001f90: 1d74 036a 04a0 057c 06a1 017d 067c 0272  .t.j...|...}.|.r
-00001fa0: 2474 00a0 067c 06a1 017d 067c 0653 0029  $t...|...}.|.S.)
-00001fb0: 064e 7201 0000 0072 1a00 0000 721b 0000  .Nr....r....r...
-00001fc0: 0072 1d00 0000 a902 721c 0000 0072 6200  .r......r....rb.
-00001fd0: 0000 2907 7220 0000 0072 2400 0000 7221  ..).r ...r$...r!
-00001fe0: 0000 00da 026b 73da 0762 6163 6b65 6e64  .....ks..backend
-00001ff0: da04 7265 6c75 da03 6162 7329 0772 2600  ..relu..abs).r&.
-00002000: 0000 7260 0000 0072 6100 0000 7262 0000  ..r`...ra...rb..
-00002010: 0072 2700 0000 7228 0000 00da 0b69 6d70  .r'...r(.....imp
-00002020: 6f72 7461 6e63 6573 720c 0000 0072 0c00  ortancesr....r..
-00002030: 0000 720d 0000 00da 1067 7261 645f 696d  ..r......grad_im
-00002040: 706f 7274 616e 6365 73d0 0000 0073 1600  portances....s..
-00002050: 0000 0c08 0401 1003 0201 0201 06fb 0407  ................
-00002060: 0c01 0401 0a01 0402 7269 0000 00e9 0200  ........ri......
-00002070: 0000 da0b 7573 655f 6176 6572 6167 65da  ....use_average.
-00002080: 0f61 7665 7261 6769 6e67 5f64 6570 7468  .averaging_depth
-00002090: 6306 0000 0000 0000 0000 0000 000b 0000  c...............
-000020a0: 0007 0000 0043 0000 0073 a200 0000 6700  .....C...s....g.
-000020b0: 7d06 7c00 4400 5d2f 5c02 7d07 7d08 7400  }.|.D.]/\.}.}.t.
-000020c0: 6a01 7c08 6401 6402 6403 8d03 7d09 7400  j.|.d.d.d...}.t.
-000020d0: 6a02 7c09 7400 6a03 7c07 6404 6405 8d02  j.|.t.j.|.d.d...
-000020e0: 1400 6406 7c05 6403 8d03 7d0a 7c02 7227  ..d.|.d...}.|.r'
-000020f0: 7404 6a05 a006 7c0a a101 7d0a 7c03 722e  t.j...|...}.|.r.
-00002100: 7400 a007 7c0a a101 7d0a 7c06 a008 7c0a  t...|...}.|...|.
-00002110: a101 0100 7104 7c01 7243 7400 6a09 7c06  ....q.|.rCt.j.|.
-00002120: 7c04 0b00 6400 8502 1900 6406 6405 8d02  |...d.....d.d...
-00002130: 7d06 6e04 7c06 6406 1900 7d06 7400 6a01  }.n.|.d...}.t.j.
-00002140: 7c06 6406 6402 6403 8d03 7d06 7c06 5300  |.d.d.d...}.|.S.
-00002150: 2907 4ee9 0100 0000 5472 6300 0000 721a  ).N.....Trc...r.
-00002160: 0000 0072 1b00 0000 721d 0000 0029 0a72  ...r....r....).r
-00002170: 2000 0000 da0b 7265 6475 6365 5f6d 6561   .....reduce_mea
-00002180: 6e72 2400 0000 7221 0000 0072 6400 0000  nr$...r!...rd...
-00002190: 7265 0000 0072 6600 0000 7267 0000 0072  re...rf...rg...r
-000021a0: 2200 0000 7223 0000 0029 0b72 2600 0000  "...r#...).r&...
-000021b0: 726b 0000 0072 6000 0000 7261 0000 0072  rk...r`...ra...r
-000021c0: 6c00 0000 7262 0000 0072 6800 0000 7227  l...rb...rh...r'
-000021d0: 0000 0072 2800 0000 da05 616c 7068 61da  ...r(.....alpha.
-000021e0: 116c 6f63 616c 5f69 6d70 6f72 7461 6e63  .local_importanc
-000021f0: 6573 720c 0000 0072 0c00 0000 720d 0000  esr....r....r...
-00002200: 00da 1467 7261 645f 6361 6d5f 696d 706f  ...grad_cam_impo
-00002210: 7274 616e 6365 73e8 0000 0073 2400 0000  rtances....s$...
-00002220: 0406 0c01 1005 0401 1003 0201 0201 06fb  ................
-00002230: 0408 0c01 0401 0a01 0c02 0402 1a01 0802  ................
-00002240: 1002 0401 7271 0000 0029 0346 4646 2905  ....rq...).FFF).
-00002250: 4646 4672 6a00 0000 4629 1ada 0674 7970  FFFrj...F)...typ
-00002260: 696e 6772 3100 0000 da0a 7465 6e73 6f72  ingr1.....tensor
-00002270: 666c 6f77 7220 0000 00da 1074 656e 736f  flowr .....tenso
-00002280: 7266 6c6f 772e 6b65 7261 73da 056b 6572  rflow.keras..ker
-00002290: 6173 7264 0000 00da 1a6b 6763 6e6e 2e6c  asrd.....kgcnn.l
-000022a0: 6179 6572 732e 636f 6e76 2e67 636e 5f63  ayers.conv.gcn_c
-000022b0: 6f6e 7672 0300 0000 da14 6b67 636e 6e2e  onvr......kgcnn.
-000022c0: 6c61 7965 7273 2e6d 6f64 756c 6573 7204  layers.modulesr.
-000022d0: 0000 00da 146b 6763 6e6e 2e6c 6179 6572  .....kgcnn.layer
-000022e0: 732e 706f 6f6c 696e 6772 0500 0000 da1b  s.poolingr......
-000022f0: 6b67 636e 6e2e 6c69 7465 7261 7475 7265  kgcnn.literature
-00002300: 2e47 4e4e 4578 706c 6169 6e72 0600 0000  .GNNExplainr....
-00002310: da06 6d6f 6465 6c73 da05 4d6f 6465 6c72  ..models..Modelr
-00002320: 0700 0000 7235 0000 0072 3200 0000 da05  ....r5...r2.....
-00002330: 5475 706c 6572 3300 0000 da04 626f 6f6c  Tupler3.....bool
-00002340: 7269 0000 0072 5d00 0000 7271 0000 0072  ri...r]...rq...r
-00002350: 0c00 0000 720c 0000 0072 0c00 0000 720d  ....r....r....r.
-00002360: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-00002370: 0073 4600 0000 0800 0802 0c01 0c01 0c01  .sF.............
-00002380: 0c01 0c01 1403 1271 0255 0201 0201 1cfd  .......q.U......
-00002390: 0201 02ff 0202 02fe 0203 0afd 0219 0201  ................
-000023a0: 0201 0201 0201 1cfb 0201 02ff 0202 02fe  ................
-000023b0: 0203 02fd 0204 02fc 0205 0efb            ............
+000000a0: 090a 090a 090a 090a 6418 640b 6501 6a13  ........d.d.e.j.
+000000b0: 6501 6a14 6503 6a15 6503 6a15 6602 1900  e.j.e.j.e.j.f...
+000000c0: 1900 640c 6516 640d 6516 640e 6516 640f  ..d.e.d.e.d.e.d.
+000000d0: 6516 6410 6503 6a17 660c 6411 6412 8405  e.d.e.j.f.d.d...
+000000e0: 5a18 090a 090a 090a 0913 090a 6419 640b  Z...........d.d.
+000000f0: 6501 6a13 6501 6a14 6503 6a15 6503 6a15  e.j.e.j.e.j.e.j.
+00000100: 6602 1900 1900 6414 6516 640c 6516 640d  f.....d.e.d.e.d.
+00000110: 6516 6415 6519 640f 6516 660c 6416 6417  e.d.e.d.e.f.d.d.
+00000120: 8405 5a1a 6401 5300 291a e900 0000 004e  ..Z.d.S.)......N
+00000130: a901 da03 4743 4e29 01da 0e44 656e 7365  ....GCN)...Dense
+00000140: 456d 6265 6464 696e 6729 01da 0c50 6f6f  Embedding)...Poo
+00000150: 6c69 6e67 4e6f 6465 7329 01da 0c47 4e4e  lingNodes)...GNN
+00000160: 496e 7465 7266 6163 6563 0000 0000 0000  Interfacec......
+00000170: 0000 0000 0000 0000 0000 0600 0000 4000  ..............@.
+00000180: 0000 7352 0000 0065 005a 0164 005a 0264  ..sR...e.Z.d.Z.d
+00000190: 015a 0364 0d64 0364 0484 015a 0464 0d64  .Z.d.d.d...Z.d.d
+000001a0: 0564 0684 015a 0564 0765 066a 0765 066a  .d...Z.d.e.j.e.j
+000001b0: 0765 086a 0919 0019 0064 0865 066a 0765  .e.j.....d.e.j.e
+000001c0: 086a 0919 0064 0965 086a 0a66 0664 0a64  .j...d.e.j.f.d.d
+000001d0: 0b84 045a 0b64 0c53 0029 0eda 1541 6273  ...Z.d.S.)...Abs
+000001e0: 7472 6163 7447 7261 6469 656e 744d 6f64  tractGradientMod
+000001f0: 656c 618c 0100 000a 2020 2020 5468 6973  ela.....    This
+00000200: 2069 7320 616e 2061 6273 7472 6163 7420   is an abstract 
+00000210: 6261 7365 2063 6c61 7373 2066 6f72 206d  base class for m
+00000220: 6f64 656c 7320 7768 6963 6820 7769 6c6c  odels which will
+00000230: 2070 726f 7669 6465 2074 6865 6972 2067   provide their g
+00000240: 7261 6469 656e 7420 696e 666f 726d 6174  radient informat
+00000250: 696f 6e20 666f 7220 6675 7274 6865 720a  ion for further.
+00000260: 2020 2020 7072 6f63 6573 7369 6e67 2e20      processing. 
+00000270: 5468 6973 206d 6561 6e73 2074 6861 7420  This means that 
+00000280: 6475 7269 6e67 2074 6865 2069 6e66 6572  during the infer
+00000290: 656e 6365 2063 616c 6c2c 2074 6865 7365  ence call, these
+000002a0: 206b 696e 6473 206f 6620 6d6f 6465 6c73   kinds of models
+000002b0: 2068 6176 6520 746f 206d 6169 6e74 6169   have to maintai
+000002c0: 6e20 7468 6569 720a 2020 2020 6f77 6e20  n their.    own 
+000002d0: 6772 6164 6965 6e74 2074 6170 6520 746f  gradient tape to
+000002e0: 2072 6563 6f72 6420 7468 6520 6675 6c6c   record the full
+000002f0: 2069 6e66 6572 656e 6365 2070 726f 6365   inference proce
+00000300: 7373 2061 6e64 2074 6865 6e20 7573 6520  ss and then use 
+00000310: 7468 6973 2074 6f20 7072 6f76 6964 6520  this to provide 
+00000320: 6772 6164 6965 6e74 7320 6f66 2074 6865  gradients of the
+00000330: 0a20 2020 2069 6e70 7574 2061 6e64 2069  .    input and i
+00000340: 6e74 6572 6d65 6469 6174 6520 6e6f 6465  ntermediate node
+00000350: 202f 2065 6467 6520 656d 6265 6464 696e   / edge embeddin
+00000360: 6773 2077 6974 6820 7265 7370 6563 7420  gs with respect 
+00000370: 746f 2074 6865 206f 7574 7075 742e 0a20  to the output.. 
+00000380: 2020 2054 6303 0000 0000 0000 0000 0000     Tc...........
+00000390: 0003 0000 0001 0000 0043 0000 0073 0600  .........C...s..
+000003a0: 0000 7400 8300 8201 2901 61e9 0300 000a  ..t.....).a.....
+000003b0: 2020 2020 2020 2020 2a2a 486f 7720 7468          **How th
+000003c0: 6520 6c69 7374 206f 6620 6772 6164 6965  e list of gradie
+000003d0: 6e74 7320 7368 6f75 6c64 206c 6f6f 6b20  nts should look 
+000003e0: 6c69 6b65 2a2a 0a0a 2020 2020 2020 2020  like**..        
+000003f0: 4173 7375 6d69 6e67 206f 7574 7075 7420  Assuming output 
+00000400: 6469 6d65 6e73 696f 6e20 482c 206e 756d  dimension H, num
+00000410: 6265 7220 6f66 206e 6f64 6573 2056 2c20  ber of nodes V, 
+00000420: 6e6f 6465 2066 6561 7475 7265 7320 4e20  node features N 
+00000430: 616e 6420 6261 7463 6820 7369 7a65 2042  and batch size B
+00000440: 2c20 6173 2077 656c 6c20 6173 2074 6865  , as well as the
+00000450: 0a20 2020 2020 2020 206e 756d 6265 7220  .        number 
+00000460: 6f66 2063 6f6e 766f 6c75 7469 6f6e 616c  of convolutional
+00000470: 206c 6179 6572 7320 4c20 696e 2074 6865   layers L in the
+00000480: 206e 6574 776f 726b 2e0a 0a20 2020 2020   network...     
+00000490: 2020 2054 6865 206c 6973 7420 7368 6f75     The list shou
+000004a0: 6c64 2063 6f6e 7369 7374 206f 6620 4c2b  ld consist of L+
+000004b0: 3120 656c 656d 656e 7473 2c20 7768 6572  1 elements, wher
+000004c0: 6520 7468 6520 6669 7273 7420 656c 656d  e the first elem
+000004d0: 656e 7420 6973 2061 6c77 6179 7320 7468  ent is always th
+000004e0: 6520 6772 6164 6965 6e74 7320 7769 7468  e gradients with
+000004f0: 2072 6573 7065 6374 0a20 2020 2020 2020   respect.       
+00000500: 2074 6f20 7468 6520 696e 7075 7420 616e   to the input an
+00000510: 6420 6166 7465 7220 7468 6174 2074 6865  d after that the
+00000520: 2067 7261 6469 656e 7473 206f 6620 7468   gradients of th
+00000530: 6520 696e 7465 726d 6564 6961 7465 206e  e intermediate n
+00000540: 6f64 652f 6564 6765 2065 6d62 6564 6469  ode/edge embeddi
+00000550: 6e67 732e 0a0a 2020 2020 2020 2020 4561  ngs...        Ea
+00000560: 6368 2065 6c65 6d65 6e74 2073 686f 756c  ch element shoul
+00000570: 6420 6265 2061 2072 6167 6765 6420 7465  d be a ragged te
+00000580: 6e73 6f72 2077 6974 6820 7468 6520 6469  nsor with the di
+00000590: 6d65 6e73 696f 6e20 285b 425d 2c20 5b56  mension ([B], [V
+000005a0: 5d2c 204e 2c20 4829 0a0a 2020 2020 2020  ], N, H)..      
+000005b0: 2020 3a72 6574 7572 6e3a 2054 6869 7320    :return: This 
+000005c0: 6861 7320 746f 2062 6520 6120 7475 706c  has to be a tupl
+000005d0: 6520 6f66 2066 6f75 7220 7661 6c75 6573  e of four values
+000005e0: 3a0a 2020 2020 2020 2020 2020 2020 2d20  :.            - 
+000005f0: 5468 6520 6d61 696e 206f 7574 7075 7420  The main output 
+00000600: 7072 6564 6963 7469 6f6e 2022 7922 206f  prediction "y" o
+00000610: 6620 7468 6520 6d6f 6465 6c0a 2020 2020  f the model.    
+00000620: 2020 2020 2020 2020 2d20 4120 6c69 7374          - A list
+00000630: 2063 6f6e 7461 696e 696e 6720 7468 6520   containing the 
+00000640: 6772 6164 6965 6e74 7320 6f66 2074 6865  gradients of the
+00000650: 2069 6e70 7574 2061 7320 7765 6c6c 2061   input as well a
+00000660: 7320 7468 6520 696e 7465 726d 6564 6961  s the intermedia
+00000670: 7465 206e 6f64 6528 2129 2065 6d62 6564  te node(!) embed
+00000680: 6469 6e67 730a 2020 2020 2020 2020 2020  dings.          
+00000690: 2020 2020 772e 722e 7420 746f 2074 6865      w.r.t to the
+000006a0: 206f 7574 7075 7420 2279 222e 0a20 2020   output "y"..   
+000006b0: 2020 2020 2020 2020 202d 2041 206c 6973           - A lis
+000006c0: 7420 636f 6e74 6169 6e69 6e67 2074 6865  t containing the
+000006d0: 2067 7261 6469 656e 7473 206f 6620 7468   gradients of th
+000006e0: 6520 696e 7075 7420 6173 2077 656c 6c20  e input as well 
+000006f0: 6173 2074 6865 2069 6e74 6572 6d65 6469  as the intermedi
+00000700: 6174 6520 6564 6765 2821 2920 656d 6265  ate edge(!) embe
+00000710: 6464 696e 6773 0a20 2020 2020 2020 2020  ddings.         
+00000720: 2020 2020 2077 2e72 2e74 2074 6f20 7468       w.r.t to th
+00000730: 6520 6f75 7470 7574 2022 7922 2e0a 2020  e output "y"..  
+00000740: 2020 2020 2020 2020 2020 2d20 5468 6520            - The 
+00000750: 6772 6164 6965 6e74 2074 6170 6520 7573  gradient tape us
+00000760: 6564 2074 6f20 6372 6561 7465 2074 6865  ed to create the
+00000770: 2070 7265 7669 6f75 736c 7920 6d65 6e74   previously ment
+00000780: 696f 6e65 6420 6772 6164 6965 6e74 730a  ioned gradients.
+00000790: 2020 2020 2020 2020 2901 da13 4e6f 7449          )...NotI
+000007a0: 6d70 6c65 6d65 6e74 6564 4572 726f 7229  mplementedError)
+000007b0: 03da 0473 656c 66da 0669 6e70 7574 73da  ...self..inputs.
+000007c0: 0874 7261 696e 696e 67a9 0072 0c00 0000  .training..r....
+000007d0: fa59 2f6d 6564 6961 2f73 7364 2f50 726f  .Y/media/ssd/Pro
+000007e0: 6772 616d 6d69 6e67 2f67 7261 7068 5f61  gramming/graph_a
+000007f0: 7474 656e 7469 6f6e 5f73 7475 6465 6e74  ttention_student
+00000800: 2f67 7261 7068 5f61 7474 656e 7469 6f6e  /graph_attention
+00000810: 5f73 7475 6465 6e74 2f6d 6f64 656c 732f  _student/models/
+00000820: 6772 6164 6965 6e74 2e70 79da 1363 616c  gradient.py..cal
+00000830: 6c5f 7769 7468 5f67 7261 6469 656e 7473  l_with_gradients
+00000840: 1300 0000 7302 0000 0006 147a 2941 6273  ....s......z)Abs
+00000850: 7472 6163 7447 7261 6469 656e 744d 6f64  tractGradientMod
+00000860: 656c 2e63 616c 6c5f 7769 7468 5f67 7261  el.call_with_gra
+00000870: 6469 656e 7473 6303 0000 0000 0000 0000  dientsc.........
+00000880: 0000 0009 0000 0004 0000 004f 0000 0073  ...........O...s
+00000890: 2600 0000 7c00 6a00 7c01 7c02 6702 7c03  &...|.j.|.|.g.|.
+000008a0: a201 5200 6900 7c04 a401 8e01 5c04 7d05  ..R.i.|.....\.}.
+000008b0: 7d06 7d07 7d08 7c05 5300 a901 4ea9 0172  }.}.}.|.S...N..r
+000008c0: 0e00 0000 2909 7209 0000 0072 0a00 0000  ....).r....r....
+000008d0: 720b 0000 00da 0461 7267 73da 066b 7761  r......args..kwa
+000008e0: 7267 73da 0179 da0e 6e6f 6465 5f67 7261  rgs..y..node_gra
+000008f0: 6469 656e 7473 da0e 6564 6765 5f67 7261  dients..edge_gra
+00000900: 6469 656e 7473 da04 7461 7065 720c 0000  dients..taper...
+00000910: 0072 0c00 0000 720d 0000 00da 0463 616c  .r....r......cal
+00000920: 6c29 0000 0073 0400 0000 2201 0401 7a1a  l)...s...."...z.
+00000930: 4162 7374 7261 6374 4772 6164 6965 6e74  AbstractGradient
+00000940: 4d6f 6465 6c2e 6361 6c6c da04 6f75 7473  Model.call..outs
+00000950: da0b 6163 7469 7661 7469 6f6e 7372 1600  ..activationsr..
+00000960: 0000 6305 0000 0000 0000 0000 0000 000c  ..c.............
+00000970: 0000 0007 0000 0043 0000 0073 aa00 0000  .......C...s....
+00000980: 6700 7d05 7c02 4400 5d4e 7d06 6700 7d07  g.}.|.D.]N}.g.}.
+00000990: 7400 7c04 8301 4400 5d30 7d08 6700 7d09  t.|...D.]0}.g.}.
+000009a0: 7c01 7c08 1900 4400 5d14 7d0a 7c03 a001  |.|...D.].}.|...
+000009b0: 7c0a 7c06 a102 7d0b 7402 6a03 7c0b 6401  |.|...}.t.j.|.d.
+000009c0: 6402 8d02 7d0b 7c09 a004 7c0b a101 0100  d...}.|...|.....
+000009d0: 7114 7402 6a05 7c09 6401 6402 8d02 7d09  q.t.j.|.d.d...}.
+000009e0: 7402 6a03 7c09 6403 6402 8d02 7d09 7c07  t.j.|.d.d...}.|.
+000009f0: a004 7c09 a101 0100 710c 7402 6a05 7c07  ..|.....q.t.j.|.
+00000a00: 6403 6402 8d02 7d07 7402 6a06 7c07 6403  d.d...}.t.j.|.d.
+00000a10: 6402 8d02 7d07 7c05 a004 7c06 7c07 6602  d...}.|...|.|.f.
+00000a20: a101 0100 7104 7c05 5300 2904 61ff 0800  ....q.|.S.).a...
+00000a30: 000a 2020 2020 2020 2020 5468 6973 206d  ..        This m
+00000a40: 6574 686f 6420 6973 2061 2062 6f69 6c65  ethod is a boile
+00000a50: 7270 6c61 7465 2069 6d70 6c65 6d65 6e74  rplate implement
+00000a60: 6174 696f 6e20 7468 6174 2077 696c 6c20  ation that will 
+00000a70: 6361 6c63 756c 6174 6520 7468 6520 6772  calculate the gr
+00000a80: 6164 6965 6e74 2069 6e66 6f20 6c69 7374  adient info list
+00000a90: 2c20 6769 7665 6e20 6120 6c69 7374 0a20  , given a list. 
+00000aa0: 2020 2020 2020 206f 6620 6d6f 6465 6c20         of model 
+00000ab0: 6f75 7470 7574 732c 2061 206c 6973 7420  outputs, a list 
+00000ac0: 6f66 206c 6179 6572 2061 6374 6976 6174  of layer activat
+00000ad0: 696f 6e20 7465 6e73 6f72 732c 2074 6865  ion tensors, the
+00000ae0: 2067 7261 6469 656e 7420 7461 7065 2061   gradient tape a
+00000af0: 6e64 2074 6865 2062 6174 6368 2073 697a  nd the batch siz
+00000b00: 652e 0a0a 2020 2020 2020 2020 4173 7375  e...        Assu
+00000b10: 6d69 6e67 2074 6865 2066 6f6c 6c6f 7769  ming the followi
+00000b20: 6e67 2076 6172 6961 626c 6573 3a0a 2020  ng variables:.  
+00000b30: 2020 2020 2020 2d20 423a 2062 6174 6368        - B: batch
+00000b40: 2064 696d 656e 7369 6f6e 0a20 2020 2020   dimension.     
+00000b50: 2020 202d 204f 3a20 6f75 7470 7574 2064     - O: output d
+00000b60: 696d 656e 7369 6f6e 0a20 2020 2020 2020  imension.       
+00000b70: 202d 204c 3a20 6e75 6d62 6572 206f 6620   - L: number of 
+00000b80: 636f 6e76 6f6c 7574 696f 6e61 6c20 6c61  convolutional la
+00000b90: 7965 7273 202f 206e 756d 6265 7220 6f66  yers / number of
+00000ba0: 2069 6e74 6572 6d65 6469 6174 6520 656d   intermediate em
+00000bb0: 6265 6464 696e 6773 2077 2e72 2e74 2077  beddings w.r.t w
+00000bc0: 6869 6368 2074 6865 2067 7261 6469 656e  hich the gradien
+00000bd0: 7473 0a20 2020 2020 2020 2020 2020 2061  ts.            a
+00000be0: 7265 2074 6f20 6265 2063 616c 6375 6c61  re to be calcula
+00000bf0: 7465 640a 2020 2020 2020 2020 2d20 563a  ted.        - V:
+00000c00: 204e 6f64 6520 6f72 2065 6467 6520 7368   Node or edge sh
+00000c10: 6170 650a 2020 2020 2020 2020 2d20 463a  ape.        - F:
+00000c20: 2046 6561 7475 7265 2073 6861 7065 0a0a   Feature shape..
+00000c30: 2020 2020 2020 2020 3a70 6172 616d 206f          :param o
+00000c40: 7574 733a 2054 6869 7320 6973 2073 7570  uts: This is sup
+00000c50: 706f 7365 6420 746f 2062 6520 6120 6c69  posed to be a li
+00000c60: 7374 206f 6620 6c69 7374 7320 6f66 207a  st of lists of z
+00000c70: 6572 6f20 6469 6d65 6e73 696f 6e61 6c20  ero dimensional 
+00000c80: 7465 6e73 6f72 732e 2047 656e 6572 616c  tensors. General
+00000c90: 6c79 2c20 7468 650a 2020 2020 2020 2020  ly, the.        
+00000ca0: 2020 2020 6f75 7470 7574 206f 6620 6120      output of a 
+00000cb0: 7265 6772 6573 7369 6f6e 202f 2063 6c61  regression / cla
+00000cc0: 7373 6966 6963 6174 696f 6e20 6e65 7477  ssification netw
+00000cd0: 6f72 6b20 7769 6c6c 2062 6520 6120 7665  ork will be a ve
+00000ce0: 6374 6f72 206f 6620 7368 6170 6520 285b  ctor of shape ([
+00000cf0: 425d 2c20 4f29 2e20 5468 6973 206c 6973  B], O). This lis
+00000d00: 740a 2020 2020 2020 2020 2020 2020 6861  t.            ha
+00000d10: 7320 746f 2062 6173 6963 616c 6c79 2062  s to basically b
+00000d20: 6520 7468 6973 2074 656e 736f 7220 6f6e  e this tensor on
+00000d30: 6c79 2069 6e20 6c69 7374 2066 6f72 6d61  ly in list forma
+00000d40: 742e 2054 6869 7320 6c69 7374 2073 686f  t. This list sho
+00000d50: 756c 6420 6265 2063 7265 6174 6564 2062  uld be created b
+00000d60: 7920 6170 706c 7969 6e67 0a20 2020 2020  y applying.     
+00000d70: 2020 2020 2020 2074 6865 2063 6f72 7265         the corre
+00000d80: 7370 6f6e 6469 6e67 2069 6e64 6578 696e  sponding indexin
+00000d90: 6720 736c 6963 6573 2074 6f20 7468 6520  g slices to the 
+00000da0: 6f75 7470 7574 2076 6563 746f 7220 746f  output vector to
+00000db0: 2073 706c 6974 2069 7420 696e 746f 2074   split it into t
+00000dc0: 6865 206e 6573 7465 6420 666f 726d 6174  he nested format
+00000dd0: 206f 660a 2020 2020 2020 2020 2020 2020   of.            
+00000de0: 7a65 726f 2064 696d 656e 7369 6f6e 616c  zero dimensional
+00000df0: 2074 656e 736f 7220 6f62 6a65 6374 732e   tensor objects.
+00000e00: 204e 6f74 6520 7468 6174 2074 6869 7320   Note that this 
+00000e10: 696e 6465 7869 6e67 206f 7065 7261 7469  indexing operati
+00000e20: 6f6e 2068 6173 2074 6f20 6265 2064 6f6e  on has to be don
+00000e30: 6520 494e 5349 4445 2074 6865 0a20 2020  e INSIDE the.   
+00000e40: 2020 2020 2020 2020 2067 7261 6469 656e           gradien
+00000e50: 7420 7461 7065 2063 6f6e 7465 7874 2c20  t tape context, 
+00000e60: 6f74 6865 7277 6973 6520 7468 6520 6361  otherwise the ca
+00000e70: 6c63 756c 6174 696f 6e20 6f66 2074 6865  lculation of the
+00000e80: 2067 7261 6469 656e 7473 2077 696c 6c20   gradients will 
+00000e90: 6e6f 7420 776f 726b 210a 2020 2020 2020  not work!.      
+00000ea0: 2020 3a70 6172 616d 2061 6374 6976 6174    :param activat
+00000eb0: 696f 6e73 3a20 5468 6973 2069 7320 6120  ions: This is a 
+00000ec0: 6c69 7374 2077 6974 6820 4c20 656c 656d  list with L elem
+00000ed0: 656e 7473 2c20 7768 6572 6520 6561 6368  ents, where each
+00000ee0: 2065 6c65 6d65 6e74 2069 7320 616e 2069   element is an i
+00000ef0: 6e74 6572 6d65 6469 6174 6520 6e6f 6465  ntermediate node
+00000f00: 202f 0a20 2020 2020 2020 2020 2020 2065   /.            e
+00000f10: 6467 6520 656d 6265 6464 696e 6720 7665  dge embedding ve
+00000f20: 6374 6f72 2066 726f 6d20 7468 6520 6361  ctor from the ca
+00000f30: 6c6c 2070 726f 6365 7373 206f 6620 7468  ll process of th
+00000f40: 6520 6e65 7477 6f72 6b2e 2049 6e20 7468  e network. In th
+00000f50: 6973 206d 6574 686f 6420 6f6e 6520 6772  is method one gr
+00000f60: 6164 6965 6e74 2076 6563 746f 720a 2020  adient vector.  
+00000f70: 2020 2020 2020 2020 2020 7769 6c6c 2062            will b
+00000f80: 6520 6372 6561 7465 6420 666f 7220 6561  e created for ea
+00000f90: 6368 206f 6620 7468 6520 6f75 7470 7574  ch of the output
+00000fa0: 7320 772e 722e 7420 746f 2065 6163 6820  s w.r.t to each 
+00000fb0: 6f66 2074 6865 7365 2065 6d62 6564 6469  of these embeddi
+00000fc0: 6e67 732e 2054 6865 2072 6573 756c 7469  ngs. The resulti
+00000fd0: 6e67 0a20 2020 2020 2020 2020 2020 2067  ng.            g
+00000fe0: 7261 6469 656e 7420 7465 6e73 6f72 7320  radient tensors 
+00000ff0: 7769 6c6c 2068 6176 6520 7468 6520 7361  will have the sa
+00001000: 6d65 2073 6861 7065 2061 7320 7468 6520  me shape as the 
+00001010: 656d 6265 6464 696e 6773 210a 2020 2020  embeddings!.    
+00001020: 2020 2020 3a70 6172 616d 2074 6170 653a      :param tape:
+00001030: 2054 6865 2047 7261 6469 656e 7454 6170   The GradientTap
+00001040: 6520 7768 6963 6820 7761 7320 7573 6564  e which was used
+00001050: 2064 7572 696e 6720 7468 6520 6361 6c6c   during the call
+00001060: 2070 726f 6365 7373 2e0a 2020 2020 2020   process..      
+00001070: 2020 3a70 6172 616d 2062 6174 6368 5f73    :param batch_s
+00001080: 697a 653a 2054 6865 2062 6174 6368 2073  ize: The batch s
+00001090: 697a 6520 4220 7468 6174 2077 6173 2075  ize B that was u
+000010a0: 7365 6420 746f 206f 6274 6169 6e20 7468  sed to obtain th
+000010b0: 6520 6f75 7470 7574 7320 616e 6420 7468  e outputs and th
+000010c0: 6520 656d 6265 6464 696e 6773 2e20 5468  e embeddings. Th
+000010d0: 6973 2068 6173 0a20 2020 2020 2020 2020  is has.         
+000010e0: 2020 2074 6f20 6265 2065 7861 6374 6c79     to be exactly
+000010f0: 2063 6f72 7265 6374 210a 2020 2020 2020   correct!.      
+00001100: 2020 3a72 6574 7572 6e3a 2041 206c 6973    :return: A lis
+00001110: 7420 6f66 2074 7570 6c65 7320 7769 7468  t of tuples with
+00001120: 2074 6865 206c 656e 6774 6820 4c2e 2045   the length L. E
+00001130: 6163 6820 7475 706c 6520 636f 6e74 6169  ach tuple contai
+00001140: 6e73 2074 776f 2065 6c65 6d65 6e74 732e  ns two elements.
+00001150: 2054 6865 2066 6972 7374 206f 6e65 2069   The first one i
+00001160: 7320 7468 650a 2020 2020 2020 2020 2020  s the.          
+00001170: 2020 6578 6163 7420 7361 6d65 2065 6d62    exact same emb
+00001180: 6564 6469 6e67 2074 656e 736f 7220 7468  edding tensor th
+00001190: 6174 2077 6173 2070 6173 7365 6420 746f  at was passed to
+000011a0: 2074 6865 206d 6574 686f 6420 696e 2074   the method in t
+000011b0: 6865 2022 6163 7469 7661 7469 6f6e 7322  he "activations"
+000011c0: 2070 6172 616d 6574 6572 2e0a 2020 2020   parameter..    
+000011d0: 2020 2020 2020 2020 5468 6973 2074 656e          This ten
+000011e0: 736f 7220 6861 7320 7468 6520 7368 6170  sor has the shap
+000011f0: 6520 285b 425d 2c20 5b56 5d2c 2046 292e  e ([B], [V], F).
+00001200: 2054 6865 2073 6563 6f6e 6420 656c 656d   The second elem
+00001210: 656e 7420 6973 2074 6865 2063 6f72 7265  ent is the corre
+00001220: 7370 6f6e 6469 6e67 2067 7261 6469 656e  sponding gradien
+00001230: 740a 2020 2020 2020 2020 2020 2020 7465  t.            te
+00001240: 6e73 6f72 2074 6861 7420 7761 7320 6372  nsor that was cr
+00001250: 6561 7465 6420 666f 7220 7468 6174 2076  eated for that v
+00001260: 6572 7920 656d 6265 6464 696e 6720 7769  ery embedding wi
+00001270: 7468 2074 6865 2073 6861 7065 2028 5b42  th the shape ([B
+00001280: 5d2c 205b 565d 2c20 462c 204f 292e 204e  ], [V], F, O). N
+00001290: 6f74 6520 7468 6174 2074 6865 0a20 2020  ote that the.   
+000012a0: 2020 2020 2020 2020 2067 7261 6469 656e           gradien
+000012b0: 7420 6861 7320 616e 2061 6464 6974 696f  t has an additio
+000012c0: 6e61 6c20 6469 6d65 6e73 696f 6e20 666f  nal dimension fo
+000012d0: 7220 7468 6520 6f75 7470 7574 2073 6861  r the output sha
+000012e0: 7065 2e20 5468 6973 2069 7320 6265 6361  pe. This is beca
+000012f0: 7573 6520 6772 6164 6965 6e74 7320 6172  use gradients ar
+00001300: 650a 2020 2020 2020 2020 2020 2020 6372  e.            cr
+00001310: 6561 7465 6420 666f 7220 6576 6572 7920  eated for every 
+00001320: 6f75 7470 7574 2e0a 2020 2020 2020 2020  output..        
+00001330: e9fe ffff ffa9 01da 0461 7869 73e9 ffff  .........axis...
+00001340: ffff 2907 da05 7261 6e67 65da 0867 7261  ..)...range..gra
+00001350: 6469 656e 74da 0274 66da 0b65 7870 616e  dient..tf..expan
+00001360: 645f 6469 6d73 da06 6170 7065 6e64 da06  d_dims..append..
+00001370: 636f 6e63 6174 da0a 7265 6475 6365 5f73  concat..reduce_s
+00001380: 756d 290c 7209 0000 0072 1800 0000 7219  um).r....r....r.
+00001390: 0000 0072 1600 0000 da0a 6261 7463 685f  ...r......batch_
+000013a0: 7369 7a65 da0d 6772 6164 6965 6e74 5f69  size..gradient_i
+000013b0: 6e66 6fda 0a61 6374 6976 6174 696f 6eda  nfo..activation.
+000013c0: 0967 7261 6469 656e 7473 da01 62da 0e67  .gradients..b..g
+000013d0: 7261 6469 656e 745f 7374 6163 6bda 036f  radient_stack..o
+000013e0: 7574 721f 0000 0072 0c00 0000 720c 0000  utr....r....r...
+000013f0: 0072 0d00 0000 da17 6361 6c63 756c 6174  .r......calculat
+00001400: 655f 6772 6164 6965 6e74 5f69 6e66 6f2d  e_gradient_info-
+00001410: 0000 0073 2000 0000 0425 0801 0401 0c01  ...s ....%......
+00001420: 0407 0c01 0c08 0e01 0c01 0e05 0e01 0c02  ................
+00001430: 0e03 0e04 1001 0402 7a2d 4162 7374 7261  ........z-Abstra
+00001440: 6374 4772 6164 6965 6e74 4d6f 6465 6c2e  ctGradientModel.
+00001450: 6361 6c63 756c 6174 655f 6772 6164 6965  calculate_gradie
+00001460: 6e74 5f69 6e66 6f4e 2901 5429 0cda 085f  nt_infoN).T)..._
+00001470: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
+00001480: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
+00001490: 5fda 075f 5f64 6f63 5f5f 720e 0000 0072  _..__doc__r....r
+000014a0: 1700 0000 da01 74da 044c 6973 7472 2000  ......t..Listr .
+000014b0: 0000 da06 5465 6e73 6f72 da0c 4772 6164  ....Tensor..Grad
+000014c0: 6965 6e74 5461 7065 722c 0000 0072 0c00  ientTaper,...r..
+000014d0: 0000 720c 0000 0072 0c00 0000 720d 0000  ..r....r....r...
+000014e0: 0072 0700 0000 0b00 0000 7316 0000 0008  .r........s.....
+000014f0: 0004 010a 070a 1602 0410 0102 ff0a 0202  ................
+00001500: fe04 030e fd72 0700 0000 6300 0000 0000  .....r....c.....
+00001510: 0000 0000 0000 0000 0000 000d 0000 0040  ...............@
+00001520: 0000 0073 6400 0000 6500 5a01 6400 5a02  ...sd...e.Z.d.Z.
+00001530: 6401 6402 8400 6403 6404 6603 6405 6503  d.d...d.d.f.d.e.
+00001540: 6406 6504 6a05 6503 1900 6407 6504 6a05  d.e.j.e...d.e.j.
+00001550: 6503 1900 6408 6504 6a06 6409 6507 640a  e...d.e.j.d.e.d.
+00001560: 6507 660c 640b 640c 8405 5a08 6414 640f  e.f.d.d...Z.d.d.
+00001570: 6410 8401 5a09 090d 090e 090d 0911 6415  d...Z.........d.
+00001580: 6412 6413 8401 5a0a 640e 5300 2916 da10  d.d...Z.d.S.)...
+00001590: 4763 6e47 7261 6469 656e 744d 6f64 656c  GcnGradientModel
+000015a0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+000015b0: 0003 0000 0043 0000 0073 0a00 0000 7400  .....C...s....t.
+000015c0: 7c00 6401 8d01 5300 2902 4ea9 01da 0575  |.d...S.).N....u
+000015d0: 6e69 7473 7202 0000 0072 3600 0000 720c  nitsr....r6...r.
+000015e0: 0000 0072 0c00 0000 720d 0000 00da 083c  ...r....r......<
+000015f0: 6c61 6d62 6461 3e82 0000 0073 0200 0000  lambda>....s....
+00001600: 0a00 7a19 4763 6e47 7261 6469 656e 744d  ..z.GcnGradientM
+00001610: 6f64 656c 2e3c 6c61 6d62 6461 3eda 046d  odel.<lambda>..m
+00001620: 6561 6eda 066c 696e 6561 7272 2500 0000  ean..linearr%...
+00001630: 7237 0000 00da 0b66 696e 616c 5f75 6e69  r7.....final_uni
+00001640: 7473 da08 6c61 7965 725f 6362 da0e 706f  ts..layer_cb..po
+00001650: 6f6c 696e 675f 6d65 7468 6f64 da10 6669  oling_method..fi
+00001660: 6e61 6c5f 6163 7469 7661 7469 6f6e 6307  nal_activationc.
+00001670: 0000 0000 0000 0000 0000 000a 0000 0005  ................
+00001680: 0000 0043 0000 0073 b600 0000 7400 a001  ...C...s....t...
+00001690: 7c00 a101 0100 7402 a001 7c00 a101 0100  |.....t...|.....
+000016a0: 7c01 7c00 5f03 7c02 7c00 5f04 7c03 6401  |.|._.|.|._.|.d.
+000016b0: 1900 7c00 5f05 6700 7c00 5f06 7c00 6a04  ..|._.g.|._.|.j.
+000016c0: 4400 5d0c 7d07 7c04 7c07 8301 7d08 7c00  D.].}.|.|...}.|.
+000016d0: 6a06 a007 7c08 a101 0100 711b 7408 7c05  j...|.....q.t.|.
+000016e0: 6402 8d01 7c00 5f09 7c03 7c00 5f0a 6403  d...|._.|.|._.d.
+000016f0: 6404 8400 7c03 4400 8301 7c00 5f0b 7c06  d...|.D...|._.|.
+00001700: 7c00 6a0b 6401 3c00 6700 7c00 5f0c 740d  |.j.d.<.g.|._.t.
+00001710: 7c00 6a0a 7c00 6a0b 8302 4400 5d10 5c02  |.j.|.j...D.].\.
+00001720: 7d07 7d09 740e 7c07 7c09 6405 8d02 7d08  }.}.t.|.|.d...}.
+00001730: 7c00 6a0c a007 7c08 a101 0100 7148 6400  |.j...|.....qHd.
+00001740: 5300 2906 4e72 1d00 0000 2901 723d 0000  S.).Nr....).r=..
+00001750: 0063 0100 0000 0000 0000 0000 0000 0200  .c..............
+00001760: 0000 0300 0000 5300 0000 7310 0000 0067  ......S...s....g
+00001770: 007c 005d 047d 0164 0091 0271 0253 0029  .|.].}.d...q.S.)
+00001780: 017a 106b 6763 6e6e 3e6c 6561 6b79 5f72  .z.kgcnn>leaky_r
+00001790: 656c 7572 0c00 0000 2902 da02 2e30 da01  elur....)....0..
+000017a0: 5f72 0c00 0000 720c 0000 0072 0d00 0000  _r....r....r....
+000017b0: da0a 3c6c 6973 7463 6f6d 703e 9400 0000  ..<listcomp>....
+000017c0: 7302 0000 0010 007a 2d47 636e 4772 6164  s......z-GcnGrad
+000017d0: 6965 6e74 4d6f 6465 6c2e 5f5f 696e 6974  ientModel.__init
+000017e0: 5f5f 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973  __.<locals>.<lis
+000017f0: 7463 6f6d 703e 2902 7237 0000 0072 2700  tcomp>).r7...r'.
+00001800: 0000 290f 7207 0000 00da 085f 5f69 6e69  ..).r......__ini
+00001810: 745f 5f72 0600 0000 7225 0000 0072 3700  t__r....r%...r7.
+00001820: 0000 da0b 6e75 6d5f 6f75 7470 7574 73da  ....num_outputs.
+00001830: 0b63 6f6e 765f 6c61 7965 7273 7222 0000  .conv_layersr"..
+00001840: 0072 0500 0000 da0b 6c61 795f 706f 6f6c  .r......lay_pool
+00001850: 696e 6772 3b00 0000 da0a 6669 6e61 6c5f  ingr;.....final_
+00001860: 6163 7473 da0c 6669 6e61 6c5f 6c61 7965  acts..final_laye
+00001870: 7273 da03 7a69 7072 0400 0000 290a 7209  rs..zipr....).r.
+00001880: 0000 0072 2500 0000 7237 0000 0072 3b00  ...r%...r7...r;.
+00001890: 0000 723c 0000 0072 3d00 0000 723e 0000  ..r<...r=...r>..
+000018a0: 00da 016b da03 6c61 79da 0361 6374 720c  ...k..lay..actr.
+000018b0: 0000 0072 0c00 0000 720d 0000 0072 4200  ...r....r....rB.
+000018c0: 0000 7e00 0000 7324 0000 000a 070a 0106  ..~...s$........
+000018d0: 0206 010a 0106 020a 0108 010e 010c 0206  ................
+000018e0: 0210 010a 0106 0116 010c 010e 0104 fe7a  ...............z
+000018f0: 1947 636e 4772 6164 6965 6e74 4d6f 6465  .GcnGradientMode
+00001900: 6c2e 5f5f 696e 6974 5f5f 544e 6305 0000  l.__init__TNc...
+00001910: 0000 0000 0000 0000 0011 0000 0008 0000  ................
+00001920: 0003 0000 0073 1201 0000 7c04 6400 7500  .....s....|.d.u.
+00001930: 7207 8801 6a00 7d04 7c01 5c03 7d05 7d06  r...j.}.|.\.}.}.
+00001940: 7d07 7c05 7d08 7401 6a02 6401 6402 8d01  }.|.}.t.j.d.d...
+00001950: 8f50 7d09 7c09 a003 7c05 a101 0100 7c09  .P}.|...|.....|.
+00001960: a003 7c06 a101 0100 7c06 6701 7d0a 7c08  ..|.....|.g.}.|.
+00001970: 6701 7d0b 8801 6a04 4400 5d0e 7d0c 7c0c  g.}...j.D.].}.|.
+00001980: 7c08 7c06 7c07 6703 8301 7d08 7c0b a005  |.|.|.g...}.|...
+00001990: 7c08 a101 0100 7128 8801 a006 7c08 a101  |.....q(....|...
+000019a0: 8900 8801 6a07 4400 5d06 7d0c 7c0c 8800  ....j.D.].}.|...
+000019b0: 8301 8900 713f 8700 6601 6403 6404 8408  ....q?..f.d.d...
+000019c0: 7408 7c04 8301 4400 8301 7d0d 8700 8701  t.|...D...}.....
+000019d0: 6602 6405 6404 8408 7408 7c04 8301 4400  f.d.d...t.|...D.
+000019e0: 8301 7d0e 5700 6400 0400 0400 8303 0100  ..}.W.d.........
+000019f0: 6e08 3100 7367 7701 0100 0100 0100 5900  n.1.sgw.......Y.
+00001a00: 0100 7c03 727f 8801 a009 7c0e 7c0a 7c09  ..|.r.....|.|.|.
+00001a10: 7c04 a104 7d0f 8801 a009 7c0e 7c0b 7c09  |...}.....|.|.|.
+00001a20: 7c04 a104 7d10 6e04 6700 7d10 6700 7d0f  |...}.n.g.}.g.}.
+00001a30: 8800 7c10 7c0f 7c09 6604 5300 2906 4e54  ..|.|.|.f.S.).NT
+00001a40: 2901 da0a 7065 7273 6973 7465 6e74 6301  )...persistentc.
+00001a50: 0000 0000 0000 0000 0000 0002 0000 0006  ................
+00001a60: 0000 0013 0000 0073 1c00 0000 6700 7c00  .......s....g.|.
+00001a70: 5d0a 7d01 8800 7c01 6400 6400 8502 6602  ].}...|.d.d...f.
+00001a80: 1900 9102 7102 5300 720f 0000 0072 0c00  ....q.S.r....r..
+00001a90: 0000 2902 723f 0000 0072 2900 0000 2901  ..).r?...r)...).
+00001aa0: 722b 0000 0072 0c00 0000 720d 0000 0072  r+...r....r....r
+00001ab0: 4100 0000 b100 0000 7302 0000 001c 007a  A.......s......z
+00001ac0: 3847 636e 4772 6164 6965 6e74 4d6f 6465  8GcnGradientMode
+00001ad0: 6c2e 6361 6c6c 5f77 6974 685f 6772 6164  l.call_with_grad
+00001ae0: 6965 6e74 732e 3c6c 6f63 616c 733e 2e3c  ients.<locals>.<
+00001af0: 6c69 7374 636f 6d70 3e63 0100 0000 0000  listcomp>c......
+00001b00: 0000 0000 0000 0100 0000 0500 0000 1300  ................
+00001b10: 0000 7326 0000 0067 007c 005d 0f89 0087  ..s&...g.|.]....
+00001b20: 0087 0166 0264 0064 0184 0874 0088 026a  ...f.d.d...t...j
+00001b30: 0183 0144 0083 0191 0271 0253 0029 0263  ...D.....q.S.).c
+00001b40: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00001b50: 0500 0000 1300 0000 7318 0000 0067 007c  ........s....g.|
+00001b60: 005d 087d 0188 0188 007c 0166 0219 0091  .].}.....|.f....
+00001b70: 0271 0253 0072 0c00 0000 720c 0000 0029  .q.S.r....r....)
+00001b80: 0272 3f00 0000 da01 6f29 0272 2900 0000  .r?.....o).r)...
+00001b90: 722b 0000 0072 0c00 0000 720d 0000 0072  r+...r....r....r
+00001ba0: 4100 0000 b200 0000 7302 0000 0018 007a  A.......s......z
+00001bb0: 4347 636e 4772 6164 6965 6e74 4d6f 6465  CGcnGradientMode
+00001bc0: 6c2e 6361 6c6c 5f77 6974 685f 6772 6164  l.call_with_grad
+00001bd0: 6965 6e74 732e 3c6c 6f63 616c 733e 2e3c  ients.<locals>.<
+00001be0: 6c69 7374 636f 6d70 3e2e 3c6c 6973 7463  listcomp>.<listc
+00001bf0: 6f6d 703e 2902 721e 0000 0072 4300 0000  omp>).r....rC...
+00001c00: 2901 723f 0000 00a9 0272 2b00 0000 7209  ).r?.....r+...r.
+00001c10: 0000 0029 0172 2900 0000 720d 0000 0072  ...).r)...r....r
+00001c20: 4100 0000 b200 0000 7302 0000 0026 0029  A.......s....&.)
+00001c30: 0a72 2500 0000 7220 0000 0072 3400 0000  .r%...r ...r4...
+00001c40: da05 7761 7463 6872 4400 0000 7222 0000  ..watchrD...r"..
+00001c50: 0072 4500 0000 7247 0000 0072 1e00 0000  .rE...rG...r....
+00001c60: 722c 0000 0029 1172 0900 0000 720a 0000  r,...).r....r...
+00001c70: 0072 0b00 0000 da10 6372 6561 7465 5f67  .r......create_g
+00001c80: 7261 6469 656e 7473 7225 0000 00da 0a6e  radientsr%.....n
+00001c90: 6f64 655f 696e 7075 74da 0a65 6467 655f  ode_input..edge_
+00001ca0: 696e 7075 74da 1065 6467 655f 696e 6465  input..edge_inde
+00001cb0: 785f 696e 7075 74da 0178 7216 0000 00da  x_input..xr.....
+00001cc0: 1065 6467 655f 6163 7469 7661 7469 6f6e  .edge_activation
+00001cd0: 73da 106e 6f64 655f 6163 7469 7661 7469  s..node_activati
+00001ce0: 6f6e 7372 4a00 0000 7218 0000 00da 0a6f  onsrJ...r......o
+00001cf0: 7574 735f 6d75 6c74 69da 1265 6467 655f  uts_multi..edge_
+00001d00: 6772 6164 6965 6e74 5f69 6e66 6fda 126e  gradient_info..n
+00001d10: 6f64 655f 6772 6164 6965 6e74 5f69 6e66  ode_gradient_inf
+00001d20: 6f72 0c00 0000 724e 0000 0072 0d00 0000  or....rN...r....
+00001d30: 720e 0000 009b 0000 0073 3000 0000 0801  r........s0.....
+00001d40: 0601 0a02 0401 0e02 0a01 0a01 0602 0601  ................
+00001d50: 0a01 0e01 0c01 0a02 0a02 0a01 1602 1a01  ................
+00001d60: 1cf0 0412 1001 1201 0402 0401 0c02 7a24  ..............z$
+00001d70: 4763 6e47 7261 6469 656e 744d 6f64 656c  GcnGradientModel
+00001d80: 2e63 616c 6c5f 7769 7468 5f67 7261 6469  .call_with_gradi
+00001d90: 656e 7473 4663 0600 0000 0000 0000 0000  entsFc..........
+00001da0: 0000 0a00 0000 0600 0000 4300 0000 732c  ..........C...s,
+00001db0: 0000 007c 006a 007c 017c 027c 037c 0464  ...|.j.|.|.|.|.d
+00001dc0: 018d 045c 047d 067d 077d 087d 097c 0572  ...\.}.}.}.}.|.r
+00001dd0: 147c 067c 077c 0866 0353 007c 0653 0029  .|.|.|.f.S.|.S.)
+00001de0: 024e 2903 720b 0000 0072 2500 0000 7250  .N).r....r%...rP
+00001df0: 0000 0072 1000 0000 290a 7209 0000 0072  ...r....).r....r
+00001e00: 0a00 0000 720b 0000 0072 2500 0000 7250  ....r....r%...rP
+00001e10: 0000 00da 1072 6574 7572 6e5f 6772 6164  .....return_grad
+00001e20: 6965 6e74 7372 1300 0000 da09 6e6f 6465  ientsr......node
+00001e30: 5f69 6e66 6fda 0965 6467 655f 696e 666f  _info..edge_info
+00001e40: 7216 0000 0072 0c00 0000 720c 0000 0072  r....r....r....r
+00001e50: 0d00 0000 7217 0000 00bd 0000 0073 1200  ....r........s..
+00001e60: 0000 0406 0201 0201 0201 0201 0efc 0407  ................
+00001e70: 0a01 0402 7a15 4763 6e47 7261 6469 656e  ....z.GcnGradien
+00001e80: 744d 6f64 656c 2e63 616c 6c29 0354 544e  tModel.call).TTN
+00001e90: 2904 544e 5446 290b 722d 0000 0072 2e00  ).TNTF).r-...r..
+00001ea0: 0000 722f 0000 00da 0369 6e74 7231 0000  ..r/.....intr1..
+00001eb0: 0072 3200 0000 da08 4361 6c6c 6162 6c65  .r2.....Callable
+00001ec0: da03 7374 7272 4200 0000 720e 0000 0072  ..strrB...r....r
+00001ed0: 1700 0000 720c 0000 0072 0c00 0000 720c  ....r....r....r.
+00001ee0: 0000 0072 0d00 0000 7235 0000 007c 0000  ...r....r5...|..
+00001ef0: 0073 2e00 0000 0800 0606 0201 0201 04fa  .s..............
+00001f00: 0201 02ff 0802 02fe 0803 02fd 0404 02fc  ................
+00001f10: 0205 02fb 0206 0afa 0a1d 0224 0201 0201  ...........$....
+00001f20: 0201 0efb 7235 0000 0046 7226 0000 00da  ....r5...Fr&....
+00001f30: 0875 7365 5f72 656c 75da 0c75 7365 5f61  .use_relu..use_a
+00001f40: 6273 6f6c 7574 65da 0b75 7365 5f73 6967  bsolute..use_sig
+00001f50: 6d6f 6964 da08 6b65 6570 6469 6d73 da06  moid..keepdims..
+00001f60: 7265 7475 726e 6305 0000 0000 0000 0000  returnc.........
+00001f70: 0000 0008 0000 0006 0000 0043 0000 0073  ...........C...s
+00001f80: 5c00 0000 7c00 6401 1900 5c02 7d05 7d06  \...|.d...\.}.}.
+00001f90: 7400 6a01 7c06 7400 6a02 7c05 6402 6403  t.j.|.t.j.|.d.d.
+00001fa0: 8d02 1400 6404 7c04 6405 8d03 7d07 7c01  ....d.|.d...}.|.
+00001fb0: 721d 7403 6a04 a005 7c07 a101 7d07 7c02  r.t.j...|...}.|.
+00001fc0: 7224 7400 a006 7c07 a101 7d07 7c03 722c  r$t...|...}.|.r,
+00001fd0: 7403 6a04 a007 7c07 a101 7d07 7c07 5300  t.j...|...}.|.S.
+00001fe0: 2906 7a06 0a0a 2020 2020 7201 0000 0072  ).z...    r....r
+00001ff0: 1a00 0000 721b 0000 0072 1d00 0000 a902  ....r....r......
+00002000: 721c 0000 0072 6300 0000 2908 7220 0000  r....rc...).r ..
+00002010: 0072 2400 0000 7221 0000 00da 026b 73da  .r$...r!.....ks.
+00002020: 0762 6163 6b65 6e64 da04 7265 6c75 da03  .backend..relu..
+00002030: 6162 73da 0773 6967 6d6f 6964 2908 7226  abs..sigmoid).r&
+00002040: 0000 0072 6000 0000 7261 0000 0072 6200  ...r`...ra...rb.
+00002050: 0000 7263 0000 0072 2700 0000 7228 0000  ..rc...r'...r(..
+00002060: 00da 0b69 6d70 6f72 7461 6e63 6573 720c  ...importancesr.
+00002070: 0000 0072 0c00 0000 720d 0000 00da 1067  ...r....r......g
+00002080: 7261 645f 696d 706f 7274 616e 6365 73d0  rad_importances.
+00002090: 0000 0073 1a00 0000 0c0e 0401 1003 0201  ...s............
+000020a0: 0201 06fb 0407 0c01 0401 0a01 0401 0c01  ................
+000020b0: 0402 726c 0000 00e9 0200 0000 da0b 7573  ..rl..........us
+000020c0: 655f 6176 6572 6167 65da 0f61 7665 7261  e_average..avera
+000020d0: 6769 6e67 5f64 6570 7468 6306 0000 0000  ging_depthc.....
+000020e0: 0000 0000 0000 000b 0000 0007 0000 0043  ...............C
+000020f0: 0000 0073 a200 0000 6700 7d06 7c00 4400  ...s....g.}.|.D.
+00002100: 5d2f 5c02 7d07 7d08 7400 6a01 7c08 6401  ]/\.}.}.t.j.|.d.
+00002110: 6402 6403 8d03 7d09 7400 6a02 7c09 7400  d.d...}.t.j.|.t.
+00002120: 6a03 7c07 6404 6405 8d02 1400 6406 7c05  j.|.d.d.....d.|.
+00002130: 6403 8d03 7d0a 7c02 7227 7404 6a05 a006  d...}.|.r't.j...
+00002140: 7c0a a101 7d0a 7c03 722e 7400 a007 7c0a  |...}.|.r.t...|.
+00002150: a101 7d0a 7c06 a008 7c0a a101 0100 7104  ..}.|...|.....q.
+00002160: 7c01 7243 7400 6a09 7c06 7c04 0b00 6400  |.rCt.j.|.|...d.
+00002170: 8502 1900 6406 6405 8d02 7d06 6e04 7c06  ....d.d...}.n.|.
+00002180: 6406 1900 7d06 7400 6a01 7c06 6406 6402  d...}.t.j.|.d.d.
+00002190: 6403 8d03 7d06 7c06 5300 2907 4ee9 0100  d...}.|.S.).N...
+000021a0: 0000 5472 6500 0000 721a 0000 0072 1b00  ..Tre...r....r..
+000021b0: 0000 721d 0000 0029 0a72 2000 0000 da0b  ..r....).r .....
+000021c0: 7265 6475 6365 5f6d 6561 6e72 2400 0000  reduce_meanr$...
+000021d0: 7221 0000 0072 6600 0000 7267 0000 0072  r!...rf...rg...r
+000021e0: 6800 0000 7269 0000 0072 2200 0000 7223  h...ri...r"...r#
+000021f0: 0000 0029 0b72 2600 0000 726e 0000 0072  ...).r&...rn...r
+00002200: 6000 0000 7261 0000 0072 6f00 0000 7263  `...ra...ro...rc
+00002210: 0000 0072 6b00 0000 7227 0000 0072 2800  ...rk...r'...r(.
+00002220: 0000 da05 616c 7068 61da 116c 6f63 616c  ....alpha..local
+00002230: 5f69 6d70 6f72 7461 6e63 6573 720c 0000  _importancesr...
+00002240: 0072 0c00 0000 720d 0000 00da 1467 7261  .r....r......gra
+00002250: 645f 6361 6d5f 696d 706f 7274 616e 6365  d_cam_importance
+00002260: 73f0 0000 0073 2400 0000 0406 0c01 1005  s....s$.........
+00002270: 0401 1003 0201 0201 06fb 0408 0c01 0401  ................
+00002280: 0a01 0c02 0402 1a01 0802 1002 0401 7274  ..............rt
+00002290: 0000 0029 0446 4646 4629 0546 4646 726d  ...).FFFF).FFFrm
+000022a0: 0000 0046 291b da06 7479 7069 6e67 7231  ...F)...typingr1
+000022b0: 0000 00da 0a74 656e 736f 7266 6c6f 7772  .....tensorflowr
+000022c0: 2000 0000 da10 7465 6e73 6f72 666c 6f77   .....tensorflow
+000022d0: 2e6b 6572 6173 da05 6b65 7261 7372 6600  .keras..kerasrf.
+000022e0: 0000 da1a 6b67 636e 6e2e 6c61 7965 7273  ....kgcnn.layers
+000022f0: 2e63 6f6e 762e 6763 6e5f 636f 6e76 7203  .conv.gcn_convr.
+00002300: 0000 00da 146b 6763 6e6e 2e6c 6179 6572  .....kgcnn.layer
+00002310: 732e 6d6f 6475 6c65 7372 0400 0000 da14  s.modulesr......
+00002320: 6b67 636e 6e2e 6c61 7965 7273 2e70 6f6f  kgcnn.layers.poo
+00002330: 6c69 6e67 7205 0000 00da 1b6b 6763 6e6e  lingr......kgcnn
+00002340: 2e6c 6974 6572 6174 7572 652e 474e 4e45  .literature.GNNE
+00002350: 7870 6c61 696e 7206 0000 00da 066d 6f64  xplainr......mod
+00002360: 656c 73da 054d 6f64 656c 7207 0000 0072  els..Modelr....r
+00002370: 3500 0000 7232 0000 00da 0554 7570 6c65  5...r2.....Tuple
+00002380: 7233 0000 00da 0462 6f6f 6cda 0c52 6167  r3.....bool..Rag
+00002390: 6765 6454 656e 736f 7272 6c00 0000 725d  gedTensorrl...r]
+000023a0: 0000 0072 7400 0000 720c 0000 0072 0c00  ...rt...r....r..
+000023b0: 0000 720c 0000 0072 0d00 0000 da08 3c6d  ..r....r......<m
+000023c0: 6f64 756c 653e 0100 0000 7350 0000 0008  odule>....sP....
+000023d0: 0008 020c 010c 010c 010c 010c 0114 0312  ................
+000023e0: 7102 5502 0102 0102 011c fc02 0102 ff02  q.U.............
+000023f0: 0202 fe02 0302 fd02 0402 fc04 050a fb02  ................
+00002400: 2102 0102 0102 0102 011c fb02 0102 ff02  !...............
+00002410: 0202 fe02 0302 fd02 0402 fc02 050e fb    ...............
```

### Comparing `graph_attention_student-0.7.0/graph_attention_student/models/__pycache__/megan.cpython-310.pyc` & `graph_attention_student-0.7.1/graph_attention_student/models/__pycache__/megan.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Mar 19 09:07:02 2023 UTC, .py size: 28472 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b6d0 1664 386f 0000  o..........d8o..
+00000000: 6f0d 0d0a 0000 0000 b8d6 2264 2e6f 0000  o........."d.o..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 dc00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c04 6d05 5a06 0100 6400 6402 6c07  d.l.m.Z...d.d.l.
 00000050: 6d08 5a08 0100 6400 6403 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6404 6c0b 6d0c 5a0c 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6405 6c0b 6d0d 5a0d 6d0e 5a0e 0100 6400  d.l.m.Z.m.Z...d.
@@ -125,15 +125,15 @@
 000007c0: 6e5f 6c69 6d69 7473 da0f 7265 6772 6573  n_limits..regres
 000007d0: 7369 6f6e 5f62 696e 73da 1472 6567 7265  sion_bins..regre
 000007e0: 7373 696f 6e5f 7265 6665 7265 6e63 65da  ssion_reference.
 000007f0: 1272 6574 7572 6e5f 696d 706f 7274 616e  .return_importan
 00000800: 6365 73da 1475 7365 5f67 7261 7068 5f61  ces..use_graph_a
 00000810: 7474 7269 6275 7465 7363 1900 0000 0000  ttributesc......
 00000820: 0000 0000 0000 2000 0000 0a00 0000 4b00  ...... .......K.
-00000830: 0000 7338 0300 0074 006a 016a 026a 037c  ..s8...t.j.j.j.|
+00000830: 0000 7336 0300 0074 006a 016a 026a 037c  ..s6...t.j.j.j.|
 00000840: 0066 0169 007c 19a4 018e 0101 007c 017c  .f.i.|.......|.|
 00000850: 005f 047c 027c 005f 057c 037c 005f 067c  ._.|.|._.|.|._.|
 00000860: 047c 005f 077c 057c 005f 087c 067c 005f  .|._.|.|._.|.|._
 00000870: 097c 077c 005f 0a7c 087c 005f 0b7c 097c  .|.|._.|.|._.|.|
 00000880: 005f 0c7c 0a7c 005f 0d7c 0b7c 005f 0e7c  ._.|.|._.|.|._.|
 00000890: 0c7c 005f 0f7c 0d7c 005f 107c 0e7c 005f  .|._.|.|._.|.|._
 000008a0: 117c 107c 005f 127c 117c 005f 137c 127c  .|.|._.|.|._.|.|
@@ -162,777 +162,777 @@
 00000a10: 006a 3564 063c 0064 1264 0d84 007c 006a  .j5d.<.d.d...|.j
 00000a20: 1244 0083 017c 005f 3664 017c 006a 3664  .D...|._6d.|.j6d
 00000a30: 063c 0067 007c 005f 3774 2f7c 006a 127c  .<.g.|._7t/|.j.|
 00000a40: 006a 357c 006a 3683 0344 005d 135c 037d  .j5|.j6..D.].\.}
 00000a50: 1a7d 1c7d 1d74 307c 1a7c 1c7c 0364 0f8d  .}.}.t0|.|.|.d..
 00000a60: 037d 1b7c 006a 37a0 1e7c 1ba1 0101 0090  .}.|.j7..|......
 00000a70: 0171 0a74 006a 38a0 39a1 007c 005f 3a74  .q.t.j8.9..|._:t
-00000a80: 3ba0 3c7c 006a 3aa1 017c 005f 3d74 006a  ;.<|.j:..|._=t.j
-00000a90: 38a0 3ea1 007c 005f 3f74 006a 38a0 40a1  8.>..|._?t.j8.@.
-00000aa0: 007c 005f 4174 3ba0 3c74 42a1 017c 005f  .|._At;.<tB..|._
-00000ab0: 437c 006a 1664 1375 0190 0172 987c 1664  C|.j.d.u...r.|.d
-00000ac0: 1375 0190 0173 4c4a 0064 1483 0182 0174  .u...sLJ.d.....t
-00000ad0: 447c 1674 4574 4666 0283 0290 0172 587c  D|.tEtFf.....rX|
-00000ae0: 1667 017c 005f 1774 477c 006a 1783 017d  .g.|._.tG|.j...}
-00000af0: 1e74 477c 006a 1683 017d 1f7c 1e64 1514  .tG|.j...}.|.d..
-00000b00: 007c 076b 0290 0173 744a 0064 167c 1e9b  .|.k...stJ.d.|..
-00000b10: 0064 177c 079b 0064 189d 0583 0182 017c  .d.|...d.......|
-00000b20: 1e7c 1064 0619 006b 0290 0173 884a 0064  .|.d...k...s.J.d
-00000b30: 197c 1e9b 0064 1a7c 1064 0619 009b 0064  .|...d.|.d.....d
-00000b40: 1b9d 0583 0182 017c 1e7c 1f6b 0290 0173  .......|.|.k...s
-00000b50: 9a4a 0064 197c 1e9b 0064 1c7c 1f9b 0064  .J.d.|...d.|...d
-00000b60: 1b9d 0583 0182 0164 1353 0064 1353 0029  .......d.S.d.S.)
-00000b70: 1d61 250f 0000 0a20 2020 2020 2020 2041  .a%....        A
-00000b80: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
-00000b90: 2075 6e69 7473 3a20 4120 6c69 7374 206f   units: A list o
-00000ba0: 6620 696e 7473 2077 6865 7265 2065 6163  f ints where eac
-00000bb0: 6820 656c 656d 656e 7420 636f 6e66 6967  h element config
-00000bc0: 7572 6573 2061 6e20 6164 6469 7469 6f6e  ures an addition
-00000bd0: 616c 2061 7474 656e 7469 6f6e 206c 6179  al attention lay
-00000be0: 6572 2e20 5468 6520 6e75 6d65 7269 630a  er. The numeric.
-00000bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c00: 7661 6c75 6520 6465 7465 726d 696e 6573  value determines
-00000c10: 2074 6865 206e 756d 6265 7220 6f66 2068   the number of h
-00000c20: 6964 6465 6e20 756e 6974 7320 746f 2062  idden units to b
-00000c30: 6520 7573 6564 2069 6e20 7468 6520 6174  e used in the at
-00000c40: 7465 6e74 696f 6e20 6865 6164 7320 6f66  tention heads of
-00000c50: 2074 6861 7420 6c61 7965 720a 2020 2020   that layer.    
-00000c60: 2020 2020 2020 2020 6163 7469 7661 7469          activati
-00000c70: 6f6e 3a20 5468 6520 6163 7469 7661 7469  on: The activati
-00000c80: 6f6e 2066 756e 6374 696f 6e20 746f 2062  on function to b
-00000c90: 6520 7573 6564 2077 6974 6869 6e20 7468  e used within th
-00000ca0: 6520 6174 7465 6e74 696f 6e20 6c61 7965  e attention laye
-00000cb0: 7273 206f 6620 7468 6520 6e65 7477 6f72  rs of the networ
-00000cc0: 6b0a 2020 2020 2020 2020 2020 2020 7573  k.            us
-00000cd0: 655f 6269 6173 3a20 5768 6574 6865 7220  e_bias: Whether 
-00000ce0: 7468 6520 6c61 7965 7273 206f 6620 7468  the layers of th
-00000cf0: 6520 6e65 7477 6f72 6b20 7368 6f75 6c64  e network should
-00000d00: 2075 7365 2062 6961 7320 7765 6967 6874   use bias weight
-00000d10: 7320 6174 2061 6c6c 0a20 2020 2020 2020  s at all.       
-00000d20: 2020 2020 2064 726f 706f 7574 5f72 6174       dropout_rat
-00000d30: 653a 2054 6865 2064 726f 706f 7574 2072  e: The dropout r
-00000d40: 6174 6520 746f 2062 6520 6170 706c 6965  ate to be applie
-00000d50: 6420 6166 7465 7220 2a65 6163 682a 206f  d after *each* o
-00000d60: 6620 7468 6520 6174 7465 6e74 696f 6e20  f the attention 
-00000d70: 6c61 7965 7273 206f 6620 7468 6520 6e65  layers of the ne
-00000d80: 7477 6f72 6b2e 0a20 2020 2020 2020 2020  twork..         
-00000d90: 2020 2075 7365 5f65 6467 655f 6665 6174     use_edge_feat
-00000da0: 7572 6573 3a20 5768 6574 6865 7220 6564  ures: Whether ed
-00000db0: 6765 2066 6561 7475 7265 7320 7368 6f75  ge features shou
-00000dc0: 6c64 2062 6520 7573 6564 2e20 4765 6e65  ld be used. Gene
-00000dd0: 7261 6c6c 7920 7468 6520 6e65 7477 6f72  rally the networ
-00000de0: 6b20 7375 7070 6f72 7473 2074 6865 0a20  k supports the. 
-00000df0: 2020 2020 2020 2020 2020 2020 2020 2075                 u
-00000e00: 7361 6765 206f 6620 6564 6765 2066 6561  sage of edge fea
-00000e10: 7475 7265 732c 2062 7574 2069 6620 7468  tures, but if th
-00000e20: 6520 696e 7075 7420 6461 7461 2064 6f65  e input data doe
-00000e30: 7320 6e6f 7420 636f 6e74 6169 6e20 6564  s not contain ed
-00000e40: 6765 2066 6561 7475 7265 732c 2074 6869  ge features, thi
-00000e50: 7320 7368 6f75 6c64 2062 650a 2020 2020  s should be.    
-00000e60: 2020 2020 2020 2020 2020 2020 7365 7420              set 
-00000e70: 746f 2046 616c 7365 2e0a 2020 2020 2020  to False..      
-00000e80: 2020 2020 2020 696d 706f 7274 616e 6365        importance
-00000e90: 5f75 6e69 7473 3a20 4120 6c69 7374 206f  _units: A list o
-00000ea0: 6620 696e 7473 2077 6865 7265 2065 6163  f ints where eac
-00000eb0: 6820 656c 656d 656e 7420 636f 6e66 6967  h element config
-00000ec0: 7572 6573 2061 6e6f 7468 6572 2064 656e  ures another den
-00000ed0: 7365 206c 6179 6572 2069 6e20 7468 650a  se layer in the.
-00000ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ef0: 7375 626e 6574 776f 726b 2074 6861 7420  subnetwork that 
-00000f00: 7072 6f64 7563 6573 2074 6865 206e 6f64  produces the nod
-00000f10: 6520 696d 706f 7274 616e 6365 2074 656e  e importance ten
-00000f20: 736f 7220 6672 6f6d 2074 6865 206d 6169  sor from the mai
-00000f30: 6e20 6e6f 6465 2065 6d62 6564 6469 6e67  n node embedding
-00000f40: 732e 2054 6865 0a20 2020 2020 2020 2020  s. The.         
-00000f50: 2020 2020 2020 206e 756d 6572 6963 2076         numeric v
-00000f60: 616c 7565 2064 6574 6572 6d69 6e65 7320  alue determines 
-00000f70: 7468 6520 6e75 6d62 6572 206f 6620 6869  the number of hi
-00000f80: 6464 656e 2075 6e69 7473 2069 6e20 7468  dden units in th
-00000f90: 6174 206c 6179 6572 2e0a 2020 2020 2020  at layer..      
-00000fa0: 2020 2020 2020 696d 706f 7274 616e 6365        importance
-00000fb0: 5f63 6861 6e6e 656c 733a 2054 6865 2069  _channels: The i
-00000fc0: 6e74 206e 756d 6265 7220 6f66 2065 7870  nt number of exp
-00000fd0: 6c61 6e61 7469 6f6e 2063 6861 6e6e 656c  lanation channel
-00000fe0: 7320 746f 2062 6520 7072 6f64 7563 6564  s to be produced
-00000ff0: 2062 7920 7468 6520 6e65 7477 6f72 6b2e   by the network.
-00001000: 2054 6869 730a 2020 2020 2020 2020 2020   This.          
-00001010: 2020 2020 2020 6973 2074 6865 2076 616c        is the val
-00001020: 7565 2072 6566 6572 7265 6420 746f 2061  ue referred to a
-00001030: 7320 224b 222e 204e 6f74 6520 7468 6174  s "K". Note that
-00001040: 2074 6869 7320 7769 6c6c 2061 6c73 6f20   this will also 
-00001050: 6465 7465 726d 696e 6520 7468 6520 6e75  determine the nu
-00001060: 6d62 6572 206f 6620 6174 7465 6e74 696f  mber of attentio
-00001070: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
-00001080: 2020 6865 6164 7320 7573 6564 2077 6974    heads used wit
-00001090: 6869 6e20 7468 6520 6174 7465 6e74 696f  hin the attentio
-000010a0: 6e20 7375 626e 6574 776f 726b 2e0a 2020  n subnetwork..  
-000010b0: 2020 2020 2020 2020 2020 696d 706f 7274            import
-000010c0: 616e 6365 5f66 6163 746f 723a 2054 6865  ance_factor: The
-000010d0: 2077 6569 6768 7420 6f66 2074 6865 2065   weight of the e
-000010e0: 7870 6c61 6e61 7469 6f6e 2d6f 6e6c 7920  xplanation-only 
-000010f0: 7472 6169 6e20 7374 6570 2e20 4966 2074  train step. If t
-00001100: 6869 7320 6973 2073 6574 2074 6f20 6578  his is set to ex
-00001110: 6163 746c 790a 2020 2020 2020 2020 2020  actly.          
-00001120: 2020 2020 2020 7a65 726f 2074 6865 6e20        zero then 
-00001130: 7468 6520 6578 706c 616e 6174 696f 6e20  the explanation 
-00001140: 7472 6169 6e20 7374 6570 2077 696c 6c20  train step will 
-00001150: 6e6f 7420 6265 2065 7865 6375 7465 6420  not be executed 
-00001160: 6174 2061 6c6c 2028 6c65 7373 2063 6f6d  at all (less com
-00001170: 7075 7461 7469 6f6e 616c 6c79 0a20 2020  putationally.   
-00001180: 2020 2020 2020 2020 2020 2020 2065 7870               exp
-00001190: 656e 7369 7665 290a 2020 2020 2020 2020  ensive).        
-000011a0: 2020 2020 696d 706f 7274 616e 6365 5f6d      importance_m
-000011b0: 756c 7469 706c 6965 723a 2041 6e20 6164  ultiplier: An ad
-000011c0: 6469 7469 6f6e 616c 2068 7970 6572 7061  ditional hyperpa
-000011d0: 7261 6d65 7465 7220 6f66 2074 6865 2065  rameter of the e
-000011e0: 7870 6c61 6e61 7469 6f6e 2d6f 6e6c 7920  xplanation-only 
-000011f0: 7472 6169 6e20 7374 6570 2e20 5468 6973  train step. This
-00001200: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001210: 2069 7320 6573 7365 6e74 6961 6c6c 7920   is essentially 
-00001220: 7468 6520 7363 616c 696e 6720 6661 6374  the scaling fact
-00001230: 6f72 2074 6861 7420 6973 2061 7070 6c69  or that is appli
-00001240: 6564 2074 6f20 7468 6520 7661 6c75 6573  ed to the values
-00001250: 206f 6620 7468 6520 6461 7461 7365 7420   of the dataset 
-00001260: 7375 6368 2074 6861 740a 2020 2020 2020  such that.      
-00001270: 2020 2020 2020 2020 2020 7468 6520 7461            the ta
-00001280: 7267 6574 2076 616c 7565 7320 6361 6e20  rget values can 
-00001290: 7265 6173 6f6e 6162 6c79 2062 6520 6170  reasonably be ap
-000012a0: 7072 6f78 696d 6174 6564 2062 7920 6120  proximated by a 
-000012b0: 7375 6d20 6f66 205b 302c 2031 5d20 696d  sum of [0, 1] im
-000012c0: 706f 7274 616e 6365 2076 616c 7565 732e  portance values.
-000012d0: 0a20 2020 2020 2020 2020 2020 2073 7061  .            spa
-000012e0: 7273 6974 795f 6661 6374 6f72 3a20 5468  rsity_factor: Th
-000012f0: 6520 636f 6566 6669 6369 656e 7420 666f  e coefficient fo
-00001300: 7220 7468 6520 7370 6172 7369 7479 2072  r the sparsity r
-00001310: 6567 756c 6172 697a 6174 696f 6e20 6f66  egularization of
-00001320: 2074 6865 206e 6f64 6520 696d 706f 7274   the node import
-00001330: 616e 6365 0a20 2020 2020 2020 2020 2020  ance.           
-00001340: 2020 2020 2074 656e 736f 722e 0a20 2020       tensor..   
-00001350: 2020 2020 2020 2020 2063 6f6e 6361 745f           concat_
-00001360: 6865 6164 733a 2057 6865 7468 6572 2074  heads: Whether t
-00001370: 6f20 636f 6e63 6174 2074 6865 2068 6561  o concat the hea
-00001380: 6473 206f 6620 7468 6520 6174 7465 6e74  ds of the attent
-00001390: 696f 6e20 7375 626e 6574 776f 726b 2e20  ion subnetwork. 
-000013a0: 5468 6520 6465 6661 756c 7420 6973 2054  The default is T
-000013b0: 7275 652e 2049 6e0a 2020 2020 2020 2020  rue. In.        
-000013c0: 2020 2020 2020 2020 7468 6174 2063 6173          that cas
-000013d0: 6520 7468 6520 6f75 7470 7574 206f 6620  e the output of 
-000013e0: 6561 6368 2069 6e64 6976 6964 7561 6c20  each individual 
-000013f0: 6174 7465 6e74 696f 6e20 6865 6164 2069  attention head i
-00001400: 7320 636f 6e63 6174 656e 6174 6564 2061  s concatenated a
-00001410: 6e64 2074 6865 2063 6f6e 6361 7465 6e61  nd the concatena
-00001420: 7465 640a 2020 2020 2020 2020 2020 2020  ted.            
-00001430: 2020 2020 7665 6374 6f72 2069 7320 7468      vector is th
-00001440: 656e 2075 7365 6420 6173 2074 6865 2069  en used as the i
-00001450: 6e70 7574 206f 6620 7468 6520 6e65 7874  nput of the next
-00001460: 2061 7474 656e 7469 6f6e 206c 6179 6572   attention layer
-00001470: 2773 2068 6561 6473 2e20 4966 2074 6869  's heads. If thi
-00001480: 7320 6973 2046 616c 7365 2c20 7468 650a  s is False, the.
-00001490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000014a0: 7665 6374 6f72 7320 6172 6520 6176 6572  vectors are aver
-000014b0: 6167 6520 706f 6f6c 6564 2069 6e73 7465  age pooled inste
-000014c0: 6164 2e0a 2020 2020 2020 2020 2020 2020  ad..            
-000014d0: 6669 6e61 6c5f 756e 6974 733a 2041 206c  final_units: A l
-000014e0: 6973 7420 6f66 2069 6e74 7320 7768 6572  ist of ints wher
-000014f0: 6520 6561 6368 2065 6c65 6d65 6e74 2063  e each element c
-00001500: 6f6e 6669 6775 7265 7320 616e 6f74 6865  onfigures anothe
-00001510: 7220 6465 6e73 6520 6c61 7965 7220 696e  r dense layer in
-00001520: 2074 6865 204d 4c50 0a20 2020 2020 2020   the MLP.       
-00001530: 2020 2020 2020 2020 2061 7420 7468 6520           at the 
-00001540: 7461 696c 2065 6e64 206f 6620 7468 6520  tail end of the 
-00001550: 6e65 7477 6f72 6b2e 2054 6865 206e 756d  network. The num
-00001560: 6572 6963 2076 616c 7565 2064 6574 6572  eric value deter
-00001570: 6d69 6e65 7320 7468 6520 6e75 6d62 6572  mines the number
-00001580: 206f 6620 7468 6520 6869 6464 656e 2075   of the hidden u
-00001590: 6e69 7473 0a20 2020 2020 2020 2020 2020  nits.           
-000015a0: 2020 2020 2069 6e20 7468 6174 206c 6179       in that lay
-000015b0: 6572 2e20 4e6f 7465 2074 6861 7420 7468  er. Note that th
-000015c0: 6520 6669 6e61 6c20 656c 656d 656e 7420  e final element 
-000015d0: 696e 2074 6869 7320 6c69 7374 2068 6173  in this list has
-000015e0: 2074 6f20 6265 2074 6865 2073 616d 6520   to be the same 
-000015f0: 6173 2074 6865 2064 696d 656e 7369 6f6e  as the dimension
-00001600: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001610: 2074 6f20 6265 2065 7870 6563 7465 6420   to be expected 
-00001620: 666f 7220 7468 6520 7361 6d70 6c65 7320  for the samples 
-00001630: 6f66 2074 6865 2074 7261 696e 696e 6720  of the training 
-00001640: 6461 7461 7365 7421 0a20 2020 2020 2020  dataset!.       
-00001650: 2020 2020 2066 696e 616c 5f64 726f 706f       final_dropo
-00001660: 7574 5f72 6174 653a 2054 6865 2064 726f  ut_rate: The dro
-00001670: 706f 7574 2072 6174 6520 746f 2062 6520  pout rate to be 
-00001680: 6170 706c 6965 6420 6166 7465 7220 2a65  applied after *e
-00001690: 7665 7279 2a20 6c61 7965 7220 6f66 2074  very* layer of t
-000016a0: 6865 2066 696e 616c 204d 4c50 2e0a 2020  he final MLP..  
-000016b0: 2020 2020 2020 2020 2020 6669 6e61 6c5f            final_
-000016c0: 6163 7469 7661 7469 6f6e 3a20 5468 6520  activation: The 
-000016d0: 6163 7469 7661 7469 6f6e 2074 6f20 6265  activation to be
-000016e0: 2061 7070 6c69 6564 2061 7420 7468 6520   applied at the 
-000016f0: 7665 7279 206c 6173 7420 6c61 7965 7220  very last layer 
-00001700: 6f66 2074 6865 204d 4c50 2074 6f20 7072  of the MLP to pr
-00001710: 6f64 7563 6520 7468 650a 2020 2020 2020  oduce the.      
-00001720: 2020 2020 2020 2020 2020 6163 7475 616c            actual
-00001730: 206f 7574 7075 7420 6f66 2074 6865 206e   output of the n
-00001740: 6574 776f 726b 2e0a 2020 2020 2020 2020  etwork..        
-00001750: 2020 2020 6669 6e61 6c5f 706f 6f6c 696e      final_poolin
-00001760: 673a 2054 6865 2070 6f6f 6c69 6e67 206d  g: The pooling m
-00001770: 6574 686f 6420 746f 2062 6520 7573 6564  ethod to be used
-00001780: 2064 7572 696e 6720 7468 6520 676c 6f62   during the glob
-00001790: 616c 2070 6f6f 6c69 6e67 2070 6861 7365  al pooling phase
-000017a0: 2069 6e20 7468 6520 6e65 7477 6f72 6b2e   in the network.
-000017b0: 0a20 2020 2020 2020 2020 2020 2072 6567  .            reg
-000017c0: 7265 7373 696f 6e5f 6c69 6d69 7473 3a20  ression_limits: 
-000017d0: 4120 7475 706c 6520 7768 6572 6520 7468  A tuple where th
-000017e0: 6520 6669 7273 7420 7661 6c75 6520 6973  e first value is
-000017f0: 2074 6865 206c 6f77 6572 206c 696d 6974   the lower limit
-00001800: 2066 6f72 2074 6865 2065 7870 6563 7465   for the expecte
-00001810: 6420 7661 6c75 6520 7261 6e67 650a 2020  d value range.  
-00001820: 2020 2020 2020 2020 2020 2020 2020 6f66                of
-00001830: 2074 6865 2072 6567 7265 7373 696f 6e20   the regression 
-00001840: 7461 736b 2061 6e64 2074 6568 2073 6563  task and teh sec
-00001850: 6f6e 6420 7661 6c75 6520 7468 6520 7570  ond value the up
-00001860: 7065 7220 6c69 6d69 742e 0a20 2020 2020  per limit..     
-00001870: 2020 2020 2020 2072 6567 7265 7373 696f         regressio
-00001880: 6e5f 7265 6665 7265 6e63 653a 2041 2072  n_reference: A r
-00001890: 6566 6572 656e 6365 2076 616c 7565 2077  eference value w
-000018a0: 6869 6368 2069 7320 696e 7369 6465 2074  hich is inside t
-000018b0: 6865 2072 616e 6765 206f 6620 6578 7065  he range of expe
-000018c0: 6374 6564 2076 616c 7565 7320 2862 6573  cted values (bes
-000018d0: 7420 6966 0a20 2020 2020 2020 2020 2020  t if.           
-000018e0: 2020 2020 2069 7420 7761 7320 696e 2074       it was in t
-000018f0: 6865 206d 6964 646c 652c 2062 7574 2064  he middle, but d
-00001900: 6f65 7320 6e6f 7420 6861 7665 2074 6f29  oes not have to)
-00001910: 2e20 4368 6f6f 7369 6e67 2064 6966 6665  . Choosing diffe
-00001920: 7265 6e74 2072 6566 6572 656e 6365 7320  rent references 
-00001930: 7769 6c6c 2072 6573 756c 740a 2020 2020  will result.    
-00001940: 2020 2020 2020 2020 2020 2020 696e 2064              in d
-00001950: 6966 6665 7265 6e74 2065 7870 6c61 6e61  ifferent explana
-00001960: 7469 6f6e 732e 0a20 2020 2020 2020 2020  tions..         
-00001970: 2020 2072 6574 7572 6e5f 696d 706f 7274     return_import
-00001980: 616e 6365 733a 2057 6865 7468 6572 2074  ances: Whether t
-00001990: 6865 2069 6d70 6f72 7461 6e63 6520 2f20  he importance / 
-000019a0: 6578 706c 616e 6174 696f 6e20 7465 6e73  explanation tens
-000019b0: 6f72 7320 7368 6f75 6c64 2062 6520 7265  ors should be re
-000019c0: 7475 726e 6564 2061 7320 616e 206f 7574  turned as an out
-000019d0: 7075 740a 2020 2020 2020 2020 2020 2020  put.            
-000019e0: 2020 2020 6f66 2074 6865 206d 6f64 656c      of the model
-000019f0: 2e20 4966 2074 6869 7320 6973 2054 7275  . If this is Tru
-00001a00: 652c 2074 6865 206f 7574 7075 7420 6f66  e, the output of
-00001a10: 2074 6865 206d 6f64 656c 2077 696c 6c20   the model will 
-00001a20: 6265 2061 2033 2d74 7570 6c65 3a0a 2020  be a 3-tuple:.  
-00001a30: 2020 2020 2020 2020 2020 2020 2020 286f                (o
-00001a40: 7574 7075 742c 206e 6f64 6520 696d 706f  utput, node impo
-00001a50: 7274 616e 6365 732c 2065 6467 6520 696d  rtances, edge im
-00001a60: 706f 7274 616e 6365 7329 2c20 6f74 6865  portances), othe
-00001a70: 7277 6973 6520 6974 2069 7320 6a75 7374  rwise it is just
-00001a80: 2074 6865 206f 7574 7075 7420 6974 7365   the output itse
-00001a90: 6c66 0a20 2020 2020 2020 2054 2907 721a  lf.        T).r.
-00001aa0: 0000 00da 096e 756d 5f68 6561 6473 721e  .....num_headsr.
-00001ab0: 0000 0072 1b00 0000 721c 0000 00da 0e68  ...r....r......h
-00001ac0: 6173 5f73 656c 665f 6c6f 6f70 7372 2700  as_self_loopsr'.
-00001ad0: 0000 2901 da04 7261 7465 2901 da06 6661  ..)...rate)...fa
-00001ae0: 6374 6f72 2901 721b 0000 00e9 ffff ffff  ctor).r.........
-00001af0: a901 da04 6178 6973 da04 6d65 616e 7201  ....axis..meanr.
-00001b00: 0000 0029 02da 0e70 6f6f 6c69 6e67 5f6d  ...)...pooling_m
-00001b10: 6574 686f 64da 0d70 6f6f 6c69 6e67 5f69  ethod..pooling_i
-00001b20: 6e64 6578 7217 0000 0063 0100 0000 0000  ndexr....c......
-00001b30: 0000 0000 0000 0200 0000 0300 0000 5300  ..............S.
-00001b40: 0000 f310 0000 0067 007c 005d 047d 0164  .......g.|.].}.d
-00001b50: 0091 0271 0253 00a9 0172 1300 0000 a900  ...q.S...r......
-00001b60: a902 da02 2e30 da01 5f72 3e00 0000 723e  .....0.._r>...r>
-00001b70: 0000 00fa 562f 6d65 6469 612f 7373 642f  ....V/media/ssd/
-00001b80: 5072 6f67 7261 6d6d 696e 672f 6772 6170  Programming/grap
-00001b90: 685f 6174 7465 6e74 696f 6e5f 7374 7564  h_attention_stud
-00001ba0: 656e 742f 6772 6170 685f 6174 7465 6e74  ent/graph_attent
-00001bb0: 696f 6e5f 7374 7564 656e 742f 6d6f 6465  ion_student/mode
-00001bc0: 6c73 2f6d 6567 616e 2e70 79da 0a3c 6c69  ls/megan.py..<li
-00001bd0: 7374 636f 6d70 3e9d 0000 00f3 0200 0000  stcomp>.........
-00001be0: 1000 7a22 4d65 6761 6e2e 5f5f 696e 6974  ..z"Megan.__init
-00001bf0: 5f5f 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973  __.<locals>.<lis
-00001c00: 7463 6f6d 703e 7218 0000 0029 0372 1a00  tcomp>r....).r..
-00001c10: 0000 721b 0000 0072 1c00 0000 2901 723a  ..r....r....).r:
-00001c20: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-00001c30: 0200 0000 0300 0000 5300 0000 723c 0000  ........S...r<..
-00001c40: 0072 3d00 0000 723e 0000 0072 3f00 0000  .r=...r>...r?...
-00001c50: 723e 0000 0072 3e00 0000 7242 0000 0072  r>...r>...rB...r
-00001c60: 4300 0000 ac00 0000 7244 0000 0063 0100  C.......rD...c..
-00001c70: 0000 0000 0000 0000 0000 0200 0000 0300  ................
-00001c80: 0000 5300 0000 723c 0000 00a9 0154 723e  ..S...r<.....Tr>
-00001c90: 0000 0072 3f00 0000 723e 0000 0072 3e00  ...r?...r>...r>.
-00001ca0: 0000 7242 0000 0072 4300 0000 ae00 0000  ..rB...rC.......
-00001cb0: 7244 0000 004e 7a4e 596f 7520 6861 7665  rD...NzNYou have
-00001cc0: 2074 6f20 7375 7070 6c79 2061 2022 7265   to supply a "re
-00001cd0: 6772 6573 7369 6f6e 5f72 6566 6572 656e  gression_referen
-00001ce0: 6365 2220 7661 6c75 6520 666f 7220 6578  ce" value for ex
-00001cf0: 706c 616e 6174 696f 6e20 636f 2d74 7261  planation co-tra
-00001d00: 696e 696e 6721 7215 0000 007a 4c66 6f72  ining!r....zLfor
-00001d10: 2065 7870 6c61 6e61 7469 6f6e 2063 6f2d   explanation co-
-00001d20: 7472 6169 6e69 6e67 2c20 7468 6520 6e75  training, the nu
-00001d30: 6d62 6572 206f 6620 7265 6772 6573 7369  mber of regressi
-00001d40: 6f6e 5f72 6566 6572 656e 6365 7320 2863  on_references (c
-00001d50: 7572 7265 6e74 6c79 207a 4629 2068 6173  urrently zF) has
-00001d60: 2074 6f20 6265 2065 7861 6374 6c79 2068   to be exactly h
-00001d70: 616c 6620 7468 6520 6e75 6d62 6572 206f  alf the number o
-00001d80: 6620 696d 706f 7274 616e 6365 2063 6861  f importance cha
-00001d90: 6e6e 656c 7320 2863 7572 7265 6e74 6c79  nnels (currently
-00001da0: 207a 0229 217a 4c46 6f72 2065 7870 6c61   z.)!zLFor expla
-00001db0: 6e61 7469 6f6e 2063 6f2d 7472 6169 6e69  nation co-traini
-00001dc0: 6e67 2c20 7468 6520 6e75 6d62 6572 206f  ng, the number o
-00001dd0: 6620 7265 6772 6573 7369 6f6e 5f72 6566  f regression_ref
-00001de0: 6572 656e 6365 7320 2863 7572 7265 6e74  erences (current
-00001df0: 6c79 207a 5429 2068 6173 2074 6f20 6265  ly zT) has to be
-00001e00: 2065 7861 6374 6c79 2074 6865 2073 616d   exactly the sam
-00001e10: 6520 6173 2074 6865 2066 696e 616c 2075  e as the final u
-00001e20: 6e69 7420 636f 756e 7420 696e 2074 6865  nit count in the
-00001e30: 204d 4c50 2074 6169 6c20 656e 6420 2863   MLP tail end (c
-00001e40: 7572 7265 6e74 6c79 20fa 0129 7a55 2920  urrently ..)zU) 
-00001e50: 6861 7320 746f 2062 6520 6578 6163 746c  has to be exactl
-00001e60: 7920 7468 6520 7361 6d65 2061 7320 7468  y the same as th
-00001e70: 6520 6e75 6d62 6572 206f 6620 7265 6772  e number of regr
-00001e80: 6573 7369 6f6e 5f6c 696d 6974 7320 696e  ession_limits in
-00001e90: 7465 7276 616c 7320 2863 7572 7265 6e74  tervals (current
-00001ea0: 6c79 2029 48da 026b 73da 066d 6f64 656c  ly )H..ks..model
-00001eb0: 73da 054d 6f64 656c da08 5f5f 696e 6974  s..Model..__init
-00001ec0: 5f5f 721a 0000 0072 1b00 0000 721c 0000  __r....r....r...
-00001ed0: 0072 1d00 0000 721e 0000 0072 1f00 0000  .r....r....r....
-00001ee0: 7220 0000 0072 2100 0000 7222 0000 0072  r ...r!...r"...r
-00001ef0: 2300 0000 7224 0000 0072 2500 0000 7226  #...r$...r%...r&
-00001f00: 0000 0072 2700 0000 7229 0000 0072 2a00  ...r'...r)...r*.
-00001f10: 0000 722b 0000 0072 2c00 0000 722d 0000  ..r+...r,...r-..
-00001f20: 0072 2f00 0000 722e 0000 0072 3000 0000  .r/...r....r0...
-00001f30: 7228 0000 0072 3100 0000 da10 6174 7465  r(...r1.....atte
-00001f40: 6e74 696f 6e5f 6c61 7965 7273 720e 0000  ntion_layersr...
-00001f50: 00da 0661 7070 656e 6472 0900 0000 da0b  ...appendr......
-00001f60: 6c61 795f 6472 6f70 6f75 7472 0d00 0000  lay_dropoutr....
-00001f70: da0c 6c61 795f 7370 6172 7369 7479 7208  ..lay_sparsityr.
-00001f80: 0000 00da 126c 6179 5f61 6374 5f69 6d70  .....lay_act_imp
-00001f90: 6f72 7461 6e63 6572 0500 0000 da11 6c61  ortancer......la
-00001fa0: 795f 636f 6e63 6174 5f61 6c70 6861 7372  y_concat_alphasr
-00001fb0: 0a00 0000 da11 6c61 795f 706f 6f6c 5f65  ......lay_pool_e
-00001fc0: 6467 6573 5f69 6eda 126c 6179 5f70 6f6f  dges_in..lay_poo
-00001fd0: 6c5f 6564 6765 735f 6f75 7472 0600 0000  l_edges_outr....
-00001fe0: da0b 6c61 795f 6176 6572 6167 65da 156e  ..lay_average..n
-00001ff0: 6f64 655f 696d 706f 7274 616e 6365 5f75  ode_importance_u
-00002000: 6e69 7473 da14 6e6f 6465 5f69 6d70 6f72  nits..node_impor
-00002010: 7461 6e63 655f 6163 7473 da16 6e6f 6465  tance_acts..node
-00002020: 5f69 6d70 6f72 7461 6e63 655f 6c61 7965  _importance_laye
-00002030: 7273 da03 7a69 7072 0700 0000 720b 0000  rs..zipr....r...
-00002040: 00da 0c6c 6179 5f70 6f6f 6c5f 6f75 74da  ...lay_pool_out.
-00002050: 0e6c 6179 5f63 6f6e 6361 745f 6f75 74da  .lay_concat_out.
-00002060: 116c 6179 5f66 696e 616c 5f64 726f 706f  .lay_final_dropo
-00002070: 7574 da0a 6669 6e61 6c5f 6163 7473 da0c  ut..final_acts..
-00002080: 6669 6e61 6c5f 6269 6173 6573 da0c 6669  final_biases..fi
-00002090: 6e61 6c5f 6c61 7965 7273 da06 6c6f 7373  nal_layers..loss
-000020a0: 6573 da12 4269 6e61 7279 4372 6f73 7365  es..BinaryCrosse
-000020b0: 6e74 726f 7079 da08 6263 655f 6c6f 7373  ntropy..bce_loss
-000020c0: 7202 0000 00da 0f4c 6f73 7365 7343 6f6e  r......LossesCon
-000020d0: 7461 696e 6572 da1c 636f 6d70 696c 6564  tainer..compiled
-000020e0: 5f63 6c61 7373 6966 6963 6174 696f 6e5f  _classification_
-000020f0: 6c6f 7373 da10 4d65 616e 5371 7561 7265  loss..MeanSquare
-00002100: 6445 7272 6f72 da08 6d73 655f 6c6f 7373  dError..mse_loss
-00002110: da11 4d65 616e 4162 736f 6c75 7465 4572  ..MeanAbsoluteEr
-00002120: 726f 72da 086d 6165 5f6c 6f73 7372 0f00  ror..mae_lossr..
-00002130: 0000 da18 636f 6d70 696c 6564 5f72 6567  ....compiled_reg
-00002140: 7265 7373 696f 6e5f 6c6f 7373 da0a 6973  ression_loss..is
-00002150: 696e 7374 616e 6365 da03 696e 74da 0566  instance..int..f
-00002160: 6c6f 6174 da03 6c65 6e29 20da 0473 656c  loat..len) ..sel
-00002170: 6672 1a00 0000 721b 0000 0072 1c00 0000  fr....r....r....
-00002180: 721d 0000 0072 1e00 0000 721f 0000 0072  r....r....r....r
-00002190: 2000 0000 7221 0000 0072 2200 0000 7223   ...r!...r"...r#
-000021a0: 0000 0072 2400 0000 7225 0000 0072 2600  ...r$...r%...r&.
-000021b0: 0000 7227 0000 0072 2800 0000 7229 0000  ..r'...r(...r)..
-000021c0: 0072 2a00 0000 722b 0000 0072 2c00 0000  .r*...r+...r,...
-000021d0: 722d 0000 0072 2e00 0000 722f 0000 0072  r-...r....r/...r
-000021e0: 3000 0000 7231 0000 00da 066b 7761 7267  0...r1.....kwarg
-000021f0: 73da 0175 da03 6c61 79da 0361 6374 da04  s..u..lay..act..
-00002200: 6269 6173 da0e 6e75 6d5f 7265 6665 7265  bias..num_refere
-00002210: 6e63 6573 da0a 6e75 6d5f 6c69 6d69 7473  nces..num_limits
-00002220: 723e 0000 0072 3e00 0000 7242 0000 0072  r>...r>...rB...r
-00002230: 4a00 0000 1e00 0000 73c2 0000 0016 4a06  J.......s.....J.
-00002240: 0106 0106 0106 0106 0106 0106 0106 0106  ................
-00002250: 0106 0106 0106 0106 0106 0106 0106 0106  ................
-00002260: 0106 0106 0106 0106 0106 0106 0106 0106  ................
-00002270: 030a 0102 0102 0104 0104 0104 0104 0102  ................
-00002280: 0104 0106 f90e 090e 020e 010e 030c 010e  ................
-00002290: 020e 0108 010e 0316 0106 0116 0102 0102  ................
-000022a0: 0102 0102 0106 fd0e 050e 030c 010e 0112  ................
-000022b0: 020c 0112 010a 0106 011c 0102 0102 0102  ................
-000022c0: 0102 0106 fd10 050c 030e 010c 020c 010c  ................
-000022d0: 010c 0612 0210 0908 010a 020a 0110 0108  ................
-000022e0: 0102 0106 ff04 ff10 0408 0106 0106 ff04  ................
-000022f0: ff0c 0408 0102 0106 ff04 ff04 e804 187a  ...............z
-00002300: 0e4d 6567 616e 2e5f 5f69 6e69 745f 5f63  .Megan.__init__c
-00002310: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00002320: 0700 0000 0300 0000 73b6 0000 0074 0074  ........s....t.t
-00002330: 017c 0083 02a0 02a1 007d 017c 01a0 0369  .|.......}.|...i
-00002340: 0064 017c 006a 0493 0164 027c 006a 0593  .d.|.j...d.|.j..
-00002350: 0164 037c 006a 0693 0164 047c 006a 0793  .d.|.j...d.|.j..
-00002360: 0164 057c 006a 0893 0164 067c 006a 0993  .d.|.j...d.|.j..
-00002370: 0164 077c 006a 0a93 0164 087c 006a 0b93  .d.|.j...d.|.j..
-00002380: 0164 097c 006a 0c93 0164 0a7c 006a 0d93  .d.|.j...d.|.j..
-00002390: 0164 0b7c 006a 0e93 0164 0c7c 006a 0f93  .d.|.j...d.|.j..
-000023a0: 0164 0d7c 006a 1093 0164 0e7c 006a 1193  .d.|.j...d.|.j..
-000023b0: 0164 0f7c 006a 1293 0164 107c 006a 1393  .d.|.j...d.|.j..
-000023c0: 0164 117c 006a 1493 017c 006a 157c 006a  .d.|.j...|.j.|.j
-000023d0: 167c 006a 1764 129c 03a5 01a1 0101 007c  .|.j.d.........|
-000023e0: 0153 0029 134e 721a 0000 0072 1b00 0000  .S.).Nr....r....
-000023f0: 721c 0000 0072 1d00 0000 721e 0000 0072  r....r....r....r
-00002400: 1f00 0000 7220 0000 0072 2100 0000 7222  ....r ...r!...r"
-00002410: 0000 0072 2300 0000 7224 0000 0072 2600  ...r#...r$...r&.
-00002420: 0000 7227 0000 0072 2900 0000 722a 0000  ..r'...r)...r*..
-00002430: 0072 2b00 0000 722c 0000 0029 0372 2d00  .r+...r,...).r-.
-00002440: 0000 722f 0000 0072 3000 0000 2918 da05  ..r/...r0...)...
-00002450: 7375 7065 7272 1200 0000 da0a 6765 745f  superr......get_
-00002460: 636f 6e66 6967 da06 7570 6461 7465 721a  config..updater.
-00002470: 0000 0072 1b00 0000 721c 0000 0072 1d00  ...r....r....r..
-00002480: 0000 721e 0000 0072 1f00 0000 7220 0000  ..r....r....r ..
-00002490: 0072 2100 0000 7222 0000 0072 2300 0000  .r!...r"...r#...
-000024a0: 7224 0000 0072 2600 0000 7227 0000 0072  r$...r&...r'...r
-000024b0: 2900 0000 722a 0000 0072 2b00 0000 722c  )...r*...r+...r,
-000024c0: 0000 0072 2d00 0000 722f 0000 0072 3000  ...r-...r/...r0.
-000024d0: 0000 2902 726c 0000 00da 0663 6f6e 6669  ..).rl.....confi
-000024e0: 67a9 01da 095f 5f63 6c61 7373 5f5f 723e  g....__class__r>
-000024f0: 0000 0072 4200 0000 7275 0000 00e2 0000  ...rB...ru......
-00002500: 0073 5200 0000 0e01 0601 0601 02ff 0602  .sR.............
-00002510: 02fe 0603 02fd 0604 02fc 0605 02fb 0606  ................
-00002520: 02fa 0607 02f9 0608 02f8 0609 02f7 060a  ................
-00002530: 02f6 060b 02f5 060c 02f4 060d 02f3 060e  ................
-00002540: 02f2 060f 02f1 0610 02f0 0611 02ef 0412  ................
-00002550: 0401 0401 0aec 0417 7a10 4d65 6761 6e2e  ........z.Megan.
-00002560: 6765 745f 636f 6e66 6967 da06 7265 7475  get_config..retu
-00002570: 726e 6301 0000 0000 0000 0000 0000 0001  rnc.............
-00002580: 0000 0002 0000 0043 0000 0073 0a00 0000  .......C...s....
-00002590: 7c00 6a00 6400 7501 5300 2901 4e29 0172  |.j.d.u.S.).N).r
-000025a0: 2d00 0000 2901 726c 0000 0072 3e00 0000  -...).rl...r>...
-000025b0: 723e 0000 0072 4200 0000 da10 646f 696e  r>...rB.....doin
-000025c0: 675f 7265 6772 6573 7369 6f6e fc00 0000  g_regression....
-000025d0: 7302 0000 000a 027a 164d 6567 616e 2e64  s......z.Megan.d
-000025e0: 6f69 6e67 5f72 6567 7265 7373 696f 6eda  oing_regression.
-000025f0: 0874 7261 696e 696e 67da 156e 6f64 655f  .training..node_
-00002600: 696d 706f 7274 616e 6365 735f 6d61 736b  importances_mask
-00002610: 6305 0000 0000 0000 0000 0000 001e 0000  c...............
-00002620: 0006 0000 004b 0000 0073 2802 0000 7c00  .....K...s(...|.
-00002630: 6a00 720a 7c01 5c04 7d06 7d07 7d08 7d09  j.r.|.\.}.}.}.}.
-00002640: 6e07 7c01 5c03 7d06 7d07 7d08 6401 7d09  n.|.\.}.}.}.d.}.
-00002650: 6700 7d0a 7c06 7d0b 7c00 6a01 4400 5d19  g.}.|.}.|.j.D.].
-00002660: 7d0c 7c0c 7c0b 7c07 7c08 6703 8301 5c02  }.|.|.|.|.g...\.
-00002670: 7d0b 7d0d 7c02 722c 7c00 6a02 7c0b 7c02  }.}.|.r,|.j.|.|.
-00002680: 6402 8d02 7d0b 7c0a a003 7c0d a101 0100  d...}.|...|.....
-00002690: 7118 7c00 a004 7c0a a101 7d0a 7405 6a06  q.|...|...}.t.j.
-000026a0: 7c0a 6403 6404 6405 8d03 7d0e 7c00 a007  |.d.d.d...}.|...
-000026b0: 7c0e a101 7d0e 7c00 a008 7c06 7c0e 7c08  |...}.|...|.|.|.
-000026c0: 6703 a101 7d0f 7c00 a009 7c06 7c0e 7c08  g...}.|...|.|.|.
-000026d0: 6703 a101 7d10 7c00 a00a 7c10 7c0f 6702  g...}.|...|.|.g.
-000026e0: a101 7d11 7c0b 7d12 7c00 6a0b 4400 5d06  ..}.|.}.|.j.D.].
-000026f0: 7d0c 7c0c 7c12 8301 7d12 7160 7c00 a007  }.|.|...}.q`|...
-00002700: 7c12 a101 7d12 7c12 7c11 1400 7d13 7c00  |...}.|.|...}.|.
-00002710: a00c 7c13 a101 0100 7c04 6401 7501 7284  ..|.....|.d.u.r.
-00002720: 7405 a00d 7c04 7405 6a0e a102 7d04 7c13  t...|.t.j...}.|.
-00002730: 7c04 1400 7d13 6700 7d14 7c00 6a0f 6403  |...}.g.}.|.j.d.
-00002740: 1900 7d15 7410 7c00 6a11 8301 4400 5d2e  ..}.t.|.j...D.].
-00002750: 7d16 7405 6a12 7c13 6401 6401 8502 6401  }.t.j.|.d.d...d.
-00002760: 6401 8502 7c16 6603 1900 6403 6406 8d02  d...|.f...d.d...
-00002770: 7d17 7c0b 7c17 1400 7d18 7c00 6a13 6401  }.|.|...}.|.j.d.
-00002780: 7501 72b4 7c00 6a13 7c16 1900 7d19 7c19  u.r.|.j.|...}.|.
-00002790: 7c18 8301 7d18 7c00 a014 7c18 a101 7d1a  |...}.|...|...}.
-000027a0: 7c14 a003 7c1a a101 0100 7190 7c00 a015  |...|.....q.|...
-000027b0: 7c14 a101 7d1a 7c00 6a00 72ce 7c00 a015  |...}.|.j.r.|...
-000027c0: 7c1a 7c09 6702 a101 7d1a 7416 7c00 6a17  |.|.g...}.t.|.j.
-000027d0: 8301 7d1b 7418 7c00 6a17 8301 4400 5d17  ..}.t.|.j...D.].
-000027e0: 5c02 7d1c 7d0c 7c0c 7c1a 8301 7d1a 7c02  \.}.}.|.|...}.|.
-000027f0: 72ef 7c1c 7c1b 6407 1800 6b00 72ef 7c00  r.|.|.d...k.r.|.
-00002800: 6a19 7c1a 7c02 6402 8d02 7d1a 71d8 7c00  j.|.|.d...}.q.|.
-00002810: 6a1a 9001 7206 7405 a01b 7c1a a101 7405  j...r.t...|...t.
-00002820: 6a1c 7c00 6a1d 7405 6a0e 6408 8d02 1400  j.|.j.t.j.d.....
-00002830: 7d1d 7c1a 7c1d 1700 7d1a 7c00 6a1e 9001  }.|.|...}.|.j...
-00002840: 730d 7c03 9001 7212 7c1a 7c13 7c0e 6603  s.|...r.|.|.|.f.
-00002850: 5300 7c1a 5300 2909 61b7 0100 000a 2020  S.|.S.).a.....  
-00002860: 2020 2020 2020 466f 7277 6172 6420 7061        Forward pa
-00002870: 7373 206f 6620 7468 6520 6d6f 6465 6c2e  ss of the model.
-00002880: 0a0a 2020 2020 2020 2020 2a2a 5368 6170  ..        **Shap
-00002890: 6520 4578 706c 616e 6174 696f 6e73 3a2a  e Explanations:*
-000028a0: 2a20 416c 6c20 7368 6170 6573 2069 6e20  * All shapes in 
-000028b0: 6272 6163 6b65 7473 205b 5d20 6172 6520  brackets [] are 
-000028c0: 7261 6767 6564 2064 696d 656e 7369 6f6e  ragged dimension
-000028d0: 7321 0a0a 2020 2020 2020 2020 2d20 563a  s!..        - V:
-000028e0: 204e 756d 206e 6f64 6573 2069 6e20 7468   Num nodes in th
-000028f0: 6520 6772 6170 680a 2020 2020 2020 2020  e graph.        
-00002900: 2d20 453a 204e 756d 2065 6467 6573 2069  - E: Num edges i
-00002910: 6e20 7468 6520 6772 6170 680a 2020 2020  n the graph.    
-00002920: 2020 2020 2d20 4e3a 204e 756d 2066 6561      - N: Num fea
-00002930: 7475 7265 2076 616c 7565 7320 7065 7220  ture values per 
-00002940: 6e6f 6465 0a20 2020 2020 2020 202d 204d  node.        - M
-00002950: 3a20 4e55 6d20 6665 6174 7572 6520 7661  : NUm feature va
-00002960: 6c75 6573 2070 6572 2065 6467 650a 2020  lues per edge.  
-00002970: 2020 2020 2020 2d20 483a 204e 756d 2066        - H: Num f
-00002980: 6561 7475 7265 2076 616c 7565 7320 7065  eature values pe
-00002990: 7220 6772 6170 680a 2020 2020 2020 2020  r graph.        
-000029a0: 2d20 423a 204e 756d 2067 7261 7068 7320  - B: Num graphs 
-000029b0: 696e 2061 2062 6174 6368 0a20 2020 2020  in a batch.     
-000029c0: 2020 202d 204b 3a20 4e75 6d20 696d 706f     - K: Num impo
-000029d0: 7274 616e 6365 2028 6578 706c 616e 6174  rtance (explanat
-000029e0: 696f 6e29 2063 6861 6e6e 656c 7320 636f  ion) channels co
-000029f0: 6e66 6967 7572 6564 2069 6e20 7468 6520  nfigured in the 
-00002a00: 636f 6e73 7472 7563 746f 720a 2020 2020  constructor.    
-00002a10: 2020 2020 4e29 0172 7c00 0000 7236 0000      N).r|...r6..
-00002a20: 0046 2902 7238 0000 00da 086b 6565 7064  .F).r8.....keepd
-00002a30: 696d 7372 3700 0000 7215 0000 0029 01da  imsr7...r....)..
-00002a40: 0564 7479 7065 291f 7231 0000 0072 4b00  .dtype).r1...rK.
-00002a50: 0000 724d 0000 0072 4c00 0000 7250 0000  ..rM...rL...rP..
-00002a60: 00da 0274 66da 0a72 6564 7563 655f 7375  ...tf..reduce_su
-00002a70: 6d72 4f00 0000 7251 0000 0072 5200 0000  mrO...rQ...rR...
-00002a80: 7253 0000 0072 5600 0000 724e 0000 00da  rS...rV...rN....
-00002a90: 0463 6173 74da 0766 6c6f 6174 3332 7229  .cast..float32r)
-00002aa0: 0000 00da 0572 616e 6765 7220 0000 00da  .....ranger ....
-00002ab0: 0b65 7870 616e 645f 6469 6d73 7225 0000  .expand_dimsr%..
-00002ac0: 0072 5800 0000 7259 0000 0072 6b00 0000  .rX...rY...rk...
-00002ad0: 725d 0000 00da 0965 6e75 6d65 7261 7465  r].....enumerate
-00002ae0: 725a 0000 0072 7b00 0000 da09 6f6e 6573  rZ...r{.....ones
-00002af0: 5f6c 696b 65da 0863 6f6e 7374 616e 7472  _like..constantr
-00002b00: 2f00 0000 7230 0000 0029 1e72 6c00 0000  /...r0...).rl...
-00002b10: da06 696e 7075 7473 727c 0000 0072 3000  ..inputsr|...r0.
-00002b20: 0000 727d 0000 0072 6d00 0000 da0a 6e6f  ..r}...rm.....no
-00002b30: 6465 5f69 6e70 7574 da0a 6564 6765 5f69  de_input..edge_i
-00002b40: 6e70 7574 da10 6564 6765 5f69 6e64 6578  nput..edge_index
-00002b50: 5f69 6e70 7574 da0b 6772 6170 685f 696e  _input..graph_in
-00002b60: 7075 74da 0661 6c70 6861 73da 0178 726f  put..alphas..xro
-00002b70: 0000 00da 0561 6c70 6861 da10 6564 6765  .....alpha..edge
-00002b80: 5f69 6d70 6f72 7461 6e63 6573 da0f 706f  _importances..po
-00002b90: 6f6c 6564 5f65 6467 6573 5f69 6eda 1070  oled_edges_in..p
-00002ba0: 6f6f 6c65 645f 6564 6765 735f 6f75 74da  ooled_edges_out.
-00002bb0: 0c70 6f6f 6c65 645f 6564 6765 73da 166e  .pooled_edges..n
-00002bc0: 6f64 655f 696d 706f 7274 616e 6365 735f  ode_importances_
-00002bd0: 7469 6c64 65da 106e 6f64 655f 696d 706f  tilde..node_impo
-00002be0: 7274 616e 6365 73da 046f 7574 73da 016e  rtances..outs..n
-00002bf0: da01 6bda 156e 6f64 655f 696d 706f 7274  ..k..node_import
-00002c00: 616e 6365 5f73 6c69 6365 da11 6d61 736b  ance_slice..mask
-00002c10: 6564 5f65 6d62 6564 6469 6e67 73da 0d6c  ed_embeddings..l
-00002c20: 6179 5f74 7261 6e73 666f 726d da03 6f75  ay_transform..ou
-00002c30: 74da 106e 756d 5f66 696e 616c 5f6c 6179  t..num_final_lay
-00002c40: 6572 73da 0163 da09 7265 6665 7265 6e63  ers..c..referenc
-00002c50: 6572 3e00 0000 723e 0000 0072 4200 0000  er>...r>...rB...
-00002c60: da04 6361 6c6c 0001 0000 7366 0000 0006  ..call....sf....
-00002c70: 1f0e 010a 0204 0104 0504 010a 0112 0304  ................
-00002c80: 010e 010c 020a 0410 010a 0110 0610 010e  ................
-00002c90: 0104 020a 010a 010a 0208 020a 0108 090e  ................
-00002ca0: 0108 0104 050a 010e 0120 0108 010a 050a  ......... ......
-00002cb0: 0108 010a 020c 030a 0306 040e 010a 0412  ................
-00002cc0: 0108 0110 010e 0102 8008 021c 0108 010e  ................
-00002cd0: 050a 0104 027a 0a4d 6567 616e 2e63 616c  .....z.Megan.cal
-00002ce0: 6c63 0200 0000 0000 0000 0000 0000 0c00  lc..............
-00002cf0: 0000 0600 0000 4300 0000 73ce 0000 0067  ......C...s....g
-00002d00: 007d 0267 007d 0374 0074 017c 006a 027c  .}.g.}.t.t.|.j.|
-00002d10: 006a 0383 0283 0144 005d 4b5c 027d 045c  .j.....D.]K\.}.\
-00002d20: 027d 057d 0674 047c 0664 0119 007c 0664  .}.}.t.|.d...|.d
-00002d30: 0219 0018 0083 017d 0774 056a 067c 0164  .......}.t.j.|.d
-00002d40: 0064 0085 027c 0466 0219 0064 0364 048d  .d...|.f...d.d..
-00002d50: 027d 0874 05a0 047c 087c 0518 00a1 017d  .}.t...|.|.....}
-00002d60: 097c 097c 006a 0714 0064 057c 0714 001b  .|.|.j...d.|....
-00002d70: 007d 0974 05a0 087c 087c 056b 0064 0664  .}.t...|.|.k.d.d
-00002d80: 07a1 037d 0a74 05a0 087c 087c 056b 0464  ...}.t...|.|.k.d
-00002d90: 0664 07a1 037d 0b7c 027c 097c 0967 0237  .d...}.|.|.|.g.7
-00002da0: 007d 027c 037c 0a7c 0b67 0237 007d 0371  .}.|.|.|.g.7.}.q
-00002db0: 0d74 056a 097c 0264 0364 048d 0274 056a  .t.j.|.d.d...t.j
-00002dc0: 097c 0364 0364 048d 0266 0253 0029 084e  .|.d.d...f.S.).N
-00002dd0: 7217 0000 0072 0100 0000 7236 0000 0072  r....r....r6...r
-00002de0: 3700 0000 6700 0000 0000 00e0 3f67 0000  7...g.......?g..
-00002df0: 0000 0000 f03f 7214 0000 0029 0a72 8600  .....?r....).r..
-00002e00: 0000 7257 0000 0072 2f00 0000 722d 0000  ..rW...r/...r-..
-00002e10: 00da 0361 6273 7280 0000 0072 8500 0000  ...absr....r....
-00002e20: 7224 0000 00da 0577 6865 7265 da06 636f  r$.....where..co
-00002e30: 6e63 6174 290c 726c 0000 00da 086f 7574  ncat).rl.....out
-00002e40: 5f74 7275 65da 0773 616d 706c 6573 da05  _true..samples..
-00002e50: 6d61 736b 73da 0169 722f 0000 0072 2d00  masks..ir/...r-.
-00002e60: 0000 da10 7265 6772 6573 7369 6f6e 5f77  ....regression_w
-00002e70: 6964 7468 da06 7661 6c75 6573 da10 6365  idth..values..ce
-00002e80: 6e74 6572 5f64 6973 7461 6e63 6573 da07  nter_distances..
-00002e90: 6c6f 5f6d 6173 6bda 0768 695f 6d61 736b  lo_mask..hi_mask
-00002ea0: 723e 0000 0072 3e00 0000 7242 0000 00da  r>...r>...rB....
-00002eb0: 1772 6567 7265 7373 696f 6e5f 6175 676d  .regression_augm
-00002ec0: 656e 7461 7469 6f6e 8601 0000 7320 0000  entation....s ..
-00002ed0: 0004 0204 0108 0104 0112 ff14 031a 010e  ................
-00002ee0: 0112 0112 0812 020c 020e 010c 030c 0104  ................
-00002ef0: fe7a 1d4d 6567 616e 2e72 6567 7265 7373  .z.Megan.regress
-00002f00: 696f 6e5f 6175 676d 656e 7461 7469 6f6e  ion_augmentation
-00002f10: da0e 7570 6461 7465 5f77 6569 6768 7473  ..update_weights
-00002f20: 6304 0000 0000 0000 0000 0000 0013 0000  c...............
-00002f30: 0008 0000 0043 0000 0073 3a01 0000 7c00  .....C...s:...|.
-00002f40: 6a00 7209 7c02 5c03 7d04 7d05 7d05 6e02  j.r.|.\.}.}.}.n.
-00002f50: 7c02 7d04 6401 7d06 7401 a002 a100 8f6c  |.}.d.}.t......l
-00002f60: 7d07 7c00 7c01 6402 6402 6403 8d03 7d08  }.|.|.d.d.d...}.
-00002f70: 7c08 5c03 7d09 7d0a 7d0b 6700 7d0c 7403  |.\.}.}.}.g.}.t.
-00002f80: 7c00 6a04 8301 4400 5d1c 7d0d 7401 6a05  |.j...D.].}.t.j.
-00002f90: 7c0a 6400 6400 8502 6400 6400 8502 7c0d  |.d.d...d.d...|.
-00002fa0: 6603 1900 6404 6405 8d02 7d0e 7c00 a006  f...d.d...}.|...
-00002fb0: 7c0e a101 7d0f 7c0c a007 7c0f a101 0100  |...}.|...|.....
-00002fc0: 7125 7c00 a008 7c0c a101 7d0c 7c00 6a09  q%|...|...}.|.j.
-00002fd0: 7261 7c00 a00a 7c04 a101 5c02 7d04 7d10  ra|...|...\.}.}.
-00002fe0: 7c0c 7d09 7c00 6a04 7c00 a00b 7c04 7c10  |.}.|.j.|...|.|.
-00002ff0: 1400 7c09 7c10 1400 a102 1400 7d06 6e10  ..|.|.......}.n.
-00003000: 740c 7c0c 7c00 6a0d 6406 6407 8d03 7d09  t.|.|.j.d.d...}.
-00003010: 7c00 a00e 7c04 7c09 7c04 1400 a102 7d06  |...|.|.|.....}.
-00003020: 7c06 7c00 6a0f 3900 7d06 5700 6400 0400  |.|.j.9.}.W.d...
-00003030: 0400 8303 0100 6e08 3100 7380 7701 0100  ......n.1.s.w...
-00003040: 0100 0100 5900 0100 7c00 6a10 7d11 7c07  ....Y...|.j.}.|.
-00003050: a011 7c06 7c11 a102 7d12 7c03 7299 7c00  ..|.|...}.|.r.|.
-00003060: 6a12 a013 7414 7c12 7c11 8302 a101 0100  j...t.|.|.......
-00003070: 6408 7c06 6901 5300 2909 4e72 0100 0000  d.|.i.S.).Nr....
-00003080: 54a9 0272 7c00 0000 7230 0000 0072 3600  T..r|...r0...r6.
-00003090: 0000 7237 0000 0072 1500 0000 a902 da05  ..r7...r........
-000030a0: 7368 6966 74da 0a6d 756c 7469 706c 6965  shift..multiplie
-000030b0: 72da 0865 7870 5f6c 6f73 7329 1572 3000  r..exp_loss).r0.
-000030c0: 0000 7280 0000 00da 0c47 7261 6469 656e  ..r......Gradien
-000030d0: 7454 6170 6572 8400 0000 7220 0000 0072  tTaper....r ...r
-000030e0: 8500 0000 7258 0000 0072 4c00 0000 7259  ....rX...rL...rY
-000030f0: 0000 0072 7b00 0000 72ae 0000 0072 6700  ...r{...r....rg.
-00003100: 0000 7211 0000 0072 2400 0000 7262 0000  ..r....r$...rb..
-00003110: 0072 2300 0000 da13 7472 6169 6e61 626c  .r#.....trainabl
-00003120: 655f 7661 7269 6162 6c65 73da 0867 7261  e_variables..gra
-00003130: 6469 656e 74da 096f 7074 696d 697a 6572  dient..optimizer
-00003140: da0f 6170 706c 795f 6772 6164 6965 6e74  ..apply_gradient
-00003150: 7372 5700 0000 2913 726c 0000 0072 8f00  srW...).rl...r..
-00003160: 0000 da01 7972 af00 0000 72a5 0000 0072  ....yr....r....r
-00003170: 4100 0000 72b4 0000 00da 0474 6170 65da  A...r......tape.
-00003180: 0679 5f70 7265 64da 086f 7574 5f70 7265  .y_pred..out_pre
-00003190: 64da 076e 695f 7072 6564 da07 6569 5f70  d..ni_pred..ei_p
-000031a0: 7265 6472 9700 0000 7299 0000 00da 166e  redr....r......n
-000031b0: 6f64 655f 696d 706f 7274 616e 6365 735f  ode_importances_
-000031c0: 736c 6963 6572 9d00 0000 da04 6d61 736b  slicer......mask
-000031d0: da0e 7472 6169 6e61 626c 655f 7661 7273  ..trainable_vars
-000031e0: da0d 6578 705f 6772 6164 6965 6e74 7372  ..exp_gradientsr
-000031f0: 3e00 0000 723e 0000 0072 4200 0000 da16  >...r>...rB.....
-00003200: 7472 6169 6e5f 7374 6570 5f65 7870 6c61  train_step_expla
-00003210: 6e61 7469 6f6e a401 0000 7338 0000 0006  nation....s8....
-00003220: 030c 0104 0204 020a 010e 020a 0104 070e  ................
-00003230: 0120 010a 010c 020a 0306 020e 0104 010e  . ..............
-00003240: 0106 0108 ff10 0510 010c 021c e106 220c  ..............".
-00003250: 0104 0312 0108 027a 1c4d 6567 616e 2e74  .......z.Megan.t
-00003260: 7261 696e 5f73 7465 705f 6578 706c 616e  rain_step_explan
-00003270: 6174 696f 6e63 0200 0000 0000 0000 0000  ationc..........
-00003280: 0000 1800 0000 0800 0000 4300 0000 73d8  ..........C...s.
-00003290: 0100 0074 007c 0183 0164 016b 0272 0c7c  ...t.|...d.k.r.|
-000032a0: 015c 037d 027d 037d 046e 0664 007d 047c  .\.}.}.}.n.d.}.|
-000032b0: 015c 027d 027d 037c 006a 0164 026b 0372  .\.}.}.|.j.d.k.r
-000032c0: 217c 006a 0272 217c 00a0 037c 027c 03a1  !|.j.r!|...|.|..
-000032d0: 027d 056e 0269 007d 0564 027d 0674 04a0  .}.n.i.}.d.}.t..
-000032e0: 05a1 008f 8c7d 077c 035c 037d 087d 097d  .....}.|.\.}.}.}
-000032f0: 0a7c 007c 0264 0364 0364 048d 035c 037d  .|.|.d.d.d...\.}
-00003300: 0b7d 0c7d 0d7c 006a 067c 087c 097c 0a67  .}.}.|.j.|.|.|.g
-00003310: 037c 0b7c 0c7c 0d67 037c 047c 006a 0764  .|.|.|.g.|.|.j.d
-00003320: 058d 047d 0e7c 006a 0164 026b 0372 ae7c  ...}.|.j.d.k.r.|
-00003330: 006a 0273 ae67 007d 0f74 087c 006a 0983  .j.s.g.}.t.|.j..
-00003340: 0144 005d 1c7d 1074 046a 0a7c 0c64 0064  .D.].}.t.j.|.d.d
-00003350: 0085 0264 0064 0085 027c 1066 0319 0064  ...d.d...|.f...d
-00003360: 0664 078d 027d 117c 00a0 0b7c 11a1 017d  .d...}.|...|...}
-00003370: 127c 0fa0 0c7c 12a1 0101 0071 587c 00a0  .|...|.....qX|..
-00003380: 0d7c 0fa1 017d 0f7c 006a 0e72 917c 00a0  .|...}.|.j.r.|..
-00003390: 0f7c 08a1 015c 027d 137d 147c 0f7d 157c  .|...\.}.}.|.}.|
-000033a0: 00a0 107c 137c 1414 007c 157c 1414 00a1  ...|.|...|.|....
-000033b0: 027d 066e 1074 117c 0f7c 006a 1264 0864  .}.n.t.|.|.j.d.d
-000033c0: 098d 037c 0814 007d 157c 00a0 137c 087c  ...|...}.|...|.|
-000033d0: 15a1 027d 067c 067c 006a 0139 007d 067c  ...}.|.|.j.9.}.|
-000033e0: 067c 0564 0a3c 007c 0e7c 0637 007d 0e57  .|.d.<.|.|.7.}.W
-000033f0: 0064 0004 0004 0083 0301 006e 0831 0073  .d.........n.1.s
-00003400: b877 0101 0001 0001 0059 0001 007c 006a  .w.......Y...|.j
-00003410: 147d 167c 07a0 157c 0e7c 16a1 027d 177c  .}.|...|.|...}.|
-00003420: 006a 16a0 1774 187c 177c 1683 02a1 0101  .j...t.|.|......
-00003430: 007c 006a 196a 1a7c 037c 006a 1b73 d87c  .|.j.j.|.|.j.s.|
-00003440: 0b6e 047c 0b7c 0c7c 0d67 037c 0464 0b8d  .n.|.|.|.g.|.d..
-00003450: 0301 0069 0064 0c64 0d84 007c 006a 1c44  ...i.d.d...|.j.D
-00003460: 0083 01a5 017c 05a5 0153 0029 0e4e e903  .....|...S.).N..
-00003470: 0000 0072 0100 0000 5472 b000 0000 2902  ...r....Tr....).
-00003480: da0d 7361 6d70 6c65 5f77 6569 6768 74da  ..sample_weight.
-00003490: 1572 6567 756c 6172 697a 6174 696f 6e5f  .regularization_
-000034a0: 6c6f 7373 6573 7236 0000 0072 3700 0000  lossesr6...r7...
-000034b0: 7217 0000 0072 b100 0000 72b4 0000 0029  r....r....r....)
-000034c0: 0172 c600 0000 6301 0000 0000 0000 0000  .r....c.........
-000034d0: 0000 0002 0000 0005 0000 0053 0000 0073  ...........S...s
-000034e0: 1800 0000 6900 7c00 5d08 7d01 7c01 6a00  ....i.|.].}.|.j.
-000034f0: 7c01 a001 a100 9302 7102 5300 723e 0000  |.......q.S.r>..
-00003500: 0029 02da 046e 616d 65da 0672 6573 756c  .)...name..resul
-00003510: 7429 0272 4000 0000 da01 6d72 3e00 0000  t).r@.....mr>...
-00003520: 723e 0000 0072 4200 0000 da0a 3c64 6963  r>...rB.....<dic
-00003530: 7463 6f6d 703e 2602 0000 7302 0000 0018  tcomp>&...s.....
-00003540: 007a 244d 6567 616e 2e74 7261 696e 5f73  .z$Megan.train_s
-00003550: 7465 702e 3c6c 6f63 616c 733e 2e3c 6469  tep.<locals>.<di
-00003560: 6374 636f 6d70 3e29 1d72 6b00 0000 7223  ctcomp>).rk...r#
-00003570: 0000 0072 2800 0000 72c4 0000 0072 8000  ...r(...r....r..
-00003580: 0000 72b5 0000 00da 0d63 6f6d 7069 6c65  ..r......compile
-00003590: 645f 6c6f 7373 725e 0000 0072 8400 0000  d_lossr^...r....
-000035a0: 7220 0000 0072 8500 0000 7258 0000 0072  r ...r....rX...r
-000035b0: 4c00 0000 7259 0000 0072 7b00 0000 72ae  L...rY...r{...r.
-000035c0: 0000 0072 6700 0000 7211 0000 0072 2400  ...rg...r....r$.
-000035d0: 0000 7262 0000 0072 b600 0000 72b7 0000  ..rb...r....r...
-000035e0: 0072 b800 0000 72b9 0000 0072 5700 0000  .r....r....rW...
-000035f0: da10 636f 6d70 696c 6564 5f6d 6574 7269  ..compiled_metri
-00003600: 6373 da0c 7570 6461 7465 5f73 7461 7465  cs..update_state
-00003610: 7230 0000 00da 076d 6574 7269 6373 2918  r0.....metrics).
-00003620: 726c 0000 00da 0464 6174 6172 8f00 0000  rl.....datar....
-00003630: 72ba 0000 0072 c600 0000 da0b 6578 705f  r....r......exp_
-00003640: 6d65 7472 6963 7372 b400 0000 72bb 0000  metricsr....r...
-00003650: 0072 a500 0000 da07 6e69 5f74 7275 65da  .r......ni_true.
-00003660: 0765 695f 7472 7565 72bd 0000 0072 be00  .ei_truer....r..
-00003670: 0000 72bf 0000 00da 046c 6f73 7372 9700  ..r......lossr..
-00003680: 0000 7299 0000 0072 c000 0000 729d 0000  ..r....r....r...
-00003690: 00da 095f 6f75 745f 7472 7565 72c1 0000  ..._out_truer...
-000036a0: 00da 095f 6f75 745f 7072 6564 72c2 0000  ..._out_predr...
-000036b0: 00da 0967 7261 6469 656e 7473 723e 0000  ...gradientsr>..
-000036c0: 0072 3e00 0000 7242 0000 00da 0a74 7261  .r>...rB.....tra
-000036d0: 696e 5f73 7465 70d8 0100 0073 7000 0000  in_step....sp...
-000036e0: 0c01 0c01 0402 0801 1006 0e01 0402 0402  ................
-000036f0: 0a01 0a02 1401 0401 0801 0801 0201 0401  ................
-00003700: 06fc 1007 0406 0e01 2001 0a01 0c02 0a03  ........ .......
-00003710: 0602 0e01 0401 0a01 0601 06ff 0206 0201  ................
-00003720: 0401 0201 04fd 0204 04fc 0c05 0a02 0801  ................
-00003730: 0801 0280 1cd3 062f 0c01 1202 0602 0201  ......./........
-00003740: 1201 0201 06fd 0208 0e01 02ff 0202 04fe  ................
-00003750: 7a10 4d65 6761 6e2e 7472 6169 6e5f 7374  z.Megan.train_st
-00003760: 6570 2903 4646 4e72 4500 0000 291a da08  ep).FFNrE...)...
-00003770: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
-00003780: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
-00003790: 5f5f da07 5f5f 646f 635f 5fda 0174 da04  __..__doc__..t..
-000037a0: 4c69 7374 7269 0000 00da 0373 7472 da04  Listri.....str..
-000037b0: 626f 6f6c 726a 0000 00da 084f 7074 696f  boolrj.....Optio
-000037c0: 6e61 6c72 4700 0000 da06 6c61 7965 7273  nalrG.....layers
-000037d0: da05 4c61 7965 72da 0554 7570 6c65 724a  ..Layer..TuplerJ
-000037e0: 0000 0072 7500 0000 da08 7072 6f70 6572  ...ru.....proper
-000037f0: 7479 727b 0000 0072 8000 0000 da0c 5261  tyr{...r......Ra
-00003800: 6767 6564 5465 6e73 6f72 72a1 0000 0072  ggedTensorr....r
-00003810: ae00 0000 72c4 0000 0072 d800 0000 da0d  ....r....r......
-00003820: 5f5f 636c 6173 7363 656c 6c5f 5f72 3e00  __classcell__r>.
-00003830: 0000 723e 0000 0072 7800 0000 7242 0000  ..r>...rx...rB..
-00003840: 0072 1200 0000 1400 0000 73be 0000 0008  .r........s.....
-00003850: 0004 0102 0c02 0102 0102 0102 0202 0102  ................
-00003860: 0102 0102 0102 0102 0102 0102 0102 0104  ................
-00003870: 0202 0102 0102 0102 0102 0102 0102 0102  ................
-00003880: 0104 e508 0202 fe02 0302 fd02 0402 fc02  ................
-00003890: 0502 fb02 0602 fa08 0802 f802 0902 f702  ................
-000038a0: 0a02 f602 0b02 f502 0c02 f402 0d02 f312  ................
-000038b0: 0e02 f202 0f02 f102 1002 f002 1102 ef08  ................
-000038c0: 1302 ed02 1402 ec02 1502 eb02 1602 ea12  ................
-000038d0: 1702 e918 1802 e808 1902 e702 1a02 e602  ................
-000038e0: 1b0a e500 7f0c 4502 1a10 0102 0502 0102  ......E.........
-000038f0: 0104 fc02 0202 fe02 0302 fd0a 040a fc00  ................
-00003900: 7f08 0702 1f04 ff02 010a ff10 3472 1200  ............4r..
-00003910: 0000 2920 da06 7479 7069 6e67 72dd 0000  ..) ..typingr...
-00003920: 00da 0a74 656e 736f 7266 6c6f 7772 8000  ...tensorflowr..
-00003930: 0000 da10 7465 6e73 6f72 666c 6f77 2e6b  ....tensorflow.k
-00003940: 6572 6173 da05 6b65 7261 7372 4700 0000  eras..kerasrG...
-00003950: da1e 7465 6e73 6f72 666c 6f77 2e70 7974  ..tensorflow.pyt
-00003960: 686f 6e2e 6b65 7261 732e 656e 6769 6e65  hon.keras.engine
-00003970: 7202 0000 00da 106b 6763 6e6e 2e64 6174  r......kgcnn.dat
-00003980: 612e 7574 696c 7372 0300 0000 da14 6b67  a.utilsr......kg
-00003990: 636e 6e2e 6c61 7965 7273 2e6d 6f64 756c  cnn.layers.modul
-000039a0: 6573 7204 0000 0072 0500 0000 7206 0000  esr....r....r...
-000039b0: 0072 0700 0000 7208 0000 0072 0900 0000  .r....r....r....
-000039c0: da14 6b67 636e 6e2e 6c61 7965 7273 2e70  ..kgcnn.layers.p
-000039d0: 6f6f 6c69 6e67 720a 0000 0072 0b00 0000  oolingr....r....
-000039e0: 720c 0000 00da 1e67 7261 7068 5f61 7474  r......graph_att
-000039f0: 656e 7469 6f6e 5f73 7475 6465 6e74 2e6c  ention_student.l
-00003a00: 6179 6572 7372 0d00 0000 720e 0000 00da  ayersr....r.....
-00003a10: 2067 7261 7068 5f61 7474 656e 7469 6f6e   graph_attention
-00003a20: 5f73 7475 6465 6e74 2e74 7261 696e 696e  _student.trainin
-00003a30: 6772 0f00 0000 7210 0000 0072 1100 0000  gr....r....r....
-00003a40: 7248 0000 0072 4900 0000 7212 0000 0072  rH...rI...r....r
-00003a50: 3e00 0000 723e 0000 0072 3e00 0000 7242  >...r>...r>...rB
-00003a60: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-00003a70: 0073 2200 0000 0800 0802 0c01 0c01 0c01  .s".............
-00003a80: 0c01 1001 1401 0c01 0c01 0c01 0c01 0c01  ................
-00003a90: 0c01 0c01 0c01 1803                      ........
+00000a80: 3ba0 3c74 3da1 017c 005f 3e74 006a 38a0  ;.<t=..|._>t.j8.
+00000a90: 3fa1 007c 005f 4074 006a 38a0 41a1 007c  ?..|._@t.j8.A..|
+00000aa0: 005f 4274 3ba0 3c74 43a1 017c 005f 447c  ._Bt;.<tC..|._D|
+00000ab0: 006a 1664 1375 0190 0172 977c 1664 1375  .j.d.u...r.|.d.u
+00000ac0: 0190 0173 4b4a 0064 1483 0182 0174 457c  ...sKJ.d.....tE|
+00000ad0: 1674 4674 4766 0283 0290 0172 577c 1667  .tFtGf.....rW|.g
+00000ae0: 017c 005f 1774 487c 006a 1783 017d 1e74  .|._.tH|.j...}.t
+00000af0: 487c 006a 1683 017d 1f7c 1e64 1514 007c  H|.j...}.|.d...|
+00000b00: 076b 0290 0173 734a 0064 167c 1e9b 0064  .k...ssJ.d.|...d
+00000b10: 177c 079b 0064 189d 0583 0182 017c 1e7c  .|...d.......|.|
+00000b20: 1064 0619 006b 0290 0173 874a 0064 197c  .d...k...s.J.d.|
+00000b30: 1e9b 0064 1a7c 1064 0619 009b 0064 1b9d  ...d.|.d.....d..
+00000b40: 0583 0182 017c 1e7c 1f6b 0290 0173 994a  .....|.|.k...s.J
+00000b50: 0064 197c 1e9b 0064 1c7c 1f9b 0064 1b9d  .d.|...d.|...d..
+00000b60: 0583 0182 0164 1353 0064 1353 0029 1d61  .....d.S.d.S.).a
+00000b70: 250f 0000 0a20 2020 2020 2020 2041 7267  %....        Arg
+00000b80: 733a 0a20 2020 2020 2020 2020 2020 2075  s:.            u
+00000b90: 6e69 7473 3a20 4120 6c69 7374 206f 6620  nits: A list of 
+00000ba0: 696e 7473 2077 6865 7265 2065 6163 6820  ints where each 
+00000bb0: 656c 656d 656e 7420 636f 6e66 6967 7572  element configur
+00000bc0: 6573 2061 6e20 6164 6469 7469 6f6e 616c  es an additional
+00000bd0: 2061 7474 656e 7469 6f6e 206c 6179 6572   attention layer
+00000be0: 2e20 5468 6520 6e75 6d65 7269 630a 2020  . The numeric.  
+00000bf0: 2020 2020 2020 2020 2020 2020 2020 7661                va
+00000c00: 6c75 6520 6465 7465 726d 696e 6573 2074  lue determines t
+00000c10: 6865 206e 756d 6265 7220 6f66 2068 6964  he number of hid
+00000c20: 6465 6e20 756e 6974 7320 746f 2062 6520  den units to be 
+00000c30: 7573 6564 2069 6e20 7468 6520 6174 7465  used in the atte
+00000c40: 6e74 696f 6e20 6865 6164 7320 6f66 2074  ntion heads of t
+00000c50: 6861 7420 6c61 7965 720a 2020 2020 2020  hat layer.      
+00000c60: 2020 2020 2020 6163 7469 7661 7469 6f6e        activation
+00000c70: 3a20 5468 6520 6163 7469 7661 7469 6f6e  : The activation
+00000c80: 2066 756e 6374 696f 6e20 746f 2062 6520   function to be 
+00000c90: 7573 6564 2077 6974 6869 6e20 7468 6520  used within the 
+00000ca0: 6174 7465 6e74 696f 6e20 6c61 7965 7273  attention layers
+00000cb0: 206f 6620 7468 6520 6e65 7477 6f72 6b0a   of the network.
+00000cc0: 2020 2020 2020 2020 2020 2020 7573 655f              use_
+00000cd0: 6269 6173 3a20 5768 6574 6865 7220 7468  bias: Whether th
+00000ce0: 6520 6c61 7965 7273 206f 6620 7468 6520  e layers of the 
+00000cf0: 6e65 7477 6f72 6b20 7368 6f75 6c64 2075  network should u
+00000d00: 7365 2062 6961 7320 7765 6967 6874 7320  se bias weights 
+00000d10: 6174 2061 6c6c 0a20 2020 2020 2020 2020  at all.         
+00000d20: 2020 2064 726f 706f 7574 5f72 6174 653a     dropout_rate:
+00000d30: 2054 6865 2064 726f 706f 7574 2072 6174   The dropout rat
+00000d40: 6520 746f 2062 6520 6170 706c 6965 6420  e to be applied 
+00000d50: 6166 7465 7220 2a65 6163 682a 206f 6620  after *each* of 
+00000d60: 7468 6520 6174 7465 6e74 696f 6e20 6c61  the attention la
+00000d70: 7965 7273 206f 6620 7468 6520 6e65 7477  yers of the netw
+00000d80: 6f72 6b2e 0a20 2020 2020 2020 2020 2020  ork..           
+00000d90: 2075 7365 5f65 6467 655f 6665 6174 7572   use_edge_featur
+00000da0: 6573 3a20 5768 6574 6865 7220 6564 6765  es: Whether edge
+00000db0: 2066 6561 7475 7265 7320 7368 6f75 6c64   features should
+00000dc0: 2062 6520 7573 6564 2e20 4765 6e65 7261   be used. Genera
+00000dd0: 6c6c 7920 7468 6520 6e65 7477 6f72 6b20  lly the network 
+00000de0: 7375 7070 6f72 7473 2074 6865 0a20 2020  supports the.   
+00000df0: 2020 2020 2020 2020 2020 2020 2075 7361               usa
+00000e00: 6765 206f 6620 6564 6765 2066 6561 7475  ge of edge featu
+00000e10: 7265 732c 2062 7574 2069 6620 7468 6520  res, but if the 
+00000e20: 696e 7075 7420 6461 7461 2064 6f65 7320  input data does 
+00000e30: 6e6f 7420 636f 6e74 6169 6e20 6564 6765  not contain edge
+00000e40: 2066 6561 7475 7265 732c 2074 6869 7320   features, this 
+00000e50: 7368 6f75 6c64 2062 650a 2020 2020 2020  should be.      
+00000e60: 2020 2020 2020 2020 2020 7365 7420 746f            set to
+00000e70: 2046 616c 7365 2e0a 2020 2020 2020 2020   False..        
+00000e80: 2020 2020 696d 706f 7274 616e 6365 5f75      importance_u
+00000e90: 6e69 7473 3a20 4120 6c69 7374 206f 6620  nits: A list of 
+00000ea0: 696e 7473 2077 6865 7265 2065 6163 6820  ints where each 
+00000eb0: 656c 656d 656e 7420 636f 6e66 6967 7572  element configur
+00000ec0: 6573 2061 6e6f 7468 6572 2064 656e 7365  es another dense
+00000ed0: 206c 6179 6572 2069 6e20 7468 650a 2020   layer in the.  
+00000ee0: 2020 2020 2020 2020 2020 2020 2020 7375                su
+00000ef0: 626e 6574 776f 726b 2074 6861 7420 7072  bnetwork that pr
+00000f00: 6f64 7563 6573 2074 6865 206e 6f64 6520  oduces the node 
+00000f10: 696d 706f 7274 616e 6365 2074 656e 736f  importance tenso
+00000f20: 7220 6672 6f6d 2074 6865 206d 6169 6e20  r from the main 
+00000f30: 6e6f 6465 2065 6d62 6564 6469 6e67 732e  node embeddings.
+00000f40: 2054 6865 0a20 2020 2020 2020 2020 2020   The.           
+00000f50: 2020 2020 206e 756d 6572 6963 2076 616c       numeric val
+00000f60: 7565 2064 6574 6572 6d69 6e65 7320 7468  ue determines th
+00000f70: 6520 6e75 6d62 6572 206f 6620 6869 6464  e number of hidd
+00000f80: 656e 2075 6e69 7473 2069 6e20 7468 6174  en units in that
+00000f90: 206c 6179 6572 2e0a 2020 2020 2020 2020   layer..        
+00000fa0: 2020 2020 696d 706f 7274 616e 6365 5f63      importance_c
+00000fb0: 6861 6e6e 656c 733a 2054 6865 2069 6e74  hannels: The int
+00000fc0: 206e 756d 6265 7220 6f66 2065 7870 6c61   number of expla
+00000fd0: 6e61 7469 6f6e 2063 6861 6e6e 656c 7320  nation channels 
+00000fe0: 746f 2062 6520 7072 6f64 7563 6564 2062  to be produced b
+00000ff0: 7920 7468 6520 6e65 7477 6f72 6b2e 2054  y the network. T
+00001000: 6869 730a 2020 2020 2020 2020 2020 2020  his.            
+00001010: 2020 2020 6973 2074 6865 2076 616c 7565      is the value
+00001020: 2072 6566 6572 7265 6420 746f 2061 7320   referred to as 
+00001030: 224b 222e 204e 6f74 6520 7468 6174 2074  "K". Note that t
+00001040: 6869 7320 7769 6c6c 2061 6c73 6f20 6465  his will also de
+00001050: 7465 726d 696e 6520 7468 6520 6e75 6d62  termine the numb
+00001060: 6572 206f 6620 6174 7465 6e74 696f 6e0a  er of attention.
+00001070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001080: 6865 6164 7320 7573 6564 2077 6974 6869  heads used withi
+00001090: 6e20 7468 6520 6174 7465 6e74 696f 6e20  n the attention 
+000010a0: 7375 626e 6574 776f 726b 2e0a 2020 2020  subnetwork..    
+000010b0: 2020 2020 2020 2020 696d 706f 7274 616e          importan
+000010c0: 6365 5f66 6163 746f 723a 2054 6865 2077  ce_factor: The w
+000010d0: 6569 6768 7420 6f66 2074 6865 2065 7870  eight of the exp
+000010e0: 6c61 6e61 7469 6f6e 2d6f 6e6c 7920 7472  lanation-only tr
+000010f0: 6169 6e20 7374 6570 2e20 4966 2074 6869  ain step. If thi
+00001100: 7320 6973 2073 6574 2074 6f20 6578 6163  s is set to exac
+00001110: 746c 790a 2020 2020 2020 2020 2020 2020  tly.            
+00001120: 2020 2020 7a65 726f 2074 6865 6e20 7468      zero then th
+00001130: 6520 6578 706c 616e 6174 696f 6e20 7472  e explanation tr
+00001140: 6169 6e20 7374 6570 2077 696c 6c20 6e6f  ain step will no
+00001150: 7420 6265 2065 7865 6375 7465 6420 6174  t be executed at
+00001160: 2061 6c6c 2028 6c65 7373 2063 6f6d 7075   all (less compu
+00001170: 7461 7469 6f6e 616c 6c79 0a20 2020 2020  tationally.     
+00001180: 2020 2020 2020 2020 2020 2065 7870 656e             expen
+00001190: 7369 7665 290a 2020 2020 2020 2020 2020  sive).          
+000011a0: 2020 696d 706f 7274 616e 6365 5f6d 756c    importance_mul
+000011b0: 7469 706c 6965 723a 2041 6e20 6164 6469  tiplier: An addi
+000011c0: 7469 6f6e 616c 2068 7970 6572 7061 7261  tional hyperpara
+000011d0: 6d65 7465 7220 6f66 2074 6865 2065 7870  meter of the exp
+000011e0: 6c61 6e61 7469 6f6e 2d6f 6e6c 7920 7472  lanation-only tr
+000011f0: 6169 6e20 7374 6570 2e20 5468 6973 0a20  ain step. This. 
+00001200: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00001210: 7320 6573 7365 6e74 6961 6c6c 7920 7468  s essentially th
+00001220: 6520 7363 616c 696e 6720 6661 6374 6f72  e scaling factor
+00001230: 2074 6861 7420 6973 2061 7070 6c69 6564   that is applied
+00001240: 2074 6f20 7468 6520 7661 6c75 6573 206f   to the values o
+00001250: 6620 7468 6520 6461 7461 7365 7420 7375  f the dataset su
+00001260: 6368 2074 6861 740a 2020 2020 2020 2020  ch that.        
+00001270: 2020 2020 2020 2020 7468 6520 7461 7267          the targ
+00001280: 6574 2076 616c 7565 7320 6361 6e20 7265  et values can re
+00001290: 6173 6f6e 6162 6c79 2062 6520 6170 7072  asonably be appr
+000012a0: 6f78 696d 6174 6564 2062 7920 6120 7375  oximated by a su
+000012b0: 6d20 6f66 205b 302c 2031 5d20 696d 706f  m of [0, 1] impo
+000012c0: 7274 616e 6365 2076 616c 7565 732e 0a20  rtance values.. 
+000012d0: 2020 2020 2020 2020 2020 2073 7061 7273             spars
+000012e0: 6974 795f 6661 6374 6f72 3a20 5468 6520  ity_factor: The 
+000012f0: 636f 6566 6669 6369 656e 7420 666f 7220  coefficient for 
+00001300: 7468 6520 7370 6172 7369 7479 2072 6567  the sparsity reg
+00001310: 756c 6172 697a 6174 696f 6e20 6f66 2074  ularization of t
+00001320: 6865 206e 6f64 6520 696d 706f 7274 616e  he node importan
+00001330: 6365 0a20 2020 2020 2020 2020 2020 2020  ce.             
+00001340: 2020 2074 656e 736f 722e 0a20 2020 2020     tensor..     
+00001350: 2020 2020 2020 2063 6f6e 6361 745f 6865         concat_he
+00001360: 6164 733a 2057 6865 7468 6572 2074 6f20  ads: Whether to 
+00001370: 636f 6e63 6174 2074 6865 2068 6561 6473  concat the heads
+00001380: 206f 6620 7468 6520 6174 7465 6e74 696f   of the attentio
+00001390: 6e20 7375 626e 6574 776f 726b 2e20 5468  n subnetwork. Th
+000013a0: 6520 6465 6661 756c 7420 6973 2054 7275  e default is Tru
+000013b0: 652e 2049 6e0a 2020 2020 2020 2020 2020  e. In.          
+000013c0: 2020 2020 2020 7468 6174 2063 6173 6520        that case 
+000013d0: 7468 6520 6f75 7470 7574 206f 6620 6561  the output of ea
+000013e0: 6368 2069 6e64 6976 6964 7561 6c20 6174  ch individual at
+000013f0: 7465 6e74 696f 6e20 6865 6164 2069 7320  tention head is 
+00001400: 636f 6e63 6174 656e 6174 6564 2061 6e64  concatenated and
+00001410: 2074 6865 2063 6f6e 6361 7465 6e61 7465   the concatenate
+00001420: 640a 2020 2020 2020 2020 2020 2020 2020  d.              
+00001430: 2020 7665 6374 6f72 2069 7320 7468 656e    vector is then
+00001440: 2075 7365 6420 6173 2074 6865 2069 6e70   used as the inp
+00001450: 7574 206f 6620 7468 6520 6e65 7874 2061  ut of the next a
+00001460: 7474 656e 7469 6f6e 206c 6179 6572 2773  ttention layer's
+00001470: 2068 6561 6473 2e20 4966 2074 6869 7320   heads. If this 
+00001480: 6973 2046 616c 7365 2c20 7468 650a 2020  is False, the.  
+00001490: 2020 2020 2020 2020 2020 2020 2020 7665                ve
+000014a0: 6374 6f72 7320 6172 6520 6176 6572 6167  ctors are averag
+000014b0: 6520 706f 6f6c 6564 2069 6e73 7465 6164  e pooled instead
+000014c0: 2e0a 2020 2020 2020 2020 2020 2020 6669  ..            fi
+000014d0: 6e61 6c5f 756e 6974 733a 2041 206c 6973  nal_units: A lis
+000014e0: 7420 6f66 2069 6e74 7320 7768 6572 6520  t of ints where 
+000014f0: 6561 6368 2065 6c65 6d65 6e74 2063 6f6e  each element con
+00001500: 6669 6775 7265 7320 616e 6f74 6865 7220  figures another 
+00001510: 6465 6e73 6520 6c61 7965 7220 696e 2074  dense layer in t
+00001520: 6865 204d 4c50 0a20 2020 2020 2020 2020  he MLP.         
+00001530: 2020 2020 2020 2061 7420 7468 6520 7461         at the ta
+00001540: 696c 2065 6e64 206f 6620 7468 6520 6e65  il end of the ne
+00001550: 7477 6f72 6b2e 2054 6865 206e 756d 6572  twork. The numer
+00001560: 6963 2076 616c 7565 2064 6574 6572 6d69  ic value determi
+00001570: 6e65 7320 7468 6520 6e75 6d62 6572 206f  nes the number o
+00001580: 6620 7468 6520 6869 6464 656e 2075 6e69  f the hidden uni
+00001590: 7473 0a20 2020 2020 2020 2020 2020 2020  ts.             
+000015a0: 2020 2069 6e20 7468 6174 206c 6179 6572     in that layer
+000015b0: 2e20 4e6f 7465 2074 6861 7420 7468 6520  . Note that the 
+000015c0: 6669 6e61 6c20 656c 656d 656e 7420 696e  final element in
+000015d0: 2074 6869 7320 6c69 7374 2068 6173 2074   this list has t
+000015e0: 6f20 6265 2074 6865 2073 616d 6520 6173  o be the same as
+000015f0: 2074 6865 2064 696d 656e 7369 6f6e 0a20   the dimension. 
+00001600: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00001610: 6f20 6265 2065 7870 6563 7465 6420 666f  o be expected fo
+00001620: 7220 7468 6520 7361 6d70 6c65 7320 6f66  r the samples of
+00001630: 2074 6865 2074 7261 696e 696e 6720 6461   the training da
+00001640: 7461 7365 7421 0a20 2020 2020 2020 2020  taset!.         
+00001650: 2020 2066 696e 616c 5f64 726f 706f 7574     final_dropout
+00001660: 5f72 6174 653a 2054 6865 2064 726f 706f  _rate: The dropo
+00001670: 7574 2072 6174 6520 746f 2062 6520 6170  ut rate to be ap
+00001680: 706c 6965 6420 6166 7465 7220 2a65 7665  plied after *eve
+00001690: 7279 2a20 6c61 7965 7220 6f66 2074 6865  ry* layer of the
+000016a0: 2066 696e 616c 204d 4c50 2e0a 2020 2020   final MLP..    
+000016b0: 2020 2020 2020 2020 6669 6e61 6c5f 6163          final_ac
+000016c0: 7469 7661 7469 6f6e 3a20 5468 6520 6163  tivation: The ac
+000016d0: 7469 7661 7469 6f6e 2074 6f20 6265 2061  tivation to be a
+000016e0: 7070 6c69 6564 2061 7420 7468 6520 7665  pplied at the ve
+000016f0: 7279 206c 6173 7420 6c61 7965 7220 6f66  ry last layer of
+00001700: 2074 6865 204d 4c50 2074 6f20 7072 6f64   the MLP to prod
+00001710: 7563 6520 7468 650a 2020 2020 2020 2020  uce the.        
+00001720: 2020 2020 2020 2020 6163 7475 616c 206f          actual o
+00001730: 7574 7075 7420 6f66 2074 6865 206e 6574  utput of the net
+00001740: 776f 726b 2e0a 2020 2020 2020 2020 2020  work..          
+00001750: 2020 6669 6e61 6c5f 706f 6f6c 696e 673a    final_pooling:
+00001760: 2054 6865 2070 6f6f 6c69 6e67 206d 6574   The pooling met
+00001770: 686f 6420 746f 2062 6520 7573 6564 2064  hod to be used d
+00001780: 7572 696e 6720 7468 6520 676c 6f62 616c  uring the global
+00001790: 2070 6f6f 6c69 6e67 2070 6861 7365 2069   pooling phase i
+000017a0: 6e20 7468 6520 6e65 7477 6f72 6b2e 0a20  n the network.. 
+000017b0: 2020 2020 2020 2020 2020 2072 6567 7265             regre
+000017c0: 7373 696f 6e5f 6c69 6d69 7473 3a20 4120  ssion_limits: A 
+000017d0: 7475 706c 6520 7768 6572 6520 7468 6520  tuple where the 
+000017e0: 6669 7273 7420 7661 6c75 6520 6973 2074  first value is t
+000017f0: 6865 206c 6f77 6572 206c 696d 6974 2066  he lower limit f
+00001800: 6f72 2074 6865 2065 7870 6563 7465 6420  or the expected 
+00001810: 7661 6c75 6520 7261 6e67 650a 2020 2020  value range.    
+00001820: 2020 2020 2020 2020 2020 2020 6f66 2074              of t
+00001830: 6865 2072 6567 7265 7373 696f 6e20 7461  he regression ta
+00001840: 736b 2061 6e64 2074 6568 2073 6563 6f6e  sk and teh secon
+00001850: 6420 7661 6c75 6520 7468 6520 7570 7065  d value the uppe
+00001860: 7220 6c69 6d69 742e 0a20 2020 2020 2020  r limit..       
+00001870: 2020 2020 2072 6567 7265 7373 696f 6e5f       regression_
+00001880: 7265 6665 7265 6e63 653a 2041 2072 6566  reference: A ref
+00001890: 6572 656e 6365 2076 616c 7565 2077 6869  erence value whi
+000018a0: 6368 2069 7320 696e 7369 6465 2074 6865  ch is inside the
+000018b0: 2072 616e 6765 206f 6620 6578 7065 6374   range of expect
+000018c0: 6564 2076 616c 7565 7320 2862 6573 7420  ed values (best 
+000018d0: 6966 0a20 2020 2020 2020 2020 2020 2020  if.             
+000018e0: 2020 2069 7420 7761 7320 696e 2074 6865     it was in the
+000018f0: 206d 6964 646c 652c 2062 7574 2064 6f65   middle, but doe
+00001900: 7320 6e6f 7420 6861 7665 2074 6f29 2e20  s not have to). 
+00001910: 4368 6f6f 7369 6e67 2064 6966 6665 7265  Choosing differe
+00001920: 6e74 2072 6566 6572 656e 6365 7320 7769  nt references wi
+00001930: 6c6c 2072 6573 756c 740a 2020 2020 2020  ll result.      
+00001940: 2020 2020 2020 2020 2020 696e 2064 6966            in dif
+00001950: 6665 7265 6e74 2065 7870 6c61 6e61 7469  ferent explanati
+00001960: 6f6e 732e 0a20 2020 2020 2020 2020 2020  ons..           
+00001970: 2072 6574 7572 6e5f 696d 706f 7274 616e   return_importan
+00001980: 6365 733a 2057 6865 7468 6572 2074 6865  ces: Whether the
+00001990: 2069 6d70 6f72 7461 6e63 6520 2f20 6578   importance / ex
+000019a0: 706c 616e 6174 696f 6e20 7465 6e73 6f72  planation tensor
+000019b0: 7320 7368 6f75 6c64 2062 6520 7265 7475  s should be retu
+000019c0: 726e 6564 2061 7320 616e 206f 7574 7075  rned as an outpu
+000019d0: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
+000019e0: 2020 6f66 2074 6865 206d 6f64 656c 2e20    of the model. 
+000019f0: 4966 2074 6869 7320 6973 2054 7275 652c  If this is True,
+00001a00: 2074 6865 206f 7574 7075 7420 6f66 2074   the output of t
+00001a10: 6865 206d 6f64 656c 2077 696c 6c20 6265  he model will be
+00001a20: 2061 2033 2d74 7570 6c65 3a0a 2020 2020   a 3-tuple:.    
+00001a30: 2020 2020 2020 2020 2020 2020 286f 7574              (out
+00001a40: 7075 742c 206e 6f64 6520 696d 706f 7274  put, node import
+00001a50: 616e 6365 732c 2065 6467 6520 696d 706f  ances, edge impo
+00001a60: 7274 616e 6365 7329 2c20 6f74 6865 7277  rtances), otherw
+00001a70: 6973 6520 6974 2069 7320 6a75 7374 2074  ise it is just t
+00001a80: 6865 206f 7574 7075 7420 6974 7365 6c66  he output itself
+00001a90: 0a20 2020 2020 2020 2054 2907 721a 0000  .        T).r...
+00001aa0: 00da 096e 756d 5f68 6561 6473 721e 0000  ...num_headsr...
+00001ab0: 0072 1b00 0000 721c 0000 00da 0e68 6173  .r....r......has
+00001ac0: 5f73 656c 665f 6c6f 6f70 7372 2700 0000  _self_loopsr'...
+00001ad0: 2901 da04 7261 7465 2901 da06 6661 6374  )...rate)...fact
+00001ae0: 6f72 2901 721b 0000 00e9 ffff ffff a901  or).r...........
+00001af0: da04 6178 6973 da04 6d65 616e 7201 0000  ..axis..meanr...
+00001b00: 0029 02da 0e70 6f6f 6c69 6e67 5f6d 6574  .)...pooling_met
+00001b10: 686f 64da 0d70 6f6f 6c69 6e67 5f69 6e64  hod..pooling_ind
+00001b20: 6578 7217 0000 0063 0100 0000 0000 0000  exr....c........
+00001b30: 0000 0000 0200 0000 0300 0000 5300 0000  ............S...
+00001b40: f310 0000 0067 007c 005d 047d 0164 0091  .....g.|.].}.d..
+00001b50: 0271 0253 00a9 0172 1300 0000 a900 a902  .q.S...r........
+00001b60: da02 2e30 da01 5f72 3e00 0000 723e 0000  ...0.._r>...r>..
+00001b70: 00fa 562f 6d65 6469 612f 7373 642f 5072  ..V/media/ssd/Pr
+00001b80: 6f67 7261 6d6d 696e 672f 6772 6170 685f  ogramming/graph_
+00001b90: 6174 7465 6e74 696f 6e5f 7374 7564 656e  attention_studen
+00001ba0: 742f 6772 6170 685f 6174 7465 6e74 696f  t/graph_attentio
+00001bb0: 6e5f 7374 7564 656e 742f 6d6f 6465 6c73  n_student/models
+00001bc0: 2f6d 6567 616e 2e70 79da 0a3c 6c69 7374  /megan.py..<list
+00001bd0: 636f 6d70 3e9d 0000 00f3 0200 0000 1000  comp>...........
+00001be0: 7a22 4d65 6761 6e2e 5f5f 696e 6974 5f5f  z"Megan.__init__
+00001bf0: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
+00001c00: 6f6d 703e 7218 0000 0029 0372 1a00 0000  omp>r....).r....
+00001c10: 721b 0000 0072 1c00 0000 2901 723a 0000  r....r....).r:..
+00001c20: 0063 0100 0000 0000 0000 0000 0000 0200  .c..............
+00001c30: 0000 0300 0000 5300 0000 723c 0000 0072  ......S...r<...r
+00001c40: 3d00 0000 723e 0000 0072 3f00 0000 723e  =...r>...r?...r>
+00001c50: 0000 0072 3e00 0000 7242 0000 0072 4300  ...r>...rB...rC.
+00001c60: 0000 ac00 0000 7244 0000 0063 0100 0000  ......rD...c....
+00001c70: 0000 0000 0000 0000 0200 0000 0300 0000  ................
+00001c80: 5300 0000 723c 0000 00a9 0154 723e 0000  S...r<.....Tr>..
+00001c90: 0072 3f00 0000 723e 0000 0072 3e00 0000  .r?...r>...r>...
+00001ca0: 7242 0000 0072 4300 0000 ae00 0000 7244  rB...rC.......rD
+00001cb0: 0000 004e 7a4e 596f 7520 6861 7665 2074  ...NzNYou have t
+00001cc0: 6f20 7375 7070 6c79 2061 2022 7265 6772  o supply a "regr
+00001cd0: 6573 7369 6f6e 5f72 6566 6572 656e 6365  ession_reference
+00001ce0: 2220 7661 6c75 6520 666f 7220 6578 706c  " value for expl
+00001cf0: 616e 6174 696f 6e20 636f 2d74 7261 696e  anation co-train
+00001d00: 696e 6721 7215 0000 007a 4c66 6f72 2065  ing!r....zLfor e
+00001d10: 7870 6c61 6e61 7469 6f6e 2063 6f2d 7472  xplanation co-tr
+00001d20: 6169 6e69 6e67 2c20 7468 6520 6e75 6d62  aining, the numb
+00001d30: 6572 206f 6620 7265 6772 6573 7369 6f6e  er of regression
+00001d40: 5f72 6566 6572 656e 6365 7320 2863 7572  _references (cur
+00001d50: 7265 6e74 6c79 207a 4629 2068 6173 2074  rently zF) has t
+00001d60: 6f20 6265 2065 7861 6374 6c79 2068 616c  o be exactly hal
+00001d70: 6620 7468 6520 6e75 6d62 6572 206f 6620  f the number of 
+00001d80: 696d 706f 7274 616e 6365 2063 6861 6e6e  importance chann
+00001d90: 656c 7320 2863 7572 7265 6e74 6c79 207a  els (currently z
+00001da0: 0229 217a 4c46 6f72 2065 7870 6c61 6e61  .)!zLFor explana
+00001db0: 7469 6f6e 2063 6f2d 7472 6169 6e69 6e67  tion co-training
+00001dc0: 2c20 7468 6520 6e75 6d62 6572 206f 6620  , the number of 
+00001dd0: 7265 6772 6573 7369 6f6e 5f72 6566 6572  regression_refer
+00001de0: 656e 6365 7320 2863 7572 7265 6e74 6c79  ences (currently
+00001df0: 207a 5429 2068 6173 2074 6f20 6265 2065   zT) has to be e
+00001e00: 7861 6374 6c79 2074 6865 2073 616d 6520  xactly the same 
+00001e10: 6173 2074 6865 2066 696e 616c 2075 6e69  as the final uni
+00001e20: 7420 636f 756e 7420 696e 2074 6865 204d  t count in the M
+00001e30: 4c50 2074 6169 6c20 656e 6420 2863 7572  LP tail end (cur
+00001e40: 7265 6e74 6c79 20fa 0129 7a55 2920 6861  rently ..)zU) ha
+00001e50: 7320 746f 2062 6520 6578 6163 746c 7920  s to be exactly 
+00001e60: 7468 6520 7361 6d65 2061 7320 7468 6520  the same as the 
+00001e70: 6e75 6d62 6572 206f 6620 7265 6772 6573  number of regres
+00001e80: 7369 6f6e 5f6c 696d 6974 7320 696e 7465  sion_limits inte
+00001e90: 7276 616c 7320 2863 7572 7265 6e74 6c79  rvals (currently
+00001ea0: 2029 49da 026b 73da 066d 6f64 656c 73da   )I..ks..models.
+00001eb0: 054d 6f64 656c da08 5f5f 696e 6974 5f5f  .Model..__init__
+00001ec0: 721a 0000 0072 1b00 0000 721c 0000 0072  r....r....r....r
+00001ed0: 1d00 0000 721e 0000 0072 1f00 0000 7220  ....r....r....r 
+00001ee0: 0000 0072 2100 0000 7222 0000 0072 2300  ...r!...r"...r#.
+00001ef0: 0000 7224 0000 0072 2500 0000 7226 0000  ..r$...r%...r&..
+00001f00: 0072 2700 0000 7229 0000 0072 2a00 0000  .r'...r)...r*...
+00001f10: 722b 0000 0072 2c00 0000 722d 0000 0072  r+...r,...r-...r
+00001f20: 2f00 0000 722e 0000 0072 3000 0000 7228  /...r....r0...r(
+00001f30: 0000 0072 3100 0000 da10 6174 7465 6e74  ...r1.....attent
+00001f40: 696f 6e5f 6c61 7965 7273 720e 0000 00da  ion_layersr.....
+00001f50: 0661 7070 656e 6472 0900 0000 da0b 6c61  .appendr......la
+00001f60: 795f 6472 6f70 6f75 7472 0d00 0000 da0c  y_dropoutr......
+00001f70: 6c61 795f 7370 6172 7369 7479 7208 0000  lay_sparsityr...
+00001f80: 00da 126c 6179 5f61 6374 5f69 6d70 6f72  ...lay_act_impor
+00001f90: 7461 6e63 6572 0500 0000 da11 6c61 795f  tancer......lay_
+00001fa0: 636f 6e63 6174 5f61 6c70 6861 7372 0a00  concat_alphasr..
+00001fb0: 0000 da11 6c61 795f 706f 6f6c 5f65 6467  ....lay_pool_edg
+00001fc0: 6573 5f69 6eda 126c 6179 5f70 6f6f 6c5f  es_in..lay_pool_
+00001fd0: 6564 6765 735f 6f75 7472 0600 0000 da0b  edges_outr......
+00001fe0: 6c61 795f 6176 6572 6167 65da 156e 6f64  lay_average..nod
+00001ff0: 655f 696d 706f 7274 616e 6365 5f75 6e69  e_importance_uni
+00002000: 7473 da14 6e6f 6465 5f69 6d70 6f72 7461  ts..node_importa
+00002010: 6e63 655f 6163 7473 da16 6e6f 6465 5f69  nce_acts..node_i
+00002020: 6d70 6f72 7461 6e63 655f 6c61 7965 7273  mportance_layers
+00002030: da03 7a69 7072 0700 0000 720b 0000 00da  ..zipr....r.....
+00002040: 0c6c 6179 5f70 6f6f 6c5f 6f75 74da 0e6c  .lay_pool_out..l
+00002050: 6179 5f63 6f6e 6361 745f 6f75 74da 116c  ay_concat_out..l
+00002060: 6179 5f66 696e 616c 5f64 726f 706f 7574  ay_final_dropout
+00002070: da0a 6669 6e61 6c5f 6163 7473 da0c 6669  ..final_acts..fi
+00002080: 6e61 6c5f 6269 6173 6573 da0c 6669 6e61  nal_biases..fina
+00002090: 6c5f 6c61 7965 7273 da06 6c6f 7373 6573  l_layers..losses
+000020a0: da12 4269 6e61 7279 4372 6f73 7365 6e74  ..BinaryCrossent
+000020b0: 726f 7079 da08 6263 655f 6c6f 7373 7202  ropy..bce_lossr.
+000020c0: 0000 00da 0f4c 6f73 7365 7343 6f6e 7461  .....LossesConta
+000020d0: 696e 6572 7210 0000 00da 1c63 6f6d 7069  inerr......compi
+000020e0: 6c65 645f 636c 6173 7369 6669 6361 7469  led_classificati
+000020f0: 6f6e 5f6c 6f73 73da 104d 6561 6e53 7175  on_loss..MeanSqu
+00002100: 6172 6564 4572 726f 72da 086d 7365 5f6c  aredError..mse_l
+00002110: 6f73 73da 114d 6561 6e41 6273 6f6c 7574  oss..MeanAbsolut
+00002120: 6545 7272 6f72 da08 6d61 655f 6c6f 7373  eError..mae_loss
+00002130: 720f 0000 00da 1863 6f6d 7069 6c65 645f  r......compiled_
+00002140: 7265 6772 6573 7369 6f6e 5f6c 6f73 73da  regression_loss.
+00002150: 0a69 7369 6e73 7461 6e63 65da 0369 6e74  .isinstance..int
+00002160: da05 666c 6f61 74da 036c 656e 2920 da04  ..float..len) ..
+00002170: 7365 6c66 721a 0000 0072 1b00 0000 721c  selfr....r....r.
+00002180: 0000 0072 1d00 0000 721e 0000 0072 1f00  ...r....r....r..
+00002190: 0000 7220 0000 0072 2100 0000 7222 0000  ..r ...r!...r"..
+000021a0: 0072 2300 0000 7224 0000 0072 2500 0000  .r#...r$...r%...
+000021b0: 7226 0000 0072 2700 0000 7228 0000 0072  r&...r'...r(...r
+000021c0: 2900 0000 722a 0000 0072 2b00 0000 722c  )...r*...r+...r,
+000021d0: 0000 0072 2d00 0000 722e 0000 0072 2f00  ...r-...r....r/.
+000021e0: 0000 7230 0000 0072 3100 0000 da06 6b77  ..r0...r1.....kw
+000021f0: 6172 6773 da01 75da 036c 6179 da03 6163  args..u..lay..ac
+00002200: 74da 0462 6961 73da 0e6e 756d 5f72 6566  t..bias..num_ref
+00002210: 6572 656e 6365 73da 0a6e 756d 5f6c 696d  erences..num_lim
+00002220: 6974 7372 3e00 0000 723e 0000 0072 4200  itsr>...r>...rB.
+00002230: 0000 724a 0000 001e 0000 0073 c200 0000  ..rJ.......s....
+00002240: 164a 0601 0601 0601 0601 0601 0601 0601  .J..............
+00002250: 0601 0601 0601 0601 0601 0601 0601 0601  ................
+00002260: 0601 0601 0601 0601 0601 0601 0601 0601  ................
+00002270: 0601 0603 0a01 0201 0201 0401 0401 0401  ................
+00002280: 0401 0201 0401 06f9 0e09 0e02 0e01 0e03  ................
+00002290: 0c01 0e02 0e01 0801 0e03 1601 0601 1601  ................
+000022a0: 0201 0201 0201 0201 06fd 0e05 0e03 0c01  ................
+000022b0: 0e01 1202 0c01 1201 0a01 0601 1c01 0201  ................
+000022c0: 0201 0201 0201 06fd 1005 0c03 0c01 0c02  ................
+000022d0: 0c01 0c01 0c06 1202 1009 0801 0a02 0a01  ................
+000022e0: 1001 0801 0201 06ff 04ff 1004 0801 0601  ................
+000022f0: 06ff 04ff 0c04 0801 0201 06ff 04ff 04e8  ................
+00002300: 0418 7a0e 4d65 6761 6e2e 5f5f 696e 6974  ..z.Megan.__init
+00002310: 5f5f 6301 0000 0000 0000 0000 0000 0002  __c.............
+00002320: 0000 0007 0000 0003 0000 0073 b600 0000  ...........s....
+00002330: 7400 7401 7c00 8302 a002 a100 7d01 7c01  t.t.|.......}.|.
+00002340: a003 6900 6401 7c00 6a04 9301 6402 7c00  ..i.d.|.j...d.|.
+00002350: 6a05 9301 6403 7c00 6a06 9301 6404 7c00  j...d.|.j...d.|.
+00002360: 6a07 9301 6405 7c00 6a08 9301 6406 7c00  j...d.|.j...d.|.
+00002370: 6a09 9301 6407 7c00 6a0a 9301 6408 7c00  j...d.|.j...d.|.
+00002380: 6a0b 9301 6409 7c00 6a0c 9301 640a 7c00  j...d.|.j...d.|.
+00002390: 6a0d 9301 640b 7c00 6a0e 9301 640c 7c00  j...d.|.j...d.|.
+000023a0: 6a0f 9301 640d 7c00 6a10 9301 640e 7c00  j...d.|.j...d.|.
+000023b0: 6a11 9301 640f 7c00 6a12 9301 6410 7c00  j...d.|.j...d.|.
+000023c0: 6a13 9301 6411 7c00 6a14 9301 7c00 6a15  j...d.|.j...|.j.
+000023d0: 7c00 6a16 7c00 6a17 6412 9c03 a501 a101  |.j.|.j.d.......
+000023e0: 0100 7c01 5300 2913 4e72 1a00 0000 721b  ..|.S.).Nr....r.
+000023f0: 0000 0072 1c00 0000 721d 0000 0072 1e00  ...r....r....r..
+00002400: 0000 721f 0000 0072 2000 0000 7221 0000  ..r....r ...r!..
+00002410: 0072 2200 0000 7223 0000 0072 2400 0000  .r"...r#...r$...
+00002420: 7226 0000 0072 2700 0000 7229 0000 0072  r&...r'...r)...r
+00002430: 2a00 0000 722b 0000 0072 2c00 0000 2903  *...r+...r,...).
+00002440: 722d 0000 0072 2f00 0000 7230 0000 0029  r-...r/...r0...)
+00002450: 18da 0573 7570 6572 7212 0000 00da 0a67  ...superr......g
+00002460: 6574 5f63 6f6e 6669 67da 0675 7064 6174  et_config..updat
+00002470: 6572 1a00 0000 721b 0000 0072 1c00 0000  er....r....r....
+00002480: 721d 0000 0072 1e00 0000 721f 0000 0072  r....r....r....r
+00002490: 2000 0000 7221 0000 0072 2200 0000 7223   ...r!...r"...r#
+000024a0: 0000 0072 2400 0000 7226 0000 0072 2700  ...r$...r&...r'.
+000024b0: 0000 7229 0000 0072 2a00 0000 722b 0000  ..r)...r*...r+..
+000024c0: 0072 2c00 0000 722d 0000 0072 2f00 0000  .r,...r-...r/...
+000024d0: 7230 0000 0029 0272 6c00 0000 da06 636f  r0...).rl.....co
+000024e0: 6e66 6967 a901 da09 5f5f 636c 6173 735f  nfig....__class_
+000024f0: 5f72 3e00 0000 7242 0000 0072 7500 0000  _r>...rB...ru...
+00002500: e200 0000 7352 0000 000e 0106 0106 0102  ....sR..........
+00002510: ff06 0202 fe06 0302 fd06 0402 fc06 0502  ................
+00002520: fb06 0602 fa06 0702 f906 0802 f806 0902  ................
+00002530: f706 0a02 f606 0b02 f506 0c02 f406 0d02  ................
+00002540: f306 0e02 f206 0f02 f106 1002 f006 1102  ................
+00002550: ef04 1204 0104 010a ec04 177a 104d 6567  ...........z.Meg
+00002560: 616e 2e67 6574 5f63 6f6e 6669 67da 0672  an.get_config..r
+00002570: 6574 7572 6e63 0100 0000 0000 0000 0000  eturnc..........
+00002580: 0000 0100 0000 0200 0000 4300 0000 730a  ..........C...s.
+00002590: 0000 007c 006a 0064 0075 0153 0029 014e  ...|.j.d.u.S.).N
+000025a0: 2901 722d 0000 0029 0172 6c00 0000 723e  ).r-...).rl...r>
+000025b0: 0000 0072 3e00 0000 7242 0000 00da 1064  ...r>...rB.....d
+000025c0: 6f69 6e67 5f72 6567 7265 7373 696f 6efc  oing_regression.
+000025d0: 0000 0073 0200 0000 0a02 7a16 4d65 6761  ...s......z.Mega
+000025e0: 6e2e 646f 696e 675f 7265 6772 6573 7369  n.doing_regressi
+000025f0: 6f6e da08 7472 6169 6e69 6e67 da15 6e6f  on..training..no
+00002600: 6465 5f69 6d70 6f72 7461 6e63 6573 5f6d  de_importances_m
+00002610: 6173 6b63 0500 0000 0000 0000 0000 0000  askc............
+00002620: 1e00 0000 0600 0000 4b00 0000 7328 0200  ........K...s(..
+00002630: 007c 006a 0072 0a7c 015c 047d 067d 077d  .|.j.r.|.\.}.}.}
+00002640: 087d 096e 077c 015c 037d 067d 077d 0864  .}.n.|.\.}.}.}.d
+00002650: 017d 0967 007d 0a7c 067d 0b7c 006a 0144  .}.g.}.|.}.|.j.D
+00002660: 005d 197d 0c7c 0c7c 0b7c 077c 0867 0383  .].}.|.|.|.|.g..
+00002670: 015c 027d 0b7d 0d7c 0272 2c7c 006a 027c  .\.}.}.|.r,|.j.|
+00002680: 0b7c 0264 028d 027d 0b7c 0aa0 037c 0da1  .|.d...}.|...|..
+00002690: 0101 0071 187c 00a0 047c 0aa1 017d 0a74  ...q.|...|...}.t
+000026a0: 056a 067c 0a64 0364 0464 058d 037d 0e7c  .j.|.d.d.d...}.|
+000026b0: 00a0 077c 0ea1 017d 0e7c 00a0 087c 067c  ...|...}.|...|.|
+000026c0: 0e7c 0867 03a1 017d 0f7c 00a0 097c 067c  .|.g...}.|...|.|
+000026d0: 0e7c 0867 03a1 017d 107c 00a0 0a7c 107c  .|.g...}.|...|.|
+000026e0: 0f67 02a1 017d 117c 0b7d 127c 006a 0b44  .g...}.|.}.|.j.D
+000026f0: 005d 067d 0c7c 0c7c 1283 017d 1271 607c  .].}.|.|...}.q`|
+00002700: 00a0 077c 12a1 017d 127c 127c 1114 007d  ...|...}.|.|...}
+00002710: 137c 00a0 0c7c 13a1 0101 007c 0464 0175  .|...|.....|.d.u
+00002720: 0172 8474 05a0 0d7c 0474 056a 0ea1 027d  .r.t...|.t.j...}
+00002730: 047c 137c 0414 007d 1367 007d 147c 006a  .|.|...}.g.}.|.j
+00002740: 0f64 0319 007d 1574 107c 006a 1183 0144  .d...}.t.|.j...D
+00002750: 005d 2e7d 1674 056a 127c 1364 0164 0185  .].}.t.j.|.d.d..
+00002760: 0264 0164 0185 027c 1666 0319 0064 0364  .d.d...|.f...d.d
+00002770: 068d 027d 177c 0b7c 1714 007d 187c 006a  ...}.|.|...}.|.j
+00002780: 1364 0175 0172 b47c 006a 137c 1619 007d  .d.u.r.|.j.|...}
+00002790: 197c 197c 1883 017d 187c 00a0 147c 18a1  .|.|...}.|...|..
+000027a0: 017d 1a7c 14a0 037c 1aa1 0101 0071 907c  .}.|...|.....q.|
+000027b0: 00a0 157c 14a1 017d 1a7c 006a 0072 ce7c  ...|...}.|.j.r.|
+000027c0: 00a0 157c 1a7c 0967 02a1 017d 1a74 167c  ...|.|.g...}.t.|
+000027d0: 006a 1783 017d 1b74 187c 006a 1783 0144  .j...}.t.|.j...D
+000027e0: 005d 175c 027d 1c7d 0c7c 0c7c 1a83 017d  .].\.}.}.|.|...}
+000027f0: 1a7c 0272 ef7c 1c7c 1b64 0718 006b 0072  .|.r.|.|.d...k.r
+00002800: ef7c 006a 197c 1a7c 0264 028d 027d 1a71  .|.j.|.|.d...}.q
+00002810: d87c 006a 1a90 0172 0674 05a0 1b7c 1aa1  .|.j...r.t...|..
+00002820: 0174 056a 1c7c 006a 1d74 056a 0e64 088d  .t.j.|.j.t.j.d..
+00002830: 0214 007d 1d7c 1a7c 1d17 007d 1a7c 006a  ...}.|.|...}.|.j
+00002840: 1e90 0173 0d7c 0390 0172 127c 1a7c 137c  ...s.|...r.|.|.|
+00002850: 0e66 0353 007c 1a53 0029 0961 b701 0000  .f.S.|.S.).a....
+00002860: 0a20 2020 2020 2020 2046 6f72 7761 7264  .        Forward
+00002870: 2070 6173 7320 6f66 2074 6865 206d 6f64   pass of the mod
+00002880: 656c 2e0a 0a20 2020 2020 2020 202a 2a53  el...        **S
+00002890: 6861 7065 2045 7870 6c61 6e61 7469 6f6e  hape Explanation
+000028a0: 733a 2a2a 2041 6c6c 2073 6861 7065 7320  s:** All shapes 
+000028b0: 696e 2062 7261 636b 6574 7320 5b5d 2061  in brackets [] a
+000028c0: 7265 2072 6167 6765 6420 6469 6d65 6e73  re ragged dimens
+000028d0: 696f 6e73 210a 0a20 2020 2020 2020 202d  ions!..        -
+000028e0: 2056 3a20 4e75 6d20 6e6f 6465 7320 696e   V: Num nodes in
+000028f0: 2074 6865 2067 7261 7068 0a20 2020 2020   the graph.     
+00002900: 2020 202d 2045 3a20 4e75 6d20 6564 6765     - E: Num edge
+00002910: 7320 696e 2074 6865 2067 7261 7068 0a20  s in the graph. 
+00002920: 2020 2020 2020 202d 204e 3a20 4e75 6d20         - N: Num 
+00002930: 6665 6174 7572 6520 7661 6c75 6573 2070  feature values p
+00002940: 6572 206e 6f64 650a 2020 2020 2020 2020  er node.        
+00002950: 2d20 4d3a 204e 556d 2066 6561 7475 7265  - M: NUm feature
+00002960: 2076 616c 7565 7320 7065 7220 6564 6765   values per edge
+00002970: 0a20 2020 2020 2020 202d 2048 3a20 4e75  .        - H: Nu
+00002980: 6d20 6665 6174 7572 6520 7661 6c75 6573  m feature values
+00002990: 2070 6572 2067 7261 7068 0a20 2020 2020   per graph.     
+000029a0: 2020 202d 2042 3a20 4e75 6d20 6772 6170     - B: Num grap
+000029b0: 6873 2069 6e20 6120 6261 7463 680a 2020  hs in a batch.  
+000029c0: 2020 2020 2020 2d20 4b3a 204e 756d 2069        - K: Num i
+000029d0: 6d70 6f72 7461 6e63 6520 2865 7870 6c61  mportance (expla
+000029e0: 6e61 7469 6f6e 2920 6368 616e 6e65 6c73  nation) channels
+000029f0: 2063 6f6e 6669 6775 7265 6420 696e 2074   configured in t
+00002a00: 6865 2063 6f6e 7374 7275 6374 6f72 0a20  he constructor. 
+00002a10: 2020 2020 2020 204e 2901 727c 0000 0072         N).r|...r
+00002a20: 3600 0000 4629 0272 3800 0000 da08 6b65  6...F).r8.....ke
+00002a30: 6570 6469 6d73 7237 0000 0072 1500 0000  epdimsr7...r....
+00002a40: 2901 da05 6474 7970 6529 1f72 3100 0000  )...dtype).r1...
+00002a50: 724b 0000 0072 4d00 0000 724c 0000 0072  rK...rM...rL...r
+00002a60: 5000 0000 da02 7466 da0a 7265 6475 6365  P.....tf..reduce
+00002a70: 5f73 756d 724f 0000 0072 5100 0000 7252  _sumrO...rQ...rR
+00002a80: 0000 0072 5300 0000 7256 0000 0072 4e00  ...rS...rV...rN.
+00002a90: 0000 da04 6361 7374 da07 666c 6f61 7433  ....cast..float3
+00002aa0: 3272 2900 0000 da05 7261 6e67 6572 2000  2r).....ranger .
+00002ab0: 0000 da0b 6578 7061 6e64 5f64 696d 7372  ....expand_dimsr
+00002ac0: 2500 0000 7258 0000 0072 5900 0000 726b  %...rX...rY...rk
+00002ad0: 0000 0072 5d00 0000 da09 656e 756d 6572  ...r].....enumer
+00002ae0: 6174 6572 5a00 0000 727b 0000 00da 096f  aterZ...r{.....o
+00002af0: 6e65 735f 6c69 6b65 da08 636f 6e73 7461  nes_like..consta
+00002b00: 6e74 722f 0000 0072 3000 0000 291e 726c  ntr/...r0...).rl
+00002b10: 0000 00da 0669 6e70 7574 7372 7c00 0000  .....inputsr|...
+00002b20: 7230 0000 0072 7d00 0000 726d 0000 00da  r0...r}...rm....
+00002b30: 0a6e 6f64 655f 696e 7075 74da 0a65 6467  .node_input..edg
+00002b40: 655f 696e 7075 74da 1065 6467 655f 696e  e_input..edge_in
+00002b50: 6465 785f 696e 7075 74da 0b67 7261 7068  dex_input..graph
+00002b60: 5f69 6e70 7574 da06 616c 7068 6173 da01  _input..alphas..
+00002b70: 7872 6f00 0000 da05 616c 7068 61da 1065  xro.....alpha..e
+00002b80: 6467 655f 696d 706f 7274 616e 6365 73da  dge_importances.
+00002b90: 0f70 6f6f 6c65 645f 6564 6765 735f 696e  .pooled_edges_in
+00002ba0: da10 706f 6f6c 6564 5f65 6467 6573 5f6f  ..pooled_edges_o
+00002bb0: 7574 da0c 706f 6f6c 6564 5f65 6467 6573  ut..pooled_edges
+00002bc0: da16 6e6f 6465 5f69 6d70 6f72 7461 6e63  ..node_importanc
+00002bd0: 6573 5f74 696c 6465 da10 6e6f 6465 5f69  es_tilde..node_i
+00002be0: 6d70 6f72 7461 6e63 6573 da04 6f75 7473  mportances..outs
+00002bf0: da01 6eda 016b da15 6e6f 6465 5f69 6d70  ..n..k..node_imp
+00002c00: 6f72 7461 6e63 655f 736c 6963 65da 116d  ortance_slice..m
+00002c10: 6173 6b65 645f 656d 6265 6464 696e 6773  asked_embeddings
+00002c20: da0d 6c61 795f 7472 616e 7366 6f72 6dda  ..lay_transform.
+00002c30: 036f 7574 da10 6e75 6d5f 6669 6e61 6c5f  .out..num_final_
+00002c40: 6c61 7965 7273 da01 63da 0972 6566 6572  layers..c..refer
+00002c50: 656e 6365 723e 0000 0072 3e00 0000 7242  encer>...r>...rB
+00002c60: 0000 00da 0463 616c 6c00 0100 0073 6600  .....call....sf.
+00002c70: 0000 061f 0e01 0a02 0401 0405 0401 0a01  ................
+00002c80: 1203 0401 0e01 0c02 0a04 1001 0a01 1006  ................
+00002c90: 1001 0e01 0402 0a01 0a01 0a02 0802 0a01  ................
+00002ca0: 0809 0e01 0801 0405 0a01 0e01 2001 0801  ............ ...
+00002cb0: 0a05 0a01 0801 0a02 0c03 0a03 0604 0e01  ................
+00002cc0: 0a04 1201 0801 1001 0e01 0280 0802 1c01  ................
+00002cd0: 0801 0e05 0a01 0402 7a0a 4d65 6761 6e2e  ........z.Megan.
+00002ce0: 6361 6c6c 6302 0000 0000 0000 0000 0000  callc...........
+00002cf0: 000c 0000 0006 0000 0043 0000 0073 ce00  .........C...s..
+00002d00: 0000 6700 7d02 6700 7d03 7400 7401 7c00  ..g.}.g.}.t.t.|.
+00002d10: 6a02 7c00 6a03 8302 8301 4400 5d4b 5c02  j.|.j.....D.]K\.
+00002d20: 7d04 5c02 7d05 7d06 7404 7c06 6401 1900  }.\.}.}.t.|.d...
+00002d30: 7c06 6402 1900 1800 8301 7d07 7405 6a06  |.d.......}.t.j.
+00002d40: 7c01 6400 6400 8502 7c04 6602 1900 6403  |.d.d...|.f...d.
+00002d50: 6404 8d02 7d08 7405 a004 7c08 7c05 1800  d...}.t...|.|...
+00002d60: a101 7d09 7c09 7c00 6a07 1400 6405 7c07  ..}.|.|.j...d.|.
+00002d70: 1400 1b00 7d09 7405 a008 7c08 7c05 6b00  ....}.t...|.|.k.
+00002d80: 6406 6407 a103 7d0a 7405 a008 7c08 7c05  d.d...}.t...|.|.
+00002d90: 6b04 6406 6407 a103 7d0b 7c02 7c09 7c09  k.d.d...}.|.|.|.
+00002da0: 6702 3700 7d02 7c03 7c0a 7c0b 6702 3700  g.7.}.|.|.|.g.7.
+00002db0: 7d03 710d 7405 6a09 7c02 6403 6404 8d02  }.q.t.j.|.d.d...
+00002dc0: 7405 6a09 7c03 6403 6404 8d02 6602 5300  t.j.|.d.d...f.S.
+00002dd0: 2908 4e72 1700 0000 7201 0000 0072 3600  ).Nr....r....r6.
+00002de0: 0000 7237 0000 0067 0000 0000 0000 e03f  ..r7...g.......?
+00002df0: 6700 0000 0000 00f0 3f72 1400 0000 290a  g.......?r....).
+00002e00: 7286 0000 0072 5700 0000 722f 0000 0072  r....rW...r/...r
+00002e10: 2d00 0000 da03 6162 7372 8000 0000 7285  -.....absr....r.
+00002e20: 0000 0072 2400 0000 da05 7768 6572 65da  ...r$.....where.
+00002e30: 0663 6f6e 6361 7429 0c72 6c00 0000 da08  .concat).rl.....
+00002e40: 6f75 745f 7472 7565 da07 7361 6d70 6c65  out_true..sample
+00002e50: 73da 056d 6173 6b73 da01 6972 2f00 0000  s..masks..ir/...
+00002e60: 722d 0000 00da 1072 6567 7265 7373 696f  r-.....regressio
+00002e70: 6e5f 7769 6474 68da 0676 616c 7565 73da  n_width..values.
+00002e80: 1063 656e 7465 725f 6469 7374 616e 6365  .center_distance
+00002e90: 73da 076c 6f5f 6d61 736b da07 6869 5f6d  s..lo_mask..hi_m
+00002ea0: 6173 6b72 3e00 0000 723e 0000 0072 4200  askr>...r>...rB.
+00002eb0: 0000 da17 7265 6772 6573 7369 6f6e 5f61  ....regression_a
+00002ec0: 7567 6d65 6e74 6174 696f 6e86 0100 0073  ugmentation....s
+00002ed0: 2000 0000 0402 0401 0801 0401 12ff 1403   ...............
+00002ee0: 1a01 0e01 1201 1208 1202 0c02 0e01 0c03  ................
+00002ef0: 0c01 04fe 7a1d 4d65 6761 6e2e 7265 6772  ....z.Megan.regr
+00002f00: 6573 7369 6f6e 5f61 7567 6d65 6e74 6174  ession_augmentat
+00002f10: 696f 6eda 0e75 7064 6174 655f 7765 6967  ion..update_weig
+00002f20: 6874 7363 0400 0000 0000 0000 0000 0000  htsc............
+00002f30: 1300 0000 0800 0000 4300 0000 733a 0100  ........C...s:..
+00002f40: 007c 006a 0072 097c 025c 037d 047d 057d  .|.j.r.|.\.}.}.}
+00002f50: 056e 027c 027d 0464 017d 0674 01a0 02a1  .n.|.}.d.}.t....
+00002f60: 008f 6c7d 077c 007c 0164 0264 0264 038d  ..l}.|.|.d.d.d..
+00002f70: 037d 087c 085c 037d 097d 0a7d 0b67 007d  .}.|.\.}.}.}.g.}
+00002f80: 0c74 037c 006a 0483 0144 005d 1c7d 0d74  .t.|.j...D.].}.t
+00002f90: 016a 057c 0a64 0064 0085 0264 0064 0085  .j.|.d.d...d.d..
+00002fa0: 027c 0d66 0319 0064 0464 058d 027d 0e7c  .|.f...d.d...}.|
+00002fb0: 00a0 067c 0ea1 017d 0f7c 0ca0 077c 0fa1  ...|...}.|...|..
+00002fc0: 0101 0071 257c 00a0 087c 0ca1 017d 0c7c  ...q%|...|...}.|
+00002fd0: 006a 0972 617c 00a0 0a7c 04a1 015c 027d  .j.ra|...|...\.}
+00002fe0: 047d 107c 0c7d 097c 006a 047c 00a0 0b7c  .}.|.}.|.j.|...|
+00002ff0: 047c 1014 007c 097c 1014 00a1 0214 007d  .|...|.|.......}
+00003000: 066e 1074 0c7c 0c7c 006a 0d64 0664 078d  .n.t.|.|.j.d.d..
+00003010: 037d 097c 00a0 0e7c 047c 097c 0414 00a1  .}.|...|.|.|....
+00003020: 027d 067c 067c 006a 0f39 007d 0657 0064  .}.|.|.j.9.}.W.d
+00003030: 0004 0004 0083 0301 006e 0831 0073 8077  .........n.1.s.w
+00003040: 0101 0001 0001 0059 0001 007c 006a 107d  .......Y...|.j.}
+00003050: 117c 07a0 117c 067c 11a1 027d 127c 0372  .|...|.|...}.|.r
+00003060: 997c 006a 12a0 1374 147c 127c 1183 02a1  .|.j...t.|.|....
+00003070: 0101 0064 087c 0669 0153 0029 094e 7201  ...d.|.i.S.).Nr.
+00003080: 0000 0054 a902 727c 0000 0072 3000 0000  ...T..r|...r0...
+00003090: 7236 0000 0072 3700 0000 7215 0000 00a9  r6...r7...r.....
+000030a0: 02da 0573 6869 6674 da0a 6d75 6c74 6970  ...shift..multip
+000030b0: 6c69 6572 da08 6578 705f 6c6f 7373 2915  lier..exp_loss).
+000030c0: 7230 0000 0072 8000 0000 da0c 4772 6164  r0...r......Grad
+000030d0: 6965 6e74 5461 7065 7284 0000 0072 2000  ientTaper....r .
+000030e0: 0000 7285 0000 0072 5800 0000 724c 0000  ..r....rX...rL..
+000030f0: 0072 5900 0000 727b 0000 0072 ae00 0000  .rY...r{...r....
+00003100: 7267 0000 0072 1100 0000 7224 0000 0072  rg...r....r$...r
+00003110: 6200 0000 7223 0000 00da 1374 7261 696e  b...r#.....train
+00003120: 6162 6c65 5f76 6172 6961 626c 6573 da08  able_variables..
+00003130: 6772 6164 6965 6e74 da09 6f70 7469 6d69  gradient..optimi
+00003140: 7a65 72da 0f61 7070 6c79 5f67 7261 6469  zer..apply_gradi
+00003150: 656e 7473 7257 0000 0029 1372 6c00 0000  entsrW...).rl...
+00003160: 728f 0000 00da 0179 72af 0000 0072 a500  r......yr....r..
+00003170: 0000 7241 0000 0072 b400 0000 da04 7461  ..rA...r......ta
+00003180: 7065 da06 795f 7072 6564 da08 6f75 745f  pe..y_pred..out_
+00003190: 7072 6564 da07 6e69 5f70 7265 64da 0765  pred..ni_pred..e
+000031a0: 695f 7072 6564 7297 0000 0072 9900 0000  i_predr....r....
+000031b0: da16 6e6f 6465 5f69 6d70 6f72 7461 6e63  ..node_importanc
+000031c0: 6573 5f73 6c69 6365 729d 0000 00da 046d  es_slicer......m
+000031d0: 6173 6bda 0e74 7261 696e 6162 6c65 5f76  ask..trainable_v
+000031e0: 6172 73da 0d65 7870 5f67 7261 6469 656e  ars..exp_gradien
+000031f0: 7473 723e 0000 0072 3e00 0000 7242 0000  tsr>...r>...rB..
+00003200: 00da 1674 7261 696e 5f73 7465 705f 6578  ...train_step_ex
+00003210: 706c 616e 6174 696f 6ea4 0100 0073 3800  planation....s8.
+00003220: 0000 0603 0c01 0402 0402 0a01 0e02 0a01  ................
+00003230: 0407 0e01 2001 0a01 0c02 0a03 0602 0e01  .... ...........
+00003240: 0401 0e01 0601 08ff 1005 1001 0c02 1ce1  ................
+00003250: 0622 0c01 0403 1201 0802 7a1c 4d65 6761  ."........z.Mega
+00003260: 6e2e 7472 6169 6e5f 7374 6570 5f65 7870  n.train_step_exp
+00003270: 6c61 6e61 7469 6f6e 6302 0000 0000 0000  lanationc.......
+00003280: 0000 0000 0018 0000 0008 0000 0043 0000  .............C..
+00003290: 0073 d801 0000 7400 7c01 8301 6401 6b02  .s....t.|...d.k.
+000032a0: 720c 7c01 5c03 7d02 7d03 7d04 6e06 6400  r.|.\.}.}.}.n.d.
+000032b0: 7d04 7c01 5c02 7d02 7d03 7c00 6a01 6402  }.|.\.}.}.|.j.d.
+000032c0: 6b03 7221 7c00 6a02 7221 7c00 a003 7c02  k.r!|.j.r!|...|.
+000032d0: 7c03 a102 7d05 6e02 6900 7d05 6402 7d06  |...}.n.i.}.d.}.
+000032e0: 7404 a005 a100 8f8c 7d07 7c03 5c03 7d08  t.......}.|.\.}.
+000032f0: 7d09 7d0a 7c00 7c02 6403 6403 6404 8d03  }.}.|.|.d.d.d...
+00003300: 5c03 7d0b 7d0c 7d0d 7c00 6a06 7c08 7c09  \.}.}.}.|.j.|.|.
+00003310: 7c0a 6703 7c0b 7c0c 7c0d 6703 7c04 7c00  |.g.|.|.|.g.|.|.
+00003320: 6a07 6405 8d04 7d0e 7c00 6a01 6402 6b03  j.d...}.|.j.d.k.
+00003330: 72ae 7c00 6a02 73ae 6700 7d0f 7408 7c00  r.|.j.s.g.}.t.|.
+00003340: 6a09 8301 4400 5d1c 7d10 7404 6a0a 7c0c  j...D.].}.t.j.|.
+00003350: 6400 6400 8502 6400 6400 8502 7c10 6603  d.d...d.d...|.f.
+00003360: 1900 6406 6407 8d02 7d11 7c00 a00b 7c11  ..d.d...}.|...|.
+00003370: a101 7d12 7c0f a00c 7c12 a101 0100 7158  ..}.|...|.....qX
+00003380: 7c00 a00d 7c0f a101 7d0f 7c00 6a0e 7291  |...|...}.|.j.r.
+00003390: 7c00 a00f 7c08 a101 5c02 7d13 7d14 7c0f  |...|...\.}.}.|.
+000033a0: 7d15 7c00 a010 7c13 7c14 1400 7c15 7c14  }.|...|.|...|.|.
+000033b0: 1400 a102 7d06 6e10 7411 7c0f 7c00 6a12  ....}.n.t.|.|.j.
+000033c0: 6408 6409 8d03 7c08 1400 7d15 7c00 a013  d.d...|...}.|...
+000033d0: 7c08 7c15 a102 7d06 7c06 7c00 6a01 3900  |.|...}.|.|.j.9.
+000033e0: 7d06 7c06 7c05 640a 3c00 7c0e 7c06 3700  }.|.|.d.<.|.|.7.
+000033f0: 7d0e 5700 6400 0400 0400 8303 0100 6e08  }.W.d.........n.
+00003400: 3100 73b8 7701 0100 0100 0100 5900 0100  1.s.w.......Y...
+00003410: 7c00 6a14 7d16 7c07 a015 7c0e 7c16 a102  |.j.}.|...|.|...
+00003420: 7d17 7c00 6a16 a017 7418 7c17 7c16 8302  }.|.j...t.|.|...
+00003430: a101 0100 7c00 6a19 6a1a 7c03 7c00 6a1b  ....|.j.j.|.|.j.
+00003440: 73d8 7c0b 6e04 7c0b 7c0c 7c0d 6703 7c04  s.|.n.|.|.|.g.|.
+00003450: 640b 8d03 0100 6900 640c 640d 8400 7c00  d.....i.d.d...|.
+00003460: 6a1c 4400 8301 a501 7c05 a501 5300 290e  j.D.....|...S.).
+00003470: 4ee9 0300 0000 7201 0000 0054 72b0 0000  N.....r....Tr...
+00003480: 0029 02da 0d73 616d 706c 655f 7765 6967  .)...sample_weig
+00003490: 6874 da15 7265 6775 6c61 7269 7a61 7469  ht..regularizati
+000034a0: 6f6e 5f6c 6f73 7365 7372 3600 0000 7237  on_lossesr6...r7
+000034b0: 0000 0072 1700 0000 72b1 0000 0072 b400  ...r....r....r..
+000034c0: 0000 2901 72c6 0000 0063 0100 0000 0000  ..).r....c......
+000034d0: 0000 0000 0000 0200 0000 0500 0000 5300  ..............S.
+000034e0: 0000 7318 0000 0069 007c 005d 087d 017c  ..s....i.|.].}.|
+000034f0: 016a 007c 01a0 01a1 0093 0271 0253 0072  .j.|.......q.S.r
+00003500: 3e00 0000 2902 da04 6e61 6d65 da06 7265  >...)...name..re
+00003510: 7375 6c74 2902 7240 0000 00da 016d 723e  sult).r@.....mr>
+00003520: 0000 0072 3e00 0000 7242 0000 00da 0a3c  ...r>...rB.....<
+00003530: 6469 6374 636f 6d70 3e26 0200 0073 0200  dictcomp>&...s..
+00003540: 0000 1800 7a24 4d65 6761 6e2e 7472 6169  ....z$Megan.trai
+00003550: 6e5f 7374 6570 2e3c 6c6f 6361 6c73 3e2e  n_step.<locals>.
+00003560: 3c64 6963 7463 6f6d 703e 291d 726b 0000  <dictcomp>).rk..
+00003570: 0072 2300 0000 7228 0000 0072 c400 0000  .r#...r(...r....
+00003580: 7280 0000 0072 b500 0000 da0d 636f 6d70  r....r......comp
+00003590: 696c 6564 5f6c 6f73 7372 5e00 0000 7284  iled_lossr^...r.
+000035a0: 0000 0072 2000 0000 7285 0000 0072 5800  ...r ...r....rX.
+000035b0: 0000 724c 0000 0072 5900 0000 727b 0000  ..rL...rY...r{..
+000035c0: 0072 ae00 0000 7267 0000 0072 1100 0000  .r....rg...r....
+000035d0: 7224 0000 0072 6200 0000 72b6 0000 0072  r$...rb...r....r
+000035e0: b700 0000 72b8 0000 0072 b900 0000 7257  ....r....r....rW
+000035f0: 0000 00da 1063 6f6d 7069 6c65 645f 6d65  .....compiled_me
+00003600: 7472 6963 73da 0c75 7064 6174 655f 7374  trics..update_st
+00003610: 6174 6572 3000 0000 da07 6d65 7472 6963  ater0.....metric
+00003620: 7329 1872 6c00 0000 da04 6461 7461 728f  s).rl.....datar.
+00003630: 0000 0072 ba00 0000 72c6 0000 00da 0b65  ...r....r......e
+00003640: 7870 5f6d 6574 7269 6373 72b4 0000 0072  xp_metricsr....r
+00003650: bb00 0000 72a5 0000 00da 076e 695f 7472  ....r......ni_tr
+00003660: 7565 da07 6569 5f74 7275 6572 bd00 0000  ue..ei_truer....
+00003670: 72be 0000 0072 bf00 0000 da04 6c6f 7373  r....r......loss
+00003680: 7297 0000 0072 9900 0000 72c0 0000 0072  r....r....r....r
+00003690: 9d00 0000 da09 5f6f 7574 5f74 7275 6572  ......_out_truer
+000036a0: c100 0000 da09 5f6f 7574 5f70 7265 6472  ......_out_predr
+000036b0: c200 0000 da09 6772 6164 6965 6e74 7372  ......gradientsr
+000036c0: 3e00 0000 723e 0000 0072 4200 0000 da0a  >...r>...rB.....
+000036d0: 7472 6169 6e5f 7374 6570 d801 0000 7370  train_step....sp
+000036e0: 0000 000c 010c 0104 0208 0110 060e 0104  ................
+000036f0: 0204 020a 010a 0214 0104 0108 0108 0102  ................
+00003700: 0104 0106 fc10 0704 060e 0120 010a 010c  ........... ....
+00003710: 020a 0306 020e 0104 010a 0106 0106 ff02  ................
+00003720: 0602 0104 0102 0104 fd02 0404 fc0c 050a  ................
+00003730: 0208 0108 0102 801c d306 2f0c 0112 0206  ........../.....
+00003740: 0202 0112 0102 0106 fd02 080e 0102 ff02  ................
+00003750: 0204 fe7a 104d 6567 616e 2e74 7261 696e  ...z.Megan.train
+00003760: 5f73 7465 7029 0346 464e 7245 0000 0029  _step).FFNrE...)
+00003770: 1ada 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
+00003780: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
+00003790: 616d 655f 5fda 075f 5f64 6f63 5f5f da01  ame__..__doc__..
+000037a0: 74da 044c 6973 7472 6900 0000 da03 7374  t..Listri.....st
+000037b0: 72da 0462 6f6f 6c72 6a00 0000 da08 4f70  r..boolrj.....Op
+000037c0: 7469 6f6e 616c 7247 0000 00da 066c 6179  tionalrG.....lay
+000037d0: 6572 73da 054c 6179 6572 da05 5475 706c  ers..Layer..Tupl
+000037e0: 6572 4a00 0000 7275 0000 00da 0870 726f  erJ...ru.....pro
+000037f0: 7065 7274 7972 7b00 0000 7280 0000 00da  pertyr{...r.....
+00003800: 0c52 6167 6765 6454 656e 736f 7272 a100  .RaggedTensorr..
+00003810: 0000 72ae 0000 0072 c400 0000 72d8 0000  ..r....r....r...
+00003820: 00da 0d5f 5f63 6c61 7373 6365 6c6c 5f5f  ...__classcell__
+00003830: 723e 0000 0072 3e00 0000 7278 0000 0072  r>...r>...rx...r
+00003840: 4200 0000 7212 0000 0014 0000 0073 be00  B...r........s..
+00003850: 0000 0800 0401 020c 0201 0201 0201 0202  ................
+00003860: 0201 0201 0201 0201 0201 0201 0201 0201  ................
+00003870: 0201 0402 0201 0201 0201 0201 0201 0201  ................
+00003880: 0201 0201 04e5 0802 02fe 0203 02fd 0204  ................
+00003890: 02fc 0205 02fb 0206 02fa 0808 02f8 0209  ................
+000038a0: 02f7 020a 02f6 020b 02f5 020c 02f4 020d  ................
+000038b0: 02f3 120e 02f2 020f 02f1 0210 02f0 0211  ................
+000038c0: 02ef 0813 02ed 0214 02ec 0215 02eb 0216  ................
+000038d0: 02ea 1217 02e9 1818 02e8 0819 02e7 021a  ................
+000038e0: 02e6 021b 0ae5 007f 0c45 021a 1001 0205  .........E......
+000038f0: 0201 0201 04fc 0202 02fe 0203 02fd 0a04  ................
+00003900: 0afc 007f 0807 021f 04ff 0201 0aff 1034  ...............4
+00003910: 7212 0000 0029 20da 0674 7970 696e 6772  r....) ..typingr
+00003920: dd00 0000 da0a 7465 6e73 6f72 666c 6f77  ......tensorflow
+00003930: 7280 0000 00da 1074 656e 736f 7266 6c6f  r......tensorflo
+00003940: 772e 6b65 7261 73da 056b 6572 6173 7247  w.keras..kerasrG
+00003950: 0000 00da 1e74 656e 736f 7266 6c6f 772e  .....tensorflow.
+00003960: 7079 7468 6f6e 2e6b 6572 6173 2e65 6e67  python.keras.eng
+00003970: 696e 6572 0200 0000 da10 6b67 636e 6e2e  iner......kgcnn.
+00003980: 6461 7461 2e75 7469 6c73 7203 0000 00da  data.utilsr.....
+00003990: 146b 6763 6e6e 2e6c 6179 6572 732e 6d6f  .kgcnn.layers.mo
+000039a0: 6475 6c65 7372 0400 0000 7205 0000 0072  dulesr....r....r
+000039b0: 0600 0000 7207 0000 0072 0800 0000 7209  ....r....r....r.
+000039c0: 0000 00da 146b 6763 6e6e 2e6c 6179 6572  .....kgcnn.layer
+000039d0: 732e 706f 6f6c 696e 6772 0a00 0000 720b  s.poolingr....r.
+000039e0: 0000 0072 0c00 0000 da1e 6772 6170 685f  ...r......graph_
+000039f0: 6174 7465 6e74 696f 6e5f 7374 7564 656e  attention_studen
+00003a00: 742e 6c61 7965 7273 720d 0000 0072 0e00  t.layersr....r..
+00003a10: 0000 da20 6772 6170 685f 6174 7465 6e74  ... graph_attent
+00003a20: 696f 6e5f 7374 7564 656e 742e 7472 6169  ion_student.trai
+00003a30: 6e69 6e67 720f 0000 0072 1000 0000 7211  ningr....r....r.
+00003a40: 0000 0072 4800 0000 7249 0000 0072 1200  ...rH...rI...r..
+00003a50: 0000 723e 0000 0072 3e00 0000 723e 0000  ..r>...r>...r>..
+00003a60: 0072 4200 0000 da08 3c6d 6f64 756c 653e  .rB.....<module>
+00003a70: 0100 0000 7322 0000 0008 0008 020c 010c  ....s"..........
+00003a80: 010c 010c 0110 0114 010c 010c 010c 010c  ................
+00003a90: 010c 010c 010c 010c 0118 03              ...........
```

### Comparing `graph_attention_student-0.7.0/graph_attention_student/models/gnes.py` & `graph_attention_student-0.7.1/graph_attention_student/models/gnes.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.0/graph_attention_student/models/gnnx.py` & `graph_attention_student-0.7.1/graph_attention_student/models/gnnx.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.0/graph_attention_student/models/gradient.py` & `graph_attention_student-0.7.1/graph_attention_student/models/gradient.py`

 * *Files 2% similar despite different names*

```diff
@@ -204,15 +204,21 @@
         else:
             return y
 
 
 def grad_importances(gradient_info: t.List[t.Tuple[tf.Tensor, tf.Tensor]],
                      use_relu: bool = False,
                      use_absolute: bool = False,
-                     keepdims: bool = False):
+                     use_sigmoid: bool = False,
+                     keepdims: bool = False
+                     ) -> tf.RaggedTensor:
+    """
+
+    """
+
     # shapes as we get them:
     # gradients: ([B], [V], O, F)
     # activation: ([B], [V], F)
 
     activation, gradients = gradient_info[0]
     importances = tf.reduce_sum(
         # We need to expand the activations here in the second last dimension to match the additional
@@ -221,14 +227,16 @@
         axis=-1,
         keepdims=keepdims
     )
     if use_relu:
         importances = ks.backend.relu(importances)
     if use_absolute:
         importances = tf.abs(importances)
+    if use_sigmoid:
+        importances = ks.backend.sigmoid(importances)
 
     return importances
 
 
 def grad_cam_importances(gradient_info: t.List[t.Tuple[tf.Tensor, tf.Tensor]],
                          use_average: bool = False,
                          use_relu: bool = False,
```

### Comparing `graph_attention_student-0.7.0/graph_attention_student/models/megan.py` & `graph_attention_student-0.7.1/graph_attention_student/models/megan.py`

 * *Files 0% similar despite different names*

```diff
@@ -180,15 +180,15 @@
                 activation=act,
                 use_bias=use_bias
             )
             self.final_layers.append(lay)
 
         # ~ EXPLANATION ONLY TRAIN STEP
         self.bce_loss = ks.losses.BinaryCrossentropy()
-        self.compiled_classification_loss = compile_utils.LossesContainer(self.bce_loss)
+        self.compiled_classification_loss = compile_utils.LossesContainer(bce)
 
         self.mse_loss = ks.losses.MeanSquaredError()
         self.mae_loss = ks.losses.MeanAbsoluteError()
         self.compiled_regression_loss = compile_utils.LossesContainer(mae)
 
         # If regression_limits have been supplied, we interprete this as the intent to perform explanation
         # co-training for a regression dataset.
```

### Comparing `graph_attention_student-0.7.0/graph_attention_student/templates/article.tex.j2` & `graph_attention_student-0.7.1/graph_attention_student/templates/article.tex.j2`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.0/graph_attention_student/typing.py` & `graph_attention_student-0.7.1/graph_attention_student/typing.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.0/graph_attention_student/util.py` & `graph_attention_student-0.7.1/graph_attention_student/util.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.0/graph_attention_student/visualization.py` & `graph_attention_student-0.7.1/graph_attention_student/visualization.py`

 * *Files identical despite different names*

### Comparing `graph_attention_student-0.7.0/pyproject.toml` & `graph_attention_student-0.7.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.2.0b2"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "graph_attention_student"
-version = "0.7.0"
+version = "0.7.1"
 description = "MEGAN: Multi Explanation Graph Attention Network"
 license = "MIT"
 authors = ["xxx <jonseb1998@gmail.com>"]
 maintainers = ["xxx <jonseb1998@gmail.com>"]
 readme = "README.rst"
 keywords = ["graph neural network", "attention", "kgcnn"]
 packages = [
```

### Comparing `graph_attention_student-0.7.0/setup.py` & `graph_attention_student-0.7.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 entry_points = \
 {'console_scripts': ['graph_attention_student = '
                      'graph_attention_student.cli:cli']}
 
 setup_kwargs = {
     'name': 'graph-attention-student',
-    'version': '0.7.0',
+    'version': '0.7.1',
     'description': 'MEGAN: Multi Explanation Graph Attention Network',
     'long_description': '|made-with-python| |made-with-kgcnn| |python-version| |os-linux|\n\n.. |os-linux| image:: https://img.shields.io/badge/os-linux-orange.svg\n   :target: https://www.python.org/\n\n.. |python-version| image:: https://img.shields.io/badge/Python-3.8.0-green.svg\n   :target: https://www.python.org/\n\n.. |made-with-kgcnn| image:: https://img.shields.io/badge/Made%20with-KGCNN-blue.svg\n   :target: https://github.com/aimat-lab/gcnn_keras\n\n.. |made-with-python| image:: https://img.shields.io/badge/Made%20with-Python-1f425f.svg\n   :target: https://www.python.org/\n\n.. image:: architecture.png\n    :width: 800\n    :alt: Architecture Overview\n\n================================================\nMEGAN: Multi Explanation Graph Attention Student\n================================================\n\nExplainable artificial intelligence (XAI) methods are expected to improve trust during human-AI interactions,\nprovide tools for model analysis and extend human understanding of complex problems. Attention-based models\nare an important subclass of XAI methods, partly due to their full differentiability and the potential to\nimprove explanations by means of explanation-supervised training. We propose the novel multi-explanation\ngraph attention network (MEGAN). Our graph regression and classification model features multiple explanation\nchannels, which can be chosen independently of the task specifications. We first validate our model on a\nsynthetic graph regression dataset, where our model produces single-channel explanations with quality\nsimilar to GNNExplainer. Furthermore, we demonstrate the advantages of multi-channel explanations on one\nsynthetic and two real-world datasets: The prediction of water solubility of molecular graphs and\nsentiment classification of movie reviews. We find that our model produces explanations consistent\nwith human intuition, opening the way to learning from our model in less well-understood tasks.\n\nInstallation\n============\n\nMain Installation\n-----------------\n\nClone the repository from github:\n\n.. code-block:: shell\n\n    git clone https://github.com/awa59kst120df/graph_attention_student.git\n\nThen in the main folder run a ``pip install``:\n\n.. code-block:: shell\n\n    cd graph_attention_student\n    pip3 install -e .\n\nAfterwards, you can check the install by invoking the CLI:\n\n.. code-block:: shell\n\n    python3 -m graph_attention_student.cli --version\n    python3 -m graph_attention_student.cli --help\n\nUsage\n=====\n\nComputational Experiments\n-------------------------\n\nIt is possible to list, show and execute all the computational experiments using a command line interface\nCLI.\n\n    *NOTE* Most of the experiments have a long runtime, ranging from ~2hrs to ~2days.\n    Furthermore, all of the experiments which do model training are currently configured to run on a GPU\n    and might crash if the GPU can either not be detected or does not have enough VRAM. This setting can\n    be changed in the corresponding experiment scripts\n\nAll the available experiments can be listed like this:\n\n.. code-block:: shell\n\n    python3 -m graph_attention_student.cli list\n\nThe details for a specific experiment can be viewed like this:\n\n.. code-block:: shell\n\n    python3 -m graph_attention_student.cli info [experiment_name]\n\nA new run of an experiment can be started like this. However, be aware that this might take some time.\n\n.. code-block::\n\n    python3 -m graph_attention_student.cli run [experiment_name]\n\nEach experiment will create a new archive folder, which will contain all the artifacts (such as visual\nexamples and the raw data) created during the runtime. The location of this archive folder can be found\nfrom the output generated by the experiment execution.\n\nArchived Experiments\n--------------------\n\nTo view the detailed data which was used in the making of the paper, go to\n``graph_attention_student/experiments``. The subfolders in that folder contain the archived experiments.\nThese contain extensive examples for each repetition of the various experiments as well as all of the raw\ndata collected during the execution of the experiments.\n\nMEGAN in code\n-------------\n\nThe MEGAN model is implemented as the ``MultiAttentionStudent`` class, which implements ``keras.Model``.\nThe implementation is based on the `kgcnn`_ library for graph convolutional networks for keras. For further\ninformation on loading graph structured data with `kgcnn`_ visit:\nhttps://github.com/aimat-lab/gcnn_keras\n\nThis is a simple example of how to use the model in the regression case:\n\n.. code-block:: python\n\n    import tensorflow as tf\n    import tensorflow.keras as ks\n    from graph_attention_student.training import NoLoss\n    from graph_attention_student.models import Megan\n\n    model = Megan(\n        # These lists define the number of layers and the number of hidden units in each layer for the\n        # various parts of the architecture\n        units=[9, 9, 9],  # The main convolutional layers\n        importance_units=[],  # The MLP that creates the node importances\n        final_units=[5, 1],  # The final MLP for graph embeddings\n        # Example for a regression problem. We need the prior knowledge about what range the values of the\n        # dataset will be expected to fall into...\n        regression_limits=(-3, +3),\n        # ... as well as a reference value.\n        regression_reference=0,\n        # This controls the weight of the explanation-only train step (gamma)\n        importance_factor=1.0,\n        importance_multiplier=5,\n        # This is the weight of the sparsity regularization\n        sparsity_factor=0.1,\n    )\n\n    # The model output is actually a three tuple: (prediction, node_importances, edge_importances).\n    # This allows the importances to be trained in a supervised fashion. If we don\'t want that,\n    # we can simply supply the NoLoss function instead.\n    model.compile(\n        loss=[ks.losses.MeanSquaredError(), NoLoss(), NoLoss()],\n        loss_weights=[1, 1, 1],\n        optimizer=ks.optimizers.Adam(0.001)\n    )\n\n    # model.fit() ...\n\n\n.. _kgcnn: https://github.com/aimat-lab/gcnn_keras\n.. _examples/solubility_regression.py: https://github.com/aimat-lab/graph_attention_student/tree/master/graph_attention_student/examples/solubility_regression.py\n.. _`GATv2`: https://github.com/tech-srl/how_attentive_are_gats\n\n---\n\nExamples\n========\n\nThe following examples show some of the *cherry picked* examples that show the explanatory capabilities of\nthe model.\n\nRB-Motifs Dataset\n-----------------\n\nThis is a synthetic dataset, which basically consists of randomly generated graphs with nodes of different\ncolors. Some of the graphs contain special sub-graph motifs, which are either blue-heavy or red-heavy\nstructures. The blue-heavy sub-graphs contribute a certain negative value to the overall value of the graph,\nwhile red-heavy structures contain a certain positive value.\n\nThis way, every graph has a certain value associated with it, which is between -3 and 3. The network was\ntrained to predict this value for each graph.\n\n.. image:: rb_motifs_example.png\n    :width: 800\n    :alt: Rb-Motifs Example\n\nThe examples shows from left to right: (1) The ground truth explanations, (2) a baseline MEGAN model trained\nonly on the prediction task, (3) explanation-supervised MEGAN model and (4) GNNExplainer explanations for a\nbasic GCN network. While the baseline MEGAN and GNNExplainer focus only on one of the ground truth motifs,\nthe explanation-supervised MEGAN model correctly finds both.\n\nWater Solubility Dataset\n------------------------\n\nThis is the `AqSolDB`_ dataset, which consists of ~10000 molecules and measured values for the solubility in\nwater (logS value).\n\nThe network was trained to predict the solubility value for each molecule.\n\n.. image:: solubility_example.png\n    :width: 800\n    :alt: Solubility Example.png\n\n.. _`AqSolDB`: https://www.nature.com/articles/s41597-019-0151-1\n\nMovie Reviews\n-------------\n\nOriginally the *MovieReviews* dataset is a natural language processing dataset from the `ERASER`_ benchmark.\nThe task is to classify the sentiment of ~2000 movie reviews collected from the IMDB database into the\nclasses "positive" and "negative". This dataset was converted into a graph dataset by considering all words\nas nodes of a graph and then connecting adjacent words by undirected edges with a sliding window of size 2.\nWords were converted into numeric feature vectors by using a pre-trained `GLOVE`_ model.\n\nExample for a positive review:\n\n.. image:: movie_reviews_pos.png\n    :width: 800\n    :alt: Positive Movie Review\n\nExample for a negative review:\n\n.. image:: movie_reviews_neg.png\n    :width: 800\n    :alt: Negative Movie Review\n\nExamples show the explanation channel for the "negative" class left and the "positive" class right.\nSentences with negative / positive adjectives are appropriately attributed to the corresponding channels.\n\n.. _`ERASER`: https://www.eraserbenchmark.com/\n.. _`GLOVE`: https://nlp.stanford.edu/projects/glove/\n\n',
     'author': 'xxx',
     'author_email': 'jonseb1998@gmail.com',
     'maintainer': 'xxx',
     'maintainer_email': 'jonseb1998@gmail.com',
     'url': 'None',
```

### Comparing `graph_attention_student-0.7.0/PKG-INFO` & `graph_attention_student-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graph-attention-student
-Version: 0.7.0
+Version: 0.7.1
 Summary: MEGAN: Multi Explanation Graph Attention Network
 License: MIT
 Keywords: graph neural network,attention,kgcnn
 Author: xxx
 Author-email: jonseb1998@gmail.com
 Maintainer: xxx
 Maintainer-email: jonseb1998@gmail.com
```

