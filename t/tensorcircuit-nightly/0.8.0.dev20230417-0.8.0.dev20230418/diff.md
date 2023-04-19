# Comparing `tmp/tensorcircuit-nightly-0.8.0.dev20230417.tar.gz` & `tmp/tensorcircuit-nightly-0.8.0.dev20230418.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorcircuit-nightly-0.8.0.dev20230417.tar", last modified: Mon Apr 17 12:41:53 2023, max compression
+gzip compressed data, was "tensorcircuit-nightly-0.8.0.dev20230418.tar", last modified: Tue Apr 18 12:40:08 2023, max compression
```

## Comparing `tensorcircuit-nightly-0.8.0.dev20230417.tar` & `tensorcircuit-nightly-0.8.0.dev20230418.tar`

### file list

```diff
@@ -1,133 +1,133 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 12:41:53.868855 tensorcircuit-nightly-0.8.0.dev20230417/
--rw-r--r--   0 runner    (1001) docker     (122)    22872 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)     1023 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      132 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    19799 2023-04-17 12:41:53.868855 tensorcircuit-nightly-0.8.0.dev20230417/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    17577 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     5352 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/README_cn.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 12:41:53.852855 tensorcircuit-nightly-0.8.0.dev20230417/docs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 12:41:53.856855 tensorcircuit-nightly-0.8.0.dev20230417/docs/source/
--rw-r--r--   0 runner    (1001) docker     (122)     6332 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/docs/source/advance.rst
--rw-r--r--   0 runner    (1001) docker     (122)     6308 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/docs/source/cnconf.py
--rw-r--r--   0 runner    (1001) docker     (122)     6367 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)     8192 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/docs/source/contribution.rst
--rw-r--r--   0 runner    (1001) docker     (122)    10971 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/docs/source/faq.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3677 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/docs/source/generate_rst.py
--rw-r--r--   0 runner    (1001) docker     (122)     2551 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)     8413 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/docs/source/infras.rst
--rw-r--r--   0 runner    (1001) docker     (122)      660 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (122)     4334 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/docs/source/modules.rst.backup
--rw-r--r--   0 runner    (1001) docker     (122)    27001 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/docs/source/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (122)     6229 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/docs/source/sharpbits.rst
--rw-r--r--   0 runner    (1001) docker     (122)      226 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/docs/source/textbooktoc.rst
--rw-r--r--   0 runner    (1001) docker     (122)      626 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/docs/source/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (122)      669 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/docs/source/tutorial_cn.rst
--rw-r--r--   0 runner    (1001) docker     (122)      509 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/docs/source/whitepapertoc.rst
--rw-r--r--   0 runner    (1001) docker     (122)      531 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/docs/source/whitepapertoc_cn.rst
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-17 12:41:53.868855 tensorcircuit-nightly-0.8.0.dev20230417/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1059 2023-04-17 12:41:48.000000 tensorcircuit-nightly-0.8.0.dev20230417/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 12:41:53.856855 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/
--rw-r--r--   0 runner    (1001) docker     (122)     1350 2023-04-17 12:41:48.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2901 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/about.py
--rw-r--r--   0 runner    (1001) docker     (122)    39188 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/abstractcircuit.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 12:41:53.860855 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/applications/
--rw-r--r--   0 runner    (1001) docker     (122)      234 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    34460 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/applications/dqas.py
--rw-r--r--   0 runner    (1001) docker     (122)    15348 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/applications/graphdata.py
--rw-r--r--   0 runner    (1001) docker     (122)    18124 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/applications/layers.py
--rw-r--r--   0 runner    (1001) docker     (122)    14032 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/applications/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    36391 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/applications/vags.py
--rw-r--r--   0 runner    (1001) docker     (122)    15117 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/applications/van.py
--rw-r--r--   0 runner    (1001) docker     (122)    23156 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/applications/vqes.py
--rw-r--r--   0 runner    (1001) docker     (122)     8235 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/asciiart.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 12:41:53.860855 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/backends/
--rw-r--r--   0 runner    (1001) docker     (122)       80 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    56998 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/backends/abstract_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)     1713 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/backends/backend_factory.py
--rw-r--r--   0 runner    (1001) docker     (122)    14946 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/backends/cupy_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)    24632 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/backends/jax_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)     4024 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/backends/jax_ops.py
--rw-r--r--   0 runner    (1001) docker     (122)    13813 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/backends/numpy_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)    24148 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/backends/pytorch_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)     3825 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/backends/pytorch_ops.py
--rw-r--r--   0 runner    (1001) docker     (122)    30672 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/backends/tensorflow_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)     3377 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/backends/tf_ops.py
--rw-r--r--   0 runner    (1001) docker     (122)    34020 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/basecircuit.py
--rw-r--r--   0 runner    (1001) docker     (122)    28637 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/channels.py
--rw-r--r--   0 runner    (1001) docker     (122)    36236 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/circuit.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 12:41:53.860855 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/cloud/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14582 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/cloud/abstraction.py
--rw-r--r--   0 runner    (1001) docker     (122)    17566 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/cloud/apis.py
--rw-r--r--   0 runner    (1001) docker     (122)     2252 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/cloud/local.py
--rw-r--r--   0 runner    (1001) docker     (122)     2238 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/cloud/quafu_provider.py
--rw-r--r--   0 runner    (1001) docker     (122)     3622 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/cloud/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     5764 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/cloud/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 12:41:53.860855 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/compiler/
--rw-r--r--   0 runner    (1001) docker     (122)      165 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/compiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1490 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/compiler/composed_compiler.py
--rw-r--r--   0 runner    (1001) docker     (122)     5215 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/compiler/qiskit_compiler.py
--rw-r--r--   0 runner    (1001) docker     (122)    28754 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/cons.py
--rw-r--r--   0 runner    (1001) docker     (122)    13806 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/densitymatrix.py
--rw-r--r--   0 runner    (1001) docker     (122)    15210 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/experimental.py
--rw-r--r--   0 runner    (1001) docker     (122)    29161 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/gates.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 12:41:53.860855 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/interfaces/
--rw-r--r--   0 runner    (1001) docker     (122)      448 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1439 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/interfaces/numpy.py
--rw-r--r--   0 runner    (1001) docker     (122)     3402 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/interfaces/scipy.py
--rw-r--r--   0 runner    (1001) docker     (122)     3355 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/interfaces/tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (122)     9942 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/interfaces/tensortrans.py
--rw-r--r--   0 runner    (1001) docker     (122)     3580 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/interfaces/torch.py
--rw-r--r--   0 runner    (1001) docker     (122)     9975 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/keras.py
--rw-r--r--   0 runner    (1001) docker     (122)    15270 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/mps_base.py
--rw-r--r--   0 runner    (1001) docker     (122)    34398 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/mpscircuit.py
--rw-r--r--   0 runner    (1001) docker     (122)    11878 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/noisemodel.py
--rw-r--r--   0 runner    (1001) docker     (122)    82850 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/quantum.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 12:41:53.864855 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/results/
--rw-r--r--   0 runner    (1001) docker     (122)       89 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3366 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/results/counts.py
--rw-r--r--   0 runner    (1001) docker     (122)    31378 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/results/readout_mitigation.py
--rw-r--r--   0 runner    (1001) docker     (122)     9413 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/simplify.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 12:41:53.864855 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/templates/
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6158 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/templates/blocks.py
--rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/templates/chems.py
--rw-r--r--   0 runner    (1001) docker     (122)     1933 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/templates/dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)     5811 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/templates/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (122)     3934 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/templates/graphs.py
--rw-r--r--   0 runner    (1001) docker     (122)    10942 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/templates/measurements.py
--rw-r--r--   0 runner    (1001) docker     (122)     3552 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/torchnn.py
--rw-r--r--   0 runner    (1001) docker     (122)    27351 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/translation.py
--rw-r--r--   0 runner    (1001) docker     (122)     6603 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    12195 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/vis.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 12:41:53.864855 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    19799 2023-04-17 12:41:53.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3438 2023-04-17 12:41:53.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-17 12:41:53.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      110 2023-04-17 12:41:53.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-04-17 12:41:53.000000 tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-17 12:41:53.868855 tensorcircuit-nightly-0.8.0.dev20230417/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)    33200 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tests/test_backends.py
--rw-r--r--   0 runner    (1001) docker     (122)     3805 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tests/test_calibrating.py
--rw-r--r--   0 runner    (1001) docker     (122)    11237 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tests/test_channels.py
--rw-r--r--   0 runner    (1001) docker     (122)    45826 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tests/test_circuit.py
--rw-r--r--   0 runner    (1001) docker     (122)     2518 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tests/test_compiler.py
--rw-r--r--   0 runner    (1001) docker     (122)    17232 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tests/test_dmcircuit.py
--rw-r--r--   0 runner    (1001) docker     (122)     1974 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tests/test_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (122)     4593 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tests/test_gates.py
--rw-r--r--   0 runner    (1001) docker     (122)    11359 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tests/test_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (122)     4656 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tests/test_keras.py
--rw-r--r--   0 runner    (1001) docker     (122)     6639 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tests/test_miscs.py
--rw-r--r--   0 runner    (1001) docker     (122)    10552 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tests/test_mpscircuit.py
--rw-r--r--   0 runner    (1001) docker     (122)     5637 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tests/test_noisemodel.py
--rw-r--r--   0 runner    (1001) docker     (122)      753 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tests/test_qaoa.py
--rw-r--r--   0 runner    (1001) docker     (122)    16823 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tests/test_quantum.py
--rw-r--r--   0 runner    (1001) docker     (122)     1245 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tests/test_quantum_attr.py
--rw-r--r--   0 runner    (1001) docker     (122)    11050 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tests/test_results.py
--rw-r--r--   0 runner    (1001) docker     (122)     1175 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tests/test_simplify.py
--rw-r--r--   0 runner    (1001) docker     (122)     5962 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tests/test_templates.py
--rw-r--r--   0 runner    (1001) docker     (122)     2039 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tests/test_torchnn.py
--rw-r--r--   0 runner    (1001) docker     (122)     3163 2023-04-17 12:18:09.000000 tensorcircuit-nightly-0.8.0.dev20230417/tests/test_van.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 12:40:08.415832 tensorcircuit-nightly-0.8.0.dev20230418/
+-rw-r--r--   0 runner    (1001) docker     (122)    23109 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1023 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      132 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    19799 2023-04-18 12:40:08.411832 tensorcircuit-nightly-0.8.0.dev20230418/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    17577 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     5352 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/README_cn.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 12:40:08.403832 tensorcircuit-nightly-0.8.0.dev20230418/docs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 12:40:08.403832 tensorcircuit-nightly-0.8.0.dev20230418/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (122)     6332 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/docs/source/advance.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6308 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/docs/source/cnconf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6367 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8192 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/docs/source/contribution.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10971 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/docs/source/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3677 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/docs/source/generate_rst.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2551 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     8413 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/docs/source/infras.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      660 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     4334 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/docs/source/modules.rst.backup
+-rw-r--r--   0 runner    (1001) docker     (122)    27001 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/docs/source/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6229 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/docs/source/sharpbits.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      226 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/docs/source/textbooktoc.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      626 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/docs/source/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      669 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/docs/source/tutorial_cn.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      509 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/docs/source/whitepapertoc.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      531 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/docs/source/whitepapertoc_cn.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-18 12:40:08.415832 tensorcircuit-nightly-0.8.0.dev20230418/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1059 2023-04-18 12:40:03.000000 tensorcircuit-nightly-0.8.0.dev20230418/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 12:40:08.407832 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/
+-rw-r--r--   0 runner    (1001) docker     (122)     1350 2023-04-18 12:40:03.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2901 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/about.py
+-rw-r--r--   0 runner    (1001) docker     (122)    39188 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/abstractcircuit.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 12:40:08.407832 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/applications/
+-rw-r--r--   0 runner    (1001) docker     (122)      234 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34460 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/applications/dqas.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15348 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/applications/graphdata.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18124 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/applications/layers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14032 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/applications/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36391 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/applications/vags.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15117 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/applications/van.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23156 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/applications/vqes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8235 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/asciiart.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 12:40:08.407832 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/backends/
+-rw-r--r--   0 runner    (1001) docker     (122)       80 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    56998 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/backends/abstract_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1713 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/backends/backend_factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14944 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/backends/cupy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24632 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/backends/jax_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4024 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/backends/jax_ops.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13813 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/backends/numpy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24148 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/backends/pytorch_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3825 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/backends/pytorch_ops.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30672 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/backends/tensorflow_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3377 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/backends/tf_ops.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34020 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/basecircuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28637 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/channels.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36236 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/circuit.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 12:40:08.407832 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/cloud/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14582 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/cloud/abstraction.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17566 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/cloud/apis.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2252 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/cloud/local.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2238 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/cloud/quafu_provider.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3622 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/cloud/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5764 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/cloud/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 12:40:08.407832 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/compiler/
+-rw-r--r--   0 runner    (1001) docker     (122)      165 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/compiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1490 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/compiler/composed_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5215 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/compiler/qiskit_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28754 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/cons.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13806 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/densitymatrix.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15210 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/experimental.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29161 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/gates.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 12:40:08.411832 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (122)      469 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1439 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/interfaces/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3402 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/interfaces/scipy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3355 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/interfaces/tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9942 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/interfaces/tensortrans.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5032 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/interfaces/torch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9975 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/keras.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15270 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/mps_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34398 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/mpscircuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11878 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/noisemodel.py
+-rw-r--r--   0 runner    (1001) docker     (122)    82850 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/quantum.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 12:40:08.411832 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/results/
+-rw-r--r--   0 runner    (1001) docker     (122)       89 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3366 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/results/counts.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31378 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/results/readout_mitigation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9413 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/simplify.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 12:40:08.411832 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6158 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/templates/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/templates/chems.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1933 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/templates/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5811 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/templates/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3934 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/templates/graphs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10942 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/templates/measurements.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3552 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/torchnn.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27351 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/translation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6603 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12195 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/vis.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 12:40:08.411832 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    19799 2023-04-18 12:40:08.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3438 2023-04-18 12:40:08.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-18 12:40:08.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      110 2023-04-18 12:40:08.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-04-18 12:40:08.000000 tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 12:40:08.411832 tensorcircuit-nightly-0.8.0.dev20230418/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33200 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tests/test_backends.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3805 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tests/test_calibrating.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11237 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tests/test_channels.py
+-rw-r--r--   0 runner    (1001) docker     (122)    45826 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tests/test_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2518 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tests/test_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17232 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tests/test_dmcircuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1974 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tests/test_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4593 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tests/test_gates.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13296 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tests/test_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4656 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tests/test_keras.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6639 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tests/test_miscs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10552 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tests/test_mpscircuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5637 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tests/test_noisemodel.py
+-rw-r--r--   0 runner    (1001) docker     (122)      753 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tests/test_qaoa.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16823 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tests/test_quantum.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1245 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tests/test_quantum_attr.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11050 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tests/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1175 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tests/test_simplify.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5962 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tests/test_templates.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2039 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tests/test_torchnn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3163 2023-04-18 12:17:24.000000 tensorcircuit-nightly-0.8.0.dev20230418/tests/test_van.py
```

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/CHANGELOG.md` & `tensorcircuit-nightly-0.8.0.dev20230418/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,20 @@
 
 ### Added
 
 - Add `tc.about()` to print related software versions and configs.
 
 - Torch support is updraded to 2.0, and now support native vmap and native functional grad, and thus `vvag`. Still jit support is conflict with these functional transformations and be turned off by default
 
+- Add `torch_interfaces_kws` that support static keyword arguments when wrapping with the interface
+
+### Fixed
+
+- Add tests and fixed some missing methods for cupy backend, cupy backend is now ready to use (though still not guaranteed)
+
 ## 0.8.0
 
 ### Added
 
 - Add `initial_mapping` circuit method to return a new circuit with given `logical_physical_mapping`
 
 - Add `get_positional_logical_mapping` circuit method to return the mapping when only part of the qubits are measured
```

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/HISTORY.md` & `tensorcircuit-nightly-0.8.0.dev20230418/HISTORY.md`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/LICENSE` & `tensorcircuit-nightly-0.8.0.dev20230418/LICENSE`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/PKG-INFO` & `tensorcircuit-nightly-0.8.0.dev20230418/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorcircuit-nightly
-Version: 0.8.0.dev20230417
+Version: 0.8.0.dev20230418
 Summary: nightly release for tensorcircuit
 Home-page: https://github.com/refraction-ray/tensorcircuit-dev
 Author: TensorCircuit Authors
 Author-email: znfesnpbh.tc@gmail.com
 License: UNKNOWN
 Description: <p align="center">
           <a href="https://github.com/tencent-quantum-lab/tensorcircuit">
