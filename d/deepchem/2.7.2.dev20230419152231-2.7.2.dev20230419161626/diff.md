# Comparing `tmp/deepchem-2.7.2.dev20230419152231.tar.gz` & `tmp/deepchem-2.7.2.dev20230419161626.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepchem-2.7.2.dev20230419152231.tar", last modified: Wed Apr 19 15:22:31 2023, max compression
+gzip compressed data, was "deepchem-2.7.2.dev20230419161626.tar", last modified: Wed Apr 19 16:16:26 2023, max compression
```

## Comparing `deepchem-2.7.2.dev20230419152231.tar` & `deepchem-2.7.2.dev20230419161626.tar`

### file list

```diff
@@ -1,287 +1,287 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:31.678510 deepchem-2.7.2.dev20230419152231/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1047 2023-04-19 15:22:21.000000 deepchem-2.7.2.dev20230419152231/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-19 15:22:31.678510 deepchem-2.7.2.dev20230419152231/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-04-19 15:22:21.000000 deepchem-2.7.2.dev20230419152231/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:31.650509 deepchem-2.7.2.dev20230419152231/deepchem/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:31.654509 deepchem-2.7.2.dev20230419152231/deepchem/data/
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    67617 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/data/data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)   118009 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/data/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/data/pytorch_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    12606 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/data/supports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:31.654509 deepchem-2.7.2.dev20230419152231/deepchem/dock/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/dock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/dock/binding_pocket.py
--rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/dock/docking.py
--rw-r--r--   0 runner    (1001) docker     (123)    19576 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/dock/pose_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/dock/pose_scoring.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:31.654509 deepchem-2.7.2.dev20230419152231/deepchem/feat/
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/feat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/feat/atomic_conformation.py
--rw-r--r--   0 runner    (1001) docker     (123)    19279 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/feat/base_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/feat/bert_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/feat/binding_pocket_features.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:31.654509 deepchem-2.7.2.dev20230419152231/deepchem/feat/complex_featurizers/
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/feat/complex_featurizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12898 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/feat/complex_featurizers/complex_atomic_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)    10769 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/feat/complex_featurizers/contact_fingerprints.py
--rw-r--r--   0 runner    (1001) docker     (123)    27676 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/feat/complex_featurizers/grid_featurizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    20248 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/feat/complex_featurizers/rdkit_grid_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11465 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/feat/complex_featurizers/splif_fingerprints.py
--rw-r--r--   0 runner    (1001) docker     (123)    10599 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/feat/dft_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    17552 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/feat/graph_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    38890 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/feat/graph_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/feat/huggingface_featurizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:31.654509 deepchem-2.7.2.dev20230419152231/deepchem/feat/material_featurizers/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/feat/material_featurizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7539 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/feat/material_featurizers/cgcnn_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/feat/material_featurizers/element_property_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/feat/material_featurizers/elemnet_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    28058 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/feat/material_featurizers/lcnn_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/feat/material_featurizers/sine_coulomb_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    14808 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/feat/mol_graphs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:31.658509 deepchem-2.7.2.dev20230419152231/deepchem/feat/molecule_featurizers/
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/feat/molecule_featurizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/feat/molecule_featurizers/atomic_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/feat/molecule_featurizers/bp_symmetry_function_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/feat/molecule_featurizers/circular_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    10925 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/feat/molecule_featurizers/coulomb_matrices.py
--rw-r--r--   0 runner    (1001) docker     (123)    19123 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/feat/molecule_featurizers/dmpnn_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/feat/molecule_featurizers/grover_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/feat/molecule_featurizers/maccs_keys_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/feat/molecule_featurizers/mat_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7587 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/feat/molecule_featurizers/mol2vec_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    20381 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/feat/molecule_featurizers/mol_graph_conv_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9346 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/feat/molecule_featurizers/molgan_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/feat/molecule_featurizers/mordred_descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/feat/molecule_featurizers/one_hot_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/feat/molecule_featurizers/pubchem_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/feat/molecule_featurizers/raw_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9855 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/feat/molecule_featurizers/rdkit_descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/feat/molecule_featurizers/smiles_to_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/feat/molecule_featurizers/smiles_to_seq.py
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/feat/molecule_featurizers/snap_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/feat/molecule_featurizers/sparse_matrix_one_hot_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/feat/reaction_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/feat/roberta_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:31.658509 deepchem-2.7.2.dev20230419152231/deepchem/feat/sequence_featurizers/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/feat/sequence_featurizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/feat/sequence_featurizers/position_frequency_matrix_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11383 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/feat/smiles_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:31.658509 deepchem-2.7.2.dev20230419152231/deepchem/feat/vocabulary_builders/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/feat/vocabulary_builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17291 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/feat/vocabulary_builders/grover_vocab.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/feat/vocabulary_builders/hf_vocab.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/feat/vocabulary_builders/vocabulary_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:31.658509 deepchem-2.7.2.dev20230419152231/deepchem/hyper/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/hyper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/hyper/base_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)    17151 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/hyper/gaussian_process.py
--rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/hyper/grid_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    12427 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/hyper/random_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:31.658509 deepchem-2.7.2.dev20230419152231/deepchem/metalearning/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/metalearning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10539 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/metalearning/maml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:31.658509 deepchem-2.7.2.dev20230419152231/deepchem/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/metrics/genomic_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    31620 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/metrics/score_function.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:31.662509 deepchem-2.7.2.dev20230419152231/deepchem/models/
--rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/models/IRV.py
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13833 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/models/atomic_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/models/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    17354 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/models/chemnet_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    15504 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/models/chemnet_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:31.662509 deepchem-2.7.2.dev20230419152231/deepchem/models/dft/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/models/dft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9576 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/models/dft/nnxc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/models/dft/scf.py
--rw-r--r--   0 runner    (1001) docker     (123)    23457 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/models/fcnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    24548 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/models/gan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:31.662509 deepchem-2.7.2.dev20230419152231/deepchem/models/gbdt_models/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/models/gbdt_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/models/gbdt_models/gbdt_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    57408 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/models/graph_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:31.662509 deepchem-2.7.2.dev20230419152231/deepchem/models/jax_models/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/models/jax_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28179 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/models/jax_models/jax_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/models/jax_models/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    17070 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/models/jax_models/pinns_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    56522 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/models/keras_model.py
--rw-r--r--   0 runner    (1001) docker     (123)   144759 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/models/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:31.662509 deepchem-2.7.2.dev20230419152231/deepchem/models/lightning/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/models/lightning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/models/lightning/dc_lightning_dataset_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/models/lightning/dc_lightning_module.py
--rw-r--r--   0 runner    (1001) docker     (123)    39719 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/models/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/models/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    13967 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/models/molgan.py
--rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/models/multitask.py
--rw-r--r--   0 runner    (1001) docker     (123)    10975 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/models/normalizing_flows.py
--rw-r--r--   0 runner    (1001) docker     (123)    26871 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/models/optimizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13095 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/models/progressive_multitask.py
--rw-r--r--   0 runner    (1001) docker     (123)    17830 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/models/robust_multitask.py
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/models/scscore.py
--rw-r--r--   0 runner    (1001) docker     (123)    25969 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/models/seqtoseq.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:31.662509 deepchem-2.7.2.dev20230419152231/deepchem/models/sklearn_models/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/models/sklearn_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/models/sklearn_models/sklearn_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    10552 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/models/text_cnn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:31.666509 deepchem-2.7.2.dev20230419152231/deepchem/models/torch_models/
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/models/torch_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/models/torch_models/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)    12226 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/models/torch_models/attentivefp.py
--rw-r--r--   0 runner    (1001) docker     (123)    14455 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/models/torch_models/cgcnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     9543 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/models/torch_models/cnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    31166 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/models/torch_models/dmpnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/models/torch_models/ferminet.py
--rw-r--r--   0 runner    (1001) docker     (123)    15845 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/models/torch_models/gat.py
--rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/models/torch_models/gcn.py
--rw-r--r--   0 runner    (1001) docker     (123)    20930 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/models/torch_models/gnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    37602 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/models/torch_models/grover.py
--rw-r--r--   0 runner    (1001) docker     (123)    38432 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/models/torch_models/grover_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    30077 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/models/torch_models/infograph.py
--rw-r--r--   0 runner    (1001) docker     (123)    19215 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/models/torch_models/kfac_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)   109518 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/models/torch_models/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18575 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/models/torch_models/lcnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    17126 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/models/torch_models/mat.py
--rw-r--r--   0 runner    (1001) docker     (123)    11170 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/models/torch_models/megnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    18074 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/models/torch_models/modular.py
--rw-r--r--   0 runner    (1001) docker     (123)    12074 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/models/torch_models/mpnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/models/torch_models/normalizing_flows_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)    12297 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/models/torch_models/pagtn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/models/torch_models/readout.py
--rw-r--r--   0 runner    (1001) docker     (123)    52629 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/models/torch_models/torch_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5249 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/models/wandblogger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:31.666509 deepchem-2.7.2.dev20230419152231/deepchem/molnet/
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/molnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11668 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/molnet/check_availability.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/molnet/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)    14702 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/molnet/dnasim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:31.670509 deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/bace_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    14202 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/bace_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/bbbc_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/bbbp_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/cell_counting_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/chembl25_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/chembl_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    10252 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/chembl_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/clearance_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/clintox_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/delaney_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/factors_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/freesolv_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/hiv_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/hopv_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/hppb_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/kaggle_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)   165414 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/kaggle_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     8104 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/kinase_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/lipo_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     9165 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/load_dataset_template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:31.670509 deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/material_datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/material_datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/material_datasets/load_Pt_NO_surface_adsorbate_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/material_datasets/load_bandgap.py
--rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/material_datasets/load_mp_formation_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/material_datasets/load_mp_metallicity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/material_datasets/load_perovskite.py
--rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/molnet_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/muv_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/nci_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/pcba_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     8586 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/pdbbind_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/ppb_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/qm7_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/qm8_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/qm9_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/sampl_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/sider_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/sweetlead_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/thermosol_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/tox21_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    18900 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/toxcast_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/uspto_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/uv_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/uv_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/zinc15_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/molnet/preset_hyper_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    13549 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/molnet/run_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/molnet/run_benchmark_low_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    36564 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/molnet/run_benchmark_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:31.674510 deepchem-2.7.2.dev20230419152231/deepchem/rl/
--rw-r--r--   0 runner    (1001) docker     (123)     9312 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23102 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/rl/a2c.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:31.674510 deepchem-2.7.2.dev20230419152231/deepchem/rl/envs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/rl/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/rl/envs/test_tictactoe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/rl/envs/tictactoe.py
--rw-r--r--   0 runner    (1001) docker     (123)    25262 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/rl/ppo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:31.674510 deepchem-2.7.2.dev20230419152231/deepchem/splits/
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/splits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    63895 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/splits/splitters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/splits/task_splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:31.674510 deepchem-2.7.2.dev20230419152231/deepchem/trans/
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/trans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/trans/duplicate.py
--rw-r--r--   0 runner    (1001) docker     (123)    91191 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/trans/transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:31.674510 deepchem-2.7.2.dev20230419152231/deepchem/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/utils/conformers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13294 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/utils/coordinate_box_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20923 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/utils/debug_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/utils/dftutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10476 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/utils/docking_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13528 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/utils/electron_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    19454 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/utils/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/utils/fake_data_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/utils/fragment_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/utils/genomics_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8259 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/utils/geometry_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/utils/grover.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/utils/hash_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    19262 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/utils/molecule_feature_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17713 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/utils/noncovalent_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11749 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/utils/pdbqt_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/utils/pytorch_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    65677 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/utils/rdkit_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/utils/save.py
--rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/utils/sequence_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:31.678510 deepchem-2.7.2.dev20230419152231/deepchem/utils/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/utils/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/utils/test/test_coordinate_box_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/utils/test/test_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/utils/test/test_dftutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/utils/test/test_docking_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/utils/test/test_electron_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12977 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/utils/test/test_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/utils/test/test_fake_data_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/utils/test/test_fragment_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/utils/test/test_generator_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/utils/test/test_genomics_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/utils/test/test_geometry_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/utils/test/test_grover.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/utils/test/test_hash_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/utils/test/test_molecule_feature_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/utils/test/test_noncovalent_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/utils/test/test_pdbqt_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/utils/test/test_rdkit_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/utils/test/test_sequence_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/utils/test/test_voxel_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/utils/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/utils/vina_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/deepchem/utils/voxel_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:31.654509 deepchem-2.7.2.dev20230419152231/deepchem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-19 15:22:31.000000 deepchem-2.7.2.dev20230419152231/deepchem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10307 2023-04-19 15:22:31.000000 deepchem-2.7.2.dev20230419152231/deepchem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 15:22:31.000000 deepchem-2.7.2.dev20230419152231/deepchem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-19 15:22:31.000000 deepchem-2.7.2.dev20230419152231/deepchem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-19 15:22:31.000000 deepchem-2.7.2.dev20230419152231/deepchem.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-19 15:22:31.678510 deepchem-2.7.2.dev20230419152231/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-04-19 15:22:22.000000 deepchem-2.7.2.dev20230419152231/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:26.906831 deepchem-2.7.2.dev20230419161626/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1047 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-19 16:16:26.906831 deepchem-2.7.2.dev20230419161626/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:26.874829 deepchem-2.7.2.dev20230419161626/deepchem/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:26.874829 deepchem-2.7.2.dev20230419161626/deepchem/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67617 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/data/data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)   118009 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/data/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/data/pytorch_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12606 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/data/supports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:26.874829 deepchem-2.7.2.dev20230419161626/deepchem/dock/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/dock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/dock/binding_pocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/dock/docking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19576 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/dock/pose_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/dock/pose_scoring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:26.878829 deepchem-2.7.2.dev20230419161626/deepchem/feat/
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/atomic_conformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19279 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/base_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/bert_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/binding_pocket_features.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:26.878829 deepchem-2.7.2.dev20230419161626/deepchem/feat/complex_featurizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/complex_featurizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12898 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/complex_featurizers/complex_atomic_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10769 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/complex_featurizers/contact_fingerprints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27676 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/complex_featurizers/grid_featurizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20248 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/complex_featurizers/rdkit_grid_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11465 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/complex_featurizers/splif_fingerprints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10599 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/dft_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17552 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/graph_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38890 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/graph_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/huggingface_featurizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:26.878829 deepchem-2.7.2.dev20230419161626/deepchem/feat/material_featurizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/material_featurizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7539 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/material_featurizers/cgcnn_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/material_featurizers/element_property_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/material_featurizers/elemnet_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28058 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/material_featurizers/lcnn_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/material_featurizers/sine_coulomb_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14808 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/mol_graphs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:26.882829 deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/atomic_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/bp_symmetry_function_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/circular_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10925 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/coulomb_matrices.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19123 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/dmpnn_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/grover_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/maccs_keys_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/mat_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7587 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/mol2vec_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20381 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/mol_graph_conv_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9346 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/molgan_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/mordred_descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/one_hot_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/pubchem_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/raw_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9855 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/rdkit_descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/smiles_to_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/smiles_to_seq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/snap_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/sparse_matrix_one_hot_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/reaction_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/roberta_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:26.882829 deepchem-2.7.2.dev20230419161626/deepchem/feat/sequence_featurizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/sequence_featurizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/sequence_featurizers/position_frequency_matrix_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11383 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/smiles_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:26.882829 deepchem-2.7.2.dev20230419161626/deepchem/feat/vocabulary_builders/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/vocabulary_builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17291 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/vocabulary_builders/grover_vocab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/vocabulary_builders/hf_vocab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/vocabulary_builders/vocabulary_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:26.882829 deepchem-2.7.2.dev20230419161626/deepchem/hyper/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/hyper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/hyper/base_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17151 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/hyper/gaussian_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/hyper/grid_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12427 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/hyper/random_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:26.882829 deepchem-2.7.2.dev20230419161626/deepchem/metalearning/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/metalearning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10539 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/metalearning/maml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:26.882829 deepchem-2.7.2.dev20230419161626/deepchem/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/metrics/genomic_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31620 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/metrics/score_function.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:26.886830 deepchem-2.7.2.dev20230419161626/deepchem/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/IRV.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13833 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/atomic_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17354 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/chemnet_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15504 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/chemnet_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:26.886830 deepchem-2.7.2.dev20230419161626/deepchem/models/dft/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/dft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9576 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/dft/nnxc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/dft/scf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23457 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/fcnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24548 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/gan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:26.886830 deepchem-2.7.2.dev20230419161626/deepchem/models/gbdt_models/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/gbdt_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/gbdt_models/gbdt_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57408 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/graph_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:26.886830 deepchem-2.7.2.dev20230419161626/deepchem/models/jax_models/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/jax_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28179 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/jax_models/jax_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/jax_models/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17070 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/jax_models/pinns_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56522 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/keras_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)   144759 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:26.890830 deepchem-2.7.2.dev20230419161626/deepchem/models/lightning/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/lightning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/lightning/dc_lightning_dataset_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/lightning/dc_lightning_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45861 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13967 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/molgan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/multitask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10975 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/normalizing_flows.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26871 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13095 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/progressive_multitask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17830 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/robust_multitask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/scscore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25969 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/seqtoseq.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:26.890830 deepchem-2.7.2.dev20230419161626/deepchem/models/sklearn_models/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/sklearn_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/sklearn_models/sklearn_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10552 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/text_cnn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:26.890830 deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12226 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/attentivefp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14455 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/cgcnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9543 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/cnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31166 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/dmpnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/ferminet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15845 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/gat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/gcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32724 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/gnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37602 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/grover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38432 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/grover_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30077 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/infograph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19215 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/kfac_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)   109518 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18575 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/lcnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17126 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/mat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11170 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/megnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18074 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/modular.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12074 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/mpnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/normalizing_flows_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12297 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/pagtn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/readout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52629 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/torch_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5249 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/wandblogger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:26.894830 deepchem-2.7.2.dev20230419161626/deepchem/molnet/
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11668 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/check_availability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14702 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/dnasim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:26.898831 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/bace_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14202 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/bace_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/bbbc_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/bbbp_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/cell_counting_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/chembl25_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/chembl_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10252 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/chembl_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/clearance_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/clintox_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/delaney_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/factors_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/freesolv_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/hiv_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/hopv_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/hppb_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/kaggle_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)   165414 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/kaggle_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8104 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/kinase_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/lipo_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9165 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/load_dataset_template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:26.898831 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/material_datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/material_datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/material_datasets/load_Pt_NO_surface_adsorbate_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/material_datasets/load_bandgap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/material_datasets/load_mp_formation_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/material_datasets/load_mp_metallicity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/material_datasets/load_perovskite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/molnet_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/muv_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/nci_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/pcba_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8586 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/pdbbind_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/ppb_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/qm7_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/qm8_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/qm9_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/sampl_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/sider_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/sweetlead_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/thermosol_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/tox21_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18900 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/toxcast_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/uspto_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/uv_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/uv_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/zinc15_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/preset_hyper_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13549 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/run_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/run_benchmark_low_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36564 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/run_benchmark_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:26.898831 deepchem-2.7.2.dev20230419161626/deepchem/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)     9312 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23102 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/rl/a2c.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:26.902831 deepchem-2.7.2.dev20230419161626/deepchem/rl/envs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/rl/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/rl/envs/test_tictactoe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/rl/envs/tictactoe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25262 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/rl/ppo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:26.902831 deepchem-2.7.2.dev20230419161626/deepchem/splits/
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/splits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63895 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/splits/splitters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/splits/task_splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:26.902831 deepchem-2.7.2.dev20230419161626/deepchem/trans/
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/trans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/trans/duplicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91191 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/trans/transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:26.906831 deepchem-2.7.2.dev20230419161626/deepchem/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/conformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13294 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/coordinate_box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20923 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/debug_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/dftutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10476 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/docking_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13528 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/electron_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19454 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/fake_data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/fragment_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/genomics_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8259 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/geometry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/grover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/hash_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19262 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/molecule_feature_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17713 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/noncovalent_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11749 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/pdbqt_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/pytorch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65677 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/rdkit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/sequence_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:26.906831 deepchem-2.7.2.dev20230419161626/deepchem/utils/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_coordinate_box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_dftutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_docking_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_electron_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12977 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_fake_data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_fragment_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_generator_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_genomics_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_geometry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_grover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_hash_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_molecule_feature_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_noncovalent_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_pdbqt_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_rdkit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_sequence_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_voxel_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/vina_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/voxel_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:26.874829 deepchem-2.7.2.dev20230419161626/deepchem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-19 16:16:26.000000 deepchem-2.7.2.dev20230419161626/deepchem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10307 2023-04-19 16:16:26.000000 deepchem-2.7.2.dev20230419161626/deepchem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 16:16:26.000000 deepchem-2.7.2.dev20230419161626/deepchem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-19 16:16:26.000000 deepchem-2.7.2.dev20230419161626/deepchem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-19 16:16:26.000000 deepchem-2.7.2.dev20230419161626/deepchem.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-19 16:16:26.906831 deepchem-2.7.2.dev20230419161626/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-04-19 16:16:15.000000 deepchem-2.7.2.dev20230419161626/setup.py
```

### Comparing `deepchem-2.7.2.dev20230419152231/LICENSE` & `deepchem-2.7.2.dev20230419161626/LICENSE`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/PKG-INFO` & `deepchem-2.7.2.dev20230419161626/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepchem
-Version: 2.7.2.dev20230419152231
+Version: 2.7.2.dev20230419161626
 Summary: Deep learning models for drug discovery,         quantum chemistry, and the life sciences.
 Home-page: https://github.com/deepchem/deepchem
 Maintainer: DeepChem contributors
 License: MIT
 Project-URL: Documentation, https://deepchem.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/deepchem/deepchem
 Keywords: deepchem,chemistry,biology,materials-science,life-science,drug-discovery
```

