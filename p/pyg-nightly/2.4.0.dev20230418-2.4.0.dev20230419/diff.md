# Comparing `tmp/pyg-nightly-2.4.0.dev20230418.tar.gz` & `tmp/pyg-nightly-2.4.0.dev20230419.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyg-nightly-2.4.0.dev20230418.tar", last modified: Tue Apr 18 06:05:52 2023, max compression
+gzip compressed data, was "pyg-nightly-2.4.0.dev20230419.tar", last modified: Wed Apr 19 06:06:11 2023, max compression
```

## Comparing `pyg-nightly-2.4.0.dev20230418.tar` & `pyg-nightly-2.4.0.dev20230419.tar`

### file list

```diff
@@ -1,545 +1,545 @@
--rw-r--r--   0        0        0    60619 2023-04-18 06:05:39.194321 pyg-nightly-2.4.0.dev20230418/README.md
--rw-r--r--   0        0        0     4024 2023-04-18 06:05:39.562328 pyg-nightly-2.4.0.dev20230418/pyproject.toml
--rw-r--r--   0        0        0     1055 2023-04-18 06:05:39.558328 pyg-nightly-2.4.0.dev20230418/torch_geometric/__init__.py
--rw-r--r--   0        0        0     3392 2023-04-18 06:05:39.230321 pyg-nightly-2.4.0.dev20230418/torch_geometric/compile.py
--rw-r--r--   0        0        0      352 2023-04-18 06:05:39.230321 pyg-nightly-2.4.0.dev20230418/torch_geometric/contrib/__init__.py
--rw-r--r--   0        0        0       23 2023-04-18 06:05:39.230321 pyg-nightly-2.4.0.dev20230418/torch_geometric/contrib/datasets/__init__.py
--rw-r--r--   0        0        0      163 2023-04-18 06:05:39.230321 pyg-nightly-2.4.0.dev20230418/torch_geometric/contrib/explain/__init__.py
--rw-r--r--   0        0        0    20540 2023-04-18 06:05:39.230321 pyg-nightly-2.4.0.dev20230418/torch_geometric/contrib/explain/graphmask_explainer.py
--rw-r--r--   0        0        0    16627 2023-04-18 06:05:39.230321 pyg-nightly-2.4.0.dev20230418/torch_geometric/contrib/explain/pgm_explainer.py
--rw-r--r--   0        0        0       72 2023-04-18 06:05:39.230321 pyg-nightly-2.4.0.dev20230418/torch_geometric/contrib/nn/__init__.py
--rw-r--r--   0        0        0       23 2023-04-18 06:05:39.230321 pyg-nightly-2.4.0.dev20230418/torch_geometric/contrib/nn/conv/__init__.py
--rw-r--r--   0        0        0      113 2023-04-18 06:05:39.230321 pyg-nightly-2.4.0.dev20230418/torch_geometric/contrib/nn/models/__init__.py
--rw-r--r--   0        0        0    33261 2023-04-18 06:05:39.230321 pyg-nightly-2.4.0.dev20230418/torch_geometric/contrib/nn/models/rbcd_attack.py
--rw-r--r--   0        0        0       23 2023-04-18 06:05:39.230321 pyg-nightly-2.4.0.dev20230418/torch_geometric/contrib/transforms/__init__.py
--rw-r--r--   0        0        0     3383 2023-04-18 06:05:39.230321 pyg-nightly-2.4.0.dev20230418/torch_geometric/data/__init__.py
--rw-r--r--   0        0        0     7436 2023-04-18 06:05:39.230321 pyg-nightly-2.4.0.dev20230418/torch_geometric/data/batch.py
--rw-r--r--   0        0        0    10432 2023-04-18 06:05:39.230321 pyg-nightly-2.4.0.dev20230418/torch_geometric/data/collate.py
--rw-r--r--   0        0        0    37570 2023-04-18 06:05:39.230321 pyg-nightly-2.4.0.dev20230418/torch_geometric/data/data.py
--rw-r--r--   0        0        0     2922 2023-04-18 06:05:39.230321 pyg-nightly-2.4.0.dev20230418/torch_geometric/data/datapipes.py
--rw-r--r--   0        0        0    14850 2023-04-18 06:05:39.230321 pyg-nightly-2.4.0.dev20230418/torch_geometric/data/dataset.py
--rw-r--r--   0        0        0     1359 2023-04-18 06:05:39.230321 pyg-nightly-2.4.0.dev20230418/torch_geometric/data/download.py
--rw-r--r--   0        0        0     2252 2023-04-18 06:05:39.230321 pyg-nightly-2.4.0.dev20230418/torch_geometric/data/extract.py
--rw-r--r--   0        0        0    21075 2023-04-18 06:05:39.230321 pyg-nightly-2.4.0.dev20230418/torch_geometric/data/feature_store.py
--rw-r--r--   0        0        0    13495 2023-04-18 06:05:39.230321 pyg-nightly-2.4.0.dev20230418/torch_geometric/data/graph_store.py
--rw-r--r--   0        0        0    42291 2023-04-18 06:05:39.230321 pyg-nightly-2.4.0.dev20230418/torch_geometric/data/hetero_data.py
--rw-r--r--   0        0        0     7091 2023-04-18 06:05:39.230321 pyg-nightly-2.4.0.dev20230418/torch_geometric/data/in_memory_dataset.py
--rw-r--r--   0        0        0      178 2023-04-18 06:05:39.230321 pyg-nightly-2.4.0.dev20230418/torch_geometric/data/lightning/__init__.py
--rw-r--r--   0        0        0    28490 2023-04-18 06:05:39.230321 pyg-nightly-2.4.0.dev20230418/torch_geometric/data/lightning/datamodule.py
--rw-r--r--   0        0        0      338 2023-04-18 06:05:39.230321 pyg-nightly-2.4.0.dev20230418/torch_geometric/data/makedirs.py
--rw-r--r--   0        0        0     3962 2023-04-18 06:05:39.230321 pyg-nightly-2.4.0.dev20230418/torch_geometric/data/remote_backend_utils.py
--rw-r--r--   0        0        0     4321 2023-04-18 06:05:39.230321 pyg-nightly-2.4.0.dev20230418/torch_geometric/data/separate.py
--rw-r--r--   0        0        0    24947 2023-04-18 06:05:39.230321 pyg-nightly-2.4.0.dev20230418/torch_geometric/data/storage.py
--rw-r--r--   0        0        0     2579 2023-04-18 06:05:39.230321 pyg-nightly-2.4.0.dev20230418/torch_geometric/data/summary.py
--rw-r--r--   0        0        0     9354 2023-04-18 06:05:39.230321 pyg-nightly-2.4.0.dev20230418/torch_geometric/data/temporal.py
--rw-r--r--   0        0        0     1046 2023-04-18 06:05:39.230321 pyg-nightly-2.4.0.dev20230418/torch_geometric/data/view.py
--rw-r--r--   0        0        0     4870 2023-04-18 06:05:39.230321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/__init__.py
--rw-r--r--   0        0        0     4220 2023-04-18 06:05:39.230321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/actor.py
--rw-r--r--   0        0        0     5584 2023-04-18 06:05:39.230321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/airfrans.py
--rw-r--r--   0        0        0     3711 2023-04-18 06:05:39.230321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/airports.py
--rw-r--r--   0        0        0     3017 2023-04-18 06:05:39.230321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/amazon.py
--rw-r--r--   0        0        0     4099 2023-04-18 06:05:39.230321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/amazon_products.py
--rw-r--r--   0        0        0     4942 2023-04-18 06:05:39.230321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/aminer.py
--rw-r--r--   0        0        0     5266 2023-04-18 06:05:39.230321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/aqsol.py
--rw-r--r--   0        0        0     5735 2023-04-18 06:05:39.230321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/attributed_graph_dataset.py
--rw-r--r--   0        0        0     4063 2023-04-18 06:05:39.230321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/ba2motif_dataset.py
--rw-r--r--   0        0        0     3518 2023-04-18 06:05:39.230321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/ba_multi_shapes.py
--rw-r--r--   0        0        0     3824 2023-04-18 06:05:39.230321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/ba_shapes.py
--rw-r--r--   0        0        0     4137 2023-04-18 06:05:39.230321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/bitcoin_otc.py
--rw-r--r--   0        0        0     3942 2023-04-18 06:05:39.230321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/citation_full.py
--rw-r--r--   0        0        0     2976 2023-04-18 06:05:39.230321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/coauthor.py
--rw-r--r--   0        0        0     4564 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/coma.py
--rw-r--r--   0        0        0     4538 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/dblp.py
--rw-r--r--   0        0        0     5608 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/dbp15k.py
--rw-r--r--   0        0        0     2308 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/deezer_europe.py
--rw-r--r--   0        0        0     3862 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/dgraph.py
--rw-r--r--   0        0        0     5865 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/dynamic_faust.py
--rw-r--r--   0        0        0     4498 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/elliptic.py
--rw-r--r--   0        0        0     2990 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/elliptic_temporal.py
--rw-r--r--   0        0        0     2631 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/email_eu_core.py
--rw-r--r--   0        0        0     7009 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/entities.py
--rw-r--r--   0        0        0     5817 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/explainer_dataset.py
--rw-r--r--   0        0        0     2228 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/facebook.py
--rw-r--r--   0        0        0    10215 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/fake.py
--rw-r--r--   0        0        0     3924 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/faust.py
--rw-r--r--   0        0        0     4099 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/flickr.py
--rw-r--r--   0        0        0     3815 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/freebase.py
--rw-r--r--   0        0        0     3416 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/gdelt.py
--rw-r--r--   0        0        0     9261 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/ged_dataset.py
--rw-r--r--   0        0        0     2626 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/gemsec.py
--rw-r--r--   0        0        0     3954 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/geometry.py
--rw-r--r--   0        0        0     2484 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/github.py
--rw-r--r--   0        0        0     6762 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/gnn_benchmark_dataset.py
--rw-r--r--   0        0        0      221 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/graph_generator/__init__.py
--rw-r--r--   0        0        0      965 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/graph_generator/ba_graph.py
--rw-r--r--   0        0        0      949 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/graph_generator/base.py
--rw-r--r--   0        0        0      918 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/graph_generator/er_graph.py
--rw-r--r--   0        0        0     1159 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/graph_generator/grid_graph.py
--rw-r--r--   0        0        0     4043 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/heterophilous_graph_dataset.py
--rw-r--r--   0        0        0     8467 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/hgb_dataset.py
--rw-r--r--   0        0        0    11053 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/hydro_net.py
--rw-r--r--   0        0        0     4447 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/icews.py
--rw-r--r--   0        0        0     4000 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/imdb.py
--rw-r--r--   0        0        0     7169 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/infection_dataset.py
--rw-r--r--   0        0        0     3439 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/jodie.py
--rw-r--r--   0        0        0     3444 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/karate.py
--rw-r--r--   0        0        0     4349 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/last_fm.py
--rw-r--r--   0        0        0     2283 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/lastfm_asia.py
--rw-r--r--   0        0        0     6582 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/linkx_dataset.py
--rw-r--r--   0        0        0    11559 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/lrgb.py
--rw-r--r--   0        0        0     5044 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/malnet_tiny.py
--rw-r--r--   0        0        0    16482 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/md17.py
--rw-r--r--   0        0        0     3770 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/mixhop_synthetic_dataset.py
--rw-r--r--   0        0        0     3136 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/mnist_superpixels.py
--rw-r--r--   0        0        0     5251 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/modelnet.py
--rw-r--r--   0        0        0     6593 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/molecule_net.py
--rw-r--r--   0        0        0      227 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/motif_generator/__init__.py
--rw-r--r--   0        0        0      910 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/motif_generator/base.py
--rw-r--r--   0        0        0     1203 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/motif_generator/custom.py
--rw-r--r--   0        0        0      984 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/motif_generator/cycle.py
--rw-r--r--   0        0        0      801 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/motif_generator/house.py
--rw-r--r--   0        0        0     3787 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/movie_lens.py
--rw-r--r--   0        0        0     2889 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/nell.py
--rw-r--r--   0        0        0     7190 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/ogb_mag.py
--rw-r--r--   0        0        0     3415 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/omdb.py
--rw-r--r--   0        0        0     3964 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/particle.py
--rw-r--r--   0        0        0    10699 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/pascal.py
--rw-r--r--   0        0        0     4602 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/pascal_pf.py
--rw-r--r--   0        0        0     5716 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/pcpnet_dataset.py
--rw-r--r--   0        0        0     7016 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/planetoid.py
--rw-r--r--   0        0        0     2842 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/polblogs.py
--rw-r--r--   0        0        0     4866 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/ppi.py
--rw-r--r--   0        0        0     3182 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/qm7.py
--rw-r--r--   0        0        0    16813 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/qm9.py
--rw-r--r--   0        0        0     2941 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/reddit.py
--rw-r--r--   0        0        0     4439 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/reddit2.py
--rw-r--r--   0        0        0     4345 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/rel_link_pred_dataset.py
--rw-r--r--   0        0        0     4173 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/s3dis.py
--rw-r--r--   0        0        0     8140 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/sbm_dataset.py
--rw-r--r--   0        0        0     8088 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/shapenet.py
--rw-r--r--   0        0        0     6150 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/shrec2016.py
--rw-r--r--   0        0        0     9283 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/snap_dataset.py
--rw-r--r--   0        0        0     3031 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/suite_sparse.py
--rw-r--r--   0        0        0     3959 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/taobao.py
--rw-r--r--   0        0        0     4451 2023-04-18 06:05:39.234321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/tosca.py
--rw-r--r--   0        0        0     7174 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/tu_dataset.py
--rw-r--r--   0        0        0     3464 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/twitch.py
--rw-r--r--   0        0        0     6929 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/upfd.py
--rw-r--r--   0        0        0      156 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/utils/__init__.py
--rw-r--r--   0        0        0     1655 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/utils/cheatsheet.py
--rw-r--r--   0        0        0     4615 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/webkb.py
--rw-r--r--   0        0        0     3674 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/wikics.py
--rw-r--r--   0        0        0     6083 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/wikipedia_network.py
--rw-r--r--   0        0        0     6322 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/willow_object_class.py
--rw-r--r--   0        0        0     7857 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/word_net.py
--rw-r--r--   0        0        0     4116 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/yelp.py
--rw-r--r--   0        0        0     6171 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/zinc.py
--rw-r--r--   0        0        0     1197 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/debug.py
--rw-r--r--   0        0        0      748 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/deprecation.py
--rw-r--r--   0        0        0     2466 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/experimental.py
--rw-r--r--   0        0        0      359 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/explain/__init__.py
--rw-r--r--   0        0        0      418 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/explain/algorithm/__init__.py
--rw-r--r--   0        0        0     4491 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/explain/algorithm/attention_explainer.py
--rw-r--r--   0        0        0     6899 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/explain/algorithm/base.py
--rw-r--r--   0        0        0    12489 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/explain/algorithm/captum.py
--rw-r--r--   0        0        0     6540 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/explain/algorithm/captum_explainer.py
--rw-r--r--   0        0        0     2867 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/explain/algorithm/dummy_explainer.py
--rw-r--r--   0        0        0    11149 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/explain/algorithm/gnn_explainer.py
--rw-r--r--   0        0        0    10370 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/explain/algorithm/pg_explainer.py
--rw-r--r--   0        0        0     2308 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/explain/algorithm/utils.py
--rw-r--r--   0        0        0     7834 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/explain/config.py
--rw-r--r--   0        0        0    10375 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/explain/explainer.py
--rw-r--r--   0        0        0    12882 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/explain/explanation.py
--rw-r--r--   0        0        0      301 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/explain/metric/__init__.py
--rw-r--r--   0        0        0     1888 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/explain/metric/basic.py
--rw-r--r--   0        0        0     3063 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/explain/metric/faithfulness.py
--rw-r--r--   0        0        0     6157 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/explain/metric/fidelity.py
--rw-r--r--   0        0        0     2045 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/__init__.py
--rw-r--r--   0        0        0      510 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/benchmark.py
--rw-r--r--   0        0        0     2371 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/checkpoint.py
--rw-r--r--   0        0        0      738 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/cmd_args.py
--rw-r--r--   0        0        0    17221 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/config.py
--rw-r--r--   0        0        0    14575 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/config_store.py
--rw-r--r--   0        0        0      389 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/contrib/__init__.py
--rw-r--r--   0        0        0      221 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/contrib/act/__init__.py
--rw-r--r--   0        0        0      221 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/contrib/config/__init__.py
--rw-r--r--   0        0        0      221 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/contrib/encoder/__init__.py
--rw-r--r--   0        0        0      221 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/contrib/head/__init__.py
--rw-r--r--   0        0        0      221 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/contrib/layer/__init__.py
--rw-r--r--   0        0        0     8304 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/contrib/layer/generalconv.py
--rw-r--r--   0        0        0      221 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/contrib/loader/__init__.py
--rw-r--r--   0        0        0      221 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/contrib/loss/__init__.py
--rw-r--r--   0        0        0      221 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/contrib/network/__init__.py
--rw-r--r--   0        0        0      221 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/contrib/optimizer/__init__.py
--rw-r--r--   0        0        0      221 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/contrib/pooling/__init__.py
--rw-r--r--   0        0        0      221 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/contrib/stage/__init__.py
--rw-r--r--   0        0        0      221 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/contrib/train/__init__.py
--rw-r--r--   0        0        0      221 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/contrib/transform/__init__.py
--rw-r--r--   0        0        0      375 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/imports.py
--rw-r--r--   0        0        0      490 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/init.py
--rw-r--r--   0        0        0    11763 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/loader.py
--rw-r--r--   0        0        0    11337 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/logger.py
--rw-r--r--   0        0        0     1474 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/loss.py
--rw-r--r--   0        0        0     2844 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/model_builder.py
--rw-r--r--   0        0        0     1121 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/models/__init__.py
--rw-r--r--   0        0        0      822 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/models/act.py
--rw-r--r--   0        0        0     2546 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/models/encoder.py
--rw-r--r--   0        0        0     5133 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/models/gnn.py
--rw-r--r--   0        0        0     4323 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/models/head.py
--rw-r--r--   0        0        0    12486 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/models/layer.py
--rw-r--r--   0        0        0      288 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/models/pooling.py
--rw-r--r--   0        0        0     1391 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/models/transform.py
--rw-r--r--   0        0        0     2544 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/optim.py
--rw-r--r--   0        0        0     3944 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/register.py
--rw-r--r--   0        0        0     1887 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/train.py
--rw-r--r--   0        0        0        0 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/utils/LICENSE
--rw-r--r--   0        0        0      641 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/utils/__init__.py
--rw-r--r--   0        0        0     9513 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/utils/agg_runs.py
--rw-r--r--   0        0        0     3056 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/utils/comp_budget.py
--rw-r--r--   0        0        0     1352 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/utils/device.py
--rw-r--r--   0        0        0      690 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/utils/epoch.py
--rw-r--r--   0        0        0     2050 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/utils/io.py
--rw-r--r--   0        0        0      606 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/utils/plot.py
--rw-r--r--   0        0        0      198 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/utils/tools.py
--rw-r--r--   0        0        0      830 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/home.py
--rw-r--r--   0        0        0      528 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/io/__init__.py
--rw-r--r--   0        0        0      943 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/io/npz.py
--rw-r--r--   0        0        0      957 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/io/obj.py
--rw-r--r--   0        0        0     2586 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/io/off.py
--rw-r--r--   0        0        0     4211 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/io/planetoid.py
--rw-r--r--   0        0        0      476 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/io/ply.py
--rw-r--r--   0        0        0     1136 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/io/sdf.py
--rw-r--r--   0        0        0     4733 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/io/tu.py
--rw-r--r--   0        0        0      562 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/io/txt_array.py
--rw-r--r--   0        0        0      768 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/lazy_loader.py
--rw-r--r--   0        0        0     1616 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/loader/__init__.py
--rw-r--r--   0        0        0     1433 2023-04-18 06:05:39.238321 pyg-nightly-2.4.0.dev20230418/torch_geometric/loader/base.py
--rw-r--r--   0        0        0     6539 2023-04-18 06:05:39.242322 pyg-nightly-2.4.0.dev20230418/torch_geometric/loader/cluster.py
--rw-r--r--   0        0        0     1449 2023-04-18 06:05:39.242322 pyg-nightly-2.4.0.dev20230418/torch_geometric/loader/data_list_loader.py
--rw-r--r--   0        0        0     3222 2023-04-18 06:05:39.242322 pyg-nightly-2.4.0.dev20230418/torch_geometric/loader/dataloader.py
--rw-r--r--   0        0        0     1683 2023-04-18 06:05:39.242322 pyg-nightly-2.4.0.dev20230418/torch_geometric/loader/dense_data_loader.py
--rw-r--r--   0        0        0     4285 2023-04-18 06:05:39.242322 pyg-nightly-2.4.0.dev20230418/torch_geometric/loader/dynamic_batch_sampler.py
--rw-r--r--   0        0        0     8448 2023-04-18 06:05:39.242322 pyg-nightly-2.4.0.dev20230418/torch_geometric/loader/graph_saint.py
--rw-r--r--   0        0        0     5715 2023-04-18 06:05:39.242322 pyg-nightly-2.4.0.dev20230418/torch_geometric/loader/hgt_loader.py
--rw-r--r--   0        0        0     3754 2023-04-18 06:05:39.242322 pyg-nightly-2.4.0.dev20230418/torch_geometric/loader/imbalanced_sampler.py
--rw-r--r--   0        0        0    13521 2023-04-18 06:05:39.242322 pyg-nightly-2.4.0.dev20230418/torch_geometric/loader/link_loader.py
--rw-r--r--   0        0        0    11594 2023-04-18 06:05:39.242322 pyg-nightly-2.4.0.dev20230418/torch_geometric/loader/link_neighbor_loader.py
--rw-r--r--   0        0        0     6282 2023-04-18 06:05:39.242322 pyg-nightly-2.4.0.dev20230418/torch_geometric/loader/mixin.py
--rw-r--r--   0        0        0    10463 2023-04-18 06:05:39.242322 pyg-nightly-2.4.0.dev20230418/torch_geometric/loader/neighbor_loader.py
--rw-r--r--   0        0        0     8513 2023-04-18 06:05:39.242322 pyg-nightly-2.4.0.dev20230418/torch_geometric/loader/neighbor_sampler.py
--rw-r--r--   0        0        0     8938 2023-04-18 06:05:39.242322 pyg-nightly-2.4.0.dev20230418/torch_geometric/loader/node_loader.py
--rw-r--r--   0        0        0     2196 2023-04-18 06:05:39.242322 pyg-nightly-2.4.0.dev20230418/torch_geometric/loader/random_node_loader.py
--rw-r--r--   0        0        0     4173 2023-04-18 06:05:39.242322 pyg-nightly-2.4.0.dev20230418/torch_geometric/loader/shadow.py
--rw-r--r--   0        0        0     1319 2023-04-18 06:05:39.242322 pyg-nightly-2.4.0.dev20230418/torch_geometric/loader/temporal_dataloader.py
--rw-r--r--   0        0        0    11532 2023-04-18 06:05:39.242322 pyg-nightly-2.4.0.dev20230418/torch_geometric/loader/utils.py
--rw-r--r--   0        0        0     3034 2023-04-18 06:05:39.242322 pyg-nightly-2.4.0.dev20230418/torch_geometric/loader/zip_loader.py
--rw-r--r--   0        0        0      832 2023-04-18 06:05:39.242322 pyg-nightly-2.4.0.dev20230418/torch_geometric/logging.py
--rw-r--r--   0        0        0      911 2023-04-18 06:05:39.242322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/__init__.py
--rw-r--r--   0        0        0     1397 2023-04-18 06:05:39.242322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/aggr/__init__.py
--rw-r--r--   0        0        0     2395 2023-04-18 06:05:39.242322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/aggr/attention.py
--rw-r--r--   0        0        0     7105 2023-04-18 06:05:39.242322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/aggr/base.py
--rw-r--r--   0        0        0    10858 2023-04-18 06:05:39.242322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/aggr/basic.py
--rw-r--r--   0        0        0     2064 2023-04-18 06:05:39.242322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/aggr/deep_sets.py
--rw-r--r--   0        0        0     6881 2023-04-18 06:05:39.242322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/aggr/equilibrium.py
--rw-r--r--   0        0        0    12074 2023-04-18 06:05:39.242322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/aggr/fused.py
--rw-r--r--   0        0        0     3062 2023-04-18 06:05:39.242322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/aggr/gmt.py
--rw-r--r--   0        0        0     1464 2023-04-18 06:05:39.242322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/aggr/gru.py
--rw-r--r--   0        0        0     1484 2023-04-18 06:05:39.242322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/aggr/lstm.py
--rw-r--r--   0        0        0     1995 2023-04-18 06:05:39.242322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/aggr/mlp.py
--rw-r--r--   0        0        0     8163 2023-04-18 06:05:39.242322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/aggr/multi.py
--rw-r--r--   0        0        0     5869 2023-04-18 06:05:39.242322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/aggr/quantile.py
--rw-r--r--   0        0        0     4642 2023-04-18 06:05:39.242322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/aggr/scaler.py
--rw-r--r--   0        0        0     2517 2023-04-18 06:05:39.242322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/aggr/set2set.py
--rw-r--r--   0        0        0     3439 2023-04-18 06:05:39.242322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/aggr/set_transformer.py
--rw-r--r--   0        0        0     1772 2023-04-18 06:05:39.242322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/aggr/sort.py
--rw-r--r--   0        0        0     8322 2023-04-18 06:05:39.242322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/aggr/utils.py
--rw-r--r--   0        0        0     3360 2023-04-18 06:05:39.242322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/__init__.py
--rw-r--r--   0        0        0     3088 2023-04-18 06:05:39.242322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/agnn_conv.py
--rw-r--r--   0        0        0     4388 2023-04-18 06:05:39.242322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/antisymmetric_conv.py
--rw-r--r--   0        0        0     6010 2023-04-18 06:05:39.242322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/appnp.py
--rw-r--r--   0        0        0     6637 2023-04-18 06:05:39.242322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/arma_conv.py
--rw-r--r--   0        0        0     4036 2023-04-18 06:05:39.242322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/cg_conv.py
--rw-r--r--   0        0        0     6444 2023-04-18 06:05:39.242322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/cheb_conv.py
--rw-r--r--   0        0        0     5303 2023-04-18 06:05:39.242322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/cluster_gcn_conv.py
--rw-r--r--   0        0        0      251 2023-04-18 06:05:39.242322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/cugraph/__init__.py
--rw-r--r--   0        0        0     8195 2023-04-18 06:05:39.242322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/cugraph/base.py
--rw-r--r--   0        0        0     2849 2023-04-18 06:05:39.242322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/cugraph/gat_conv.py
--rw-r--r--   0        0        0     4218 2023-04-18 06:05:39.242322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/cugraph/rgcn_conv.py
--rw-r--r--   0        0        0     2802 2023-04-18 06:05:39.242322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/cugraph/sage_conv.py
--rw-r--r--   0        0        0    12105 2023-04-18 06:05:39.242322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/dna_conv.py
--rw-r--r--   0        0        0     5550 2023-04-18 06:05:39.242322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/edge_conv.py
--rw-r--r--   0        0        0    10482 2023-04-18 06:05:39.242322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/eg_conv.py
--rw-r--r--   0        0        0     7927 2023-04-18 06:05:39.242322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/fa_conv.py
--rw-r--r--   0        0        0     4453 2023-04-18 06:05:39.242322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/feast_conv.py
--rw-r--r--   0        0        0     6332 2023-04-18 06:05:39.242322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/film_conv.py
--rw-r--r--   0        0        0     4242 2023-04-18 06:05:39.242322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/fused_gat_conv.py
--rw-r--r--   0        0        0    13610 2023-04-18 06:05:39.242322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/gat_conv.py
--rw-r--r--   0        0        0     3582 2023-04-18 06:05:39.242322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/gated_graph_conv.py
--rw-r--r--   0        0        0    12423 2023-04-18 06:05:39.242322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/gatv2_conv.py
--rw-r--r--   0        0        0     7022 2023-04-18 06:05:39.242322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/gcn2_conv.py
--rw-r--r--   0        0        0     9333 2023-04-18 06:05:39.242322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/gcn_conv.py
--rw-r--r--   0        0        0     9992 2023-04-18 06:05:39.242322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/gen_conv.py
--rw-r--r--   0        0        0     7512 2023-04-18 06:05:39.242322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/general_conv.py
--rw-r--r--   0        0        0     7444 2023-04-18 06:05:39.242322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/gin_conv.py
--rw-r--r--   0        0        0     8320 2023-04-18 06:05:39.242322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/gmm_conv.py
--rw-r--r--   0        0        0     5764 2023-04-18 06:05:39.242322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/gps_conv.py
--rw-r--r--   0        0        0     3547 2023-04-18 06:05:39.242322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/graph_conv.py
--rw-r--r--   0        0        0     5023 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/gravnet_conv.py
--rw-r--r--   0        0        0     7354 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/han_conv.py
--rw-r--r--   0        0        0     6063 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/heat_conv.py
--rw-r--r--   0        0        0     6470 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/hetero_conv.py
--rw-r--r--   0        0        0     9001 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/hgt_conv.py
--rw-r--r--   0        0        0     7580 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/hypergraph_conv.py
--rw-r--r--   0        0        0     3523 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/le_conv.py
--rw-r--r--   0        0        0     2418 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/lg_conv.py
--rw-r--r--   0        0        0    11524 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/message_passing.jinja
--rw-r--r--   0        0        0    40230 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/message_passing.py
--rw-r--r--   0        0        0     4321 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/mf_conv.py
--rw-r--r--   0        0        0     4743 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/nn_conv.py
--rw-r--r--   0        0        0     4928 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/pan_conv.py
--rw-r--r--   0        0        0     4916 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/pdn_conv.py
--rw-r--r--   0        0        0     8242 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/pna_conv.py
--rw-r--r--   0        0        0     4522 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/point_conv.py
--rw-r--r--   0        0        0     3288 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/point_gnn_conv.py
--rw-r--r--   0        0        0     5889 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/point_transformer_conv.py
--rw-r--r--   0        0        0     5422 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/ppf_conv.py
--rw-r--r--   0        0        0     4180 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/res_gated_graph_conv.py
--rw-r--r--   0        0        0    22785 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/rgat_conv.py
--rw-r--r--   0        0        0    14623 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/rgcn_conv.py
--rw-r--r--   0        0        0     5813 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/sage_conv.py
--rw-r--r--   0        0        0     4597 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/sg_conv.py
--rw-r--r--   0        0        0     6283 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/signed_conv.py
--rw-r--r--   0        0        0     3142 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/simple_conv.py
--rw-r--r--   0        0        0     6330 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/spline_conv.py
--rw-r--r--   0        0        0     5185 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/ssg_conv.py
--rw-r--r--   0        0        0    11980 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/supergat_conv.py
--rw-r--r--   0        0        0     4215 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/tag_conv.py
--rw-r--r--   0        0        0     9425 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/transformer_conv.py
--rw-r--r--   0        0        0      823 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/utils/__init__.py
--rw-r--r--   0        0        0     2692 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/utils/cheatsheet.py
--rw-r--r--   0        0        0      186 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/utils/helpers.py
--rw-r--r--   0        0        0     3267 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/utils/inspector.py
--rw-r--r--   0        0        0      679 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/utils/jit.py
--rw-r--r--   0        0        0     3859 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/utils/typing.py
--rw-r--r--   0        0        0     3103 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/wl_conv.py
--rw-r--r--   0        0        0     2349 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/wl_conv_continuous.py
--rw-r--r--   0        0        0     5955 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/x_conv.py
--rw-r--r--   0        0        0     3960 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/data_parallel.py
--rw-r--r--   0        0        0      712 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/dense/__init__.py
--rw-r--r--   0        0        0     4228 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/dense/dense_gat_conv.py
--rw-r--r--   0        0        0     2989 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/dense/dense_gcn_conv.py
--rw-r--r--   0        0        0     2357 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/dense/dense_gin_conv.py
--rw-r--r--   0        0        0     2737 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/dense/dense_graph_conv.py
--rw-r--r--   0        0        0     2658 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/dense/dense_sage_conv.py
--rw-r--r--   0        0        0     3050 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/dense/diff_pool.py
--rw-r--r--   0        0        0     5671 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/dense/dmon_pool.py
--rw-r--r--   0        0        0    15564 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/dense/linear.py
--rw-r--r--   0        0        0     4111 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/dense/mincut_pool.py
--rw-r--r--   0        0        0     3125 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/encoding.py
--rw-r--r--   0        0        0       92 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/functional/__init__.py
--rw-r--r--   0        0        0     1549 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/functional/bro.py
--rw-r--r--   0        0        0      863 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/functional/gini.py
--rw-r--r--   0        0        0    15559 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/fx.py
--rw-r--r--   0        0        0     1088 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/glob.py
--rw-r--r--   0        0        0     2457 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/inits.py
--rw-r--r--   0        0        0      241 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/kge/__init__.py
--rw-r--r--   0        0        0     5739 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/kge/base.py
--rw-r--r--   0        0        0     3234 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/kge/complex.py
--rw-r--r--   0        0        0     2462 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/kge/distmult.py
--rw-r--r--   0        0        0      771 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/kge/loader.py
--rw-r--r--   0        0        0     3208 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/kge/rotate.py
--rw-r--r--   0        0        0     3088 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/kge/transe.py
--rw-r--r--   0        0        0     8937 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/lr_scheduler.py
--rw-r--r--   0        0        0     9464 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/model_hub.py
--rw-r--r--   0        0        0     1612 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/models/__init__.py
--rw-r--r--   0        0        0     6591 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/models/attentive_fp.py
--rw-r--r--   0        0        0    10656 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/models/autoencoder.py
--rw-r--r--   0        0        0    27754 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/models/basic_gnn.py
--rw-r--r--   0        0        0     4138 2023-04-18 06:05:39.246322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/models/captum.py
--rw-r--r--   0        0        0     6799 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/models/correct_and_smooth.py
--rw-r--r--   0        0        0     3972 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/models/deep_graph_infomax.py
--rw-r--r--   0        0        0     4223 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/models/deepgcn.py
--rw-r--r--   0        0        0    34432 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/models/dimenet.py
--rw-r--r--   0        0        0     4611 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/models/dimenet_utils.py
--rw-r--r--   0        0        0     7859 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/models/gnnff.py
--rw-r--r--   0        0        0     5381 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/models/graph_unet.py
--rw-r--r--   0        0        0     3397 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/models/jumping_knowledge.py
--rw-r--r--   0        0        0     3725 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/models/label_prop.py
--rw-r--r--   0        0        0    10918 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/models/lightgcn.py
--rw-r--r--   0        0        0     7901 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/models/linkx.py
--rw-r--r--   0        0        0     2566 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/models/mask_label.py
--rw-r--r--   0        0        0     6529 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/models/meta.py
--rw-r--r--   0        0        0    10318 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/models/metapath2vec.py
--rw-r--r--   0        0        0     8676 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/models/mlp.py
--rw-r--r--   0        0        0     7171 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/models/node2vec.py
--rw-r--r--   0        0        0     8987 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/models/re_net.py
--rw-r--r--   0        0        0     5789 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/models/rect.py
--rw-r--r--   0        0        0    11818 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/models/rev_gnn.py
--rw-r--r--   0        0        0    16599 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/models/schnet.py
--rw-r--r--   0        0        0     9840 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/models/signed_gcn.py
--rw-r--r--   0        0        0    11587 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/models/tgn.py
--rw-r--r--   0        0        0     1576 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/module_dict.py
--rw-r--r--   0        0        0      638 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/norm/__init__.py
--rw-r--r--   0        0        0     8258 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/norm/batch_norm.py
--rw-r--r--   0        0        0     4706 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/norm/diff_group_norm.py
--rw-r--r--   0        0        0     2715 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/norm/graph_norm.py
--rw-r--r--   0        0        0     1492 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/norm/graph_size_norm.py
--rw-r--r--   0        0        0     4670 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/norm/instance_norm.py
--rw-r--r--   0        0        0     6673 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/norm/layer_norm.py
--rw-r--r--   0        0        0     1311 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/norm/mean_subtraction_norm.py
--rw-r--r--   0        0        0     1654 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/norm/msg_norm.py
--rw-r--r--   0        0        0     2809 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/norm/pair_norm.py
--rw-r--r--   0        0        0     1453 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/parameter_dict.py
--rw-r--r--   0        0        0    10718 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/pool/__init__.py
--rw-r--r--   0        0        0     6868 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/pool/asap.py
--rw-r--r--   0        0        0     3749 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/pool/avg_pool.py
--rw-r--r--   0        0        0     3345 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/pool/base.py
--rw-r--r--   0        0        0       56 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/pool/connect/__init__.py
--rw-r--r--   0        0        0     1369 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/pool/connect/base.py
--rw-r--r--   0        0        0      273 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/pool/consecutive.py
--rw-r--r--   0        0        0     1600 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/pool/decimation.py
--rw-r--r--   0        0        0     8567 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/pool/edge_pool.py
--rw-r--r--   0        0        0     3627 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/pool/glob.py
--rw-r--r--   0        0        0     1292 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/pool/graclus.py
--rw-r--r--   0        0        0     4045 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/pool/max_pool.py
--rw-r--r--   0        0        0     4832 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/pool/mem_pool.py
--rw-r--r--   0        0        0     4353 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/pool/pan_pool.py
--rw-r--r--   0        0        0      631 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/pool/pool.py
--rw-r--r--   0        0        0     5919 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/pool/sag_pool.py
--rw-r--r--   0        0        0       54 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/pool/select/__init__.py
--rw-r--r--   0        0        0     1308 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/pool/select/base.py
--rw-r--r--   0        0        0     8347 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/pool/topk_pool.py
--rw-r--r--   0        0        0     2727 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/pool/voxel_grid.py
--rw-r--r--   0        0        0      412 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/reshape.py
--rw-r--r--   0        0        0     5675 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/resolver.py
--rw-r--r--   0        0        0     1071 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/sequential.jinja
--rw-r--r--   0        0        0     4577 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/sequential.py
--rw-r--r--   0        0        0     5616 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/summary.py
--rw-r--r--   0        0        0     1282 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/to_fixed_size_transformer.py
--rw-r--r--   0        0        0     6395 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/to_hetero_module.py
--rw-r--r--   0        0        0    18095 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/to_hetero_transformer.py
--rw-r--r--   0        0        0    23139 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/to_hetero_with_bases_transformer.py
--rw-r--r--   0        0        0      102 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/unpool/__init__.py
--rw-r--r--   0        0        0     2586 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/unpool/knn_interpolate.py
--rw-r--r--   0        0        0      740 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/profile/__init__.py
--rw-r--r--   0        0        0     3356 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/profile/benchmark.py
--rw-r--r--   0        0        0     8089 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/profile/profile.py
--rw-r--r--   0        0        0    16665 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/profile/profiler.py
--rw-r--r--   0        0        0     4563 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/profile/utils.py
--rw-r--r--   0        0        0     1391 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/resolver.py
--rw-r--r--   0        0        0      481 2023-04-18 06:05:39.250322 pyg-nightly-2.4.0.dev20230418/torch_geometric/sampler/__init__.py
--rw-r--r--   0        0        0    19075 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/sampler/base.py
--rw-r--r--   0        0        0     2734 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/sampler/hgt_sampler.py
--rw-r--r--   0        0        0    25362 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/sampler/neighbor_sampler.py
--rw-r--r--   0        0        0     4537 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/sampler/utils.py
--rw-r--r--   0        0        0      354 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/seed.py
--rw-r--r--   0        0        0      710 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/testing/__init__.py
--rw-r--r--   0        0        0     4368 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/testing/asserts.py
--rw-r--r--   0        0        0     1755 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/testing/data.py
--rw-r--r--   0        0        0     3842 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/testing/decorators.py
--rw-r--r--   0        0        0     1847 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/testing/feature_store.py
--rw-r--r--   0        0        0     1009 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/testing/graph_store.py
--rw-r--r--   0        0        0     3971 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/__init__.py
--rw-r--r--   0        0        0    13966 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/add_metapaths.py
--rw-r--r--   0        0        0     4838 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/add_positional_encoding.py
--rw-r--r--   0        0        0     2019 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/add_self_loops.py
--rw-r--r--   0        0        0     1141 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/base_transform.py
--rw-r--r--   0        0        0     1937 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/cartesian.py
--rw-r--r--   0        0        0      641 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/center.py
--rw-r--r--   0        0        0     1659 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/compose.py
--rw-r--r--   0        0        0     1961 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/constant.py
--rw-r--r--   0        0        0     1223 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/delaunay.py
--rw-r--r--   0        0        0     1810 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/distance.py
--rw-r--r--   0        0        0     1035 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/face_to_edge.py
--rw-r--r--   0        0        0     2953 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/feature_propagation.py
--rw-r--r--   0        0        0     2368 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/fixed_points.py
--rw-r--r--   0        0        0     1398 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/gcn_norm.py
--rw-r--r--   0        0        0    24216 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/gdc.py
--rw-r--r--   0        0        0     1019 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/generate_mesh_normals.py
--rw-r--r--   0        0        0     2512 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/grid_sampling.py
--rw-r--r--   0        0        0     2544 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/knn_graph.py
--rw-r--r--   0        0        0     2466 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/laplacian_lambda_max.py
--rw-r--r--   0        0        0     2001 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/largest_connected_components.py
--rw-r--r--   0        0        0     3724 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/line_graph.py
--rw-r--r--   0        0        0     1998 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/linear_transformation.py
--rw-r--r--   0        0        0     1699 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/local_cartesian.py
--rw-r--r--   0        0        0     1405 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/local_degree_profile.py
--rw-r--r--   0        0        0     4600 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/mask.py
--rw-r--r--   0        0        0      979 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/normalize_features.py
--rw-r--r--   0        0        0     1739 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/normalize_rotation.py
--rw-r--r--   0        0        0      621 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/normalize_scale.py
--rw-r--r--   0        0        0     1534 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/one_hot_degree.py
--rw-r--r--   0        0        0    21080 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/pad.py
--rw-r--r--   0        0        0     1794 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/point_pair_features.py
--rw-r--r--   0        0        0     2127 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/polar.py
--rw-r--r--   0        0        0     2051 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/radius_graph.py
--rw-r--r--   0        0        0      989 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/random_flip.py
--rw-r--r--   0        0        0     1511 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/random_jitter.py
--rw-r--r--   0        0        0    14298 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/random_link_split.py
--rw-r--r--   0        0        0     5769 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/random_node_split.py
--rw-r--r--   0        0        0     1904 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/random_rotate.py
--rw-r--r--   0        0        0     1216 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/random_scale.py
--rw-r--r--   0        0        0     1320 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/random_shear.py
--rw-r--r--   0        0        0     1806 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/remove_duplicated_edges.py
--rw-r--r--   0        0        0     2284 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/remove_isolated_nodes.py
--rw-r--r--   0        0        0      960 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/remove_training_classes.py
--rw-r--r--   0        0        0     6112 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/rooted_subgraph.py
--rw-r--r--   0        0        0     2141 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/sample_points.py
--rw-r--r--   0        0        0     2129 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/sign.py
--rw-r--r--   0        0        0     2242 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/spherical.py
--rw-r--r--   0        0        0     1003 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/svd_feature_reduction.py
--rw-r--r--   0        0        0     1608 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/target_indegree.py
--rw-r--r--   0        0        0     2328 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/to_dense.py
--rw-r--r--   0        0        0     1456 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/to_device.py
--rw-r--r--   0        0        0     5354 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/to_sparse_tensor.py
--rw-r--r--   0        0        0     2622 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/to_superpixels.py
--rw-r--r--   0        0        0     2973 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/to_undirected.py
--rw-r--r--   0        0        0     1215 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/two_hop.py
--rw-r--r--   0        0        0     2784 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/virtual_node.py
--rw-r--r--   0        0        0     8111 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/typing.py
--rw-r--r--   0        0        0     4474 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/__init__.py
--rw-r--r--   0        0        0     2347 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/assortativity.py
--rw-r--r--   0        0        0     9080 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/augmentation.py
--rw-r--r--   0        0        0     4941 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/coalesce.py
--rw-r--r--   0        0        0    19515 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/convert.py
--rw-r--r--   0        0        0     1018 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/degree.py
--rw-r--r--   0        0        0    11323 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/dropout.py
--rw-r--r--   0        0        0     1657 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/embedding.py
--rw-r--r--   0        0        0     4042 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/geodesic.py
--rw-r--r--   0        0        0     3755 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/get_laplacian.py
--rw-r--r--   0        0        0     4424 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/get_mesh_laplacian.py
--rw-r--r--   0        0        0     2536 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/grid.py
--rw-r--r--   0        0        0     5044 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/hetero.py
--rw-r--r--   0        0        0     4818 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/homophily.py
--rw-r--r--   0        0        0     3574 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/isolated.py
--rw-r--r--   0        0        0    15855 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/loop.py
--rw-r--r--   0        0        0     1884 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/mask.py
--rw-r--r--   0        0        0      608 2023-04-18 06:05:39.254322 pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/mixin.py
--rw-r--r--   0        0        0    14643 2023-04-18 06:05:39.258322 pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/negative_sampling.py
--rw-r--r--   0        0        0     3344 2023-04-18 06:05:39.258322 pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/nested.py
--rw-r--r--   0        0        0     1169 2023-04-18 06:05:39.258322 pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/normalized_cut.py
--rw-r--r--   0        0        0     1468 2023-04-18 06:05:39.258322 pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/num_nodes.py
--rw-r--r--   0        0        0     1404 2023-04-18 06:05:39.258322 pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/one_hot.py
--rw-r--r--   0        0        0     5154 2023-04-18 06:05:39.258322 pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/random.py
--rw-r--r--   0        0        0      361 2023-04-18 06:05:39.258322 pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/repeat.py
--rw-r--r--   0        0        0     7429 2023-04-18 06:05:39.258322 pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/scatter.py
--rw-r--r--   0        0        0     1110 2023-04-18 06:05:39.258322 pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/segment.py
--rw-r--r--   0        0        0     2149 2023-04-18 06:05:39.258322 pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/select.py
--rw-r--r--   0        0        0     6016 2023-04-18 06:05:39.258322 pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/smiles.py
--rw-r--r--   0        0        0     2718 2023-04-18 06:05:39.258322 pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/softmax.py
--rw-r--r--   0        0        0     1017 2023-04-18 06:05:39.258322 pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/sort.py
--rw-r--r--   0        0        0     3034 2023-04-18 06:05:39.258322 pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/sort_edge_index.py
--rw-r--r--   0        0        0    11835 2023-04-18 06:05:39.258322 pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/sparse.py
--rw-r--r--   0        0        0     5547 2023-04-18 06:05:39.258322 pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/spmm.py
--rw-r--r--   0        0        0    12370 2023-04-18 06:05:39.258322 pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/subgraph.py
--rw-r--r--   0        0        0     3439 2023-04-18 06:05:39.258322 pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/to_dense_adj.py
--rw-r--r--   0        0        0     4267 2023-04-18 06:05:39.258322 pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/to_dense_batch.py
--rw-r--r--   0        0        0     3489 2023-04-18 06:05:39.258322 pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/train_test_split_edges.py
--rw-r--r--   0        0        0     4867 2023-04-18 06:05:39.258322 pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/tree_decomposition.py
--rw-r--r--   0        0        0     6350 2023-04-18 06:05:39.258322 pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/trim_to_layer.py
--rw-r--r--   0        0        0     2125 2023-04-18 06:05:39.258322 pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/unbatch.py
--rw-r--r--   0        0        0     5770 2023-04-18 06:05:39.258322 pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/undirected.py
--rw-r--r--   0        0        0      123 2023-04-18 06:05:39.258322 pyg-nightly-2.4.0.dev20230418/torch_geometric/visualization/__init__.py
--rw-r--r--   0        0        0     4149 2023-04-18 06:05:39.258322 pyg-nightly-2.4.0.dev20230418/torch_geometric/visualization/graph.py
--rw-r--r--   0        0        0      388 2023-04-18 06:05:39.258322 pyg-nightly-2.4.0.dev20230418/torch_geometric/visualization/influence.py
--rw-r--r--   0        0        0    63628 1970-01-01 00:00:00.000000 pyg-nightly-2.4.0.dev20230418/PKG-INFO
+-rw-r--r--   0        0        0    60619 2023-04-19 06:06:04.198545 pyg-nightly-2.4.0.dev20230419/README.md
+-rw-r--r--   0        0        0     4073 2023-04-19 06:06:04.562547 pyg-nightly-2.4.0.dev20230419/pyproject.toml
+-rw-r--r--   0        0        0     1055 2023-04-19 06:06:04.558547 pyg-nightly-2.4.0.dev20230419/torch_geometric/__init__.py
+-rw-r--r--   0        0        0     3392 2023-04-19 06:06:04.234545 pyg-nightly-2.4.0.dev20230419/torch_geometric/compile.py
+-rw-r--r--   0        0        0      352 2023-04-19 06:06:04.234545 pyg-nightly-2.4.0.dev20230419/torch_geometric/contrib/__init__.py
+-rw-r--r--   0        0        0       23 2023-04-19 06:06:04.234545 pyg-nightly-2.4.0.dev20230419/torch_geometric/contrib/datasets/__init__.py
+-rw-r--r--   0        0        0      163 2023-04-19 06:06:04.234545 pyg-nightly-2.4.0.dev20230419/torch_geometric/contrib/explain/__init__.py
+-rw-r--r--   0        0        0    20540 2023-04-19 06:06:04.234545 pyg-nightly-2.4.0.dev20230419/torch_geometric/contrib/explain/graphmask_explainer.py
+-rw-r--r--   0        0        0    16627 2023-04-19 06:06:04.234545 pyg-nightly-2.4.0.dev20230419/torch_geometric/contrib/explain/pgm_explainer.py
+-rw-r--r--   0        0        0       72 2023-04-19 06:06:04.234545 pyg-nightly-2.4.0.dev20230419/torch_geometric/contrib/nn/__init__.py
+-rw-r--r--   0        0        0       23 2023-04-19 06:06:04.234545 pyg-nightly-2.4.0.dev20230419/torch_geometric/contrib/nn/conv/__init__.py
+-rw-r--r--   0        0        0      113 2023-04-19 06:06:04.234545 pyg-nightly-2.4.0.dev20230419/torch_geometric/contrib/nn/models/__init__.py
+-rw-r--r--   0        0        0    33261 2023-04-19 06:06:04.234545 pyg-nightly-2.4.0.dev20230419/torch_geometric/contrib/nn/models/rbcd_attack.py
+-rw-r--r--   0        0        0       23 2023-04-19 06:06:04.234545 pyg-nightly-2.4.0.dev20230419/torch_geometric/contrib/transforms/__init__.py
+-rw-r--r--   0        0        0     3383 2023-04-19 06:06:04.234545 pyg-nightly-2.4.0.dev20230419/torch_geometric/data/__init__.py
+-rw-r--r--   0        0        0     7436 2023-04-19 06:06:04.234545 pyg-nightly-2.4.0.dev20230419/torch_geometric/data/batch.py
+-rw-r--r--   0        0        0    10432 2023-04-19 06:06:04.234545 pyg-nightly-2.4.0.dev20230419/torch_geometric/data/collate.py
+-rw-r--r--   0        0        0    37570 2023-04-19 06:06:04.234545 pyg-nightly-2.4.0.dev20230419/torch_geometric/data/data.py
+-rw-r--r--   0        0        0     2922 2023-04-19 06:06:04.234545 pyg-nightly-2.4.0.dev20230419/torch_geometric/data/datapipes.py
+-rw-r--r--   0        0        0    14850 2023-04-19 06:06:04.234545 pyg-nightly-2.4.0.dev20230419/torch_geometric/data/dataset.py
+-rw-r--r--   0        0        0     1359 2023-04-19 06:06:04.234545 pyg-nightly-2.4.0.dev20230419/torch_geometric/data/download.py
+-rw-r--r--   0        0        0     2252 2023-04-19 06:06:04.234545 pyg-nightly-2.4.0.dev20230419/torch_geometric/data/extract.py
+-rw-r--r--   0        0        0    21075 2023-04-19 06:06:04.234545 pyg-nightly-2.4.0.dev20230419/torch_geometric/data/feature_store.py
+-rw-r--r--   0        0        0    13495 2023-04-19 06:06:04.234545 pyg-nightly-2.4.0.dev20230419/torch_geometric/data/graph_store.py
+-rw-r--r--   0        0        0    42291 2023-04-19 06:06:04.234545 pyg-nightly-2.4.0.dev20230419/torch_geometric/data/hetero_data.py
+-rw-r--r--   0        0        0     7091 2023-04-19 06:06:04.234545 pyg-nightly-2.4.0.dev20230419/torch_geometric/data/in_memory_dataset.py
+-rw-r--r--   0        0        0      178 2023-04-19 06:06:04.234545 pyg-nightly-2.4.0.dev20230419/torch_geometric/data/lightning/__init__.py
+-rw-r--r--   0        0        0    28490 2023-04-19 06:06:04.234545 pyg-nightly-2.4.0.dev20230419/torch_geometric/data/lightning/datamodule.py
+-rw-r--r--   0        0        0      338 2023-04-19 06:06:04.234545 pyg-nightly-2.4.0.dev20230419/torch_geometric/data/makedirs.py
+-rw-r--r--   0        0        0     3962 2023-04-19 06:06:04.234545 pyg-nightly-2.4.0.dev20230419/torch_geometric/data/remote_backend_utils.py
+-rw-r--r--   0        0        0     4321 2023-04-19 06:06:04.234545 pyg-nightly-2.4.0.dev20230419/torch_geometric/data/separate.py
+-rw-r--r--   0        0        0    24947 2023-04-19 06:06:04.234545 pyg-nightly-2.4.0.dev20230419/torch_geometric/data/storage.py
+-rw-r--r--   0        0        0     2579 2023-04-19 06:06:04.234545 pyg-nightly-2.4.0.dev20230419/torch_geometric/data/summary.py
+-rw-r--r--   0        0        0     9354 2023-04-19 06:06:04.234545 pyg-nightly-2.4.0.dev20230419/torch_geometric/data/temporal.py
+-rw-r--r--   0        0        0     1046 2023-04-19 06:06:04.234545 pyg-nightly-2.4.0.dev20230419/torch_geometric/data/view.py
+-rw-r--r--   0        0        0     4870 2023-04-19 06:06:04.234545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/__init__.py
+-rw-r--r--   0        0        0     4220 2023-04-19 06:06:04.234545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/actor.py
+-rw-r--r--   0        0        0     5584 2023-04-19 06:06:04.234545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/airfrans.py
+-rw-r--r--   0        0        0     3711 2023-04-19 06:06:04.234545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/airports.py
+-rw-r--r--   0        0        0     3017 2023-04-19 06:06:04.234545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/amazon.py
+-rw-r--r--   0        0        0     4099 2023-04-19 06:06:04.234545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/amazon_products.py
+-rw-r--r--   0        0        0     4942 2023-04-19 06:06:04.234545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/aminer.py
+-rw-r--r--   0        0        0     5266 2023-04-19 06:06:04.234545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/aqsol.py
+-rw-r--r--   0        0        0     5735 2023-04-19 06:06:04.234545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/attributed_graph_dataset.py
+-rw-r--r--   0        0        0     4063 2023-04-19 06:06:04.234545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/ba2motif_dataset.py
+-rw-r--r--   0        0        0     3518 2023-04-19 06:06:04.234545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/ba_multi_shapes.py
+-rw-r--r--   0        0        0     3824 2023-04-19 06:06:04.234545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/ba_shapes.py
+-rw-r--r--   0        0        0     4137 2023-04-19 06:06:04.234545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/bitcoin_otc.py
+-rw-r--r--   0        0        0     3942 2023-04-19 06:06:04.234545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/citation_full.py
+-rw-r--r--   0        0        0     2976 2023-04-19 06:06:04.234545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/coauthor.py
+-rw-r--r--   0        0        0     4564 2023-04-19 06:06:04.234545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/coma.py
+-rw-r--r--   0        0        0     4538 2023-04-19 06:06:04.234545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/dblp.py
+-rw-r--r--   0        0        0     5608 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/dbp15k.py
+-rw-r--r--   0        0        0     2308 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/deezer_europe.py
+-rw-r--r--   0        0        0     3862 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/dgraph.py
+-rw-r--r--   0        0        0     5865 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/dynamic_faust.py
+-rw-r--r--   0        0        0     4498 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/elliptic.py
+-rw-r--r--   0        0        0     2990 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/elliptic_temporal.py
+-rw-r--r--   0        0        0     2631 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/email_eu_core.py
+-rw-r--r--   0        0        0     7009 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/entities.py
+-rw-r--r--   0        0        0     5817 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/explainer_dataset.py
+-rw-r--r--   0        0        0     2228 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/facebook.py
+-rw-r--r--   0        0        0    10215 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/fake.py
+-rw-r--r--   0        0        0     3924 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/faust.py
+-rw-r--r--   0        0        0     4099 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/flickr.py
+-rw-r--r--   0        0        0     3815 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/freebase.py
+-rw-r--r--   0        0        0     3416 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/gdelt.py
+-rw-r--r--   0        0        0     9261 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/ged_dataset.py
+-rw-r--r--   0        0        0     2626 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/gemsec.py
+-rw-r--r--   0        0        0     3954 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/geometry.py
+-rw-r--r--   0        0        0     2484 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/github.py
+-rw-r--r--   0        0        0     6762 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/gnn_benchmark_dataset.py
+-rw-r--r--   0        0        0      221 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/graph_generator/__init__.py
+-rw-r--r--   0        0        0      965 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/graph_generator/ba_graph.py
+-rw-r--r--   0        0        0      949 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/graph_generator/base.py
+-rw-r--r--   0        0        0      918 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/graph_generator/er_graph.py
+-rw-r--r--   0        0        0     1159 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/graph_generator/grid_graph.py
+-rw-r--r--   0        0        0     4043 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/heterophilous_graph_dataset.py
+-rw-r--r--   0        0        0     8467 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/hgb_dataset.py
+-rw-r--r--   0        0        0    11053 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/hydro_net.py
+-rw-r--r--   0        0        0     4447 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/icews.py
+-rw-r--r--   0        0        0     4000 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/imdb.py
+-rw-r--r--   0        0        0     7169 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/infection_dataset.py
+-rw-r--r--   0        0        0     3439 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/jodie.py
+-rw-r--r--   0        0        0     3444 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/karate.py
+-rw-r--r--   0        0        0     4349 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/last_fm.py
+-rw-r--r--   0        0        0     2283 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/lastfm_asia.py
+-rw-r--r--   0        0        0     6582 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/linkx_dataset.py
+-rw-r--r--   0        0        0    11559 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/lrgb.py
+-rw-r--r--   0        0        0     5044 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/malnet_tiny.py
+-rw-r--r--   0        0        0    16482 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/md17.py
+-rw-r--r--   0        0        0     3770 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/mixhop_synthetic_dataset.py
+-rw-r--r--   0        0        0     3136 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/mnist_superpixels.py
+-rw-r--r--   0        0        0     5251 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/modelnet.py
+-rw-r--r--   0        0        0     6593 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/molecule_net.py
+-rw-r--r--   0        0        0      227 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/motif_generator/__init__.py
+-rw-r--r--   0        0        0      910 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/motif_generator/base.py
+-rw-r--r--   0        0        0     1203 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/motif_generator/custom.py
+-rw-r--r--   0        0        0      984 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/motif_generator/cycle.py
+-rw-r--r--   0        0        0      801 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/motif_generator/house.py
+-rw-r--r--   0        0        0     3787 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/movie_lens.py
+-rw-r--r--   0        0        0     2889 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/nell.py
+-rw-r--r--   0        0        0     7190 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/ogb_mag.py
+-rw-r--r--   0        0        0     3415 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/omdb.py
+-rw-r--r--   0        0        0     3964 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/particle.py
+-rw-r--r--   0        0        0    10699 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/pascal.py
+-rw-r--r--   0        0        0     4602 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/pascal_pf.py
+-rw-r--r--   0        0        0     5716 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/pcpnet_dataset.py
+-rw-r--r--   0        0        0     7016 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/planetoid.py
+-rw-r--r--   0        0        0     2842 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/polblogs.py
+-rw-r--r--   0        0        0     4866 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/ppi.py
+-rw-r--r--   0        0        0     3182 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/qm7.py
+-rw-r--r--   0        0        0    16813 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/qm9.py
+-rw-r--r--   0        0        0     2941 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/reddit.py
+-rw-r--r--   0        0        0     4439 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/reddit2.py
+-rw-r--r--   0        0        0     4345 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/rel_link_pred_dataset.py
+-rw-r--r--   0        0        0     4173 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/s3dis.py
+-rw-r--r--   0        0        0     8140 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/sbm_dataset.py
+-rw-r--r--   0        0        0     8088 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/shapenet.py
+-rw-r--r--   0        0        0     6150 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/shrec2016.py
+-rw-r--r--   0        0        0     9283 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/snap_dataset.py
+-rw-r--r--   0        0        0     3031 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/suite_sparse.py
+-rw-r--r--   0        0        0     3959 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/taobao.py
+-rw-r--r--   0        0        0     4451 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/tosca.py
+-rw-r--r--   0        0        0     7174 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/tu_dataset.py
+-rw-r--r--   0        0        0     3464 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/twitch.py
+-rw-r--r--   0        0        0     6929 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/upfd.py
+-rw-r--r--   0        0        0      156 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/utils/__init__.py
+-rw-r--r--   0        0        0     1655 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/utils/cheatsheet.py
+-rw-r--r--   0        0        0     4615 2023-04-19 06:06:04.238545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/webkb.py
+-rw-r--r--   0        0        0     3674 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/wikics.py
+-rw-r--r--   0        0        0     6083 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/wikipedia_network.py
+-rw-r--r--   0        0        0     6322 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/willow_object_class.py
+-rw-r--r--   0        0        0     7857 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/word_net.py
+-rw-r--r--   0        0        0     4116 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/yelp.py
+-rw-r--r--   0        0        0     6171 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/zinc.py
+-rw-r--r--   0        0        0     1197 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/debug.py
+-rw-r--r--   0        0        0      748 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/deprecation.py
+-rw-r--r--   0        0        0     2466 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/experimental.py
+-rw-r--r--   0        0        0      359 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/explain/__init__.py
+-rw-r--r--   0        0        0      418 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/explain/algorithm/__init__.py
+-rw-r--r--   0        0        0     4491 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/explain/algorithm/attention_explainer.py
+-rw-r--r--   0        0        0     6899 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/explain/algorithm/base.py
+-rw-r--r--   0        0        0    12489 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/explain/algorithm/captum.py
+-rw-r--r--   0        0        0     6540 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/explain/algorithm/captum_explainer.py
+-rw-r--r--   0        0        0     2867 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/explain/algorithm/dummy_explainer.py
+-rw-r--r--   0        0        0    11149 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/explain/algorithm/gnn_explainer.py
+-rw-r--r--   0        0        0    10370 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/explain/algorithm/pg_explainer.py
+-rw-r--r--   0        0        0     2308 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/explain/algorithm/utils.py
+-rw-r--r--   0        0        0     7834 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/explain/config.py
+-rw-r--r--   0        0        0    10375 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/explain/explainer.py
+-rw-r--r--   0        0        0    12882 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/explain/explanation.py
+-rw-r--r--   0        0        0      301 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/explain/metric/__init__.py
+-rw-r--r--   0        0        0     1888 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/explain/metric/basic.py
+-rw-r--r--   0        0        0     3063 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/explain/metric/faithfulness.py
+-rw-r--r--   0        0        0     6157 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/explain/metric/fidelity.py
+-rw-r--r--   0        0        0     2045 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/__init__.py
+-rw-r--r--   0        0        0      510 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/benchmark.py
+-rw-r--r--   0        0        0     2371 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/checkpoint.py
+-rw-r--r--   0        0        0      738 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/cmd_args.py
+-rw-r--r--   0        0        0    17221 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/config.py
+-rw-r--r--   0        0        0    14575 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/config_store.py
+-rw-r--r--   0        0        0      389 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/contrib/__init__.py
+-rw-r--r--   0        0        0      221 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/contrib/act/__init__.py
+-rw-r--r--   0        0        0      221 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/contrib/config/__init__.py
+-rw-r--r--   0        0        0      221 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/contrib/encoder/__init__.py
+-rw-r--r--   0        0        0      221 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/contrib/head/__init__.py
+-rw-r--r--   0        0        0      221 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/contrib/layer/__init__.py
+-rw-r--r--   0        0        0     8304 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/contrib/layer/generalconv.py
+-rw-r--r--   0        0        0      221 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/contrib/loader/__init__.py
+-rw-r--r--   0        0        0      221 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/contrib/loss/__init__.py
+-rw-r--r--   0        0        0      221 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/contrib/network/__init__.py
+-rw-r--r--   0        0        0      221 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/contrib/optimizer/__init__.py
+-rw-r--r--   0        0        0      221 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/contrib/pooling/__init__.py
+-rw-r--r--   0        0        0      221 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/contrib/stage/__init__.py
+-rw-r--r--   0        0        0      221 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/contrib/train/__init__.py
+-rw-r--r--   0        0        0      221 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/contrib/transform/__init__.py
+-rw-r--r--   0        0        0      375 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/imports.py
+-rw-r--r--   0        0        0      490 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/init.py
+-rw-r--r--   0        0        0    11763 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/loader.py
+-rw-r--r--   0        0        0    11337 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/logger.py
+-rw-r--r--   0        0        0     1474 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/loss.py
+-rw-r--r--   0        0        0     2844 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/model_builder.py
+-rw-r--r--   0        0        0     1121 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/models/__init__.py
+-rw-r--r--   0        0        0      822 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/models/act.py
+-rw-r--r--   0        0        0     2546 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/models/encoder.py
+-rw-r--r--   0        0        0     5133 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/models/gnn.py
+-rw-r--r--   0        0        0     4323 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/models/head.py
+-rw-r--r--   0        0        0    12486 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/models/layer.py
+-rw-r--r--   0        0        0      288 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/models/pooling.py
+-rw-r--r--   0        0        0     1391 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/models/transform.py
+-rw-r--r--   0        0        0     2544 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/optim.py
+-rw-r--r--   0        0        0     3944 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/register.py
+-rw-r--r--   0        0        0     1887 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/train.py
+-rw-r--r--   0        0        0        0 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/utils/LICENSE
+-rw-r--r--   0        0        0      641 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/utils/__init__.py
+-rw-r--r--   0        0        0     9513 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/utils/agg_runs.py
+-rw-r--r--   0        0        0     3056 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/utils/comp_budget.py
+-rw-r--r--   0        0        0     1352 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/utils/device.py
+-rw-r--r--   0        0        0      690 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/utils/epoch.py
+-rw-r--r--   0        0        0     2050 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/utils/io.py
+-rw-r--r--   0        0        0      606 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/utils/plot.py
+-rw-r--r--   0        0        0      198 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/utils/tools.py
+-rw-r--r--   0        0        0      830 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/home.py
+-rw-r--r--   0        0        0      528 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/io/__init__.py
+-rw-r--r--   0        0        0      943 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/io/npz.py
+-rw-r--r--   0        0        0      957 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/io/obj.py
+-rw-r--r--   0        0        0     2586 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/io/off.py
+-rw-r--r--   0        0        0     4211 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/io/planetoid.py
+-rw-r--r--   0        0        0      476 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/io/ply.py
+-rw-r--r--   0        0        0     1136 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/io/sdf.py
+-rw-r--r--   0        0        0     4733 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/io/tu.py
+-rw-r--r--   0        0        0      562 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/io/txt_array.py
+-rw-r--r--   0        0        0      768 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/lazy_loader.py
+-rw-r--r--   0        0        0     1616 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/loader/__init__.py
+-rw-r--r--   0        0        0     1433 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/loader/base.py
+-rw-r--r--   0        0        0     6539 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/loader/cluster.py
+-rw-r--r--   0        0        0     1449 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/loader/data_list_loader.py
+-rw-r--r--   0        0        0     3222 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/loader/dataloader.py
+-rw-r--r--   0        0        0     1683 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/loader/dense_data_loader.py
+-rw-r--r--   0        0        0     4285 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/loader/dynamic_batch_sampler.py
+-rw-r--r--   0        0        0     8448 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/loader/graph_saint.py
+-rw-r--r--   0        0        0     5715 2023-04-19 06:06:04.242545 pyg-nightly-2.4.0.dev20230419/torch_geometric/loader/hgt_loader.py
+-rw-r--r--   0        0        0     3754 2023-04-19 06:06:04.246545 pyg-nightly-2.4.0.dev20230419/torch_geometric/loader/imbalanced_sampler.py
+-rw-r--r--   0        0        0    13521 2023-04-19 06:06:04.246545 pyg-nightly-2.4.0.dev20230419/torch_geometric/loader/link_loader.py
+-rw-r--r--   0        0        0    12216 2023-04-19 06:06:04.246545 pyg-nightly-2.4.0.dev20230419/torch_geometric/loader/link_neighbor_loader.py
+-rw-r--r--   0        0        0     6282 2023-04-19 06:06:04.246545 pyg-nightly-2.4.0.dev20230419/torch_geometric/loader/mixin.py
+-rw-r--r--   0        0        0    11085 2023-04-19 06:06:04.246545 pyg-nightly-2.4.0.dev20230419/torch_geometric/loader/neighbor_loader.py
+-rw-r--r--   0        0        0     8513 2023-04-19 06:06:04.246545 pyg-nightly-2.4.0.dev20230419/torch_geometric/loader/neighbor_sampler.py
+-rw-r--r--   0        0        0     8938 2023-04-19 06:06:04.246545 pyg-nightly-2.4.0.dev20230419/torch_geometric/loader/node_loader.py
+-rw-r--r--   0        0        0     2196 2023-04-19 06:06:04.246545 pyg-nightly-2.4.0.dev20230419/torch_geometric/loader/random_node_loader.py
+-rw-r--r--   0        0        0     4173 2023-04-19 06:06:04.246545 pyg-nightly-2.4.0.dev20230419/torch_geometric/loader/shadow.py
+-rw-r--r--   0        0        0     1319 2023-04-19 06:06:04.246545 pyg-nightly-2.4.0.dev20230419/torch_geometric/loader/temporal_dataloader.py
+-rw-r--r--   0        0        0    11743 2023-04-19 06:06:04.246545 pyg-nightly-2.4.0.dev20230419/torch_geometric/loader/utils.py
+-rw-r--r--   0        0        0     3034 2023-04-19 06:06:04.246545 pyg-nightly-2.4.0.dev20230419/torch_geometric/loader/zip_loader.py
+-rw-r--r--   0        0        0      832 2023-04-19 06:06:04.246545 pyg-nightly-2.4.0.dev20230419/torch_geometric/logging.py
+-rw-r--r--   0        0        0      911 2023-04-19 06:06:04.246545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/__init__.py
+-rw-r--r--   0        0        0     1397 2023-04-19 06:06:04.246545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/aggr/__init__.py
+-rw-r--r--   0        0        0     2395 2023-04-19 06:06:04.246545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/aggr/attention.py
+-rw-r--r--   0        0        0     7105 2023-04-19 06:06:04.246545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/aggr/base.py
+-rw-r--r--   0        0        0    10858 2023-04-19 06:06:04.246545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/aggr/basic.py
+-rw-r--r--   0        0        0     2064 2023-04-19 06:06:04.246545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/aggr/deep_sets.py
+-rw-r--r--   0        0        0     6881 2023-04-19 06:06:04.246545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/aggr/equilibrium.py
+-rw-r--r--   0        0        0    12074 2023-04-19 06:06:04.246545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/aggr/fused.py
+-rw-r--r--   0        0        0     3062 2023-04-19 06:06:04.246545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/aggr/gmt.py
+-rw-r--r--   0        0        0     1464 2023-04-19 06:06:04.246545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/aggr/gru.py
+-rw-r--r--   0        0        0     1484 2023-04-19 06:06:04.246545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/aggr/lstm.py
+-rw-r--r--   0        0        0     1995 2023-04-19 06:06:04.246545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/aggr/mlp.py
+-rw-r--r--   0        0        0     8163 2023-04-19 06:06:04.246545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/aggr/multi.py
+-rw-r--r--   0        0        0     5869 2023-04-19 06:06:04.246545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/aggr/quantile.py
+-rw-r--r--   0        0        0     4642 2023-04-19 06:06:04.246545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/aggr/scaler.py
+-rw-r--r--   0        0        0     2517 2023-04-19 06:06:04.246545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/aggr/set2set.py
+-rw-r--r--   0        0        0     3439 2023-04-19 06:06:04.246545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/aggr/set_transformer.py
+-rw-r--r--   0        0        0     1772 2023-04-19 06:06:04.246545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/aggr/sort.py
+-rw-r--r--   0        0        0     8322 2023-04-19 06:06:04.246545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/aggr/utils.py
+-rw-r--r--   0        0        0     3360 2023-04-19 06:06:04.246545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/__init__.py
+-rw-r--r--   0        0        0     3088 2023-04-19 06:06:04.246545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/agnn_conv.py
+-rw-r--r--   0        0        0     4388 2023-04-19 06:06:04.246545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/antisymmetric_conv.py
+-rw-r--r--   0        0        0     6010 2023-04-19 06:06:04.246545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/appnp.py
+-rw-r--r--   0        0        0     6637 2023-04-19 06:06:04.246545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/arma_conv.py
+-rw-r--r--   0        0        0     4036 2023-04-19 06:06:04.246545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/cg_conv.py
+-rw-r--r--   0        0        0     6444 2023-04-19 06:06:04.246545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/cheb_conv.py
+-rw-r--r--   0        0        0     5303 2023-04-19 06:06:04.246545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/cluster_gcn_conv.py
+-rw-r--r--   0        0        0      251 2023-04-19 06:06:04.246545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/cugraph/__init__.py
+-rw-r--r--   0        0        0     8195 2023-04-19 06:06:04.246545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/cugraph/base.py
+-rw-r--r--   0        0        0     2849 2023-04-19 06:06:04.246545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/cugraph/gat_conv.py
+-rw-r--r--   0        0        0     4218 2023-04-19 06:06:04.246545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/cugraph/rgcn_conv.py
+-rw-r--r--   0        0        0     2802 2023-04-19 06:06:04.246545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/cugraph/sage_conv.py
+-rw-r--r--   0        0        0    12105 2023-04-19 06:06:04.246545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/dna_conv.py
+-rw-r--r--   0        0        0     5550 2023-04-19 06:06:04.246545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/edge_conv.py
+-rw-r--r--   0        0        0    10482 2023-04-19 06:06:04.246545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/eg_conv.py
+-rw-r--r--   0        0        0     7927 2023-04-19 06:06:04.246545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/fa_conv.py
+-rw-r--r--   0        0        0     4453 2023-04-19 06:06:04.246545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/feast_conv.py
+-rw-r--r--   0        0        0     6332 2023-04-19 06:06:04.246545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/film_conv.py
+-rw-r--r--   0        0        0     4242 2023-04-19 06:06:04.246545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/fused_gat_conv.py
+-rw-r--r--   0        0        0    13610 2023-04-19 06:06:04.246545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/gat_conv.py
+-rw-r--r--   0        0        0     3582 2023-04-19 06:06:04.246545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/gated_graph_conv.py
+-rw-r--r--   0        0        0    12423 2023-04-19 06:06:04.246545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/gatv2_conv.py
+-rw-r--r--   0        0        0     7022 2023-04-19 06:06:04.246545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/gcn2_conv.py
+-rw-r--r--   0        0        0     9333 2023-04-19 06:06:04.246545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/gcn_conv.py
+-rw-r--r--   0        0        0     9992 2023-04-19 06:06:04.246545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/gen_conv.py
+-rw-r--r--   0        0        0     7512 2023-04-19 06:06:04.246545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/general_conv.py
+-rw-r--r--   0        0        0     7444 2023-04-19 06:06:04.246545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/gin_conv.py
+-rw-r--r--   0        0        0     8320 2023-04-19 06:06:04.246545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/gmm_conv.py
+-rw-r--r--   0        0        0     5764 2023-04-19 06:06:04.246545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/gps_conv.py
+-rw-r--r--   0        0        0     3547 2023-04-19 06:06:04.246545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/graph_conv.py
+-rw-r--r--   0        0        0     5023 2023-04-19 06:06:04.246545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/gravnet_conv.py
+-rw-r--r--   0        0        0     7354 2023-04-19 06:06:04.246545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/han_conv.py
+-rw-r--r--   0        0        0     6063 2023-04-19 06:06:04.246545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/heat_conv.py
+-rw-r--r--   0        0        0     6470 2023-04-19 06:06:04.246545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/hetero_conv.py
+-rw-r--r--   0        0        0     9001 2023-04-19 06:06:04.246545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/hgt_conv.py
+-rw-r--r--   0        0        0     7580 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/hypergraph_conv.py
+-rw-r--r--   0        0        0     3523 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/le_conv.py
+-rw-r--r--   0        0        0     2418 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/lg_conv.py
+-rw-r--r--   0        0        0    11524 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/message_passing.jinja
+-rw-r--r--   0        0        0    40230 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/message_passing.py
+-rw-r--r--   0        0        0     4321 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/mf_conv.py
+-rw-r--r--   0        0        0     4743 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/nn_conv.py
+-rw-r--r--   0        0        0     4928 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/pan_conv.py
+-rw-r--r--   0        0        0     4916 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/pdn_conv.py
+-rw-r--r--   0        0        0     8242 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/pna_conv.py
+-rw-r--r--   0        0        0     4522 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/point_conv.py
+-rw-r--r--   0        0        0     3288 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/point_gnn_conv.py
+-rw-r--r--   0        0        0     5889 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/point_transformer_conv.py
+-rw-r--r--   0        0        0     5422 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/ppf_conv.py
+-rw-r--r--   0        0        0     4180 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/res_gated_graph_conv.py
+-rw-r--r--   0        0        0    22785 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/rgat_conv.py
+-rw-r--r--   0        0        0    14623 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/rgcn_conv.py
+-rw-r--r--   0        0        0     5813 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/sage_conv.py
+-rw-r--r--   0        0        0     4597 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/sg_conv.py
+-rw-r--r--   0        0        0     6283 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/signed_conv.py
+-rw-r--r--   0        0        0     3142 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/simple_conv.py
+-rw-r--r--   0        0        0     6330 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/spline_conv.py
+-rw-r--r--   0        0        0     5185 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/ssg_conv.py
+-rw-r--r--   0        0        0    11980 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/supergat_conv.py
+-rw-r--r--   0        0        0     4215 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/tag_conv.py
+-rw-r--r--   0        0        0     9425 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/transformer_conv.py
+-rw-r--r--   0        0        0      823 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/utils/__init__.py
+-rw-r--r--   0        0        0     2692 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/utils/cheatsheet.py
+-rw-r--r--   0        0        0      186 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/utils/helpers.py
+-rw-r--r--   0        0        0     3267 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/utils/inspector.py
+-rw-r--r--   0        0        0      679 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/utils/jit.py
+-rw-r--r--   0        0        0     3859 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/utils/typing.py
+-rw-r--r--   0        0        0     3103 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/wl_conv.py
+-rw-r--r--   0        0        0     2349 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/wl_conv_continuous.py
+-rw-r--r--   0        0        0     5955 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/x_conv.py
+-rw-r--r--   0        0        0     3960 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/data_parallel.py
+-rw-r--r--   0        0        0      712 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/dense/__init__.py
+-rw-r--r--   0        0        0     4228 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/dense/dense_gat_conv.py
+-rw-r--r--   0        0        0     2989 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/dense/dense_gcn_conv.py
+-rw-r--r--   0        0        0     2357 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/dense/dense_gin_conv.py
+-rw-r--r--   0        0        0     2737 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/dense/dense_graph_conv.py
+-rw-r--r--   0        0        0     2658 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/dense/dense_sage_conv.py
+-rw-r--r--   0        0        0     3050 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/dense/diff_pool.py
+-rw-r--r--   0        0        0     5671 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/dense/dmon_pool.py
+-rw-r--r--   0        0        0    15564 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/dense/linear.py
+-rw-r--r--   0        0        0     4111 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/dense/mincut_pool.py
+-rw-r--r--   0        0        0     3125 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/encoding.py
+-rw-r--r--   0        0        0       92 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/functional/__init__.py
+-rw-r--r--   0        0        0     1549 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/functional/bro.py
+-rw-r--r--   0        0        0      863 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/functional/gini.py
+-rw-r--r--   0        0        0    15559 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/fx.py
+-rw-r--r--   0        0        0     1088 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/glob.py
+-rw-r--r--   0        0        0     2457 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/inits.py
+-rw-r--r--   0        0        0      241 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/kge/__init__.py
+-rw-r--r--   0        0        0     5739 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/kge/base.py
+-rw-r--r--   0        0        0     3234 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/kge/complex.py
+-rw-r--r--   0        0        0     2462 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/kge/distmult.py
+-rw-r--r--   0        0        0      771 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/kge/loader.py
+-rw-r--r--   0        0        0     3208 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/kge/rotate.py
+-rw-r--r--   0        0        0     3088 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/kge/transe.py
+-rw-r--r--   0        0        0     8937 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/lr_scheduler.py
+-rw-r--r--   0        0        0     9464 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/model_hub.py
+-rw-r--r--   0        0        0     1612 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/models/__init__.py
+-rw-r--r--   0        0        0     6591 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/models/attentive_fp.py
+-rw-r--r--   0        0        0    10656 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/models/autoencoder.py
+-rw-r--r--   0        0        0    27754 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/models/basic_gnn.py
+-rw-r--r--   0        0        0     4138 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/models/captum.py
+-rw-r--r--   0        0        0     6799 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/models/correct_and_smooth.py
+-rw-r--r--   0        0        0     3972 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/models/deep_graph_infomax.py
+-rw-r--r--   0        0        0     4223 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/models/deepgcn.py
+-rw-r--r--   0        0        0    34432 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/models/dimenet.py
+-rw-r--r--   0        0        0     4611 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/models/dimenet_utils.py
+-rw-r--r--   0        0        0     7859 2023-04-19 06:06:04.250545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/models/gnnff.py
+-rw-r--r--   0        0        0     5381 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/models/graph_unet.py
+-rw-r--r--   0        0        0     3397 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/models/jumping_knowledge.py
+-rw-r--r--   0        0        0     3725 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/models/label_prop.py
+-rw-r--r--   0        0        0    10918 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/models/lightgcn.py
+-rw-r--r--   0        0        0     7901 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/models/linkx.py
+-rw-r--r--   0        0        0     2566 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/models/mask_label.py
+-rw-r--r--   0        0        0     6529 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/models/meta.py
+-rw-r--r--   0        0        0    10318 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/models/metapath2vec.py
+-rw-r--r--   0        0        0     8676 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/models/mlp.py
+-rw-r--r--   0        0        0     7171 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/models/node2vec.py
+-rw-r--r--   0        0        0     8987 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/models/re_net.py
+-rw-r--r--   0        0        0     5789 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/models/rect.py
+-rw-r--r--   0        0        0    11818 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/models/rev_gnn.py
+-rw-r--r--   0        0        0    16599 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/models/schnet.py
+-rw-r--r--   0        0        0     9840 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/models/signed_gcn.py
+-rw-r--r--   0        0        0    11587 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/models/tgn.py
+-rw-r--r--   0        0        0     1576 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/module_dict.py
+-rw-r--r--   0        0        0      638 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/norm/__init__.py
+-rw-r--r--   0        0        0     8258 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/norm/batch_norm.py
+-rw-r--r--   0        0        0     4706 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/norm/diff_group_norm.py
+-rw-r--r--   0        0        0     2715 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/norm/graph_norm.py
+-rw-r--r--   0        0        0     1492 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/norm/graph_size_norm.py
+-rw-r--r--   0        0        0     4670 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/norm/instance_norm.py
+-rw-r--r--   0        0        0     6673 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/norm/layer_norm.py
+-rw-r--r--   0        0        0     1311 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/norm/mean_subtraction_norm.py
+-rw-r--r--   0        0        0     1654 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/norm/msg_norm.py
+-rw-r--r--   0        0        0     2809 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/norm/pair_norm.py
+-rw-r--r--   0        0        0     1453 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/parameter_dict.py
+-rw-r--r--   0        0        0    10718 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/pool/__init__.py
+-rw-r--r--   0        0        0     6868 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/pool/asap.py
+-rw-r--r--   0        0        0     3749 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/pool/avg_pool.py
+-rw-r--r--   0        0        0     3345 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/pool/base.py
+-rw-r--r--   0        0        0       56 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/pool/connect/__init__.py
+-rw-r--r--   0        0        0     1369 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/pool/connect/base.py
+-rw-r--r--   0        0        0      273 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/pool/consecutive.py
+-rw-r--r--   0        0        0     1600 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/pool/decimation.py
+-rw-r--r--   0        0        0     8567 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/pool/edge_pool.py
+-rw-r--r--   0        0        0     3627 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/pool/glob.py
+-rw-r--r--   0        0        0     1292 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/pool/graclus.py
+-rw-r--r--   0        0        0     4045 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/pool/max_pool.py
+-rw-r--r--   0        0        0     4832 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/pool/mem_pool.py
+-rw-r--r--   0        0        0     4353 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/pool/pan_pool.py
+-rw-r--r--   0        0        0      631 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/pool/pool.py
+-rw-r--r--   0        0        0     5919 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/pool/sag_pool.py
+-rw-r--r--   0        0        0       54 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/pool/select/__init__.py
+-rw-r--r--   0        0        0     1308 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/pool/select/base.py
+-rw-r--r--   0        0        0     8347 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/pool/topk_pool.py
+-rw-r--r--   0        0        0     2727 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/pool/voxel_grid.py
+-rw-r--r--   0        0        0      412 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/reshape.py
+-rw-r--r--   0        0        0     5675 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/resolver.py
+-rw-r--r--   0        0        0     1071 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/sequential.jinja
+-rw-r--r--   0        0        0     4577 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/sequential.py
+-rw-r--r--   0        0        0     5616 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/summary.py
+-rw-r--r--   0        0        0     1282 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/to_fixed_size_transformer.py
+-rw-r--r--   0        0        0     6395 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/to_hetero_module.py
+-rw-r--r--   0        0        0    18095 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/to_hetero_transformer.py
+-rw-r--r--   0        0        0    23139 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/to_hetero_with_bases_transformer.py
+-rw-r--r--   0        0        0      102 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/unpool/__init__.py
+-rw-r--r--   0        0        0     2586 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/unpool/knn_interpolate.py
+-rw-r--r--   0        0        0      803 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/profile/__init__.py
+-rw-r--r--   0        0        0     3356 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/profile/benchmark.py
+-rw-r--r--   0        0        0    10364 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/profile/profile.py
+-rw-r--r--   0        0        0    16665 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/profile/profiler.py
+-rw-r--r--   0        0        0     4563 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/profile/utils.py
+-rw-r--r--   0        0        0     1391 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/resolver.py
+-rw-r--r--   0        0        0      481 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/sampler/__init__.py
+-rw-r--r--   0        0        0    22714 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/sampler/base.py
+-rw-r--r--   0        0        0     2734 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/sampler/hgt_sampler.py
+-rw-r--r--   0        0        0    26144 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/sampler/neighbor_sampler.py
+-rw-r--r--   0        0        0     5252 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/sampler/utils.py
+-rw-r--r--   0        0        0      354 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/seed.py
+-rw-r--r--   0        0        0      710 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/testing/__init__.py
+-rw-r--r--   0        0        0     4368 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/testing/asserts.py
+-rw-r--r--   0        0        0     1933 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/testing/data.py
+-rw-r--r--   0        0        0     3842 2023-04-19 06:06:04.254545 pyg-nightly-2.4.0.dev20230419/torch_geometric/testing/decorators.py
+-rw-r--r--   0        0        0     1847 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/testing/feature_store.py
+-rw-r--r--   0        0        0     1009 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/testing/graph_store.py
+-rw-r--r--   0        0        0     3971 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/__init__.py
+-rw-r--r--   0        0        0    13966 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/add_metapaths.py
+-rw-r--r--   0        0        0     4838 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/add_positional_encoding.py
+-rw-r--r--   0        0        0     2019 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/add_self_loops.py
+-rw-r--r--   0        0        0     1141 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/base_transform.py
+-rw-r--r--   0        0        0     1937 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/cartesian.py
+-rw-r--r--   0        0        0      641 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/center.py
+-rw-r--r--   0        0        0     1659 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/compose.py
+-rw-r--r--   0        0        0     1961 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/constant.py
+-rw-r--r--   0        0        0     1223 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/delaunay.py
+-rw-r--r--   0        0        0     1810 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/distance.py
+-rw-r--r--   0        0        0     1035 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/face_to_edge.py
+-rw-r--r--   0        0        0     2953 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/feature_propagation.py
+-rw-r--r--   0        0        0     2368 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/fixed_points.py
+-rw-r--r--   0        0        0     1398 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/gcn_norm.py
+-rw-r--r--   0        0        0    24216 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/gdc.py
+-rw-r--r--   0        0        0     1019 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/generate_mesh_normals.py
+-rw-r--r--   0        0        0     2512 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/grid_sampling.py
+-rw-r--r--   0        0        0     2544 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/knn_graph.py
+-rw-r--r--   0        0        0     2466 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/laplacian_lambda_max.py
+-rw-r--r--   0        0        0     2001 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/largest_connected_components.py
+-rw-r--r--   0        0        0     3724 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/line_graph.py
+-rw-r--r--   0        0        0     1998 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/linear_transformation.py
+-rw-r--r--   0        0        0     1699 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/local_cartesian.py
+-rw-r--r--   0        0        0     1405 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/local_degree_profile.py
+-rw-r--r--   0        0        0     4600 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/mask.py
+-rw-r--r--   0        0        0      979 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/normalize_features.py
+-rw-r--r--   0        0        0     1739 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/normalize_rotation.py
+-rw-r--r--   0        0        0      621 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/normalize_scale.py
+-rw-r--r--   0        0        0     1534 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/one_hot_degree.py
+-rw-r--r--   0        0        0    21080 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/pad.py
+-rw-r--r--   0        0        0     1794 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/point_pair_features.py
+-rw-r--r--   0        0        0     2127 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/polar.py
+-rw-r--r--   0        0        0     2051 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/radius_graph.py
+-rw-r--r--   0        0        0      989 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/random_flip.py
+-rw-r--r--   0        0        0     1511 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/random_jitter.py
+-rw-r--r--   0        0        0    14298 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/random_link_split.py
+-rw-r--r--   0        0        0     5769 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/random_node_split.py
+-rw-r--r--   0        0        0     1904 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/random_rotate.py
+-rw-r--r--   0        0        0     1216 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/random_scale.py
+-rw-r--r--   0        0        0     1320 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/random_shear.py
+-rw-r--r--   0        0        0     1806 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/remove_duplicated_edges.py
+-rw-r--r--   0        0        0     2284 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/remove_isolated_nodes.py
+-rw-r--r--   0        0        0      960 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/remove_training_classes.py
+-rw-r--r--   0        0        0     6112 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/rooted_subgraph.py
+-rw-r--r--   0        0        0     2141 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/sample_points.py
+-rw-r--r--   0        0        0     2129 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/sign.py
+-rw-r--r--   0        0        0     2242 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/spherical.py
+-rw-r--r--   0        0        0     1003 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/svd_feature_reduction.py
+-rw-r--r--   0        0        0     1608 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/target_indegree.py
+-rw-r--r--   0        0        0     2328 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/to_dense.py
+-rw-r--r--   0        0        0     1456 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/to_device.py
+-rw-r--r--   0        0        0     5354 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/to_sparse_tensor.py
+-rw-r--r--   0        0        0     2622 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/to_superpixels.py
+-rw-r--r--   0        0        0     2973 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/to_undirected.py
+-rw-r--r--   0        0        0     1215 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/two_hop.py
+-rw-r--r--   0        0        0     2784 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/virtual_node.py
+-rw-r--r--   0        0        0     8111 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/typing.py
+-rw-r--r--   0        0        0     4474 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/__init__.py
+-rw-r--r--   0        0        0     2347 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/assortativity.py
+-rw-r--r--   0        0        0     9080 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/augmentation.py
+-rw-r--r--   0        0        0     5037 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/coalesce.py
+-rw-r--r--   0        0        0    19515 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/convert.py
+-rw-r--r--   0        0        0     1018 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/degree.py
+-rw-r--r--   0        0        0    11323 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/dropout.py
+-rw-r--r--   0        0        0     1657 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/embedding.py
+-rw-r--r--   0        0        0     4042 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/geodesic.py
+-rw-r--r--   0        0        0     3755 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/get_laplacian.py
+-rw-r--r--   0        0        0     4424 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/get_mesh_laplacian.py
+-rw-r--r--   0        0        0     2536 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/grid.py
+-rw-r--r--   0        0        0     5044 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/hetero.py
+-rw-r--r--   0        0        0     4818 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/homophily.py
+-rw-r--r--   0        0        0     3574 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/isolated.py
+-rw-r--r--   0        0        0    15855 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/loop.py
+-rw-r--r--   0        0        0     1884 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/mask.py
+-rw-r--r--   0        0        0      608 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/mixin.py
+-rw-r--r--   0        0        0    14643 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/negative_sampling.py
+-rw-r--r--   0        0        0     3344 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/nested.py
+-rw-r--r--   0        0        0     1169 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/normalized_cut.py
+-rw-r--r--   0        0        0     1468 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/num_nodes.py
+-rw-r--r--   0        0        0     1404 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/one_hot.py
+-rw-r--r--   0        0        0     5154 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/random.py
+-rw-r--r--   0        0        0      361 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/repeat.py
+-rw-r--r--   0        0        0     7429 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/scatter.py
+-rw-r--r--   0        0        0     1110 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/segment.py
+-rw-r--r--   0        0        0     2149 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/select.py
+-rw-r--r--   0        0        0     6016 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/smiles.py
+-rw-r--r--   0        0        0     2718 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/softmax.py
+-rw-r--r--   0        0        0     1017 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/sort.py
+-rw-r--r--   0        0        0     3034 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/sort_edge_index.py
+-rw-r--r--   0        0        0    11835 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/sparse.py
+-rw-r--r--   0        0        0     5547 2023-04-19 06:06:04.258545 pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/spmm.py
+-rw-r--r--   0        0        0    12370 2023-04-19 06:06:04.262545 pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/subgraph.py
+-rw-r--r--   0        0        0     3439 2023-04-19 06:06:04.262545 pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/to_dense_adj.py
+-rw-r--r--   0        0        0     4267 2023-04-19 06:06:04.262545 pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/to_dense_batch.py
+-rw-r--r--   0        0        0     3489 2023-04-19 06:06:04.262545 pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/train_test_split_edges.py
+-rw-r--r--   0        0        0     4867 2023-04-19 06:06:04.262545 pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/tree_decomposition.py
+-rw-r--r--   0        0        0     6350 2023-04-19 06:06:04.262545 pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/trim_to_layer.py
+-rw-r--r--   0        0        0     2125 2023-04-19 06:06:04.262545 pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/unbatch.py
+-rw-r--r--   0        0        0     5770 2023-04-19 06:06:04.262545 pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/undirected.py
+-rw-r--r--   0        0        0      123 2023-04-19 06:06:04.262545 pyg-nightly-2.4.0.dev20230419/torch_geometric/visualization/__init__.py
+-rw-r--r--   0        0        0     4149 2023-04-19 06:06:04.262545 pyg-nightly-2.4.0.dev20230419/torch_geometric/visualization/graph.py
+-rw-r--r--   0        0        0      388 2023-04-19 06:06:04.262545 pyg-nightly-2.4.0.dev20230419/torch_geometric/visualization/influence.py
+-rw-r--r--   0        0        0    63628 1970-01-01 00:00:00.000000 pyg-nightly-2.4.0.dev20230419/PKG-INFO
```

### Comparing `pyg-nightly-2.4.0.dev20230418/README.md` & `pyg-nightly-2.4.0.dev20230419/README.md`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/pyproject.toml` & `pyg-nightly-2.4.0.dev20230419/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires=["flit_core >=3.2,<4"]
 build-backend="flit_core.buildapi"
 
 [project]
 name="pyg-nightly"
-version="2.4.0.dev20230418"
+version="2.4.0.dev20230419"
 authors=[
     {name="Matthias Fey", email="matthias@pyg.org"},
 ]
 description="Graph Neural Network Library for PyTorch"
 readme="README.md"
 requires-python=">=3.7"
 keywords=[
@@ -163,7 +163,10 @@
     "raise",
     "except",
     "register_parameter",
     "warn",
     "torch.cuda.is_available",
     "WITH_PT2",
 ]
+
+[tool.flake8]
+ignore = ["F811", "W503", "W504"]
```

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/__init__.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from .experimental import (is_experimental_mode_enabled, experimental_mode,
                            set_experimental_mode)
 from .lazy_loader import LazyLoader
 
 contrib = LazyLoader('contrib', globals(), 'torch_geometric.contrib')
 graphgym = LazyLoader('graphgym', globals(), 'torch_geometric.graphgym')
 