```

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/README.md` & `tensorcircuit-nightly-0.8.0.dev20230418/README.md`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/README_cn.md` & `tensorcircuit-nightly-0.8.0.dev20230418/README_cn.md`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/docs/source/advance.rst` & `tensorcircuit-nightly-0.8.0.dev20230418/docs/source/advance.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/docs/source/cnconf.py` & `tensorcircuit-nightly-0.8.0.dev20230418/docs/source/cnconf.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/docs/source/conf.py` & `tensorcircuit-nightly-0.8.0.dev20230418/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/docs/source/contribution.rst` & `tensorcircuit-nightly-0.8.0.dev20230418/docs/source/contribution.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/docs/source/faq.rst` & `tensorcircuit-nightly-0.8.0.dev20230418/docs/source/faq.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/docs/source/generate_rst.py` & `tensorcircuit-nightly-0.8.0.dev20230418/docs/source/generate_rst.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/docs/source/index.rst` & `tensorcircuit-nightly-0.8.0.dev20230418/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/docs/source/infras.rst` & `tensorcircuit-nightly-0.8.0.dev20230418/docs/source/infras.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/docs/source/modules.rst` & `tensorcircuit-nightly-0.8.0.dev20230418/docs/source/modules.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/docs/source/modules.rst.backup` & `tensorcircuit-nightly-0.8.0.dev20230418/docs/source/modules.rst.backup`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/docs/source/quickstart.rst` & `tensorcircuit-nightly-0.8.0.dev20230418/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/docs/source/sharpbits.rst` & `tensorcircuit-nightly-0.8.0.dev20230418/docs/source/sharpbits.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/docs/source/tutorial.rst` & `tensorcircuit-nightly-0.8.0.dev20230418/docs/source/tutorial.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/docs/source/tutorial_cn.rst` & `tensorcircuit-nightly-0.8.0.dev20230418/docs/source/tutorial_cn.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/docs/source/whitepapertoc_cn.rst` & `tensorcircuit-nightly-0.8.0.dev20230418/docs/source/whitepapertoc_cn.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/setup.py` & `tensorcircuit-nightly-0.8.0.dev20230418/setup.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/__init__.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.8.0.dev20230417"
+__version__ = "0.8.0.dev20230418"
 __author__ = "TensorCircuit Authors"
 __creator__ = "refraction-ray"
 
 from .about import about
 from .cons import (
     backend,
     set_backend,
```

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/about.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/about.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/abstractcircuit.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/abstractcircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/applications/dqas.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/applications/dqas.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/applications/graphdata.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/applications/graphdata.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/applications/layers.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/applications/layers.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/applications/utils.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/applications/utils.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/applications/vags.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/applications/vags.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/applications/van.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/applications/van.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/applications/vqes.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/applications/vqes.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/asciiart.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/asciiart.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/backends/abstract_backend.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/backends/abstract_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/backends/backend_factory.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/backends/backend_factory.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/backends/cupy_backend.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/backends/cupy_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -377,30 +377,30 @@
             return true_fun()
         return false_fun()
 
     def switch(self, index: Tensor, branches: Sequence[Callable[[], Tensor]]) -> Tensor:
         return branches[index]()
 
     def device(self, a: Tensor) -> str:
-        return "gpu"
+        return self._dev2str(a.device)
 
     def device_move(self, a: Tensor, dev: Any) -> Tensor:
-        if dev == "gpu":
-            return a
-        raise ValueError("CuPy backend only support GPU device")
+        if isinstance(dev, str):
+            dev = self._str2dev(dev)
+        with dev:
+            return cp.asarray(a)
 
     def _dev2str(self, dev: Any) -> str:
-        if dev == "gpu":
-            return "gpu"
-        raise ValueError("CuPy backend only support GPU device")
+        return f"gpu:{dev.id}"
 
     def _str2dev(self, str_: str) -> Any:
-        if str_ == "gpu":
-            return "gpu"
-        raise ValueError("CuPy backend only support GPU device")
+        if str_ == "cpu":
+            raise ValueError("CuPy backend only support GPU device")
+        else:
+            return cp.cuda.Device(int(str_.split(":")[-1]))
 
     def stop_gradient(self, a: Tensor) -> Tensor:
         raise NotImplementedError("CuPy backend doesn't support AD")
 
     def grad(
         self,
         f: Callable[..., Any],
@@ -418,15 +418,15 @@
         raise NotImplementedError("CuPy backend doesn't support AD")
 
     def jit(
         self,
         f: Callable[..., Any],
         static_argnums: Optional[Union[int, Sequence[int]]] = None,
         jit_compile: Optional[bool] = None,
-        **kws: Any
+        **kws: Any,
     ) -> Callable[..., Any]:
         logger.warning("CuPy backend has no jit interface, just do nothing")
         return f
         # raise NotImplementedError("numpy backend doesn't support jit compiling")
 
     def vmap(
         self, f: Callable[..., Any], vectorized_argnums: Union[int, Sequence[int]] = 0
```

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/backends/jax_backend.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/backends/jax_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/backends/jax_ops.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/backends/jax_ops.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/backends/numpy_backend.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/backends/numpy_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/backends/pytorch_backend.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/backends/pytorch_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/backends/pytorch_ops.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/backends/pytorch_ops.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/backends/tensorflow_backend.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/backends/tensorflow_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/backends/tf_ops.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/backends/tf_ops.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/basecircuit.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/basecircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/channels.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/channels.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/circuit.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/circuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/cloud/abstraction.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/cloud/abstraction.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/cloud/apis.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/cloud/apis.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/cloud/local.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/cloud/local.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/cloud/quafu_provider.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/cloud/quafu_provider.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/cloud/utils.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/cloud/utils.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/cloud/wrapper.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/cloud/wrapper.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/compiler/composed_compiler.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/compiler/composed_compiler.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/compiler/qiskit_compiler.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/compiler/qiskit_compiler.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/cons.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/cons.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/densitymatrix.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/densitymatrix.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/experimental.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/experimental.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/gates.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/gates.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/interfaces/numpy.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/interfaces/numpy.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/interfaces/scipy.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/interfaces/scipy.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/interfaces/tensorflow.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/interfaces/tensorflow.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/interfaces/tensortrans.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/interfaces/tensortrans.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/keras.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/keras.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/mps_base.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/mps_base.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/mpscircuit.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/mpscircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/noisemodel.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/noisemodel.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/quantum.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/quantum.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/results/counts.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/results/counts.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/results/readout_mitigation.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/results/readout_mitigation.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/simplify.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/simplify.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/templates/blocks.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/templates/blocks.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/templates/chems.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/templates/chems.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/templates/dataset.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/templates/dataset.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/templates/ensemble.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/templates/ensemble.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/templates/graphs.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/templates/graphs.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/templates/measurements.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/templates/measurements.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/torchnn.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/torchnn.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/translation.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/translation.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/utils.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/utils.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit/vis.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit/vis.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit_nightly.egg-info/PKG-INFO` & `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorcircuit-nightly
-Version: 0.8.0.dev20230417
+Version: 0.8.0.dev20230418
 Summary: nightly release for tensorcircuit
 Home-page: https://github.com/refraction-ray/tensorcircuit-dev
 Author: TensorCircuit Authors
 Author-email: znfesnpbh.tc@gmail.com
 License: UNKNOWN
 Description: <p align="center">
           <a href="https://github.com/tencent-quantum-lab/tensorcircuit">
```

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tensorcircuit_nightly.egg-info/SOURCES.txt` & `tensorcircuit-nightly-0.8.0.dev20230418/tensorcircuit_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tests/conftest.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tests/test_backends.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tests/test_calibrating.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tests/test_calibrating.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tests/test_channels.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tests/test_channels.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tests/test_circuit.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tests/test_circuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tests/test_compiler.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tests/test_compiler.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tests/test_dmcircuit.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tests/test_dmcircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tests/test_ensemble.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tests/test_ensemble.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tests/test_gates.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tests/test_gates.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tests/test_interfaces.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tests/test_interfaces.py`

 * *Files 10% similar despite different names*

```diff
@@ -105,14 +105,82 @@
     l3 = torch.sum(l3)
     l3.backward()
     pg = param3.grad
     np.testing.assert_allclose(pg, 2 * np.ones([2]).astype(np.complex64), atol=1e-5)
 
 
 @pytest.mark.skipif(is_torch is False, reason="torch not installed")
+@pytest.mark.parametrize("backend", [lf("tfb"), lf("jaxb")])
+def test_torch_interface_kws(backend):
+    def f(param, n):
+        c = tc.Circuit(n)
+        c = tc.templates.blocks.example_block(c, param)
+        loss = c.expectation(
+            [
+                tc.gates.x(),
+                [
+                    1,
+                ],
+            ]
+        )
+        return tc.backend.real(loss)
+
+    f_jit_torch = tc.interfaces.torch_interface_kws(f, jit=True, enable_dlpack=True)
+
+    param = torch.ones([4, 4], requires_grad=True)
+    l = f_jit_torch(param, n=4)
+    l = l**2
+    l.backward()
+
+    pg = param.grad
+    np.testing.assert_allclose(pg.shape, [4, 4])
+    np.testing.assert_allclose(pg[0, 1], -2.146e-3, atol=1e-5)
+
+    def f2(paramzz, paramx, n, nlayer):
+        c = tc.Circuit(n)
+        for i in range(n):
+            c.H(i)
+        for j in range(nlayer):  # 2
+            for i in range(n - 1):
+                c.exp1(i, i + 1, unitary=tc.gates._zz_matrix, theta=paramzz[j, i])
+            for i in range(n):
+                c.rx(i, theta=paramx[j, i])
+        loss1 = c.expectation(
+            [
+                tc.gates.x(),
+                [
+                    1,
+                ],
+            ]
+        )
+        loss2 = c.expectation(
+            [
+                tc.gates.x(),
+                [
+                    2,
+                ],
+            ]
+        )
+        return tc.backend.real(loss1), tc.backend.real(loss2)
+
+    f2_torch = tc.interfaces.torch_interface_kws(f2, jit=True, enable_dlpack=True)
+
+    paramzz = torch.ones([2, 4], requires_grad=True)
+    paramx = torch.ones([2, 4], requires_grad=True)
+
+    l1, l2 = f2_torch(paramzz, paramx, n=4, nlayer=2)
+    l = l1 - l2
+    l.backward()
+
+    pg = paramzz.grad
+    np.testing.assert_allclose(pg.shape, [2, 4])
+    np.testing.assert_allclose(pg[0, 0], -0.41609, atol=1e-5)
+
+
+@pytest.mark.skipif(is_torch is False, reason="torch not installed")
 @pytest.mark.xfail(
     (int(tf.__version__.split(".")[1]) < 9)
     or (int("".join(jax.__version__.split(".")[1:])) < 314),
     reason="version too low for tf or jax",
 )
 @pytest.mark.parametrize("backend", [lf("tfb"), lf("jaxb")])
 def test_torch_interface_dlpack_complex(backend):
```

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tests/test_keras.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tests/test_keras.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tests/test_miscs.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tests/test_miscs.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tests/test_mpscircuit.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tests/test_mpscircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tests/test_noisemodel.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tests/test_noisemodel.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tests/test_qaoa.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tests/test_qaoa.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tests/test_quantum.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tests/test_quantum.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tests/test_quantum_attr.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tests/test_quantum_attr.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tests/test_results.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tests/test_simplify.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tests/test_simplify.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tests/test_templates.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tests/test_torchnn.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tests/test_torchnn.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.8.0.dev20230417/tests/test_van.py` & `tensorcircuit-nightly-0.8.0.dev20230418/tests/test_van.py`

 * *Files identical despite different names*