### Comparing `deepchem-2.7.2.dev20230419152231/README.md` & `deepchem-2.7.2.dev20230419161626/README.md`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/data/__init__.py` & `deepchem-2.7.2.dev20230419161626/deepchem/data/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/data/data_loader.py` & `deepchem-2.7.2.dev20230419161626/deepchem/data/data_loader.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/data/datasets.py` & `deepchem-2.7.2.dev20230419161626/deepchem/data/datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/data/pytorch_datasets.py` & `deepchem-2.7.2.dev20230419161626/deepchem/data/pytorch_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/data/supports.py` & `deepchem-2.7.2.dev20230419161626/deepchem/data/supports.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/dock/binding_pocket.py` & `deepchem-2.7.2.dev20230419161626/deepchem/dock/binding_pocket.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/dock/docking.py` & `deepchem-2.7.2.dev20230419161626/deepchem/dock/docking.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/dock/pose_generation.py` & `deepchem-2.7.2.dev20230419161626/deepchem/dock/pose_generation.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/dock/pose_scoring.py` & `deepchem-2.7.2.dev20230419161626/deepchem/dock/pose_scoring.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/feat/__init__.py` & `deepchem-2.7.2.dev20230419161626/deepchem/feat/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/feat/atomic_conformation.py` & `deepchem-2.7.2.dev20230419161626/deepchem/feat/atomic_conformation.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/feat/base_classes.py` & `deepchem-2.7.2.dev20230419161626/deepchem/feat/base_classes.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/feat/bert_tokenizer.py` & `deepchem-2.7.2.dev20230419161626/deepchem/feat/bert_tokenizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/feat/binding_pocket_features.py` & `deepchem-2.7.2.dev20230419161626/deepchem/feat/binding_pocket_features.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/feat/complex_featurizers/__init__.py` & `deepchem-2.7.2.dev20230419161626/deepchem/feat/complex_featurizers/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/feat/complex_featurizers/complex_atomic_coordinates.py` & `deepchem-2.7.2.dev20230419161626/deepchem/feat/complex_featurizers/complex_atomic_coordinates.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/feat/complex_featurizers/contact_fingerprints.py` & `deepchem-2.7.2.dev20230419161626/deepchem/feat/complex_featurizers/contact_fingerprints.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/feat/complex_featurizers/grid_featurizers.py` & `deepchem-2.7.2.dev20230419161626/deepchem/feat/complex_featurizers/grid_featurizers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/feat/complex_featurizers/rdkit_grid_featurizer.py` & `deepchem-2.7.2.dev20230419161626/deepchem/feat/complex_featurizers/rdkit_grid_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/feat/complex_featurizers/splif_fingerprints.py` & `deepchem-2.7.2.dev20230419161626/deepchem/feat/complex_featurizers/splif_fingerprints.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/feat/dft_data.py` & `deepchem-2.7.2.dev20230419161626/deepchem/feat/dft_data.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/feat/graph_data.py` & `deepchem-2.7.2.dev20230419161626/deepchem/feat/graph_data.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/feat/graph_features.py` & `deepchem-2.7.2.dev20230419161626/deepchem/feat/graph_features.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/feat/huggingface_featurizer.py` & `deepchem-2.7.2.dev20230419161626/deepchem/feat/huggingface_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/feat/material_featurizers/cgcnn_featurizer.py` & `deepchem-2.7.2.dev20230419161626/deepchem/feat/material_featurizers/cgcnn_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/feat/material_featurizers/element_property_fingerprint.py` & `deepchem-2.7.2.dev20230419161626/deepchem/feat/material_featurizers/element_property_fingerprint.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/feat/material_featurizers/elemnet_featurizer.py` & `deepchem-2.7.2.dev20230419161626/deepchem/feat/material_featurizers/elemnet_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/feat/material_featurizers/lcnn_featurizer.py` & `deepchem-2.7.2.dev20230419161626/deepchem/feat/material_featurizers/lcnn_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/feat/material_featurizers/sine_coulomb_matrix.py` & `deepchem-2.7.2.dev20230419161626/deepchem/feat/material_featurizers/sine_coulomb_matrix.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/feat/mol_graphs.py` & `deepchem-2.7.2.dev20230419161626/deepchem/feat/mol_graphs.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/feat/molecule_featurizers/__init__.py` & `deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/feat/molecule_featurizers/atomic_coordinates.py` & `deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/atomic_coordinates.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/feat/molecule_featurizers/bp_symmetry_function_input.py` & `deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/bp_symmetry_function_input.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/feat/molecule_featurizers/circular_fingerprint.py` & `deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/circular_fingerprint.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/feat/molecule_featurizers/coulomb_matrices.py` & `deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/coulomb_matrices.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/feat/molecule_featurizers/dmpnn_featurizer.py` & `deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/dmpnn_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/feat/molecule_featurizers/grover_featurizer.py` & `deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/grover_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/feat/molecule_featurizers/maccs_keys_fingerprint.py` & `deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/maccs_keys_fingerprint.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/feat/molecule_featurizers/mat_featurizer.py` & `deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/mat_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/feat/molecule_featurizers/mol2vec_fingerprint.py` & `deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/mol2vec_fingerprint.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/feat/molecule_featurizers/mol_graph_conv_featurizer.py` & `deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/mol_graph_conv_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/feat/molecule_featurizers/molgan_featurizer.py` & `deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/molgan_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/feat/molecule_featurizers/mordred_descriptors.py` & `deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/mordred_descriptors.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/feat/molecule_featurizers/one_hot_featurizer.py` & `deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/one_hot_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/feat/molecule_featurizers/pubchem_fingerprint.py` & `deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/pubchem_fingerprint.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/feat/molecule_featurizers/raw_featurizer.py` & `deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/raw_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/feat/molecule_featurizers/rdkit_descriptors.py` & `deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/rdkit_descriptors.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/feat/molecule_featurizers/smiles_to_image.py` & `deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/smiles_to_image.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/feat/molecule_featurizers/smiles_to_seq.py` & `deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/smiles_to_seq.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/feat/molecule_featurizers/snap_featurizer.py` & `deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/snap_featurizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 from deepchem.feat import MolecularFeaturizer
 from rdkit import Chem
 import numpy as np
 from deepchem.feat.graph_data import GraphData
 
 allowable_features = {
     'possible_atomic_num_list':
-    list(range(1, 119)),
+        list(range(0, 119)),  # 0 represents a masked atom
     'possible_formal_charge_list': [-5, -4, -3, -2, -1, 0, 1, 2, 3, 4, 5],
     'possible_chirality_list': [
         Chem.rdchem.ChiralType.CHI_UNSPECIFIED,
         Chem.rdchem.ChiralType.CHI_TETRAHEDRAL_CW,
         Chem.rdchem.ChiralType.CHI_TETRAHEDRAL_CCW,
         Chem.rdchem.ChiralType.CHI_OTHER
-    ],
+    ],  # noqa: E122
     'possible_hybridization_list': [
         Chem.rdchem.HybridizationType.S, Chem.rdchem.HybridizationType.SP,
         Chem.rdchem.HybridizationType.SP2, Chem.rdchem.HybridizationType.SP3,
         Chem.rdchem.HybridizationType.SP3D, Chem.rdchem.HybridizationType.SP3D2,
         Chem.rdchem.HybridizationType.UNSPECIFIED
-    ],
+    ],  # noqa: E122
     'possible_numH_list': [0, 1, 2, 3, 4, 5, 6, 7, 8],
     'possible_implicit_valence_list': [0, 1, 2, 3, 4, 5, 6],
     'possible_degree_list': [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10],