-__version__ = '2.4.0.dev20230418'
+__version__ = '2.4.0.dev20230419'
 
 __all__ = [
     'seed_everything',
     'get_home_dir',
     'set_home_dir',
     'compile',
     'is_debug_enabled',
```

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/compile.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/compile.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/contrib/explain/graphmask_explainer.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/contrib/explain/graphmask_explainer.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/contrib/explain/pgm_explainer.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/contrib/explain/pgm_explainer.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/contrib/nn/models/rbcd_attack.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/contrib/nn/models/rbcd_attack.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/data/__init__.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/data/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/data/batch.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/data/batch.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/data/collate.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/data/collate.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/data/data.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/data/data.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/data/datapipes.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/data/datapipes.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/data/dataset.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/data/dataset.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/data/download.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/data/download.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/data/extract.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/data/extract.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/data/feature_store.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/data/feature_store.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/data/graph_store.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/data/graph_store.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/data/hetero_data.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/data/hetero_data.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/data/in_memory_dataset.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/data/in_memory_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/data/lightning/datamodule.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/data/lightning/datamodule.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/data/remote_backend_utils.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/data/remote_backend_utils.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/data/separate.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/data/separate.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/data/storage.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/data/storage.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/data/summary.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/data/summary.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/data/temporal.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/data/temporal.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/data/view.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/data/view.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/__init__.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/actor.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/actor.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/airfrans.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/airfrans.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/airports.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/airports.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/amazon.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/amazon.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/amazon_products.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/amazon_products.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/aminer.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/aminer.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/aqsol.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/aqsol.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/attributed_graph_dataset.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/attributed_graph_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/ba2motif_dataset.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/ba2motif_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/ba_multi_shapes.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/ba_multi_shapes.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/ba_shapes.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/ba_shapes.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/bitcoin_otc.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/bitcoin_otc.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/citation_full.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/citation_full.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/coauthor.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/coauthor.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/coma.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/coma.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/dblp.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/dblp.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/dbp15k.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/dbp15k.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/deezer_europe.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/deezer_europe.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/dgraph.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/dgraph.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/dynamic_faust.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/dynamic_faust.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/elliptic.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/elliptic.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/elliptic_temporal.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/elliptic_temporal.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/email_eu_core.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/email_eu_core.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/entities.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/entities.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/explainer_dataset.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/explainer_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/facebook.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/facebook.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/fake.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/fake.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/faust.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/faust.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/flickr.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/flickr.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/freebase.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/freebase.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/gdelt.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/gdelt.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/ged_dataset.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/ged_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/gemsec.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/gemsec.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/geometry.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/geometry.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/github.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/github.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/gnn_benchmark_dataset.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/gnn_benchmark_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/graph_generator/ba_graph.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/graph_generator/ba_graph.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/graph_generator/base.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/graph_generator/base.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/graph_generator/er_graph.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/graph_generator/er_graph.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/graph_generator/grid_graph.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/graph_generator/grid_graph.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/heterophilous_graph_dataset.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/heterophilous_graph_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/hgb_dataset.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/hgb_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/hydro_net.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/hydro_net.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/icews.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/icews.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/imdb.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/imdb.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/infection_dataset.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/infection_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/jodie.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/jodie.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/karate.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/karate.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/last_fm.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/last_fm.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/lastfm_asia.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/lastfm_asia.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/linkx_dataset.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/linkx_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/lrgb.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/lrgb.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/malnet_tiny.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/malnet_tiny.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/md17.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/md17.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/mixhop_synthetic_dataset.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/mixhop_synthetic_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/mnist_superpixels.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/mnist_superpixels.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/modelnet.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/modelnet.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/molecule_net.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/molecule_net.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/motif_generator/base.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/motif_generator/base.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/motif_generator/custom.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/motif_generator/custom.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/motif_generator/cycle.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/motif_generator/cycle.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/motif_generator/house.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/motif_generator/house.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/movie_lens.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/movie_lens.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/nell.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/nell.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/ogb_mag.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/ogb_mag.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/omdb.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/omdb.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/particle.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/particle.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/pascal.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/pascal.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/pascal_pf.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/pascal_pf.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/pcpnet_dataset.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/pcpnet_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/planetoid.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/planetoid.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/polblogs.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/polblogs.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/ppi.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/ppi.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/qm7.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/qm7.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/qm9.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/qm9.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/reddit.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/reddit.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/reddit2.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/reddit2.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/rel_link_pred_dataset.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/rel_link_pred_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/s3dis.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/s3dis.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/sbm_dataset.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/sbm_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/shapenet.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/shapenet.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/shrec2016.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/shrec2016.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/snap_dataset.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/snap_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/suite_sparse.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/suite_sparse.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/taobao.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/taobao.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/tosca.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/tosca.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/tu_dataset.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/tu_dataset.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/twitch.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/twitch.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/upfd.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/upfd.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/utils/cheatsheet.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/utils/cheatsheet.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/webkb.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/webkb.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/wikics.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/wikics.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/wikipedia_network.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/wikipedia_network.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/willow_object_class.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/willow_object_class.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/word_net.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/word_net.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/yelp.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/yelp.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/datasets/zinc.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/datasets/zinc.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/debug.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/debug.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/deprecation.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/deprecation.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/experimental.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/experimental.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/explain/algorithm/attention_explainer.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/explain/algorithm/attention_explainer.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/explain/algorithm/base.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/explain/algorithm/base.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/explain/algorithm/captum.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/explain/algorithm/captum.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/explain/algorithm/captum_explainer.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/explain/algorithm/captum_explainer.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/explain/algorithm/dummy_explainer.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/explain/algorithm/dummy_explainer.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/explain/algorithm/gnn_explainer.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/explain/algorithm/gnn_explainer.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/explain/algorithm/pg_explainer.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/explain/algorithm/pg_explainer.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/explain/algorithm/utils.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/explain/algorithm/utils.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/explain/config.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/explain/config.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/explain/explainer.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/explain/explainer.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/explain/explanation.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/explain/explanation.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/explain/metric/basic.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/explain/metric/basic.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/explain/metric/faithfulness.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/explain/metric/faithfulness.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/explain/metric/fidelity.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/explain/metric/fidelity.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/__init__.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/checkpoint.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/checkpoint.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/cmd_args.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/cmd_args.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/config.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/config.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/config_store.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/config_store.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/contrib/layer/generalconv.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/contrib/layer/generalconv.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/loader.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/loader.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/logger.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/logger.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/loss.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/loss.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/model_builder.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/model_builder.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/models/__init__.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/models/act.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/models/act.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/models/encoder.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/models/encoder.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/models/gnn.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/models/gnn.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/models/head.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/models/head.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/models/layer.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/models/layer.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/models/transform.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/models/transform.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/optim.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/optim.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/register.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/register.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/train.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/train.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/utils/__init__.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/utils/agg_runs.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/utils/agg_runs.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/utils/comp_budget.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/utils/comp_budget.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/utils/device.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/utils/device.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/utils/epoch.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/utils/epoch.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/utils/io.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/utils/io.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/graphgym/utils/plot.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/graphgym/utils/plot.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/home.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/home.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/io/__init__.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/io/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/io/npz.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/io/npz.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/io/obj.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/io/obj.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/io/off.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/io/off.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/io/planetoid.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/io/planetoid.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/io/sdf.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/io/sdf.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/io/tu.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/io/tu.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/io/txt_array.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/io/txt_array.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/lazy_loader.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/lazy_loader.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/loader/__init__.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/loader/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/loader/base.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/loader/base.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/loader/cluster.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/loader/cluster.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/loader/data_list_loader.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/loader/data_list_loader.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/loader/dataloader.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/loader/dataloader.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/loader/dense_data_loader.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/loader/dense_data_loader.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/loader/dynamic_batch_sampler.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/loader/dynamic_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/loader/graph_saint.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/loader/graph_saint.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/loader/hgt_loader.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/loader/hgt_loader.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/loader/imbalanced_sampler.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/loader/imbalanced_sampler.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/loader/link_loader.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/loader/link_loader.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/loader/link_neighbor_loader.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/loader/link_neighbor_loader.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Callable, Dict, List, Optional, Tuple, Union
 
 from torch_geometric.data import Data, FeatureStore, GraphStore, HeteroData
 from torch_geometric.loader.link_loader import LinkLoader
 from torch_geometric.sampler import NegativeSampling, NeighborSampler
+from torch_geometric.sampler.base import SubgraphType
 from torch_geometric.typing import EdgeType, InputEdges, OptTensor
 
 
 class LinkNeighborLoader(LinkLoader):
     r"""A link-based data loader derived as an extension of the node-based
     :class:`torch_geometric.loader.NeighborLoader`.
     This loader allows for mini-batch training of GNNs on large-scale graphs
@@ -93,16 +94,24 @@
             :obj:`edge_label_index`. If set, temporal sampling will be
             used such that neighbors are guaranteed to fulfill temporal
             constraints, *i.e.*, neighbors have an earlier timestamp than
             the ouput edge. The :obj:`time_attr` needs to be set for this
             to work. (default: :obj:`None`)
         replace (bool, optional): If set to :obj:`True`, will sample with
             replacement. (default: :obj:`False`)
-        directed (bool, optional): If set to :obj:`False`, will include all
-            edges between all sampled nodes. (default: :obj:`True`)
+        subgraph_type (SubgraphType or str, optional): The type of the returned
+            subgraph.
+            If set to :obj:`"directional"`, the returned subgraph only holds
+            the sampled (directed) edges which are necessary to compute
+            representations for the sampled seed nodes.
+            If set to :obj:`"bidirectional"`, sampled edges are converted to
+            bidirectional edges.
+            If set to :obj:`"induced"`, the returned subgraph contains the
+            induced subgraph of all sampled nodes.
+            (default: :obj:`"directional"`)
         disjoint (bool, optional): If set to :obj: `True`, each seed node will
             create its own disjoint subgraph.
             If set to :obj:`True`, mini-batch outputs will have a :obj:`batch`
             vector holding the mapping of nodes to their respective subgraph.
             Will get automatically set to :obj:`True` in case of temporal
             sampling. (default: :obj:`False`)
         temporal_strategy (str, optional): The sampling strategy when using
@@ -177,25 +186,26 @@
         self,
         data: Union[Data, HeteroData, Tuple[FeatureStore, GraphStore]],
         num_neighbors: Union[List[int], Dict[EdgeType, List[int]]],
         edge_label_index: InputEdges = None,
         edge_label: OptTensor = None,
         edge_label_time: OptTensor = None,
         replace: bool = False,
-        directed: bool = True,
+        subgraph_type: Union[SubgraphType, str] = 'directional',
         disjoint: bool = False,
         temporal_strategy: str = 'uniform',
         neg_sampling: Optional[NegativeSampling] = None,
         neg_sampling_ratio: Optional[Union[int, float]] = None,
         time_attr: Optional[str] = None,
         transform: Optional[Callable] = None,
         transform_sampler_output: Optional[Callable] = None,
         is_sorted: bool = False,
         filter_per_worker: bool = False,
         neighbor_sampler: Optional[NeighborSampler] = None,
+        directed: bool = True,  # Deprecated.
         **kwargs,
     ):
         if (edge_label_time is not None) != (time_attr is not None):
             raise ValueError(
                 f"Received conflicting 'edge_label_time' and 'time_attr' "
                 f"arguments: 'edge_label_time' is "
                 f"{'set' if edge_label_time is not None else 'not set'} "
@@ -203,20 +213,21 @@
                 f"{'set' if time_attr is not None else 'not set'}.")
 
         if neighbor_sampler is None:
             neighbor_sampler = NeighborSampler(
                 data,
                 num_neighbors=num_neighbors,
                 replace=replace,
-                directed=directed,
+                subgraph_type=subgraph_type,
                 disjoint=disjoint,
                 temporal_strategy=temporal_strategy,
                 time_attr=time_attr,
                 is_sorted=is_sorted,
                 share_memory=kwargs.get('num_workers', 0) > 0,
+                directed=directed,
             )
 
         super().__init__(
             data=data,
             link_sampler=neighbor_sampler,
             edge_label_index=edge_label_index,
             edge_label=edge_label,
```

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/loader/mixin.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/loader/mixin.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/loader/neighbor_loader.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/loader/neighbor_loader.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Callable, Dict, List, Optional, Tuple, Union
 
 from torch_geometric.data import Data, FeatureStore, GraphStore, HeteroData
 from torch_geometric.loader.node_loader import NodeLoader
 from torch_geometric.sampler import NeighborSampler
+from torch_geometric.sampler.base import SubgraphType
 from torch_geometric.typing import EdgeType, InputNodes, OptTensor
 
 
 class NeighborLoader(NodeLoader):
     r"""A data loader that performs neighbor sampling as introduced in the
     `"Inductive Representation Learning on Large Graphs"
     <https://arxiv.org/abs/1706.02216>`_ paper.
@@ -121,16 +122,24 @@
         input_time (torch.Tensor, optional): Optional values to override the
             timestamp for the input nodes given in :obj:`input_nodes`. If not
             set, will use the timestamps in :obj:`time_attr` as default (if
             present). The :obj:`time_attr` needs to be set for this to work.
             (default: :obj:`None`)
         replace (bool, optional): If set to :obj:`True`, will sample with
             replacement. (default: :obj:`False`)
-        directed (bool, optional): If set to :obj:`False`, will include all
-            edges between all sampled nodes. (default: :obj:`True`)
+        subgraph_type (SubgraphType or str, optional): The type of the returned
+            subgraph.
+            If set to :obj:`"directional"`, the returned subgraph only holds
+            the sampled (directed) edges which are necessary to compute
+            representations for the sampled seed nodes.
+            If set to :obj:`"bidirectional"`, sampled edges are converted to
+            bidirectional edges.
+            If set to :obj:`"induced"`, the returned subgraph contains the
+            induced subgraph of all sampled nodes.
+            (default: :obj:`"directional"`)
         disjoint (bool, optional): If set to :obj: `True`, each seed node will
             create its own disjoint subgraph.
             If set to :obj:`True`, mini-batch outputs will have a :obj:`batch`
             vector holding the mapping of nodes to their respective subgraph.
             Will get automatically set to :obj:`True` in case of temporal
             sampling. (default: :obj:`False`)
         temporal_strategy (str, optional): The sampling strategy when using
@@ -174,41 +183,43 @@
     def __init__(
         self,
         data: Union[Data, HeteroData, Tuple[FeatureStore, GraphStore]],
         num_neighbors: Union[List[int], Dict[EdgeType, List[int]]],
         input_nodes: InputNodes = None,
         input_time: OptTensor = None,
         replace: bool = False,
-        directed: bool = True,
+        subgraph_type: Union[SubgraphType, str] = 'directional',
         disjoint: bool = False,
         temporal_strategy: str = 'uniform',
         time_attr: Optional[str] = None,
         transform: Optional[Callable] = None,
         transform_sampler_output: Optional[Callable] = None,
         is_sorted: bool = False,
         filter_per_worker: bool = False,
         neighbor_sampler: Optional[NeighborSampler] = None,
+        directed: bool = True,  # Deprecated.
         **kwargs,
     ):
         if input_time is not None and time_attr is None:
             raise ValueError("Received conflicting 'input_time' and "
                              "'time_attr' arguments: 'input_time' is set "
                              "while 'time_attr' is not set.")
 
         if neighbor_sampler is None:
             neighbor_sampler = NeighborSampler(
                 data,
                 num_neighbors=num_neighbors,
                 replace=replace,
-                directed=directed,
+                subgraph_type=subgraph_type,
                 disjoint=disjoint,
                 temporal_strategy=temporal_strategy,
                 time_attr=time_attr,
                 is_sorted=is_sorted,
                 share_memory=kwargs.get('num_workers', 0) > 0,
+                directed=directed,
             )
 
         super().__init__(
             data=data,
             node_sampler=neighbor_sampler,
             input_nodes=input_nodes,
             input_time=input_time,
```

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/loader/neighbor_sampler.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/loader/neighbor_sampler.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/loader/node_loader.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/loader/node_loader.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/loader/random_node_loader.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/loader/random_node_loader.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/loader/shadow.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/loader/shadow.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/loader/temporal_dataloader.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/loader/temporal_dataloader.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/loader/utils.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/loader/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,38 +66,45 @@
             elif isinstance(value, np.ndarray):
                 index = index.cpu()
             dim = store._parent().__cat_dim__(key, value, store)
             out_store[key] = index_select(value, index, dim=dim)
 
 
 def filter_edge_store_(store: EdgeStorage, out_store: EdgeStorage, row: Tensor,
-                       col: Tensor, index: Tensor, perm: OptTensor = None):
+                       col: Tensor, index: OptTensor, perm: OptTensor = None):
     # Filters a edge storage object to only hold the edges in `index`,
     # which represents the new graph as denoted by `(row, col)`:
     for key, value in store.items():
         if key == 'edge_index':
             edge_index = torch.stack([row, col], dim=0)
             out_store.edge_index = edge_index.to(value.device)
 
         elif key == 'adj_t':
             # NOTE: We expect `(row, col)` to be sorted by `col` (CSC layout).
             row = row.to(value.device())
             col = col.to(value.device())
             edge_attr = value.storage.value()
             if edge_attr is not None:
-                index = index.to(edge_attr.device)
-                edge_attr = index_select(edge_attr, index, dim=0)
+                if index is not None:
+                    index = index.to(edge_attr.device)
+                    edge_attr = index_select(edge_attr, index, dim=0)
+                else:
+                    edge_attr = None
             sparse_sizes = out_store.size()[::-1]
             # TODO Currently, we set `is_sorted=False`, see:
             # https://github.com/pyg-team/pytorch_geometric/issues/4346
             out_store.adj_t = SparseTensor(row=col, col=row, value=edge_attr,
                                            sparse_sizes=sparse_sizes,
                                            is_sorted=False, trust_data=True)
 
         elif store.is_edge_attr(key):
+            if index is None:
+                out_store[key] = None
+                continue
+
             dim = store._parent().__cat_dim__(key, value, store)
             if isinstance(value, Tensor):
                 index = index.to(value.device)
             elif isinstance(value, np.ndarray):
                 index = index.cpu()
             if perm is None:
                 out_store[key] = index_select(value, index, dim=dim)
@@ -110,28 +117,28 @@
                     value,
                     perm[index.to(torch.int64)],
                     dim=dim,
                 )
 
 
 def filter_data(data: Data, node: Tensor, row: Tensor, col: Tensor,
-                edge: Tensor, perm: OptTensor = None) -> Data:
+                edge: OptTensor, perm: OptTensor = None) -> Data:
     # Filters a data object to only hold nodes in `node` and edges in `edge`:
     out = copy.copy(data)
     filter_node_store_(data._store, out._store, node)
     filter_edge_store_(data._store, out._store, row, col, edge, perm)
     return out
 
 
 def filter_hetero_data(
     data: HeteroData,
     node_dict: Dict[NodeType, Tensor],
     row_dict: Dict[EdgeType, Tensor],
     col_dict: Dict[EdgeType, Tensor],
-    edge_dict: Dict[EdgeType, Tensor],
+    edge_dict: Dict[EdgeType, OptTensor],
     perm_dict: Optional[Dict[EdgeType, OptTensor]] = None,
 ) -> HeteroData:
     # Filters a heterogeneous data object to only hold nodes in `node` and
     # edges in `edge` for each node and edge type, respectively:
     out = copy.copy(data)
 
     for node_type in out.node_types:
@@ -165,15 +172,15 @@
 
 def filter_custom_store(
     feature_store: FeatureStore,
     graph_store: GraphStore,
     node_dict: Dict[str, Tensor],
     row_dict: Dict[str, Tensor],
     col_dict: Dict[str, Tensor],
-    edge_dict: Dict[str, Tensor],
+    edge_dict: Dict[str, OptTensor],
     custom_cls: Optional[HeteroData] = None,
 ) -> HeteroData:
     r"""Constructs a `HeteroData` object from a feature store that only holds
     nodes in `node` end edges in `edge` for each node and edge type,
     respectively."""
 
     # Construct a new `HeteroData` object:
```

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/loader/zip_loader.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/loader/zip_loader.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/logging.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/logging.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/__init__.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/aggr/__init__.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/aggr/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/aggr/attention.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/aggr/attention.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/aggr/base.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/aggr/base.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/aggr/basic.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/aggr/basic.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/aggr/deep_sets.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/aggr/deep_sets.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/aggr/equilibrium.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/aggr/equilibrium.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/aggr/fused.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/aggr/fused.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/aggr/gmt.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/aggr/gmt.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/aggr/gru.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/aggr/gru.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/aggr/lstm.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/aggr/lstm.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/aggr/mlp.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/aggr/mlp.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/aggr/multi.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/aggr/multi.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/aggr/quantile.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/aggr/quantile.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/aggr/scaler.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/aggr/scaler.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/aggr/set2set.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/aggr/set2set.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/aggr/set_transformer.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/aggr/set_transformer.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/aggr/sort.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/aggr/sort.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/aggr/utils.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/aggr/utils.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/__init__.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/agnn_conv.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/agnn_conv.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/antisymmetric_conv.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/antisymmetric_conv.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/appnp.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/appnp.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/arma_conv.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/arma_conv.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/cg_conv.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/cg_conv.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/cheb_conv.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/cheb_conv.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/cluster_gcn_conv.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/cluster_gcn_conv.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/cugraph/base.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/cugraph/base.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/cugraph/gat_conv.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/cugraph/gat_conv.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/cugraph/rgcn_conv.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/cugraph/rgcn_conv.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/cugraph/sage_conv.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/cugraph/sage_conv.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/dna_conv.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/dna_conv.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/edge_conv.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/edge_conv.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/eg_conv.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/eg_conv.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/fa_conv.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/fa_conv.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/feast_conv.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/feast_conv.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/film_conv.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/film_conv.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/fused_gat_conv.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/fused_gat_conv.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/gat_conv.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/gat_conv.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/gated_graph_conv.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/gated_graph_conv.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/gatv2_conv.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/gatv2_conv.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/gcn2_conv.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/gcn2_conv.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/gcn_conv.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/gcn_conv.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/gen_conv.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/gen_conv.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/general_conv.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/general_conv.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/gin_conv.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/gin_conv.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/gmm_conv.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/gmm_conv.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/gps_conv.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/gps_conv.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/graph_conv.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/graph_conv.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/gravnet_conv.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/gravnet_conv.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/han_conv.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/han_conv.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/heat_conv.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/heat_conv.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/hetero_conv.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/hetero_conv.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/hgt_conv.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/hgt_conv.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/hypergraph_conv.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/hypergraph_conv.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/le_conv.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/le_conv.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/lg_conv.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/lg_conv.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/message_passing.jinja` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/message_passing.jinja`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/message_passing.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/message_passing.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/mf_conv.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/mf_conv.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/nn_conv.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/nn_conv.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/pan_conv.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/pan_conv.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/pdn_conv.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/pdn_conv.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/pna_conv.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/pna_conv.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/point_conv.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/point_conv.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/point_gnn_conv.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/point_gnn_conv.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/point_transformer_conv.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/point_transformer_conv.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/ppf_conv.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/ppf_conv.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/res_gated_graph_conv.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/res_gated_graph_conv.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/rgat_conv.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/rgat_conv.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/rgcn_conv.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/rgcn_conv.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/sage_conv.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/sage_conv.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/sg_conv.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/sg_conv.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/signed_conv.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/signed_conv.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/simple_conv.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/simple_conv.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/spline_conv.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/spline_conv.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/ssg_conv.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/ssg_conv.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/supergat_conv.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/supergat_conv.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/tag_conv.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/tag_conv.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/transformer_conv.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/transformer_conv.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/utils/__init__.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/utils/cheatsheet.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/utils/cheatsheet.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/utils/inspector.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/utils/inspector.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/utils/jit.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/utils/jit.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/utils/typing.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/utils/typing.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/wl_conv.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/wl_conv.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/wl_conv_continuous.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/wl_conv_continuous.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/conv/x_conv.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/conv/x_conv.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/data_parallel.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/data_parallel.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/dense/__init__.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/dense/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/dense/dense_gat_conv.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/dense/dense_gat_conv.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/dense/dense_gcn_conv.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/dense/dense_gcn_conv.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/dense/dense_gin_conv.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/dense/dense_gin_conv.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/dense/dense_graph_conv.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/dense/dense_graph_conv.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/dense/dense_sage_conv.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/dense/dense_sage_conv.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/dense/diff_pool.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/dense/diff_pool.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/dense/dmon_pool.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/dense/dmon_pool.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/dense/linear.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/dense/linear.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/dense/mincut_pool.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/dense/mincut_pool.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/encoding.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/encoding.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/functional/bro.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/functional/bro.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/functional/gini.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/functional/gini.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/fx.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/fx.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/glob.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/glob.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/inits.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/inits.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/kge/base.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/kge/base.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/kge/complex.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/kge/complex.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/kge/distmult.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/kge/distmult.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/kge/loader.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/kge/loader.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/kge/rotate.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/kge/rotate.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/kge/transe.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/kge/transe.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/lr_scheduler.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/model_hub.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/model_hub.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/models/__init__.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/models/attentive_fp.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/models/attentive_fp.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/models/autoencoder.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/models/autoencoder.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/models/basic_gnn.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/models/basic_gnn.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/models/captum.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/models/captum.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/models/correct_and_smooth.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/models/correct_and_smooth.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/models/deep_graph_infomax.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/models/deep_graph_infomax.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/models/deepgcn.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/models/deepgcn.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/models/dimenet.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/models/dimenet.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/models/dimenet_utils.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/models/dimenet_utils.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/models/gnnff.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/models/gnnff.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/models/graph_unet.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/models/graph_unet.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/models/jumping_knowledge.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/models/jumping_knowledge.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/models/label_prop.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/models/label_prop.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/models/lightgcn.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/models/lightgcn.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/models/linkx.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/models/linkx.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/models/mask_label.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/models/mask_label.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/models/meta.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/models/meta.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/models/metapath2vec.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/models/metapath2vec.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/models/mlp.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/models/mlp.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/models/node2vec.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/models/node2vec.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/models/re_net.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/models/re_net.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/models/rect.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/models/rect.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/models/rev_gnn.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/models/rev_gnn.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/models/schnet.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/models/schnet.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/models/signed_gcn.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/models/signed_gcn.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/models/tgn.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/models/tgn.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/module_dict.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/module_dict.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/norm/__init__.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/norm/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/norm/batch_norm.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/norm/batch_norm.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/norm/diff_group_norm.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/norm/diff_group_norm.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/norm/graph_norm.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/norm/graph_norm.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/norm/graph_size_norm.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/norm/graph_size_norm.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/norm/instance_norm.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/norm/instance_norm.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/norm/layer_norm.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/norm/layer_norm.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/norm/mean_subtraction_norm.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/norm/mean_subtraction_norm.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/norm/msg_norm.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/norm/msg_norm.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/norm/pair_norm.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/norm/pair_norm.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/parameter_dict.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/parameter_dict.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/pool/__init__.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/pool/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/pool/asap.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/pool/asap.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/pool/avg_pool.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/pool/avg_pool.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/pool/base.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/pool/base.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/pool/connect/base.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/pool/connect/base.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/pool/decimation.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/pool/decimation.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/pool/edge_pool.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/pool/edge_pool.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/pool/glob.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/pool/glob.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/pool/graclus.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/pool/graclus.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/pool/max_pool.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/pool/max_pool.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/pool/mem_pool.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/pool/mem_pool.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/pool/pan_pool.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/pool/pan_pool.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/pool/pool.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/pool/pool.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/pool/sag_pool.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/pool/sag_pool.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/pool/select/base.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/pool/select/base.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/pool/topk_pool.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/pool/topk_pool.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/pool/voxel_grid.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/pool/voxel_grid.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/resolver.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/resolver.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/sequential.jinja` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/sequential.jinja`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/sequential.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/sequential.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/summary.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/summary.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/to_fixed_size_transformer.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/to_fixed_size_transformer.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/to_hetero_module.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/to_hetero_module.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/to_hetero_transformer.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/to_hetero_transformer.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/to_hetero_with_bases_transformer.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/to_hetero_with_bases_transformer.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/nn/unpool/knn_interpolate.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/nn/unpool/knn_interpolate.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/profile/__init__.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/profile/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 from .profile import profileit, timeit, get_stats_summary
-from .profile import trace_handler, rename_profile_file, torch_profile
+from .profile import (
+    trace_handler,
+    print_time_total,
+    rename_profile_file,
+    torch_profile,
+)
 from .utils import count_parameters
 from .utils import get_model_size
 from .utils import get_data_size
 from .utils import get_cpu_memory_from_gc
 from .utils import get_gpu_memory_from_gc
 from .utils import get_gpu_memory_from_nvidia_smi
 from .benchmark import benchmark
 
 __all__ = [
     'profileit',
     'timeit',
     'get_stats_summary',
     'trace_handler',
+    'print_time_total',
     'rename_profile_file',
     'torch_profile',
     'count_parameters',
     'get_model_size',
     'get_data_size',
     'get_cpu_memory_from_gc',
     'get_gpu_memory_from_gc',
```

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/profile/benchmark.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/profile/benchmark.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/profile/profiler.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/profile/profiler.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/profile/utils.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/profile/utils.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/resolver.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/resolver.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/sampler/base.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/sampler/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import copy
 import math
+import warnings
 from abc import ABC
+from collections import defaultdict
 from dataclasses import dataclass
 from enum import Enum
 from typing import Any, Dict, List, Optional, Union
 
 import torch
 from torch import Tensor
 
 from torch_geometric.data import Data, FeatureStore, GraphStore, HeteroData
+from torch_geometric.sampler.utils import to_bidirectional
 from torch_geometric.typing import EdgeType, EdgeTypeStr, NodeType, OptTensor
 from torch_geometric.utils.mixin import CastMixin
 
 
 class DataType(Enum):
     r"""The data type a sampler is operating on."""
     homogeneous = 'homogeneous'
@@ -31,14 +34,21 @@
             return cls.remote
 
         raise ValueError(f"Expected a 'Data', 'HeteroData', or a tuple of "
                          f"'FeatureStore' and 'GraphStore' "
                          f"(got '{type(data)}')")
 
 
+class SubgraphType(Enum):
+    r"""The type of the returned subgraph."""
+    directional = 'directional'
+    bidirectional = 'bidirectional'
+    induced = 'induced'
+
+
 @dataclass
 class NodeSamplerInput(CastMixin):
     r"""The sampling input of
     :meth:`~torch_geometric.sampler.BaseSampler.sample_from_nodes`.
 
     Args:
         input_id (torch.Tensor, optional): The indices of the data loader input
@@ -140,14 +150,31 @@
     batch: OptTensor = None
     num_sampled_nodes: Optional[List[int]] = None
     num_sampled_edges: Optional[List[int]] = None
     # TODO(manan): refine this further; it does not currently define a proper
     # API for the expected output of a sampler.
     metadata: Optional[Any] = None
 
+    def to_bidirectional(self) -> 'SamplerOutput':
+        r"""Converts the sampled subgraph into a bidirectional variant, in
+        which all sampled edges are guaranteed to be bidirectional."""
+        out = copy.copy(self)
+
+        out.row, out.col, out.edge = to_bidirectional(
+            row=self.row,
+            col=self.col,
+            rev_row=self.row,
+            rev_col=self.col,
+            edge_id=self.edge,
+            rev_edge_id=self.edge,
+        )
+        out.num_sampled_edges = None
+
+        return out
+
 
 @dataclass
 class HeteroSamplerOutput(CastMixin):
     r"""The sampling output of a :class:`~torch_geometric.sampler.BaseSampler`
     on heterogeneous graphs.
 
     Args:
@@ -179,22 +206,88 @@
             (default: :obj:`None`)
         metadata: (Any, optional): Additional metadata information.
             (default: :obj:`None`)
     """
     node: Dict[NodeType, Tensor]
     row: Dict[EdgeType, Tensor]
     col: Dict[EdgeType, Tensor]
-    edge: Optional[Dict[EdgeType, Tensor]]
+    edge: Dict[EdgeType, OptTensor]
     batch: Optional[Dict[NodeType, Tensor]] = None
     num_sampled_nodes: Optional[Dict[NodeType, List[int]]] = None
     num_sampled_edges: Optional[Dict[EdgeType, List[int]]] = None
     # TODO(manan): refine this further; it does not currently define a proper
     # API for the expected output of a sampler.
     metadata: Optional[Any] = None
 
+    def to_bidirectional(self) -> 'SamplerOutput':
+        r"""Converts the sampled subgraph into a bidirectional variant, in
+        which all sampled edges are guaranteed to be bidirectional."""
+        out = copy.copy(self)
+        out.row = copy.copy(self.row)
+        out.col = copy.copy(self.col)
+        out.edge = copy.copy(self.edge)
+
+        src_dst_dict = defaultdict(list)
+        edge_types = self.row.keys()
+        edge_types = [k for k in edge_types if not k[1].startswith('rev_')]
+        for edge_type in edge_types:
+            src, rel, dst = edge_type
+            rev_edge_type = (dst, f'rev_{rel}', src)
+
+            if src == dst and rev_edge_type not in self.row:
+                out.row[edge_type], out.col[edge_type], _ = to_bidirectional(
+                    row=self.row[edge_type],
+                    col=self.col[edge_type],
+                    rev_row=self.row[edge_type],
+                    rev_col=self.col[edge_type],
+                )
+                if out.edge is not None:
+                    out.edge[edge_type] = None
+
+            elif rev_edge_type in self.row:
+                out.row[edge_type], out.col[edge_type], _ = to_bidirectional(
+                    row=self.row[edge_type],
+                    col=self.col[edge_type],
+                    rev_row=self.row[rev_edge_type],
+                    rev_col=self.col[rev_edge_type],
+                )
+                out.row[rev_edge_type] = out.col[edge_type]
+                out.col[rev_edge_type] = out.row[edge_type]
+                if out.edge is not None:
+                    out.edge[edge_type] = None
+                    out.edge[rev_edge_type] = None
+
+            else:  # Find the reverse edge type (if it is unique):
+                if len(src_dst_dict) == 0:  # Create mapping lazily.
+                    for key in self.row.keys():
+                        v1, _, v2 = key
+                        src_dst_dict[(v1, v2)].append(key)
+
+                if len(src_dst_dict[(dst, src)]) == 1:
+                    rev_edge_type = src_dst_dict[(dst, src)][0]
+                    row, col, _ = to_bidirectional(
+                        row=self.row[edge_type],
+                        col=self.col[edge_type],
+                        rev_row=self.row[rev_edge_type],
+                        rev_col=self.col[rev_edge_type],
+                    )
+                    out.row[edge_type] = row
+                    out.col[edge_type] = col
+                    if out.edge is not None:
+                        out.edge[edge_type] = None
+
+                else:
+                    warnings.warn(f"Cannot convert to bidirectional graph "
+                                  f"since the edge type {edge_type} does not "
+                                  f"seem to have a reverse edge type")
+
+        out.num_sampled_edges = None
+
+        return out
+
 
 @dataclass(frozen=True)
 class NumNeighbors:
     r"""The number of neighbors to sample in a homogeneous or heterogeneous
     graph. In heterogeneous graphs, may also take in a dictionary denoting
     the amount of neighbors to sample for individual edge types.
```

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/sampler/hgt_sampler.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/sampler/hgt_sampler.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/sampler/neighbor_sampler.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/sampler/neighbor_sampler.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,36 +20,44 @@
     BaseSampler,
     EdgeSamplerInput,
     HeteroSamplerOutput,
     NegativeSampling,
     NodeSamplerInput,
     SamplerOutput,
 )
-from torch_geometric.sampler.base import DataType, NumNeighbors
+from torch_geometric.sampler.base import DataType, NumNeighbors, SubgraphType
 from torch_geometric.sampler.utils import remap_keys, to_csc, to_hetero_csc
 from torch_geometric.typing import EdgeType, NodeType, OptTensor
 
 NumNeighborsType = Union[NumNeighbors, List[int], Dict[EdgeType, List[int]]]
 
 
 class NeighborSampler(BaseSampler):
     r"""An implementation of an in-memory (heterogeneous) neighbor sampler used
     by :class:`~torch_geometric.loader.NeighborLoader`."""
     def __init__(
         self,
         data: Union[Data, HeteroData, Tuple[FeatureStore, GraphStore]],
         num_neighbors: NumNeighborsType,
+        subgraph_type: Union[SubgraphType, str] = 'directional',
         replace: bool = False,
-        directed: bool = True,
         disjoint: bool = False,
         temporal_strategy: str = 'uniform',
         time_attr: Optional[str] = None,
         is_sorted: bool = False,
         share_memory: bool = False,
+        # Deprecated:
+        directed: bool = True,
     ):
+        if not directed:
+            subgraph_type = SubgraphType.induced
+            warnings.warn(f"The usage of the 'directed' argument in "
+                          f"'{self.__class__.__name__}' is deprecated. Use "
+                          f"`subgraph_type='induced'` instead.")
+
         if not torch_geometric.typing.WITH_PYG_LIB and sys.platform == 'linux':
             warnings.warn("Using '{self.__class__.__name__}' without a "
                           "'pyg-lib' installation is deprecated and will be "
                           "removed soon. Please install 'pyg-lib' for "
                           "accelerated neighborhood sampling")
 
         self.data_type = DataType.from_data(data)
@@ -134,15 +142,15 @@
             # Convert the graph data into CSC format for sampling:
             row_dict, colptr_dict, self.perm = graph_store.csc()
             self.row_dict = remap_keys(row_dict, self.to_rel_type)
             self.colptr_dict = remap_keys(colptr_dict, self.to_rel_type)
 
         self.num_neighbors = num_neighbors
         self.replace = replace
-        self.directed = directed
+        self.subgraph_type = SubgraphType(subgraph_type)
         self.disjoint = disjoint
         self.temporal_strategy = temporal_strategy
 
     @property
     def num_neighbors(self) -> NumNeighbors:
         return self._num_neighbors
 
@@ -167,24 +175,30 @@
 
     # Node-based sampling #####################################################
 
     def sample_from_nodes(
         self,
         inputs: NodeSamplerInput,
     ) -> Union[SamplerOutput, HeteroSamplerOutput]:
-        return node_sample(inputs, self._sample)
+        out = node_sample(inputs, self._sample)
+        if self.subgraph_type == SubgraphType.bidirectional:
+            out = out.to_bidirectional()
+        return out
 
     # Edge-based sampling #####################################################
 
     def sample_from_edges(
         self, inputs: EdgeSamplerInput,
         neg_sampling: Optional[NegativeSampling] = None
     ) -> Union[SamplerOutput, HeteroSamplerOutput]:
-        return edge_sample(inputs, self._sample, self.num_nodes, self.disjoint,
-                           self.node_time, neg_sampling)
+        out = edge_sample(inputs, self._sample, self.num_nodes, self.disjoint,
+                          self.node_time, neg_sampling)
+        if self.subgraph_type == SubgraphType.bidirectional:
+            out = out.to_bidirectional()
+        return out
 
     # Other Utilities #########################################################
 
     @property
     def edge_permutation(self) -> Union[OptTensor, Dict[EdgeType, OptTensor]]:
         return self.perm
 
@@ -193,15 +207,15 @@
     def _sample(
         self,
         seed: Union[Tensor, Dict[NodeType, Tensor]],
         seed_time: Optional[Union[Tensor, Dict[NodeType, Tensor]]] = None,
         **kwargs,
     ) -> Union[SamplerOutput, HeteroSamplerOutput]:
         r"""Implements neighbor sampling by calling either :obj:`pyg-lib` (if
-        installed) or :obj:`torch-sparse` sampling routines."""
+        installed) or :obj:`torch-sparse` (if installed) sampling routines."""
         if isinstance(seed, dict):  # Heterogeneous sampling:
             if torch_geometric.typing.WITH_PYG_LIB:
                 # TODO (matthias) `return_edge_id` if edge features present
                 # TODO (matthias) Ideally, `seed` inherits dtype from `colptr`
                 colptrs = list(self.colptr_dict.values())
                 dtype = colptrs[0].dtype if len(colptrs) > 0 else torch.int64
                 seed = {k: v.to(dtype) for k, v in seed.items()}
@@ -213,15 +227,15 @@
                     self.row_dict,
                     seed,
                     self.num_neighbors.get_mapped_values(self.edge_types),
                     self.node_time,
                     seed_time,
                     True,  # csc
                     self.replace,
-                    self.directed,
+                    self.subgraph_type != SubgraphType.induced,
                     self.disjoint,
                     self.temporal_strategy,
                     True,  # return_edge_id
                 )
                 row, col, node, edge, batch = out[:4] + (None, )
 
                 # `pyg-lib>0.1.0` returns sampled number of nodes/edges:
@@ -246,15 +260,15 @@
                     self.edge_types,
                     self.colptr_dict,
                     self.row_dict,
                     seed,  # seed_dict
                     self.num_neighbors.get_mapped_values(self.edge_types),
                     self.num_neighbors.num_hops,
                     self.replace,
-                    self.directed,
+                    self.subgraph_type != SubgraphType.induced,
                 )
                 node, row, col, edge, batch = out + (None, )
                 num_sampled_nodes = num_sampled_edges = None
 
             else:
                 raise ImportError(f"'{self.__class__.__name__}' requires "
                                   f"either 'pyg-lib' or 'torch-sparse'")
@@ -284,15 +298,15 @@
                     self.row,
                     seed.to(self.colptr.dtype),  # seed
                     self.num_neighbors.get_mapped_values(),
                     self.node_time,
                     seed_time,
                     True,  # csc
                     self.replace,
-                    self.directed,
+                    self.subgraph_type != SubgraphType.induced,
                     self.disjoint,
                     self.temporal_strategy,
                     True,  # return_edge_id
                 )
                 row, col, node, edge, batch = out[:4] + (None, )
 
                 # `pyg-lib>0.1.0` returns sampled number of nodes/edges:
@@ -312,15 +326,15 @@
 
                 out = torch.ops.torch_sparse.neighbor_sample(
                     self.colptr,
                     self.row,
                     seed,  # seed
                     self.num_neighbors.get_mapped_values(),
                     self.replace,
-                    self.directed,
+                    self.subgraph_type != SubgraphType.induced,
                 )
                 node, row, col, edge, batch = out + (None, )
                 num_sampled_nodes = num_sampled_edges = None
 
             else:
                 raise ImportError(f"'{self.__class__.__name__}' requires "
                                   f"either 'pyg-lib' or 'torch-sparse'")