+    # 0 represents a masked bond
     'possible_bonds': [
-        Chem.rdchem.BondType.SINGLE, Chem.rdchem.BondType.DOUBLE,
+        0, Chem.rdchem.BondType.SINGLE, Chem.rdchem.BondType.DOUBLE,
         Chem.rdchem.BondType.TRIPLE, Chem.rdchem.BondType.AROMATIC
-    ],
+    ],  # noqa: E122
     'possible_bond_dirs': [  # only for double bond stereo information
         Chem.rdchem.BondDir.NONE, Chem.rdchem.BondDir.ENDUPRIGHT,
         Chem.rdchem.BondDir.ENDDOWNRIGHT
-    ]
+    ]  # noqa: E122
 }
 
 
 class SNAPFeaturizer(MolecularFeaturizer):
     """
     This featurizer is based on the SNAP featurizer used in the paper [1].
```

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/feat/molecule_featurizers/sparse_matrix_one_hot_featurizer.py` & `deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/sparse_matrix_one_hot_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/feat/reaction_featurizer.py` & `deepchem-2.7.2.dev20230419161626/deepchem/feat/reaction_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/feat/roberta_tokenizer.py` & `deepchem-2.7.2.dev20230419161626/deepchem/feat/roberta_tokenizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/feat/sequence_featurizers/position_frequency_matrix_featurizer.py` & `deepchem-2.7.2.dev20230419161626/deepchem/feat/sequence_featurizers/position_frequency_matrix_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/feat/smiles_tokenizer.py` & `deepchem-2.7.2.dev20230419161626/deepchem/feat/smiles_tokenizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/feat/vocabulary_builders/grover_vocab.py` & `deepchem-2.7.2.dev20230419161626/deepchem/feat/vocabulary_builders/grover_vocab.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/feat/vocabulary_builders/hf_vocab.py` & `deepchem-2.7.2.dev20230419161626/deepchem/feat/vocabulary_builders/hf_vocab.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/feat/vocabulary_builders/vocabulary_builder.py` & `deepchem-2.7.2.dev20230419161626/deepchem/feat/vocabulary_builders/vocabulary_builder.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/hyper/base_classes.py` & `deepchem-2.7.2.dev20230419161626/deepchem/hyper/base_classes.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/hyper/gaussian_process.py` & `deepchem-2.7.2.dev20230419161626/deepchem/hyper/gaussian_process.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/hyper/grid_search.py` & `deepchem-2.7.2.dev20230419161626/deepchem/hyper/grid_search.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/hyper/random_search.py` & `deepchem-2.7.2.dev20230419161626/deepchem/hyper/random_search.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/metalearning/maml.py` & `deepchem-2.7.2.dev20230419161626/deepchem/metalearning/maml.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/metrics/__init__.py` & `deepchem-2.7.2.dev20230419161626/deepchem/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/metrics/genomic_metrics.py` & `deepchem-2.7.2.dev20230419161626/deepchem/metrics/genomic_metrics.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/metrics/metric.py` & `deepchem-2.7.2.dev20230419161626/deepchem/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/metrics/score_function.py` & `deepchem-2.7.2.dev20230419161626/deepchem/metrics/score_function.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/models/IRV.py` & `deepchem-2.7.2.dev20230419161626/deepchem/models/IRV.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/models/__init__.py` & `deepchem-2.7.2.dev20230419161626/deepchem/models/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/models/atomic_conv.py` & `deepchem-2.7.2.dev20230419161626/deepchem/models/atomic_conv.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/models/callbacks.py` & `deepchem-2.7.2.dev20230419161626/deepchem/models/callbacks.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/models/chemnet_layers.py` & `deepchem-2.7.2.dev20230419161626/deepchem/models/chemnet_layers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/models/chemnet_models.py` & `deepchem-2.7.2.dev20230419161626/deepchem/models/chemnet_models.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/models/dft/nnxc.py` & `deepchem-2.7.2.dev20230419161626/deepchem/models/dft/nnxc.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/models/dft/scf.py` & `deepchem-2.7.2.dev20230419161626/deepchem/models/dft/scf.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/models/fcnet.py` & `deepchem-2.7.2.dev20230419161626/deepchem/models/fcnet.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/models/gan.py` & `deepchem-2.7.2.dev20230419161626/deepchem/models/gan.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/models/gbdt_models/gbdt_model.py` & `deepchem-2.7.2.dev20230419161626/deepchem/models/gbdt_models/gbdt_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/models/graph_models.py` & `deepchem-2.7.2.dev20230419161626/deepchem/models/graph_models.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/models/jax_models/jax_model.py` & `deepchem-2.7.2.dev20230419161626/deepchem/models/jax_models/jax_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/models/jax_models/layers.py` & `deepchem-2.7.2.dev20230419161626/deepchem/models/jax_models/layers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/models/jax_models/pinns_model.py` & `deepchem-2.7.2.dev20230419161626/deepchem/models/jax_models/pinns_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/models/keras_model.py` & `deepchem-2.7.2.dev20230419161626/deepchem/models/keras_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/models/layers.py` & `deepchem-2.7.2.dev20230419161626/deepchem/models/layers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/models/lightning/dc_lightning_dataset_module.py` & `deepchem-2.7.2.dev20230419161626/deepchem/models/lightning/dc_lightning_dataset_module.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/models/lightning/dc_lightning_module.py` & `deepchem-2.7.2.dev20230419161626/deepchem/models/lightning/dc_lightning_module.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/models/losses.py` & `deepchem-2.7.2.dev20230419161626/deepchem/models/losses.py`

 * *Files 10% similar despite different names*

```diff
@@ -972,14 +972,150 @@
                 torch.ones_like(positive_score)) + self.criterion(
                     negative_score, torch.zeros_like(negative_score))
             return edge_pred_loss
 
         return loss
 
 
+class GraphNodeMaskingLoss(Loss):
+    """
+    GraphNodeMaskingLoss is an unsupervised graph node masking loss function that calculates the loss based on the predicted node labels and true node labels. This loss function is designed for graph neural networks and is particularly useful for pre-training tasks.
+
+    This loss function encourages the model to learn node embeddings that can effectively predict the masked node labels in the graph.
+
+    The loss is computed using the CrossEntropyLoss between the predicted node labels and the true node labels.
+
+    To use this loss function, the input must be a BatchGraphData object transformed by the mask_nodes function. The loss function takes the predicted node labels, predicted edge labels, and the input graph data (with masked node labels) as inputs and returns the node masking loss.
+
+    Parameters
+    ----------
+    pred_node: torch.Tensor
+        Predicted node labels
+    pred_edge: Optional(torch.Tensor)
+        Predicted edge labels
+    inputs: BatchGraphData
+        Input graph data with masked node and edge labels
+
+    Examples
+    --------
+    >>> from deepchem.models.losses import GraphNodeMaskingLoss
+    >>> from deepchem.feat.graph_data import BatchGraphData, GraphData
+    >>> from deepchem.models.torch_models.gnn import mask_nodes
+    >>> import torch
+    >>> import numpy as np
+    >>> num_nodes_list, num_edge_list = [3, 4, 5], [2, 4, 5]
+    >>> num_node_features, num_edge_features = 32, 32
+    >>> edge_index_list = [
+    ...     np.array([[0, 1], [1, 2]]),
+    ...     np.array([[0, 1, 2, 3], [1, 2, 0, 2]]),
+    ...     np.array([[0, 1, 2, 3, 4], [1, 2, 3, 4, 0]]),
+    ... ]
+    >>> graph_list = [
+    ...     GraphData(node_features=np.random.random_sample(
+    ...         (num_nodes_list[i], num_node_features)),
+    ...               edge_index=edge_index_list[i],
+    ...               edge_features=np.random.random_sample(
+    ...                   (num_edge_list[i], num_edge_features)),
+    ...               node_pos_features=None) for i in range(len(num_edge_list))
+    ... ]
+    >>> batched_graph = BatchGraphData(graph_list)
+    >>> batched_graph = batched_graph.numpy_to_torch()
+    >>> masked_graph = mask_nodes(batched_graph, 0.1)
+    >>> pred_node = torch.randn((sum(num_nodes_list), num_node_features))
+    >>> pred_edge = torch.randn((sum(num_edge_list), num_edge_features))
+    >>> loss_func = GraphNodeMaskingLoss()._create_pytorch_loss()
+    >>> loss = loss_func(pred_node[masked_graph.masked_node_indices],
+    ...                  pred_edge[masked_graph.connected_edge_indices], masked_graph)
+
+    References
+    ----------
+    .. [1] Hu, W. et al. Strategies for Pre-training Graph Neural Networks. Preprint at https://doi.org/10.48550/arXiv.1905.12265 (2020).
+    """
+
+    def _create_pytorch_loss(self, mask_edge=True):
+        import torch
+        self.mask_edge = mask_edge
+        self.criterion = torch.nn.CrossEntropyLoss()
+
+        def loss(pred_node, pred_edge, inputs):
+
+            # loss for nodes
+            loss = self.criterion(pred_node, inputs.mask_node_label)
+
+            if self.mask_edge:
+                loss += self.criterion(pred_edge, inputs.mask_edge_label)
+            return loss
+
+        return loss
+
+
+class GraphEdgeMaskingLoss(Loss):
+    """
+    GraphEdgeMaskingLoss is an unsupervised graph edge masking loss function that calculates the loss based on the predicted edge labels and true edge labels. This loss function is designed for graph neural networks and is particularly useful for pre-training tasks.
+
+    This loss function encourages the model to learn node embeddings that can effectively predict the masked edge labels in the graph.
+
+    The loss is computed using the CrossEntropyLoss between the predicted edge labels and the true edge labels.
+
+    To use this loss function, the input must be a BatchGraphData object transformed by the mask_edges function. The loss function takes the predicted edge labels and the true edge labels as inputs and returns the edge masking loss.
+
+    Parameters
+    ----------
+    pred_edge: torch.Tensor
+        Predicted edge labels.
+    inputs: BatchGraphData
+        Input graph data (with masked edge labels).
+
+    Examples
+    --------
+    >>> from deepchem.models.losses import GraphEdgeMaskingLoss
+    >>> from deepchem.feat.graph_data import BatchGraphData, GraphData
+    >>> from deepchem.models.torch_models.gnn import mask_edges
+    >>> import torch
+    >>> import numpy as np
+    >>> num_nodes_list, num_edge_list = [3, 4, 5], [2, 4, 5]
+    >>> num_node_features, num_edge_features = 32, 32
+    >>> edge_index_list = [
+    ...     np.array([[0, 1], [1, 2]]),
+    ...     np.array([[0, 1, 2, 3], [1, 2, 0, 2]]),
+    ...     np.array([[0, 1, 2, 3, 4], [1, 2, 3, 4, 0]]),
+    ... ]
+    >>> graph_list = [
+    ...     GraphData(node_features=np.random.random_sample(
+    ...         (num_nodes_list[i], num_node_features)),
+    ...               edge_index=edge_index_list[i],
+    ...               edge_features=np.random.random_sample(
+    ...                   (num_edge_list[i], num_edge_features)),
+    ...               node_pos_features=None) for i in range(len(num_edge_list))
+    ... ]
+    >>> batched_graph = BatchGraphData(graph_list)
+    >>> batched_graph = batched_graph.numpy_to_torch()
+    >>> masked_graph = mask_edges(batched_graph, .1)
+    >>> pred_edge = torch.randn((sum(num_edge_list), num_edge_features))
+    >>> loss_func = GraphEdgeMaskingLoss()._create_pytorch_loss()
+    >>> loss = loss_func(pred_edge[masked_graph.masked_edge_idx], masked_graph)
+
+    References
+    ----------
+    .. [1] Hu, W. et al. Strategies for Pre-training Graph Neural Networks. Preprint at https://doi.org/10.48550/arXiv.1905.12265 (2020).
+    """
+
+    def _create_pytorch_loss(self):
+        import torch
+        self.criterion = torch.nn.CrossEntropyLoss()
+
+        def loss(pred_edge, inputs):
+            # converting the binary classification to multiclass classification
+            labels = torch.argmax(inputs.mask_edge_label, dim=1)
+            loss = self.criterion(pred_edge, labels)
+            return loss
+
+        return loss
+
+
 def _make_tf_shapes_consistent(output, labels):
     """Try to make inputs have the same shape by adding dimensions of size 1."""
     import tensorflow as tf
     shape1 = output.shape
     shape2 = labels.shape
     len1 = len(shape1)
     len2 = len(shape2)
```

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/models/models.py` & `deepchem-2.7.2.dev20230419161626/deepchem/models/models.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/models/molgan.py` & `deepchem-2.7.2.dev20230419161626/deepchem/models/molgan.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/models/multitask.py` & `deepchem-2.7.2.dev20230419161626/deepchem/models/multitask.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/models/normalizing_flows.py` & `deepchem-2.7.2.dev20230419161626/deepchem/models/normalizing_flows.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/models/optimizers.py` & `deepchem-2.7.2.dev20230419161626/deepchem/models/optimizers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/models/progressive_multitask.py` & `deepchem-2.7.2.dev20230419161626/deepchem/models/progressive_multitask.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/models/robust_multitask.py` & `deepchem-2.7.2.dev20230419161626/deepchem/models/robust_multitask.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/models/scscore.py` & `deepchem-2.7.2.dev20230419161626/deepchem/models/scscore.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/models/seqtoseq.py` & `deepchem-2.7.2.dev20230419161626/deepchem/models/seqtoseq.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/models/sklearn_models/sklearn_model.py` & `deepchem-2.7.2.dev20230419161626/deepchem/models/sklearn_models/sklearn_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/models/text_cnn.py` & `deepchem-2.7.2.dev20230419161626/deepchem/models/text_cnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/models/torch_models/__init__.py` & `deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/models/torch_models/attention.py` & `deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/attention.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/models/torch_models/attentivefp.py` & `deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/attentivefp.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/models/torch_models/cgcnn.py` & `deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/cgcnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/models/torch_models/cnn.py` & `deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/cnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/models/torch_models/dmpnn.py` & `deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/dmpnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/models/torch_models/ferminet.py` & `deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/ferminet.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/models/torch_models/gat.py` & `deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/gat.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/models/torch_models/gcn.py` & `deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/gcn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/models/torch_models/gnn.py` & `deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/kfac_optimizer.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,512 +1,486 @@
-import torch
-from torch_geometric.nn import GINEConv, global_add_pool, global_mean_pool, global_max_pool
-from torch_geometric.nn.aggr import AttentionalAggregation, Set2Set
-from torch.functional import F
-from deepchem.data import Dataset
-from deepchem.models.losses import SoftmaxCrossEntropy, EdgePredictionLoss
-from deepchem.models.torch_models import ModularTorchModel
-from deepchem.feat.graph_data import BatchGraphData
-from typing import Iterable, List, Tuple
-from deepchem.metrics import to_one_hot
-
-num_atom_type = 120
-num_chirality_tag = 3
-# Relevant in future PRs
-# num_bond_type = 6
-# num_bond_direction = 3
-
-
-class GNN(torch.nn.Module):
-    """
-    GNN module for the GNNModular model.
+"""
+Implementation of KFAC, a second order optimizer, in PyTorch.
+"""
+import math
+from typing import Optional, Callable, Dict, Tuple, List, Union
+try:
+    import torch
+    import torch.optim as optim
+    has_pytorch = True
 
-    This module is responsible for the graph neural network layers in the GNNModular model.
+except ModuleNotFoundError:
+    has_pytorch = False
 
-    Parameters
-    ----------
-    atom_type_embedding: torch.nn.Embedding
-        Embedding layer for atom types.
-    chirality_embedding: torch.nn.Embedding
-        Embedding layer for chirality tags.
-    gconvs: torch.nn.ModuleList
-        ModuleList of graph convolutional layers.
-    batch_norms: torch.nn.ModuleList
-        ModuleList of batch normalization layers.
-    dropout: int
-        Dropout probability.
-    jump_knowledge: str
-        The type of jump knowledge to use. [1] Must be one of "last", "sum", "max", "concat" or "none".
-        "last": Use the node representation from the last GNN layer.
-        "concat": Concatenate the node representations from all GNN layers.
-        "max": Take the element-wise maximum of the node representations from all GNN layers.
-        "sum": Take the element-wise sum of the node representations from all GNN layers.
-    init_emb: bool
-        Whether to initialize the embedding layers with Xavier uniform initialization.
-
-    References
-    ----------
-    .. [1] Xu, K. et al. Representation Learning on Graphs with Jumping Knowledge Networks. Preprint at https://doi.org/10.48550/arXiv.1806.03536 (2018).
-
-    Example
-    -------
-    >>> from deepchem.models.torch_models.gnn import GNNModular
-    >>> from deepchem.feat.graph_data import BatchGraphData
-    >>> from deepchem.feat.molecule_featurizers import SNAPFeaturizer
-    >>> featurizer = SNAPFeaturizer()
-    >>> smiles = ["C1=CC=CC=C1", "C1=CC=CC=C1C=O", "C1=CC=CC=C1C(=O)O"]
-    >>> features = featurizer.featurize(smiles)
-    >>> batched_graph = BatchGraphData(features).numpy_to_torch(device="cuda")
-    >>> modular = GNNModular(emb_dim = 8, task = "edge_pred")
-    >>> gnnmodel = modular.gnn
-    >>> print(gnnmodel(batched_graph)[0].shape)
-    torch.Size([23, 32])
 