```

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/sampler/utils.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/sampler/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import numpy as np
 import torch
 from torch import Tensor
 
 from torch_geometric.data import Data, HeteroData
 from torch_geometric.data.storage import EdgeStorage
 from torch_geometric.typing import NodeType, OptTensor
-from torch_geometric.utils import index_sort
+from torch_geometric.utils import coalesce, index_sort
 from torch_geometric.utils.sparse import index2ptr
 
 # Edge Layout Conversion ######################################################
 
 
 def sort_csc(
     row: Tensor,
@@ -108,14 +108,40 @@
         src_node_time = (node_time_dict or {}).get(edge_type[0], None)
         out = to_csc(store, device, share_memory, is_sorted, src_node_time)
         colptr_dict[edge_type], row_dict[edge_type], perm_dict[edge_type] = out
 
     return colptr_dict, row_dict, perm_dict
 
 
+def to_bidirectional(
+    row: Tensor,
+    col: Tensor,
+    rev_row: Tensor,
+    rev_col: Tensor,
+    edge_id: OptTensor = None,
+    rev_edge_id: OptTensor = None,
+) -> Tuple[Tensor, Tensor, OptTensor]:
+
+    assert row.numel() == col.numel()
+    assert rev_row.numel() == rev_col.numel()
+
+    edge_index = row.new_empty(2, row.numel() + rev_row.numel())
+    edge_index[0, :row.numel()] = row
+    edge_index[1, :row.numel()] = col
+    edge_index[0, row.numel():] = rev_col
+    edge_index[1, row.numel():] = rev_row
+
+    if edge_id is not None:
+        edge_id = torch.cat([edge_id, rev_edge_id], dim=0)
+
+    (row, col), edge_id = coalesce(edge_index, edge_id, reduce='any')
+
+    return row, col, edge_id
+
+
 ###############################################################################
 
 X, Y = TypeVar('X'), TypeVar('Y')
 
 
 def remap_keys(
     inputs: Dict[X, Any],
```

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/testing/__init__.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/testing/asserts.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/testing/asserts.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/testing/data.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/testing/data.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 from typing import Callable, Optional
 
 import torch
 from torch import Tensor
 
 from torch_geometric.data import HeteroData, InMemoryDataset