+class KFACOptimizer(optim.Optimizer):
+    """"
+    This class implement the second order optimizer - KFAC, which uses Kronecker factor products of inputs and the gradients to
+    get the approximate inverse fisher matrix, which is used to update the model parameters. Presently this optimizer works only
+    on liner and 2D convolution layers. If you want to know more details about KFAC, please check the paper [1]_ and [2]_.
+
+    References:
+    -----------
+    [1] Martens, James, and Roger Grosse. Optimizing Neural Networks with Kronecker-Factored Approximate Curvature.
+    arXiv:1503.05671, arXiv, 7 June 2020. arXiv.org, http://arxiv.org/abs/1503.05671.
+    [2] Grosse, Roger, and James Martens. A Kronecker-Factored Approximate Fisher Matrix for Convolution Layers.
+    arXiv:1602.01407, arXiv, 23 May 2016. arXiv.org, http://arxiv.org/abs/1602.01407.
     """
 
     def __init__(self,
-                 atom_type_embedding,
-                 chirality_embedding,
-                 gconvs,
-                 batch_norms,
-                 dropout,
-                 jump_knowledge,
-                 init_emb=False):
-        super(GNN, self).__init__()
-
-        self.atom_type_embedding = atom_type_embedding
-        self.chirality_embedding = chirality_embedding
-        self.gconv = gconvs
-        self.batch_norms = batch_norms
-        self.dropout = dropout
-        self.num_layer = len(gconvs)
-        self.jump_knowledge = jump_knowledge
-
-        # may mess with loading pretrained weights
-        if init_emb:
-            torch.nn.init.xavier_uniform_(self.atom_type_embedding.weight.data)
-            torch.nn.init.xavier_uniform_(self.chirality_embedding.weight.data)
+                 model: torch.nn.Module,
+                 lr: float = 0.001,
+                 momentum: float = 0.9,
+                 stat_decay: float = 0.95,
+                 damping: float = 0.001,
+                 kl_clip: float = 0.001,
+                 weight_decay: float = 0,
+                 TCov: int = 10,
+                 TInv: int = 100,
+                 batch_averaged: bool = True,
+                 mean: bool = False):
+        """
+        Parameters:
+        -----------
+        model: torch.nn.Module
+            The model to be optimized.
+        lr: float (default: 0.001)
+            Learning rate for the optimizer.
+        momentum: float (default: 0.9)
+            Momentum for the optimizer.
+        stat_decay: float (default: 0.95)
+            Decay rate for the update of covariance matrix with mean.
+        damping: float (default: 0.001)
+            damping factor for the update of covariance matrix.
+        kl_clip: float (default: 0.001)
+            Clipping value for the update of covariance matrix.
+        weight_decay: float (default: 0)
+            weight decay for the optimizer.
+        Tcov: int (default: 10)
+            The number of steps to update the covariance matrix.
+        Tinv: int (default: 100)
+            The number of steps to calculate the inverse of covariance matrix.
+        batch_averaged: bool (default: True)
+            States whether to use batch averaged covariance matrix.
+        mean: bool (default: False)
+            States whether to use mean centered covariance matrix.
+        """
+
+        if lr < 0.0:
+            raise ValueError("Invalid learning rate: {}".format(lr))
+        if momentum < 0.0:
+            raise ValueError("Invalid momentum value: {}".format(momentum))
+        if weight_decay < 0.0:
+            raise ValueError(
+                "Invalid weight_decay value: {}".format(weight_decay))
+        defaults = dict(lr=lr,
+                        momentum=momentum,
+                        damping=damping,
+                        weight_decay=weight_decay)
+        super(KFACOptimizer, self).__init__(model.parameters(), defaults)
+        self.batch_averaged = batch_averaged
+
+        self.known_modules = {'Linear', 'Conv2d'}
+
+        self.modules: List[torch.nn.Module] = []
+
+        self.model = model
+        self._prepare_model()
+
+        self.steps = 0
+
+        self.m_aa: Dict[torch.nn.Module, torch.Tensor] = {}
+        self.m_gg: Dict[torch.nn.Module, torch.Tensor] = {}
+        self.Q_a: Dict[torch.nn.Module, torch.Tensor] = {}
+        self.Q_g: Dict[torch.nn.Module, torch.Tensor] = {}
+        self.d_a: Dict[torch.nn.Module, torch.Tensor] = {}
+        self.d_g: Dict[torch.nn.Module, torch.Tensor] = {}
+        self.stat_decay = stat_decay
+
+        self.kl_clip = kl_clip
+        self.TCov = TCov
+        self.TInv = TInv
+
+        self.mean = mean
+
+    def try_contiguous(self, x: torch.Tensor) -> torch.Tensor:
+        """
+        Checks the memory layout of the input tensor and changes it to contiguous type.
+
+        Parameters:
+        -----------
+        x: torch.Tensor
+            The input tensor to be made contiguous in memory, if it is not so.
 
-    def forward(self, data: BatchGraphData):
-        """
-        Forward pass for the GNN module.
-
-        Parameters
-        ----------
-        data: BatchGraphData
-            Batched graph data.
+        Return:
+        -------
+        torch.Tensor
+            Tensor with contiguous memory
         """
+        if not x.is_contiguous():
+            x = x.contiguous()
 
-        node_feats = data.node_features[:, 0].long()  # type: ignore
-        chiral_feats = data.node_features[:, 1].long()  # type: ignore
-        x = self.atom_type_embedding(node_feats) + self.chirality_embedding(
-            chiral_feats)
-
-        h_list = [x]
-        for i, conv_layer in enumerate(self.gconv):
-            h = conv_layer(h_list[i], data.edge_index, data.edge_features)
-            h = self.batch_norms[i](h)
-            h = F.dropout(F.relu(h), self.dropout, training=self.training)
-            if i == self.num_layer - 1:
-                # remove relu for the last layer
-                h = F.dropout(h, self.dropout, training=self.training)
-            else:
-                h = F.dropout(F.relu(h), self.dropout, training=self.training)
-            h_list.append(h)
-
-        # Different implementations of jump_knowledge
-        if self.jump_knowledge == "concat":
-            node_representation = torch.cat(h_list, dim=1)
-        elif self.jump_knowledge == "last":
-            node_representation = h_list[-1]
-        elif self.jump_knowledge == "max":
-            h_list = [h.unsqueeze_(0) for h in h_list]
-            node_representation = torch.max(torch.cat(h_list, dim=0), dim=0)[0]
-        elif self.jump_knowledge == "sum":
-            h_list = [h.unsqueeze_(0) for h in h_list]
-            node_representation = torch.sum(torch.cat(h_list, dim=0), dim=0)[0]
+        return x
 
-        return (node_representation, data)
-
-
-class GNNHead(torch.nn.Module):
-    """
-    Prediction head module for the GNNModular model.
+    def _extract_patches(
+            self, x: torch.Tensor, kernel_size: Tuple[int,
+                                                      ...], stride: Tuple[int,
+                                                                          ...],
+            padding: Union[int, str, Tuple[int, ...]]) -> torch.Tensor:
+        """
+        Extract patches of a given size from the input tensor given. Used in calculating
+        the matrices for the kronecker product in the case of 2d Convolutions.
+
+        Parameters:
+        -----------
+        x: torch.Tensor
+            The input feature maps. with the size of (batch_size, in_c, h, w)
+        kernel_size: Tuple[int, ...]
+            the kernel size of the conv filter.
+        stride: Tuple[int, ...]
+            the stride of conv operation.
+        padding: Union[int, str, Tuple[int, ...]]
+            number of paddings. be a tuple of two elements
 
-    Parameters
-    ----------
-    pool: Union[function,torch.nn.Module]
-        Pooling function or nn.Module to use
-    head: torch.nn.Module
-        Prediction head to use
-    task: str
-        The type of task. Must be one of "regression", "classification".
-    num_tasks: int
-        Number of tasks.
-    num_classes: int
-        Number of classes for classification.
-    """
+        Return:
+        -------
+        torch.Tensor:
+            Extracted patches with shape (batch_size, out_h, out_w, in_c*kh*kw)
+        """
+        if isinstance(padding, tuple):
+            if padding[0] + padding[1] > 0:
+                x = torch.nn.functional.pad(
+                    x, (padding[1], padding[1], padding[0],
+                        padding[0])).data  # Actually check dims
+        elif isinstance(padding, int):
+            if padding > 0:
+                x = torch.nn.functional.pad(
+                    x, (padding, padding, padding, padding)).data
+        elif isinstance(padding, str):
+            if padding == 'VALID':
+                pad = int((kernel_size[0] - 1) / 2)
+                x = torch.nn.functional.pad(x, (pad, pad, pad, pad)).data
+
+        x = x.unfold(2, kernel_size[0], stride[0])
+        x = x.unfold(3, kernel_size[1], stride[1])
+        x = x.transpose_(1, 2).transpose_(2, 3).contiguous()
+        x = x.view(x.size(0), x.size(1), x.size(2),
+                   x.size(3) * x.size(4) * x.size(5))
+        return x
+
+    def compute_cov_a(self, a: torch.Tensor,
+                      layer: torch.nn.Module) -> torch.Tensor:
+        """
+        Compute the covariance matrix of the A matrix (the output of each layer).
+
+        Parameters:
+        -----------
+        a: torch.Tensor
+            It is the output of the layer for which the covariance matrix should be calculated.
+        layer: torch.nn.Module
+            It specifies the type of layer from which the output of the layer is taken.
+
+        Returns:
+        --------
+        torch.Tensor
+            The covariance matrix of the A matrix.
+        """
+        if isinstance(layer, torch.nn.Linear):
+            batch_size = a.size(0)
+            if layer.bias is not None:
+                a = torch.cat((a, a.new(a.size(0), 1).fill_(1)), 1)
+
+        elif isinstance(layer, torch.nn.Conv2d):
+            batch_size = a.size(0)
+            a = self._extract_patches(a, layer.kernel_size, layer.stride,
+                                      layer.padding)
+            spatial_size = a.size(1) * a.size(2)
+            a = a.view(-1, a.size(-1))
+            if layer.bias is not None:
+                a = torch.cat((a, a.new(a.size(0), 1).fill_(1)), 1)
+            a = a / spatial_size
+
+        return a.t() @ (a / batch_size)
+
+    def compute_cov_g(self, g: torch.Tensor,
+                      layer: torch.nn.Module) -> torch.Tensor:
+        """
+        Compute the covariance matrix of the G matrix (the gradient of the layer).
+
+        Parameters:
+        -----------
+        g: torch.Tensor
+            It is the gradient of the layer for which the covariance matrix should be calculated.
+        layer: torch.nn.Module
+            It specifies the type of layer from which the output of the layer is taken.
+
+        Returns:
+        --------
+        torch.Tensor
+            The covariance matrix of the G matrix.
+        """
+        if isinstance(layer, torch.nn.Linear):
+            batch_size = g.size(0)
+            if self.batch_averaged:
+                cov_g = g.t() @ (g * batch_size)
+            else:
+                cov_g = g.t() @ (g / batch_size)
 
-    def __init__(self, pool, head, task, num_tasks, num_classes):
-        super().__init__()
-        self.pool = pool
-        self.head = head
-        self.task = task
-        self.num_tasks = num_tasks
-        self.num_classes = num_classes
+        elif isinstance(layer, torch.nn.Conv2d):
+            spatial_size = g.size(2) * g.size(3)
+            batch_size = g.shape[0]
+            g = g.transpose(1, 2).transpose(2, 3)
+            g = self.try_contiguous(g)
+            g = g.view(-1, g.size(-1))
+            if self.batch_averaged:
+                g = g * batch_size
+            g = g * spatial_size
+            cov_g = g.t() @ (g / g.size(0))
+
+        return cov_g
+
+    def _save_input(self, module: torch.nn.Module, input: torch.Tensor):
+        """
+        Updates the input of the layer using exponentially weighted averages of the layer input.
+
+        Parameters:
+        -----------
+        module: torch.nn.Module
+            specifies the layer for which the input should be taken
+        input: torch.Tensor
+            the input matrix which should get updated
+        """
+        if self.steps % self.TCov == 0:
+            aa = self.compute_cov_a(input[0].data, module)
+            # Initialize buffers
+            if self.steps == 0:
+                self.m_aa[module] = torch.diag(aa.new(aa.size(0)).fill_(1))
+            self.m_aa[module] *= self.stat_decay + aa * (1 - self.stat_decay)
+
+    def _save_grad_output(self, module: torch.nn.Module,
+                          grad_input: torch.Tensor, grad_output: torch.Tensor):
+        """
+        Updates the backward gradient of the layer using exponentially weighted averages of the layer input.
+
+        Parameters:
+        -----------
+        module: torch.nn.Module
+            specifies the layer for which the gradient should be taken
+        input: torch.Tensor
+            the gradient matrix which should get updated
+        """
+        # Accumulate statistics for Fisher matrices
+        if self.steps % self.TCov == 0:
+            gg = self.compute_cov_g(grad_output[0].data, module)
+            # Initialize buffers
+            if self.steps == 0:
+                self.m_gg[module] = torch.diag(gg.new(gg.size(0)).fill_(1))
+            self.m_gg[module] *= self.stat_decay + gg * (1 - self.stat_decay)
+
+    def _prepare_model(self):
+        """"
+        Attaches hooks(saving the ouptut and grad according to the update function) to the model for
+        to calculate gradients at every step.
+        """
+        count = 0
+        for module in self.model.modules():
+            classname = module.__class__.__name__
+            if classname in self.known_modules:
+                self.modules.append(module)
+                module.register_forward_pre_hook(self._save_input)
+                module.register_backward_hook(self._save_grad_output)
+                count += 1
 
-    def forward(self, data):
+    def _update_inv(self, m: torch.nn.Module):
         """
-        Forward pass for the GNN head module.
+        Does eigen decomposition of the input(A) and gradient(G) matrix for computing inverse of the ~ fisher.
 
-        Parameters
+        Parameter:
         ----------
-        data: tuple
-            A tuple containing the node representations and the input graph data.
-            node_representation is a torch.Tensor created after passing input through the GNN layers.
-            input_batch is the original input BatchGraphData.
+        m: torch.nn.Module
+            This is the layer for which the eigen decomposition should be done on.
         """
-        node_representation, input_batch = data
-
-        pooled = self.pool(node_representation, input_batch.graph_index)
-        out = self.head(pooled)
-        if self.task == "classification":
-            out = torch.reshape(out, (-1, self.num_tasks, self.num_classes))
-        return out
-
+        eps = 1e-10  # for numerical stability
 
-class GNNModular(ModularTorchModel):
-    """
-    Modular GNN which allows for easy swapping of GNN layers.
-
-    Parameters
-    ----------
-    gnn_type: str
-        The type of GNN layer to use. Must be one of "gin", "gcn", "graphsage", or "gat".
-    num_layer: int
-        The number of GNN layers to use.
-    emb_dim: int
-        The dimensionality of the node embeddings.
-    num_tasks: int
-        The number of tasks.
-    graph_pooling: str
-        The type of graph pooling to use. Must be one of "sum", "mean", "max", "attention" or "set2set".
-    dropout: float, optional (default 0)
-        The dropout probability.
-    jump_knowledge: str, optional (default "last")
-        The type of jump knowledge to use. [1] Must be one of "last", "sum", "max", "concat" or "none".
-        "last": Use the node representation from the last GNN layer.
-        "concat": Concatenate the node representations from all GNN layers.
-        "max": Take the element-wise maximum of the node representations from all GNN layers.
-        "sum": Take the element-wise sum of the node representations from all GNN layers.
-    task: str, optional (default "regression")
-        The type of task. Can be unsupervised tasks "edge_pred" or "node_pred" or supervised tasks like "regression" or "classification".
-
-    Examples
-    --------
-    >>> import numpy as np
-    >>> import deepchem as dc
-    >>> from deepchem.feat.molecule_featurizers import SNAPFeaturizer
-    >>> from deepchem.models.torch_models.gnn import GNNModular
-    >>> featurizer = SNAPFeaturizer()
-    >>> smiles = ["C1=CC=CC=C1", "C1=CC=CC=C1C=O", "C1=CC=CC=C1C(=O)O"]
-    >>> features = featurizer.featurize(smiles)
-    >>> dataset = dc.data.NumpyDataset(features, np.zeros(len(features)))
-    >>> model = GNNModular(task="edge_pred")
-    >>> loss = model.fit(dataset, nb_epoch=1)
-
-    References
-    ----------
-    .. [1] Xu, K. et al. Representation Learning on Graphs with Jumping Knowledge Networks. Preprint at https://doi.org/10.48550/arXiv.1806.03536 (2018).
-    .. [2] Hu, W. et al. Strategies for Pre-training Graph Neural Networks. Preprint at https://doi.org/10.48550/arXiv.1905.12265 (2020).
-    """
-
-    def __init__(self,
-                 gnn_type: str = "gin",
-                 num_layer: int = 3,
-                 emb_dim: int = 64,
-                 num_tasks: int = 1,
-                 num_classes: int = 2,
-                 graph_pooling: str = "attention",
-                 dropout: int = 0,
-                 jump_knowledge: str = "concat",
-                 task: str = "edge_pred",
-                 **kwargs):
-        self.gnn_type = gnn_type
-        self.num_layer = num_layer
-        self.emb_dim = emb_dim
-
-        self.num_tasks = num_tasks
-        self.num_classes = num_classes
-        if task == "classification":
-            self.output_dim = num_classes * num_tasks
-            self.criterion = SoftmaxCrossEntropy()._create_pytorch_loss()
-        elif task == "regression":
-            self.output_dim = num_tasks
-            self.criterion = F.mse_loss
-        elif task == "edge_pred":
-            self.output_dim = num_tasks
-            self.edge_pred_loss = EdgePredictionLoss()._create_pytorch_loss()
-
-        self.graph_pooling = graph_pooling
-        self.dropout = dropout
-        self.jump_knowledge = jump_knowledge
-        self.task = task
-
-        self.components = self.build_components()
-        self.model = self.build_model()
-        super().__init__(self.model, self.components, **kwargs)
-
-    def build_components(self):
-        """
-        Builds the components of the GNNModular model. It initializes the encoders, batch normalization layers, pooling layers, and head layers based on the provided configuration. The method returns a dictionary containing the following components:
-
-        Components list, type and description:
-        --------------------------------------
-        atom_type_embedding: torch.nn.Embedding, an embedding layer for atom types.
-
-        chirality_embedding: torch.nn.Embedding, an embedding layer for chirality tags.
-
-        gconvs: torch_geometric.nn.conv.MessagePassing, a list of graph convolutional layers (encoders) based on the specified GNN type (GIN, GCN, or GAT).
-
-        batch_norms: torch.nn.BatchNorm1d, a list of batch normalization layers corresponding to the encoders.
-
-        pool: Union[function,torch_geometric.nn.aggr.Aggregation], a pooling layer based on the specified graph pooling type (sum, mean, max, attention, or set2set).
-
-        head: nn.Linear, a linear layer for the head of the model.
-
-        These components are then used to construct the GNN and GNN_head modules for the GNNModular model.
-        """
-        encoders = []
-        batch_norms = []
-        for layer in range(self.num_layer):
-            if self.gnn_type == "gin":
-                encoders.append(
-                    GINEConv(
-                        torch.nn.Linear(self.emb_dim, self.emb_dim),
-                        edge_dim=2,  # bond type, bond direction
-                        aggr="add"))
-            else:
-                raise ValueError("Only GIN is supported for now")
-            # Relevent for future PRs
-            # elif self.gnn_type == "gcn":
-            #     encoders.append(GCNConv(self.emb_dim))
-            # elif self.gnn_type == "gat":
-            #     encoders.append(GATConv(self.emb_dim))
-            batch_norms.append(torch.nn.BatchNorm1d(self.emb_dim))
-        encoders = torch.nn.ModuleList(encoders)
-        batch_norms = torch.nn.ModuleList(batch_norms)
-
-        if self.graph_pooling == "sum":
-            pool = global_add_pool
-        elif self.graph_pooling == "mean":
-            pool = global_mean_pool
-        elif self.graph_pooling == "max":
-            pool = global_max_pool
-        elif self.graph_pooling == "attention":
-            if self.jump_knowledge == "concat":
-                pool = AttentionalAggregation(
-                    gate_nn=torch.nn.Linear((self.num_layer + 1) *
-                                            self.emb_dim, 1))
-            else:
-                pool = AttentionalAggregation(
-                    gate_nn=torch.nn.Linear(self.emb_dim, 1))
-        elif self.graph_pooling == "set2set":
-            set2setiter = 3
-            if self.jump_knowledge == "concat":
-                pool = Set2Set((self.num_layer + 1) * self.emb_dim, set2setiter)
-            else:
-                pool = Set2Set(self.emb_dim, processing_steps=set2setiter)
-
-        if self.graph_pooling == "set2set":
-            mult = 2
-        else:
-            mult = 1
-
-        if self.jump_knowledge == "concat":
-            head = torch.nn.Linear(mult * (self.num_layer + 1) * self.emb_dim,
-                                   self.output_dim)
-        else:
-            head = torch.nn.Linear(mult * self.emb_dim, self.output_dim)
-
-        components = {
-            'atom_type_embedding':
-                torch.nn.Embedding(num_atom_type, self.emb_dim),
-            'chirality_embedding':
-                torch.nn.Embedding(num_chirality_tag, self.emb_dim),
-            'gconvs':
-                encoders,
-            'batch_norms':
-                batch_norms,
-            'pool':
-                pool,
-            'head':
-                head
-        }
-        self.gnn = GNN(components['atom_type_embedding'],
-                       components['chirality_embedding'], components['gconvs'],
-                       components['batch_norms'], self.dropout,
-                       self.jump_knowledge)
-        self.gnn_head = GNNHead(components['pool'], components['head'],
-                                self.task, self.num_tasks, self.num_classes)
-        return components
-
-    def build_model(self):
-        """
-        Builds the appropriate model based on the specified task.
-
-        For the edge prediction task, the model is simply the GNN module because it is an unsupervised task and does not require a prediction head.
-
-        Supervised tasks such as node classification and graph regression require a prediction head, so the model is a sequential module consisting of the GNN module followed by the GNN_head module.
-        """
-
-        if self.task == "edge_pred":  # unsupervised task, does not need pred head
-            return self.gnn
-        elif self.task in ("regression", "classification"):
-            return torch.nn.Sequential(self.gnn, self.gnn_head)
+        if self.mean:
+            self.d_a[m], self.Q_a[m] = torch.symeig(self.m_aa[m] -
+                                                    torch.mean(self.m_aa[m]),
+                                                    eigenvectors=True)
+            self.d_g[m], self.Q_g[m] = torch.symeig(self.m_gg[m] -
+                                                    torch.mean(self.m_gg[m]),
+                                                    eigenvectors=True)
         else:
-            raise ValueError(f"Task {self.task} is not supported.")
-
-    def loss_func(self, inputs, labels, weights):
-        """
-        The loss function executed in the training loop, which is based on the specified task.
-        """
-        if self.task == "edge_pred":
-            node_emb, inputs = self.model(inputs)
-            loss = self.edge_pred_loss(node_emb, inputs)
-        elif self.task == "regression":
-            loss = self.regression_loss(inputs, labels)
-        elif self.task == "classification":
-            loss = self.classification_loss(inputs, labels)
-        return (loss * weights).mean()
-
-    def regression_loss(self, inputs, labels):
-        out = self.model(inputs)
-        reg_loss = self.criterion(out, labels)
-        return reg_loss
+            self.d_a[m], self.Q_a[m] = torch.symeig(self.m_aa[m],
+                                                    eigenvectors=True)
+            self.d_g[m], self.Q_g[m] = torch.symeig(self.m_gg[m],
+                                                    eigenvectors=True)
 
-    def classification_loss(self, inputs, labels):
-        out = self.model(inputs)
-        out = F.softmax(out, dim=2)
-        class_loss = self.criterion(out, labels)
-        return class_loss
+        self.d_a[m].mul_((self.d_a[m] > eps).float())
+        self.d_g[m].mul_((self.d_g[m] > eps).float())
 
-    def _prepare_batch(self, batch):
+    @staticmethod
+    def _get_matrix_form_grad(m: torch.nn.Module):
         """