+from torch_geometric.utils import coalesce as coalesce_fn
 
 
 def get_random_edge_index(
     num_src_nodes: int,
     num_dst_nodes: int,
     num_edges: int,
     dtype: Optional[torch.dtype] = None,
     device: Optional[torch.device] = None,
+    coalesce: bool = False,
 ) -> Tensor:
     row = torch.randint(num_src_nodes, (num_edges, ), dtype=dtype,
                         device=device)
     col = torch.randint(num_dst_nodes, (num_edges, ), dtype=dtype,
                         device=device)
-    return torch.stack([row, col], dim=0)
+    edge_index = torch.stack([row, col], dim=0)
+
+    if coalesce:
+        edge_index = coalesce_fn(edge_index)
+
+    return edge_index
 
 
 class FakeHeteroDataset(InMemoryDataset):
     def __init__(self, transform: Optional[Callable] = None):
         super().__init__(transform=transform)
 
         data = HeteroData()
```

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/testing/decorators.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/testing/decorators.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/testing/feature_store.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/testing/feature_store.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/testing/graph_store.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/testing/graph_store.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/__init__.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/add_metapaths.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/add_metapaths.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/add_positional_encoding.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/add_positional_encoding.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/add_self_loops.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/add_self_loops.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/base_transform.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/base_transform.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/cartesian.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/cartesian.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/center.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/center.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/compose.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/compose.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/constant.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/constant.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/delaunay.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/delaunay.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/distance.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/distance.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/face_to_edge.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/face_to_edge.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/feature_propagation.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/feature_propagation.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/fixed_points.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/fixed_points.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/gcn_norm.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/gcn_norm.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/gdc.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/gdc.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/generate_mesh_normals.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/generate_mesh_normals.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/grid_sampling.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/grid_sampling.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/knn_graph.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/knn_graph.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/laplacian_lambda_max.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/laplacian_lambda_max.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/largest_connected_components.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/largest_connected_components.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/line_graph.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/line_graph.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/linear_transformation.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/linear_transformation.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/local_cartesian.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/local_cartesian.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/local_degree_profile.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/local_degree_profile.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/mask.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/mask.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/normalize_features.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/normalize_features.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/normalize_rotation.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/normalize_rotation.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/normalize_scale.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/normalize_scale.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/one_hot_degree.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/one_hot_degree.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/pad.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/pad.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/point_pair_features.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/point_pair_features.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/polar.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/polar.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/radius_graph.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/radius_graph.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/random_flip.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/random_flip.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/random_jitter.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/random_jitter.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/random_link_split.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/random_link_split.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/random_node_split.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/random_node_split.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/random_rotate.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/random_rotate.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/random_scale.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/random_scale.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/random_shear.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/random_shear.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/remove_duplicated_edges.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/remove_duplicated_edges.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/remove_isolated_nodes.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/remove_isolated_nodes.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/remove_training_classes.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/remove_training_classes.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/rooted_subgraph.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/rooted_subgraph.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/sample_points.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/sample_points.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/sign.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/sign.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/spherical.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/spherical.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/svd_feature_reduction.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/svd_feature_reduction.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/target_indegree.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/target_indegree.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/to_dense.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/to_dense.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/to_device.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/to_device.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/to_sparse_tensor.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/to_sparse_tensor.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/to_superpixels.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/to_superpixels.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/to_undirected.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/to_undirected.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/two_hop.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/two_hop.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/transforms/virtual_node.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/transforms/virtual_node.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/typing.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/typing.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/__init__.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/assortativity.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/assortativity.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/augmentation.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/augmentation.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/coalesce.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/coalesce.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,22 +113,24 @@
         if edge_attr is None or isinstance(edge_attr, (Tensor, list, tuple)):
             return edge_index, edge_attr
         return edge_index
 
     edge_index = edge_index[:, mask]
 
     dim_size: Optional[int] = None
-    if isinstance(edge_attr, (Tensor, list, tuple)):
+    if isinstance(edge_attr, (Tensor, list, tuple)) and len(edge_attr) > 0:
         dim_size = edge_index.size(1)
         idx = torch.arange(0, nnz, device=edge_index.device)
         idx.sub_(mask.logical_not_().cumsum(dim=0))
 
     if edge_attr is None:
         return edge_index, None
     if isinstance(edge_attr, Tensor):
         edge_attr = scatter(edge_attr, idx, 0, dim_size, reduce)
         return edge_index, edge_attr
     if isinstance(edge_attr, (list, tuple)):
+        if len(edge_attr) == 0:
+            return edge_index, edge_attr
         edge_attr = [scatter(e, idx, 0, dim_size, reduce) for e in edge_attr]
         return edge_index, edge_attr
 
     return edge_index
```

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/convert.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/convert.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/degree.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/degree.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/dropout.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/dropout.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/embedding.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/embedding.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/geodesic.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/geodesic.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/get_laplacian.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/get_laplacian.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/get_mesh_laplacian.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/get_mesh_laplacian.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/grid.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/grid.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/hetero.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/hetero.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/homophily.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/homophily.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/isolated.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/isolated.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/loop.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/loop.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/mask.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/mask.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/mixin.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/mixin.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/negative_sampling.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/negative_sampling.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/nested.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/nested.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/normalized_cut.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/normalized_cut.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/num_nodes.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/num_nodes.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/one_hot.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/one_hot.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/random.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/random.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/scatter.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/scatter.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/segment.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/segment.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/select.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/select.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/smiles.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/smiles.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/softmax.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/softmax.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/sort.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/sort.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/sort_edge_index.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/sort_edge_index.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/sparse.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/sparse.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/spmm.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/spmm.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/subgraph.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/subgraph.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/to_dense_adj.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/to_dense_adj.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/to_dense_batch.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/to_dense_batch.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/train_test_split_edges.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/train_test_split_edges.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/tree_decomposition.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/tree_decomposition.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/trim_to_layer.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/trim_to_layer.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/unbatch.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/unbatch.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/utils/undirected.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/utils/undirected.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/torch_geometric/visualization/graph.py` & `pyg-nightly-2.4.0.dev20230419/torch_geometric/visualization/graph.py`

 * *Files identical despite different names*

### Comparing `pyg-nightly-2.4.0.dev20230418/PKG-INFO` & `pyg-nightly-2.4.0.dev20230419/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyg-nightly
-Version: 2.4.0.dev20230418
+Version: 2.4.0.dev20230419
 Summary: Graph Neural Network Library for PyTorch
 Keywords: deep-learning,pytorch,geometric-deep-learning,graph-neural-networks,graph-convolutional-networks
 Author-email: Matthias Fey <matthias@pyg.org>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