-        Prepares the batch for the model by converting the GraphData numpy arrays to BatchedGraphData torch tensors and moving them to the device, then transforming the input to the appropriate format for the task.
+        Returns the gradient of the layer in a matrix form
 
-        Parameters
+        Parameter:
         ----------
-        batch: tuple
-            A tuple containing the inputs, labels, and weights for the batch.
+        m: torch.nn.Module
+            the layer for which the gradient must be calculated
 
-        Returns
+        Return:
         -------
-        inputs: BatchGraphData
-            The inputs for the batch, converted to a BatchGraphData object, moved to the device, and transformed to the appropriate format for the task.
-        labels: torch.Tensor
-            The labels for the batch, moved to the device.
-        weights: torch.Tensor
-            The weights for the batch, moved to the device.
-        """
-        inputs, labels, weights = batch
-        inputs = BatchGraphData(inputs[0]).numpy_to_torch(self.device)
-        if self.task == "edge_pred":
-            inputs = negative_edge_sampler(inputs)
-
-        _, labels, weights = super()._prepare_batch(([], labels, weights))
-
-        if (len(labels) != 0) and (len(weights) != 0):
-            labels = labels[0]
-            weights = weights[0]
-
-        return inputs, labels, weights
-
-    def default_generator(
-            self,
-            dataset: Dataset,
-            epochs: int = 1,
-            mode: str = 'fit',
-            deterministic: bool = True,
-            pad_batches: bool = True) -> Iterable[Tuple[List, List, List]]:
-        """
-        This default generator is modified from the default generator in dc.models.tensorgraph.tensor_graph.py to support multitask classification. If the task is classification, the labels y_b are converted to a one-hot encoding and reshaped according to the number of tasks and classes.
-        """
-
-        for epoch in range(epochs):
-            for (X_b, y_b, w_b,
-                 ids_b) in dataset.iterbatches(batch_size=self.batch_size,
-                                               deterministic=deterministic,
-                                               pad_batches=pad_batches):
-                if self.task == 'classification' and y_b is not None:
-                    y_b = to_one_hot(y_b.flatten(), self.num_classes).reshape(
-                        -1, self.num_tasks, self.num_classes)
-                yield ([X_b], [y_b], [w_b])
-
+        torch.tensor
+            a matrix form of the gradient. it should be a [output_dim, input_dim] matrix.
+        """
+        if isinstance(m, torch.nn.Conv2d):
+            p_grad_mat = m.weight.grad.data.view(
+                m.weight.grad.data.size(0), -1)  # n_filters * (in_c * kw * kh)
+        elif isinstance(m, torch.nn.Linear):
+            p_grad_mat = m.weight.grad.data
+        else:
+            raise NotImplementedError(
+                "KFAC optimizer currently support only Linear and Conv2d layers"
+            )
+
+        if m.bias is not None:
+            if isinstance(m.bias.grad.data, torch.Tensor):
+                p_grad_mat = torch.cat(
+                    [p_grad_mat, m.bias.grad.data.view(-1, 1)], 1)
+            else:
+                raise TypeError("bias.grad.data should be a Tensor")
+        return p_grad_mat
 
-def negative_edge_sampler(data: BatchGraphData):
-    """
-    NegativeEdge is a function that adds negative edges to the input graph data. It randomly samples negative edges (edges that do not exist in the original graph) and adds them to the input graph data.
-    The number of negative edges added is equal to half the number of edges in the original graph. This is useful for tasks like edge prediction, where the model needs to learn to differentiate between existing and non-existing edges.
+    def _get_natural_grad(self, m: torch.nn.Module, p_grad_mat: torch.Tensor,
+                          damping: float) -> List[torch.Tensor]:
+        """
+        This function returns the product of inverse of the fisher matrix and the weights gradient.
 
-    Parameters
-    ----------
-    data: dc.feat.graph_data.BatchGraphData
-        The input graph data.
-
-    Returns
-    -------
-    BatchGraphData
-        A new BatchGraphData object with the additional attribute `negative_edge_index`.
-
-    Example
-    -------
-    >>> import numpy as np
-    >>> import torch
-    >>> from deepchem.feat.graph_data import BatchGraphData, GraphData
-    >>> from deepchem.models.torch_models.gnn import negative_edge_sampler
-    >>> num_nodes_list, num_edge_list = [3, 4, 5], [2, 4, 5]
-    >>> num_node_features, num_edge_features = 32, 32
-    >>> edge_index_list = [
-    ...     np.array([[0, 1], [1, 2]]),
-    ...     np.array([[0, 1, 2, 3], [1, 2, 0, 2]]),
-    ...     np.array([[0, 1, 2, 3, 4], [1, 2, 3, 4, 0]]),
-    ... ]
-    >>> graph_list = [
-    ...     GraphData(node_features=np.random.random_sample(
-    ...         (num_nodes_list[i], num_node_features)),
-    ...               edge_index=edge_index_list[i],
-    ...               edge_features=np.random.random_sample(
-    ...                   (num_edge_list[i], num_edge_features)),
-    ...               node_pos_features=None) for i in range(len(num_edge_list))
-    ... ]
-    >>> batched_graph = BatchGraphData(graph_list)
-    >>> batched_graph = batched_graph.numpy_to_torch()
-    >>> neg_sampled = negative_edge_sampler(batched_graph)
-    """
-    import torch
+        Parameters:
+        -----------
+        m: torch.nn.Module
+            Specifies the layer for which the calculation must be done on.
+        p_grad_mat: torch.Tensor
+            the gradients in matrix form isinstance(m.weight.grad.data, torch.Tensor) and i
+        damping: float
+            the damping factor for the calculation
 
-    num_nodes = data.num_nodes
-    num_edges = data.num_edges
+        Return:
+        -------
+        torch.Tensor
+            the product of inverse of the fisher matrix and the weights gradient.
+        """
+        # p_grad_mat is of output_dim * input_dim
+        # inv((ss')) p_grad_mat inv(aa') = [ Q_g (1/R_g) Q_g^T ] @ p_grad_mat @ [Q_a (1/R_a) Q_a^T]
+        v1 = self.Q_g[m].t() @ p_grad_mat @ self.Q_a[m]
+        v2 = v1 / (self.d_g[m].unsqueeze(1) * self.d_a[m].unsqueeze(0) +
+                   damping)
+        a = self.Q_g[m] @ v2 @ self.Q_a[m].t()
+        if m.bias is not None:
+            # we always put gradient w.r.t weight in [0]
+            # and w.r.t bias in [1]
+            if isinstance(m.weight.grad.data, torch.Tensor) and isinstance(
+                    m.bias.grad.data, torch.Tensor):
+                v = [a[:, :-1], a[:, -1:]]
+                v[0] = v[0].view(m.weight.grad.data.size())
+                v[1] = v[1].view(m.bias.grad.data.size())
+            else:
+                raise TypeError(
+                    "weight.grad.data and bias.grad.data should be a Tensor")
+        else:
+            v = [a.view(m.weight.grad.data.size())]
 
-    edge_set = set([
-        str(data.edge_index[0, i].cpu().item()) + "," +
-        str(data.edge_index[1, i].cpu().item())
-        for i in range(data.edge_index.shape[1])
-    ])
-
-    redandunt_sample = torch.randint(0, num_nodes, (2, 5 * num_edges))
-    sampled_ind = []
-    sampled_edge_set = set([])
-    for i in range(5 * num_edges):
-        node1 = redandunt_sample[0, i].cpu().item()
-        node2 = redandunt_sample[1, i].cpu().item()
-        edge_str = str(node1) + "," + str(node2)
-        if edge_str not in edge_set and edge_str not in sampled_edge_set and not node1 == node2:
-            sampled_edge_set.add(edge_str)
-            sampled_ind.append(i)
-        if len(sampled_ind) == num_edges / 2:
-            break
+        return v
 
-    data.negative_edge_index = redandunt_sample[:, sampled_ind]  # type: ignore
+    def _kl_clip_and_update_grad(self, updates: Dict[torch.nn.Module,
+                                                     List[torch.Tensor]],
+                                 lr: float):
+        """
+        Performs clipping on the updates matrix, if the value is large. Then final value is updated in the backwards gradient data
+
+        Parameters:
+        -----------
+        updates: Dict[torch.nn.Module,List[torch.Tensor]]
+            A dicitonary containing the product of gradient and fisher inverse of each layer.
+        lr: float
+            learning rate of the optimizer
+        """
+        # do kl clip
+        vg_sum = 0.0
+        for m in self.modules:
+            v = updates[m]
+            vg_sum += (v[0] * m.weight.grad.data * lr**2).sum().item()
+            if m.bias is not None:
+                vg_sum += (v[1] * m.bias.grad.data * lr**2).sum().item()
+        nu = min(1.0, math.sqrt(self.kl_clip / vg_sum))
+
+        for m in self.modules:
+            v = updates[m]
+            if isinstance(m.weight.grad.data, torch.Tensor):
+                m.weight.grad.data.copy_(v[0])
+                m.weight.grad.data.mul_(nu)
+            else:
+                raise TypeError("weight.grad.data should be a Tensor")
+            if m.bias is not None:
+                if isinstance(m.bias.grad.data, torch.Tensor):
+                    m.bias.grad.data.copy_(v[1])
+                    m.bias.grad.data.mul_(nu)
+                else:
+                    raise TypeError("bias.grad.data should be a Tensor")
+
+    def _step(self, closure: Optional[Callable] = None):
+        """
+        Called in every step of the optimizer, updating the model parameters from the gradient by the KFAC equation.
+        Also, performs weight decay and adds momentum if any.
+
+        Parameters:
+        -----------
+        closure: Callable, optional(default: None)
+            an optional customizable function to be passed which can be used to clear the gradients and other compute loss for every step.
+        """
+        for group in self.param_groups:
+            weight_decay = group['weight_decay']
+            momentum = group['momentum']
+            lr = group['lr']
+
+            for p in group['params']:
+                if p.grad is None:
+                    continue
+                d_p = p.grad.data
+                if weight_decay != 0 and self.steps >= 20 * self.TCov:
+                    d_p.add_(weight_decay, p.data)
+                if momentum != 0:
+                    param_state = self.state[p]
+                    if 'momentum_buffer' not in param_state:
+                        buf = param_state['momentum_buffer'] = torch.zeros_like(
+                            p.data)
+                        buf.mul_(momentum).add_(d_p)
+                    else:
+                        buf = param_state['momentum_buffer']
+                        buf.mul_(momentum).add_(d_p)
+                    d_p = buf
+
+                torch.add(p.data, -lr, d_p, out=p.data)
+
+    def step(self, closure: Optional[Callable] = None):
+        """
+        This is the function that gets called in each step of the optimizer to update the weights and biases of the model.
+
+        Parameters:
+        -----------
+        closure: Callable, optional(default: None)
+            an optional customizable function to be passed which can be used to clear the gradients and other compute loss for every step.
+        """
+        group = self.param_groups[0]
+        lr = group['lr']
+        damping = group['damping']
+        updates = {}
+        for m in self.modules:
+            if self.steps % self.TInv == 0:
+                self._update_inv(m)
+            p_grad_mat = self._get_matrix_form_grad(m)
+            v = self._get_natural_grad(m, p_grad_mat, damping)
+            updates[m] = v
+        self._kl_clip_and_update_grad(updates, lr)
 
-    return data
+        self._step(closure)
+        self.steps += 1
```

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/models/torch_models/grover.py` & `deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/grover.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/models/torch_models/grover_layers.py` & `deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/grover_layers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/models/torch_models/infograph.py` & `deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/infograph.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/models/torch_models/layers.py` & `deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/layers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/models/torch_models/lcnn.py` & `deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/lcnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/models/torch_models/mat.py` & `deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/mat.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/models/torch_models/megnet.py` & `deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/megnet.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/models/torch_models/modular.py` & `deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/modular.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/models/torch_models/mpnn.py` & `deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/mpnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/models/torch_models/normalizing_flows_pytorch.py` & `deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/normalizing_flows_pytorch.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/models/torch_models/pagtn.py` & `deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/pagtn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/models/torch_models/readout.py` & `deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/readout.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/models/torch_models/torch_model.py` & `deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/torch_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/models/wandblogger.py` & `deepchem-2.7.2.dev20230419161626/deepchem/models/wandblogger.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/molnet/__init__.py` & `deepchem-2.7.2.dev20230419161626/deepchem/molnet/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/molnet/check_availability.py` & `deepchem-2.7.2.dev20230419161626/deepchem/molnet/check_availability.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/molnet/defaults.py` & `deepchem-2.7.2.dev20230419161626/deepchem/molnet/defaults.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/molnet/dnasim.py` & `deepchem-2.7.2.dev20230419161626/deepchem/molnet/dnasim.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/bace_datasets.py` & `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/bace_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/bace_features.py` & `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/bace_features.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/bbbc_datasets.py` & `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/bbbc_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/bbbp_datasets.py` & `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/bbbp_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/cell_counting_datasets.py` & `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/cell_counting_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/chembl25_datasets.py` & `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/chembl25_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/chembl_datasets.py` & `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/chembl_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/chembl_tasks.py` & `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/chembl_tasks.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/clearance_datasets.py` & `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/clearance_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/clintox_datasets.py` & `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/clintox_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/delaney_datasets.py` & `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/delaney_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/factors_datasets.py` & `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/factors_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/freesolv_dataset.py` & `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/freesolv_dataset.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/hiv_datasets.py` & `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/hiv_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/hopv_datasets.py` & `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/hopv_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/hppb_datasets.py` & `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/hppb_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/kaggle_datasets.py` & `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/kaggle_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/kaggle_features.py` & `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/kaggle_features.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/kinase_datasets.py` & `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/kinase_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/lipo_datasets.py` & `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/lipo_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/load_dataset_template.py` & `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/load_dataset_template.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/material_datasets/load_Pt_NO_surface_adsorbate_energy.py` & `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/material_datasets/load_Pt_NO_surface_adsorbate_energy.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/material_datasets/load_bandgap.py` & `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/material_datasets/load_bandgap.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/material_datasets/load_mp_formation_energy.py` & `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/material_datasets/load_mp_formation_energy.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/material_datasets/load_mp_metallicity.py` & `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/material_datasets/load_mp_metallicity.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/material_datasets/load_perovskite.py` & `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/material_datasets/load_perovskite.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/molnet_loader.py` & `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/molnet_loader.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/muv_datasets.py` & `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/muv_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/nci_datasets.py` & `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/nci_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/pcba_datasets.py` & `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/pcba_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/pdbbind_datasets.py` & `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/pdbbind_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/ppb_datasets.py` & `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/ppb_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/qm7_datasets.py` & `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/qm7_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/qm8_datasets.py` & `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/qm8_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/qm9_datasets.py` & `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/qm9_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/sampl_datasets.py` & `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/sampl_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/sider_datasets.py` & `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/sider_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/sweetlead_datasets.py` & `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/sweetlead_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/thermosol_datasets.py` & `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/thermosol_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/tox21_datasets.py` & `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/tox21_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/toxcast_datasets.py` & `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/toxcast_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/uspto_datasets.py` & `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/uspto_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/uv_datasets.py` & `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/uv_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/uv_tasks.py` & `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/uv_tasks.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/molnet/load_function/zinc15_datasets.py` & `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/zinc15_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/molnet/preset_hyper_parameters.py` & `deepchem-2.7.2.dev20230419161626/deepchem/molnet/preset_hyper_parameters.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/molnet/run_benchmark.py` & `deepchem-2.7.2.dev20230419161626/deepchem/molnet/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/molnet/run_benchmark_low_data.py` & `deepchem-2.7.2.dev20230419161626/deepchem/molnet/run_benchmark_low_data.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/molnet/run_benchmark_models.py` & `deepchem-2.7.2.dev20230419161626/deepchem/molnet/run_benchmark_models.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/rl/__init__.py` & `deepchem-2.7.2.dev20230419161626/deepchem/rl/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/rl/a2c.py` & `deepchem-2.7.2.dev20230419161626/deepchem/rl/a2c.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/rl/envs/test_tictactoe.py` & `deepchem-2.7.2.dev20230419161626/deepchem/rl/envs/test_tictactoe.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/rl/envs/tictactoe.py` & `deepchem-2.7.2.dev20230419161626/deepchem/rl/envs/tictactoe.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/rl/ppo.py` & `deepchem-2.7.2.dev20230419161626/deepchem/rl/ppo.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/splits/__init__.py` & `deepchem-2.7.2.dev20230419161626/deepchem/splits/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/splits/splitters.py` & `deepchem-2.7.2.dev20230419161626/deepchem/splits/splitters.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/splits/task_splitter.py` & `deepchem-2.7.2.dev20230419161626/deepchem/splits/task_splitter.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/trans/__init__.py` & `deepchem-2.7.2.dev20230419161626/deepchem/trans/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/trans/duplicate.py` & `deepchem-2.7.2.dev20230419161626/deepchem/trans/duplicate.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/trans/transformers.py` & `deepchem-2.7.2.dev20230419161626/deepchem/trans/transformers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/utils/__init__.py` & `deepchem-2.7.2.dev20230419161626/deepchem/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/utils/conformers.py` & `deepchem-2.7.2.dev20230419161626/deepchem/utils/conformers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/utils/coordinate_box_utils.py` & `deepchem-2.7.2.dev20230419161626/deepchem/utils/coordinate_box_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/utils/data_utils.py` & `deepchem-2.7.2.dev20230419161626/deepchem/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/utils/debug_utils.py` & `deepchem-2.7.2.dev20230419161626/deepchem/utils/debug_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/utils/dftutils.py` & `deepchem-2.7.2.dev20230419161626/deepchem/utils/dftutils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/utils/docking_utils.py` & `deepchem-2.7.2.dev20230419161626/deepchem/utils/docking_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/utils/electron_sampler.py` & `deepchem-2.7.2.dev20230419161626/deepchem/utils/electron_sampler.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/utils/evaluate.py` & `deepchem-2.7.2.dev20230419161626/deepchem/utils/evaluate.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/utils/fake_data_generator.py` & `deepchem-2.7.2.dev20230419161626/deepchem/utils/fake_data_generator.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/utils/fragment_utils.py` & `deepchem-2.7.2.dev20230419161626/deepchem/utils/fragment_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/utils/genomics_utils.py` & `deepchem-2.7.2.dev20230419161626/deepchem/utils/genomics_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/utils/geometry_utils.py` & `deepchem-2.7.2.dev20230419161626/deepchem/utils/geometry_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/utils/grover.py` & `deepchem-2.7.2.dev20230419161626/deepchem/utils/grover.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/utils/hash_utils.py` & `deepchem-2.7.2.dev20230419161626/deepchem/utils/hash_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/utils/molecule_feature_utils.py` & `deepchem-2.7.2.dev20230419161626/deepchem/utils/molecule_feature_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/utils/noncovalent_utils.py` & `deepchem-2.7.2.dev20230419161626/deepchem/utils/noncovalent_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/utils/pdbqt_utils.py` & `deepchem-2.7.2.dev20230419161626/deepchem/utils/pdbqt_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/utils/pytorch_utils.py` & `deepchem-2.7.2.dev20230419161626/deepchem/utils/pytorch_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/utils/rdkit_utils.py` & `deepchem-2.7.2.dev20230419161626/deepchem/utils/rdkit_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/utils/save.py` & `deepchem-2.7.2.dev20230419161626/deepchem/utils/save.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/utils/sequence_utils.py` & `deepchem-2.7.2.dev20230419161626/deepchem/utils/sequence_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/utils/test/test_coordinate_box_utils.py` & `deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_coordinate_box_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/utils/test/test_data_utils.py` & `deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/utils/test/test_dftutils.py` & `deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_dftutils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/utils/test/test_docking_utils.py` & `deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_docking_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/utils/test/test_electron_sampler.py` & `deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_electron_sampler.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/utils/test/test_evaluate.py` & `deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_evaluate.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/utils/test/test_fake_data_generator.py` & `deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_fake_data_generator.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/utils/test/test_fragment_utils.py` & `deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_fragment_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/utils/test/test_generator_evaluator.py` & `deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_generator_evaluator.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/utils/test/test_genomics_utils.py` & `deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_genomics_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/utils/test/test_geometry_utils.py` & `deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_geometry_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/utils/test/test_grover.py` & `deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_grover.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/utils/test/test_hash_utils.py` & `deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_hash_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/utils/test/test_molecule_feature_utils.py` & `deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_molecule_feature_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/utils/test/test_noncovalent_utils.py` & `deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_noncovalent_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/utils/test/test_pdbqt_utils.py` & `deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_pdbqt_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/utils/test/test_rdkit_utils.py` & `deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_rdkit_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/utils/test/test_sequence_utils.py` & `deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_sequence_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/utils/test/test_voxel_utils.py` & `deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_voxel_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/utils/typing.py` & `deepchem-2.7.2.dev20230419161626/deepchem/utils/typing.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/utils/vina_utils.py` & `deepchem-2.7.2.dev20230419161626/deepchem/utils/vina_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem/utils/voxel_utils.py` & `deepchem-2.7.2.dev20230419161626/deepchem/utils/voxel_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem.egg-info/PKG-INFO` & `deepchem-2.7.2.dev20230419161626/deepchem.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepchem
-Version: 2.7.2.dev20230419152231
+Version: 2.7.2.dev20230419161626
 Summary: Deep learning models for drug discovery,         quantum chemistry, and the life sciences.
 Home-page: https://github.com/deepchem/deepchem
 Maintainer: DeepChem contributors
 License: MIT
 Project-URL: Documentation, https://deepchem.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/deepchem/deepchem
 Keywords: deepchem,chemistry,biology,materials-science,life-science,drug-discovery
```

### Comparing `deepchem-2.7.2.dev20230419152231/deepchem.egg-info/SOURCES.txt` & `deepchem-2.7.2.dev20230419161626/deepchem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/setup.cfg` & `deepchem-2.7.2.dev20230419161626/setup.cfg`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419152231/setup.py` & `deepchem-2.7.2.dev20230419161626/setup.py`

 * *Files identical despite different names*

