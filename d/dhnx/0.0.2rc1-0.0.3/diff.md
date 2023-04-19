# Comparing `tmp/dhnx-0.0.2rc1.tar.gz` & `tmp/dhnx-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\dhnx-0.0.2rc1.tar", last modified: Thu Jul  8 18:30:13 2021, max compression
+gzip compressed data, was "dhnx-0.0.3.tar", last modified: Wed Apr 19 08:32:47 2023, max compression
```

## Comparing `dhnx-0.0.2rc1.tar` & `dhnx-0.0.3.tar`

### file list

```diff
@@ -1,38 +1,372 @@
-drwxrwxrwx   0        0        0        0 2021-07-08 18:30:13.757491 dhnx-0.0.2rc1/
--rw-rw-rw-   0        0        0      134 2021-07-08 17:37:48.000000 dhnx-0.0.2rc1/AUTHORS.rst
--rw-rw-rw-   0        0        0     1100 2021-07-08 17:37:48.000000 dhnx-0.0.2rc1/LICENSE
--rw-rw-rw-   0        0        0     3924 2021-07-08 18:30:13.757491 dhnx-0.0.2rc1/PKG-INFO
--rw-rw-rw-   0        0        0     3461 2021-07-08 17:37:48.000000 dhnx-0.0.2rc1/README.rst
-drwxrwxrwx   0        0        0        0 2021-07-08 18:30:13.695006 dhnx-0.0.2rc1/dhnx/
--rw-rw-rw-   0        0        0      330 2021-07-08 18:27:10.000000 dhnx-0.0.2rc1/dhnx/__init__.py
-drwxrwxrwx   0        0        0        0 2021-07-08 18:30:13.741869 dhnx-0.0.2rc1/dhnx/component_attrs/
--rw-rw-rw-   0        0        0      608 2021-07-08 17:37:48.000000 dhnx-0.0.2rc1/dhnx/component_attrs/consumers.csv
--rw-rw-rw-   0        0        0      202 2021-07-08 17:37:48.000000 dhnx-0.0.2rc1/dhnx/component_attrs/environment.csv
--rw-rw-rw-   0        0        0      450 2021-07-08 17:37:48.000000 dhnx-0.0.2rc1/dhnx/component_attrs/forks.csv
--rw-rw-rw-   0        0        0      535 2021-07-08 17:37:48.000000 dhnx-0.0.2rc1/dhnx/component_attrs/pipes.csv
--rw-rw-rw-   0        0        0      541 2021-07-08 17:37:48.000000 dhnx-0.0.2rc1/dhnx/component_attrs/producers.csv
--rw-rw-rw-   0        0        0      277 2021-07-08 17:37:48.000000 dhnx-0.0.2rc1/dhnx/components.csv
--rw-rw-rw-   0        0        0     2432 2021-07-08 17:37:48.000000 dhnx-0.0.2rc1/dhnx/dhn_from_osm.py
-drwxrwxrwx   0        0        0        0 2021-07-08 18:30:13.757491 dhnx-0.0.2rc1/dhnx/gistools/
--rw-rw-rw-   0        0        0       65 2021-07-08 17:37:48.000000 dhnx-0.0.2rc1/dhnx/gistools/__init__.py
--rw-rw-rw-   0        0        0    13903 2021-07-08 17:37:48.000000 dhnx-0.0.2rc1/dhnx/gistools/connect_points.py
--rw-rw-rw-   0        0        0    18485 2021-07-08 17:37:48.000000 dhnx-0.0.2rc1/dhnx/gistools/geometry_operations.py
--rw-rw-rw-   0        0        0     2748 2021-07-08 17:37:48.000000 dhnx-0.0.2rc1/dhnx/graph.py
--rw-rw-rw-   0        0        0      508 2021-07-08 17:37:48.000000 dhnx-0.0.2rc1/dhnx/helpers.py
--rw-rw-rw-   0        0        0    15079 2021-07-08 17:37:48.000000 dhnx-0.0.2rc1/dhnx/input_output.py
--rw-rw-rw-   0        0        0     1738 2021-07-08 17:37:48.000000 dhnx-0.0.2rc1/dhnx/model.py
--rw-rw-rw-   0        0        0     9414 2021-07-08 17:37:48.000000 dhnx-0.0.2rc1/dhnx/network.py
--rw-rw-rw-   0        0        0    29431 2021-07-08 17:37:48.000000 dhnx-0.0.2rc1/dhnx/optimization.py
--rw-rw-rw-   0        0        0    16458 2021-07-08 17:37:48.000000 dhnx-0.0.2rc1/dhnx/optimization_add_components.py
--rw-rw-rw-   0        0        0    10916 2021-07-08 17:37:48.000000 dhnx-0.0.2rc1/dhnx/optimization_dhs_nodes.py
--rw-rw-rw-   0        0        0    15649 2021-07-08 17:37:48.000000 dhnx-0.0.2rc1/dhnx/optimization_oemof_heatpipe.py
--rw-rw-rw-   0        0        0    10232 2021-07-08 17:37:48.000000 dhnx-0.0.2rc1/dhnx/plotting.py
--rw-rw-rw-   0        0        0    26414 2021-07-08 17:37:48.000000 dhnx-0.0.2rc1/dhnx/simulation.py
-drwxrwxrwx   0        0        0        0 2021-07-08 18:30:13.726251 dhnx-0.0.2rc1/dhnx.egg-info/
--rw-rw-rw-   0        0        0     3924 2021-07-08 18:30:13.000000 dhnx-0.0.2rc1/dhnx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      751 2021-07-08 18:30:13.000000 dhnx-0.0.2rc1/dhnx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-07-08 18:30:13.000000 dhnx-0.0.2rc1/dhnx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      151 2021-07-08 18:30:13.000000 dhnx-0.0.2rc1/dhnx.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2021-07-08 18:30:13.000000 dhnx-0.0.2rc1/dhnx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       87 2021-07-08 18:30:13.757491 dhnx-0.0.2rc1/setup.cfg
--rw-rw-rw-   0        0        0     1075 2021-07-08 18:27:10.000000 dhnx-0.0.2rc1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.966623 dhnx-0.0.3/
+-rw-rw-rw-   0        0        0      197 2023-04-19 08:22:25.000000 dhnx-0.0.3/.coveragerc
+-rw-rw-rw-   0        0        0      152 2023-04-19 08:22:25.000000 dhnx-0.0.3/AUTHORS.rst
+-rw-rw-rw-   0        0        0     1100 2021-07-08 17:37:48.000000 dhnx-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      343 2023-04-19 08:22:25.000000 dhnx-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     3883 2023-04-19 08:32:47.966623 dhnx-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3461 2023-04-19 08:22:25.000000 dhnx-0.0.3/README.rst
+-rw-rw-rw-   0        0        0       23 2023-04-19 08:22:25.000000 dhnx-0.0.3/VERSION
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.496671 dhnx-0.0.3/dhnx/
+-rw-rw-rw-   0        0        0      723 2023-04-19 08:22:25.000000 dhnx-0.0.3/dhnx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.527915 dhnx-0.0.3/dhnx/component_attrs/
+-rw-rw-rw-   0        0        0      608 2021-07-08 17:37:48.000000 dhnx-0.0.3/dhnx/component_attrs/consumers.csv
+-rw-rw-rw-   0        0        0      202 2021-07-08 17:37:48.000000 dhnx-0.0.3/dhnx/component_attrs/environment.csv
+-rw-rw-rw-   0        0        0      450 2021-07-08 17:37:48.000000 dhnx-0.0.3/dhnx/component_attrs/forks.csv
+-rw-rw-rw-   0        0        0      535 2021-07-08 17:37:48.000000 dhnx-0.0.3/dhnx/component_attrs/pipes.csv
+-rw-rw-rw-   0        0        0      541 2021-07-08 17:37:48.000000 dhnx-0.0.3/dhnx/component_attrs/producers.csv
+-rw-rw-rw-   0        0        0      277 2021-07-08 17:37:48.000000 dhnx-0.0.3/dhnx/components.csv
+-rw-rw-rw-   0        0        0     2432 2023-04-19 08:22:25.000000 dhnx-0.0.3/dhnx/dhn_from_osm.py
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.527915 dhnx-0.0.3/dhnx/gistools/
+-rw-rw-rw-   0        0        0        0 2023-04-19 08:22:25.000000 dhnx-0.0.3/dhnx/gistools/__init__.py
+-rw-rw-rw-   0        0        0    23241 2023-04-19 08:22:25.000000 dhnx-0.0.3/dhnx/gistools/connect_points.py
+-rw-rw-rw-   0        0        0    19125 2023-04-19 08:22:25.000000 dhnx-0.0.3/dhnx/gistools/geometry_operations.py
+-rw-rw-rw-   0        0        0     2744 2023-04-19 08:22:25.000000 dhnx-0.0.3/dhnx/graph.py
+-rw-rw-rw-   0        0        0      508 2021-07-08 17:37:48.000000 dhnx-0.0.3/dhnx/helpers.py
+-rw-rw-rw-   0        0        0    15077 2023-04-19 08:22:25.000000 dhnx-0.0.3/dhnx/input_output.py
+-rw-rw-rw-   0        0        0     1738 2021-07-08 17:37:48.000000 dhnx-0.0.3/dhnx/model.py
+-rw-rw-rw-   0        0        0     9559 2023-04-19 08:22:25.000000 dhnx-0.0.3/dhnx/network.py
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.543533 dhnx-0.0.3/dhnx/optimization/
+-rw-rw-rw-   0        0        0      223 2023-04-19 08:22:25.000000 dhnx-0.0.3/dhnx/optimization/__init__.py
+-rw-rw-rw-   0        0        0    16899 2023-04-19 08:22:25.000000 dhnx-0.0.3/dhnx/optimization/add_components.py
+-rw-rw-rw-   0        0        0    10918 2023-04-19 08:22:25.000000 dhnx-0.0.3/dhnx/optimization/dhs_nodes.py
+-rw-rw-rw-   0        0        0    16156 2023-04-19 08:22:25.000000 dhnx-0.0.3/dhnx/optimization/oemof_heatpipe.py
+-rw-rw-rw-   0        0        0    30811 2023-04-19 08:22:25.000000 dhnx-0.0.3/dhnx/optimization/optimization_models.py
+-rw-rw-rw-   0        0        0    19008 2023-04-19 08:22:25.000000 dhnx-0.0.3/dhnx/optimization/precalc_hydraulic.py
+-rw-rw-rw-   0        0        0    10233 2023-04-19 08:22:25.000000 dhnx-0.0.3/dhnx/plotting.py
+-rw-rw-rw-   0        0        0    26508 2023-04-19 08:22:25.000000 dhnx-0.0.3/dhnx/simulation.py
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.527915 dhnx-0.0.3/dhnx.egg-info/
+-rw-rw-rw-   0        0        0     3883 2023-04-19 08:32:47.000000 dhnx-0.0.3/dhnx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    16192 2023-04-19 08:32:47.000000 dhnx-0.0.3/dhnx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 08:32:47.000000 dhnx-0.0.3/dhnx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      185 2023-04-19 08:32:47.000000 dhnx-0.0.3/dhnx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-19 08:32:47.000000 dhnx-0.0.3/dhnx.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.565660 dhnx-0.0.3/docs/
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.565660 dhnx-0.0.3/docs/_build/
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.596906 dhnx-0.0.3/docs/_build/.doctrees/
+-rw-rw-rw-   0        0        0     2985 2023-03-30 08:56:15.000000 dhnx-0.0.3/docs/_build/.doctrees/analyze_and_plot.doctree
+-rw-rw-rw-   0        0        0   582952 2023-03-30 08:56:18.000000 dhnx-0.0.3/docs/_build/.doctrees/api.doctree
+-rw-rw-rw-   0        0        0     3921 2023-03-30 08:56:18.000000 dhnx-0.0.3/docs/_build/.doctrees/authors.doctree
+-rw-rw-rw-   0        0        0  1585682 2023-03-30 08:56:18.000000 dhnx-0.0.3/docs/_build/.doctrees/environment.pickle
+-rw-rw-rw-   0        0        0     4366 2023-03-30 08:56:18.000000 dhnx-0.0.3/docs/_build/.doctrees/examples.doctree
+-rw-rw-rw-   0        0        0     5528 2023-03-30 08:56:18.000000 dhnx-0.0.3/docs/_build/.doctrees/geometry_preparation.doctree
+-rw-rw-rw-   0        0        0    12492 2023-03-30 08:56:18.000000 dhnx-0.0.3/docs/_build/.doctrees/getting_started.doctree
+-rw-rw-rw-   0        0        0     5582 2023-03-30 08:56:18.000000 dhnx-0.0.3/docs/_build/.doctrees/index.doctree
+-rw-rw-rw-   0        0        0     2911 2023-03-30 08:56:18.000000 dhnx-0.0.3/docs/_build/.doctrees/model_coupling.doctree
+-rw-rw-rw-   0        0        0    62609 2023-03-30 08:56:18.000000 dhnx-0.0.3/docs/_build/.doctrees/network.doctree
+-rw-rw-rw-   0        0        0   196036 2023-03-30 08:56:18.000000 dhnx-0.0.3/docs/_build/.doctrees/optimization_models.doctree
+-rw-rw-rw-   0        0        0    65923 2023-03-30 08:56:18.000000 dhnx-0.0.3/docs/_build/.doctrees/simulation_models.doctree
+-rw-rw-rw-   0        0        0    24361 2023-03-30 08:56:18.000000 dhnx-0.0.3/docs/_build/.doctrees/whats_new.doctree
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.443552 dhnx-0.0.3/docs/_build/_images/
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.697163 dhnx-0.0.3/docs/_build/_images/math/
+-rw-rw-rw-   0        0        0     1019 2023-03-30 08:57:05.000000 dhnx-0.0.3/docs/_build/_images/math/0125e10e116e78855389b3b5d3218de621004598.png
+-rw-rw-rw-   0        0        0      209 2023-03-30 08:56:31.000000 dhnx-0.0.3/docs/_build/_images/math/02d98909b5d6acd6a7ff927d4d42790bdd407d58.png
+-rw-rw-rw-   0        0        0      321 2023-03-30 08:56:36.000000 dhnx-0.0.3/docs/_build/_images/math/08c4e3b3342e2ccf4f7fa5bcdbd3b4afce332b5a.png
+-rw-rw-rw-   0        0        0      913 2023-03-30 08:56:51.000000 dhnx-0.0.3/docs/_build/_images/math/0cf17db0ed3ec29a9036b704c3b9a9e5cead7e56.png
+-rw-rw-rw-   0        0        0      237 2023-03-30 08:56:46.000000 dhnx-0.0.3/docs/_build/_images/math/141bbefb74014fc5e43499901bf78607ae335583.png
+-rw-rw-rw-   0        0        0      220 2023-03-30 08:56:32.000000 dhnx-0.0.3/docs/_build/_images/math/14eb89266154200b9c81dcfc3bd058638fa221bf.png
+-rw-rw-rw-   0        0        0      724 2023-03-30 08:56:44.000000 dhnx-0.0.3/docs/_build/_images/math/16e243bf1f0879278f889ba5e21441a675db0f81.png
+-rw-rw-rw-   0        0        0      232 2023-03-30 08:57:12.000000 dhnx-0.0.3/docs/_build/_images/math/1c74485fdd094fc0242d5a0e1a357dc89527ca7e.png
+-rw-rw-rw-   0        0        0      577 2023-03-30 08:57:01.000000 dhnx-0.0.3/docs/_build/_images/math/25b73d2a0c31d066ca53d779178a695f0574b213.png
+-rw-rw-rw-   0        0        0      237 2023-03-30 08:56:35.000000 dhnx-0.0.3/docs/_build/_images/math/27dc86f9f1b1c3435b2403a869b5870c582facea.png
+-rw-rw-rw-   0        0        0      299 2023-03-30 08:56:26.000000 dhnx-0.0.3/docs/_build/_images/math/2b9dc6842eff2f1339d77b755c207da63892d789.png
+-rw-rw-rw-   0        0        0      511 2023-03-30 08:56:47.000000 dhnx-0.0.3/docs/_build/_images/math/31606e454592dc221f49415cffc55197a958c30b.png
+-rw-rw-rw-   0        0        0      674 2023-03-30 08:56:40.000000 dhnx-0.0.3/docs/_build/_images/math/3b90295a6bccaee3d100e8960ce9ace78d12de06.png
+-rw-rw-rw-   0        0        0      387 2023-03-30 08:56:38.000000 dhnx-0.0.3/docs/_build/_images/math/3e7c256ec506a29f18f9d6342534cedb3969abfe.png
+-rw-rw-rw-   0        0        0      492 2023-03-30 08:56:24.000000 dhnx-0.0.3/docs/_build/_images/math/3f190eebd81c600bce81e72c993a4dbe05e331fd.png
+-rw-rw-rw-   0        0        0     1113 2023-03-30 08:56:20.000000 dhnx-0.0.3/docs/_build/_images/math/4051701eca15dfd86ab9e74dbfe40596afa8d1e8.png
+-rw-rw-rw-   0        0        0      499 2023-03-30 08:56:22.000000 dhnx-0.0.3/docs/_build/_images/math/42d358ede121f6fb299bc413bca5d628a8eb8188.png
+-rw-rw-rw-   0        0        0      256 2023-03-30 08:57:00.000000 dhnx-0.0.3/docs/_build/_images/math/43bd1c95aa14e04c04b30ebe6966d528c544f79d.png
+-rw-rw-rw-   0        0        0      292 2023-03-30 08:56:30.000000 dhnx-0.0.3/docs/_build/_images/math/450be0ae9e6ac153dee6f0bc9cb83f5ffded69e7.png
+-rw-rw-rw-   0        0        0      211 2023-03-30 08:56:29.000000 dhnx-0.0.3/docs/_build/_images/math/470aa65888a2971c9346e573f12b37ea406b8ec9.png
+-rw-rw-rw-   0        0        0      979 2023-03-30 08:56:55.000000 dhnx-0.0.3/docs/_build/_images/math/47e62ebdc6da7194ce61e8ff66e12b8b68cea6d6.png
+-rw-rw-rw-   0        0        0      394 2023-03-30 08:57:03.000000 dhnx-0.0.3/docs/_build/_images/math/49235d4e6c49390c4e7d06a7719855b6fb681232.png
+-rw-rw-rw-   0        0        0      658 2023-03-30 08:57:21.000000 dhnx-0.0.3/docs/_build/_images/math/4e7e228db7528236e15e57188c66616287a45729.png
+-rw-rw-rw-   0        0        0      253 2023-03-30 08:56:58.000000 dhnx-0.0.3/docs/_build/_images/math/51ac9faa380f2ad5849c324de2e51854a229090b.png
+-rw-rw-rw-   0        0        0      884 2023-03-30 08:56:43.000000 dhnx-0.0.3/docs/_build/_images/math/534b7b4cd1eaefe50647b4d69d7e95dae82c8d88.png
+-rw-rw-rw-   0        0        0      258 2023-03-30 08:56:31.000000 dhnx-0.0.3/docs/_build/_images/math/54082d366e30a6599eb4acf68fb943b5f94743c8.png
+-rw-rw-rw-   0        0        0      292 2023-03-30 08:56:39.000000 dhnx-0.0.3/docs/_build/_images/math/68132fbd6f413bd35c80cc0f70f464cb95921a0c.png
+-rw-rw-rw-   0        0        0      374 2023-03-30 08:57:04.000000 dhnx-0.0.3/docs/_build/_images/math/6c430aa82a375c8fbd9cf3bb567e0550a4027e08.png
+-rw-rw-rw-   0        0        0      606 2023-03-30 08:56:59.000000 dhnx-0.0.3/docs/_build/_images/math/702c60165a215d02bd52e5d0451a82929c3de6d8.png
+-rw-rw-rw-   0        0        0      251 2023-03-30 08:57:11.000000 dhnx-0.0.3/docs/_build/_images/math/774f61298184dd7a26ef4f69ec711017409f7bdd.png
+-rw-rw-rw-   0        0        0      300 2023-03-30 08:56:49.000000 dhnx-0.0.3/docs/_build/_images/math/78ac1b6338a0dbd25a6176bbbba458aad01b81ad.png
+-rw-rw-rw-   0        0        0      391 2023-03-30 08:56:52.000000 dhnx-0.0.3/docs/_build/_images/math/805fa299717a2abeb36c174d582915650eb62342.png
+-rw-rw-rw-   0        0        0      213 2023-03-30 08:57:06.000000 dhnx-0.0.3/docs/_build/_images/math/888f7c323ac0341871e867220ae2d76467d74d6e.png
+-rw-rw-rw-   0        0        0      324 2023-03-30 08:57:08.000000 dhnx-0.0.3/docs/_build/_images/math/8aa10f3a225bc240638bd37b3d731be87608a588.png
+-rw-rw-rw-   0        0        0      611 2023-03-30 08:57:13.000000 dhnx-0.0.3/docs/_build/_images/math/8b16404d2b1400a8e3de876defb789c52959d636.png
+-rw-rw-rw-   0        0        0      330 2023-03-30 08:56:57.000000 dhnx-0.0.3/docs/_build/_images/math/8e2367fd9e55e667c9248af150fcb0e40748e6c7.png
+-rw-rw-rw-   0        0        0      253 2023-03-30 08:56:53.000000 dhnx-0.0.3/docs/_build/_images/math/9098c1c4618d7a0f321cee441aabee7f1b57a19b.png
+-rw-rw-rw-   0        0        0      452 2023-03-30 08:56:25.000000 dhnx-0.0.3/docs/_build/_images/math/962b2728f1db4765c555b270187e68c176c5f84f.png
+-rw-rw-rw-   0        0        0      225 2023-03-30 08:56:41.000000 dhnx-0.0.3/docs/_build/_images/math/9630132210b904754c9ab272b61cb527d12263ca.png
+-rw-rw-rw-   0        0        0      235 2023-03-30 08:56:37.000000 dhnx-0.0.3/docs/_build/_images/math/97db043c7cba573ac389b71add78b048077e8a13.png
+-rw-rw-rw-   0        0        0      374 2023-03-30 08:57:02.000000 dhnx-0.0.3/docs/_build/_images/math/9e2bc05bc7d1a3f0af84f55f8a476963a8e92c15.png
+-rw-rw-rw-   0        0        0      256 2023-03-30 08:57:09.000000 dhnx-0.0.3/docs/_build/_images/math/a19b663853286eef414965f74ae365870ade1302.png
+-rw-rw-rw-   0        0        0      701 2023-03-30 08:57:20.000000 dhnx-0.0.3/docs/_build/_images/math/a8da2c8ea325d30fe4eee535c805a0b9e9b34ba2.png
+-rw-rw-rw-   0        0        0      873 2023-03-30 08:56:21.000000 dhnx-0.0.3/docs/_build/_images/math/a9b22fc234cd35157125f51ff4c036a229f06060.png
+-rw-rw-rw-   0        0        0     1137 2023-03-30 08:57:07.000000 dhnx-0.0.3/docs/_build/_images/math/b2d6dc4fcda6f6f3f2680612e6b7a18f566cfd71.png
+-rw-rw-rw-   0        0        0      821 2023-03-30 08:57:16.000000 dhnx-0.0.3/docs/_build/_images/math/b606db855d29e72cc630e8dc0d4b876dd7dc3939.png
+-rw-rw-rw-   0        0        0      236 2023-03-30 08:57:10.000000 dhnx-0.0.3/docs/_build/_images/math/b69a0d1ac6a8b838873d4de3cf73b8d5f886bb32.png
+-rw-rw-rw-   0        0        0      321 2023-03-30 08:56:56.000000 dhnx-0.0.3/docs/_build/_images/math/b7dbb459b1082a088ef44dd443608334a6d895f2.png
+-rw-rw-rw-   0        0        0      613 2023-03-30 08:56:33.000000 dhnx-0.0.3/docs/_build/_images/math/b91f685ffa4212b42bf9ce83cb3f4c9461d432b7.png
+-rw-rw-rw-   0        0        0     1773 2023-03-30 08:57:19.000000 dhnx-0.0.3/docs/_build/_images/math/bb51093d70168e72cbc974f40aa65b871fe23e8d.png
+-rw-rw-rw-   0        0        0      468 2023-03-30 08:56:23.000000 dhnx-0.0.3/docs/_build/_images/math/bf02f64401f09bd54bb29badbcf6481bbd3951ea.png
+-rw-rw-rw-   0        0        0      891 2023-03-30 08:57:15.000000 dhnx-0.0.3/docs/_build/_images/math/bf29cc27a3b9db8053c757eaec38435262938461.png
+-rw-rw-rw-   0        0        0      715 2023-03-30 08:56:42.000000 dhnx-0.0.3/docs/_build/_images/math/bf5c111491fc9d0abcf4dcf3fbe73c7e77bf7888.png
+-rw-rw-rw-   0        0        0      317 2023-03-30 08:56:50.000000 dhnx-0.0.3/docs/_build/_images/math/c169b424e57d974694c091fda6f50659df79a1c4.png
+-rw-rw-rw-   0        0        0      247 2023-03-30 08:56:48.000000 dhnx-0.0.3/docs/_build/_images/math/c2aa3dff9bffb099e9dff196fd36aed56ec16baf.png
+-rw-rw-rw-   0        0        0      456 2023-03-30 08:56:28.000000 dhnx-0.0.3/docs/_build/_images/math/c7d75575e76de17f63e0ab8ceb14b31f042300d0.png
+-rw-rw-rw-   0        0        0      234 2023-03-30 08:56:34.000000 dhnx-0.0.3/docs/_build/_images/math/cefc603e5658facb747581f9567192993f21c7ab.png
+-rw-rw-rw-   0        0        0      406 2023-03-30 08:56:54.000000 dhnx-0.0.3/docs/_build/_images/math/cf5cadc1060646f2311ff6f403ada02cb756d063.png
+-rw-rw-rw-   0        0        0      726 2023-03-30 08:57:14.000000 dhnx-0.0.3/docs/_build/_images/math/e5a44337e542130e2431752c5907693c764ed5b9.png
+-rw-rw-rw-   0        0        0      274 2023-03-30 08:56:27.000000 dhnx-0.0.3/docs/_build/_images/math/e97bcbb05e77c30b2b660c3d96ea770b65110c19.png
+-rw-rw-rw-   0        0        0      722 2023-03-30 08:57:18.000000 dhnx-0.0.3/docs/_build/_images/math/e9a30abeda6909ef7f5c230d9160126c2ccecc5e.png
+-rw-rw-rw-   0        0        0      316 2023-03-30 08:56:45.000000 dhnx-0.0.3/docs/_build/_images/math/f12ce3b406b4c58f728cff19ce0a989e0455e15a.png
+-rw-rw-rw-   0        0        0      908 2023-03-30 08:57:17.000000 dhnx-0.0.3/docs/_build/_images/math/f4e6c7b4acf05d839965874b76a7bfd301cdf2a5.png
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.697163 dhnx-0.0.3/docs/_build/_sources/
+-rw-rw-rw-   0        0        0      125 2021-07-08 17:37:48.000000 dhnx-0.0.3/docs/_build/_sources/analyze_and_plot.rst.txt
+-rw-rw-rw-   0        0        0     1892 2022-05-17 08:24:28.000000 dhnx-0.0.3/docs/_build/_sources/api.rst.txt
+-rw-rw-rw-   0        0        0     5831 2023-03-30 08:56:18.000000 dhnx-0.0.3/docs/_build/analyze_and_plot.html
+-rw-rw-rw-   0        0        0   224253 2023-03-30 08:57:21.000000 dhnx-0.0.3/docs/_build/api.html
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.728405 dhnx-0.0.3/docs/_static/
+-rw-rw-rw-   0        0        0    56682 2021-07-08 17:37:48.000000 dhnx-0.0.3/docs/_static/DHNx_Input_data.svg
+-rw-rw-rw-   0        0        0      119 2021-07-08 17:37:48.000000 dhnx-0.0.3/docs/_static/intro_consumers.csv
+-rw-rw-rw-   0        0        0    35606 2021-07-08 17:37:48.000000 dhnx-0.0.3/docs/_static/intro_opti_network.svg
+-rw-rw-rw-   0        0        0    35310 2021-07-08 17:37:48.000000 dhnx-0.0.3/docs/_static/intro_opti_network_results.svg
+-rw-rw-rw-   0        0        0    34691 2021-07-08 17:37:48.000000 dhnx-0.0.3/docs/_static/intro_opti_network_results_2.svg
+-rw-rw-rw-   0        0        0      125 2021-07-08 17:37:48.000000 dhnx-0.0.3/docs/_static/intro_pipes.csv
+-rw-rw-rw-   0        0        0       39 2021-07-08 17:37:48.000000 dhnx-0.0.3/docs/_static/intro_producers_deactive.csv
+-rw-rw-rw-   0        0        0       40 2021-07-08 17:37:48.000000 dhnx-0.0.3/docs/_static/opti_consumer_demand.csv
+-rw-rw-rw-   0        0        0       38 2021-07-08 17:37:48.000000 dhnx-0.0.3/docs/_static/opti_consumers-heat_flow_example.csv
+-rw-rw-rw-   0        0        0      214 2021-07-08 17:37:48.000000 dhnx-0.0.3/docs/_static/opti_consumers.csv
+-rw-rw-rw-   0        0        0      435 2021-07-08 17:37:48.000000 dhnx-0.0.3/docs/_static/opti_edges.csv
+-rw-rw-rw-   0        0        0      106 2021-07-08 17:37:48.000000 dhnx-0.0.3/docs/_static/opti_forks.csv
+-rw-rw-rw-   0        0        0      367 2021-07-08 17:37:48.000000 dhnx-0.0.3/docs/_static/opti_label_sys.csv
+-rw-rw-rw-   0        0        0      121 2021-07-08 17:37:48.000000 dhnx-0.0.3/docs/_static/opti_pipes.csv
+-rw-rw-rw-   0        0        0       24 2021-07-08 17:37:48.000000 dhnx-0.0.3/docs/_static/opti_producer_source.csv
+-rw-rw-rw-   0        0        0      140 2021-07-08 17:37:48.000000 dhnx-0.0.3/docs/_static/opti_producers.csv
+-rw-rw-rw-   0        0        0      913 2021-07-08 17:37:48.000000 dhnx-0.0.3/docs/_static/opti_results.csv
+-rw-rw-rw-   0        0        0      998 2021-07-08 17:37:48.000000 dhnx-0.0.3/docs/_static/opti_settings.csv
+-rw-rw-rw-   0        0        0    24536 2021-07-08 17:37:48.000000 dhnx-0.0.3/docs/_static/radial_network_details.svg
+-rw-rw-rw-   0        0        0     1863 2021-07-08 17:37:48.000000 dhnx-0.0.3/docs/_static/simulation_models.csv
+-rw-rw-rw-   0        0        0       69 2021-07-08 17:37:48.000000 dhnx-0.0.3/docs/_static/theme_overrides.css
+-rw-rw-rw-   0        0        0      125 2021-07-08 17:37:48.000000 dhnx-0.0.3/docs/analyze_and_plot.rst
+-rw-rw-rw-   0        0        0     1892 2023-04-19 08:22:25.000000 dhnx-0.0.3/docs/api.rst
+-rw-rw-rw-   0        0        0       29 2021-07-08 17:37:48.000000 dhnx-0.0.3/docs/authors.rst
+-rw-rw-rw-   0        0        0     1562 2023-04-19 08:22:25.000000 dhnx-0.0.3/docs/conf.py
+-rw-rw-rw-   0        0        0      744 2022-04-21 14:23:27.000000 dhnx-0.0.3/docs/examples.rst
+-rw-rw-rw-   0        0        0      692 2022-04-21 14:23:27.000000 dhnx-0.0.3/docs/geometry_preparation.rst
+-rw-rw-rw-   0        0        0     2208 2023-04-19 08:22:25.000000 dhnx-0.0.3/docs/getting_started.rst
+-rw-rw-rw-   0        0        0      775 2023-04-19 08:22:25.000000 dhnx-0.0.3/docs/index.rst
+-rw-rw-rw-   0        0        0       75 2021-07-08 17:37:48.000000 dhnx-0.0.3/docs/model_coupling.rst
+-rw-rw-rw-   0        0        0     1841 2021-07-08 17:37:48.000000 dhnx-0.0.3/docs/network.rst
+-rw-rw-rw-   0        0        0    25890 2023-04-19 08:22:25.000000 dhnx-0.0.3/docs/optimization_models.rst
+-rw-rw-rw-   0        0        0       37 2023-04-19 08:22:25.000000 dhnx-0.0.3/docs/requirements.txt
+-rw-rw-rw-   0        0        0     9962 2023-04-19 08:22:25.000000 dhnx-0.0.3/docs/simulation_models.rst
+-rw-rw-rw-   0        0        0      275 2023-04-19 08:22:25.000000 dhnx-0.0.3/docs/whats_new.rst
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.728405 dhnx-0.0.3/docs/whatsnew/
+-rw-rw-rw-   0        0        0      223 2021-07-08 17:37:48.000000 dhnx-0.0.3/docs/whatsnew/v0-0-1.rst
+-rw-rw-rw-   0        0        0     1259 2023-04-19 08:22:25.000000 dhnx-0.0.3/docs/whatsnew/v0-0-2.rst
+-rw-rw-rw-   0        0        0     1215 2023-04-19 08:22:25.000000 dhnx-0.0.3/docs/whatsnew/v0-0-3.rst
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.465425 dhnx-0.0.3/examples/
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.728405 dhnx-0.0.3/examples/import_export_plot/
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.744026 dhnx-0.0.3/examples/import_export_plot/data_csv_input/
+-rw-rw-rw-   0        0        0       56 2021-07-08 17:37:48.000000 dhnx-0.0.3/examples/import_export_plot/data_csv_input/consumers.csv
+-rw-rw-rw-   0        0        0       65 2021-07-08 17:37:48.000000 dhnx-0.0.3/examples/import_export_plot/data_csv_input/forks.csv
+-rw-rw-rw-   0        0        0      299 2021-07-08 17:37:48.000000 dhnx-0.0.3/examples/import_export_plot/data_csv_input/pipes.csv
+-rw-rw-rw-   0        0        0       31 2021-07-08 17:37:48.000000 dhnx-0.0.3/examples/import_export_plot/data_csv_input/producers.csv
+-rw-rw-rw-   0        0        0      829 2023-04-19 08:22:25.000000 dhnx-0.0.3/examples/import_export_plot/import_export_plot.py
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.744026 dhnx-0.0.3/examples/import_osmnx/
+-rw-rw-rw-   0        0        0      489 2023-04-19 08:22:25.000000 dhnx-0.0.3/examples/import_osmnx/import_osmnx.py
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.465425 dhnx-0.0.3/examples/optimisation/
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.744026 dhnx-0.0.3/examples/optimisation/discrete_DN_numbers/
+-rw-rw-rw-   0        0        0     3105 2023-04-19 08:22:25.000000 dhnx-0.0.3/examples/optimisation/discrete_DN_numbers/discrete_DN_numbers.py
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.443552 dhnx-0.0.3/examples/optimisation/discrete_DN_numbers/invest_data/
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.744026 dhnx-0.0.3/examples/optimisation/discrete_DN_numbers/invest_data/consumers/
+-rw-rw-rw-   0        0        0       84 2023-04-19 08:22:25.000000 dhnx-0.0.3/examples/optimisation/discrete_DN_numbers/invest_data/consumers/bus.csv
+-rw-rw-rw-   0        0        0       40 2023-04-19 08:22:25.000000 dhnx-0.0.3/examples/optimisation/discrete_DN_numbers/invest_data/consumers/demand.csv
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.744026 dhnx-0.0.3/examples/optimisation/discrete_DN_numbers/invest_data/network/
+-rw-rw-rw-   0        0        0      263 2023-04-19 08:22:25.000000 dhnx-0.0.3/examples/optimisation/discrete_DN_numbers/invest_data/network/pipes.csv
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.744026 dhnx-0.0.3/examples/optimisation/discrete_DN_numbers/invest_data/producers/
+-rw-rw-rw-   0        0        0       85 2023-04-19 08:22:25.000000 dhnx-0.0.3/examples/optimisation/discrete_DN_numbers/invest_data/producers/bus.csv
+-rw-rw-rw-   0        0        0       24 2023-04-19 08:22:25.000000 dhnx-0.0.3/examples/optimisation/discrete_DN_numbers/invest_data/producers/source.csv
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.759648 dhnx-0.0.3/examples/optimisation/discrete_DN_numbers/twn_data/
+-rw-rw-rw-   0        0        0      119 2023-04-19 08:22:25.000000 dhnx-0.0.3/examples/optimisation/discrete_DN_numbers/twn_data/consumers.csv
+-rw-rw-rw-   0        0        0      112 2023-04-19 08:22:25.000000 dhnx-0.0.3/examples/optimisation/discrete_DN_numbers/twn_data/forks.csv
+-rw-rw-rw-   0        0        0      520 2023-04-19 08:22:25.000000 dhnx-0.0.3/examples/optimisation/discrete_DN_numbers/twn_data/pipes.csv
+-rw-rw-rw-   0        0        0       29 2023-04-19 08:22:25.000000 dhnx-0.0.3/examples/optimisation/discrete_DN_numbers/twn_data/producers.csv
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.759648 dhnx-0.0.3/examples/optimisation/import_osm_invest/
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.797400 dhnx-0.0.3/examples/optimisation/import_osm_invest/cache/
+-rw-rw-rw-   0        0        0    92396 2022-06-12 12:04:42.000000 dhnx-0.0.3/examples/optimisation/import_osm_invest/cache/000234cf69ecb32b91774c749533af761504b2b5.json
+-rw-rw-rw-   0        0        0   244517 2022-06-12 12:09:38.000000 dhnx-0.0.3/examples/optimisation/import_osm_invest/cache/04bd6206691751601e55bd05f11a5f52d4210601.json
+-rw-rw-rw-   0        0        0   392809 2022-06-12 12:16:23.000000 dhnx-0.0.3/examples/optimisation/import_osm_invest/cache/292d7b70e78df37d3399b135bdd737b095e0637d.json
+-rw-rw-rw-   0        0        0  1173061 2022-06-12 11:49:54.000000 dhnx-0.0.3/examples/optimisation/import_osm_invest/cache/30c0cc99f6bea44290bde1bc0d0e7a67dd1652e4.json
+-rw-rw-rw-   0        0        0   145228 2022-06-12 12:30:19.000000 dhnx-0.0.3/examples/optimisation/import_osm_invest/cache/3a4c66cc6dbdd36c265cea5570d4329f1a01cef2.json
+-rw-rw-rw-   0        0        0   168407 2022-06-12 12:24:10.000000 dhnx-0.0.3/examples/optimisation/import_osm_invest/cache/448b9ee83074da6c964f1a68567176fee10aa2c9.json
+-rw-rw-rw-   0        0        0    24010 2022-10-05 12:06:58.000000 dhnx-0.0.3/examples/optimisation/import_osm_invest/cache/6999363322f2627c411f53b3ec0fe37d337aabd2.json
+-rw-rw-rw-   0        0        0  2439342 2022-06-12 12:14:00.000000 dhnx-0.0.3/examples/optimisation/import_osm_invest/cache/69befc6adcf582e656d480b99389d31e8059285b.json
+-rw-rw-rw-   0        0        0   684588 2022-06-12 11:50:59.000000 dhnx-0.0.3/examples/optimisation/import_osm_invest/cache/85bddb52dd2525c91505559c999b57cbec45fc96.json
+-rw-rw-rw-   0        0        0    37844 2022-06-12 12:25:11.000000 dhnx-0.0.3/examples/optimisation/import_osm_invest/cache/8eabe7f19a83624f666697f09411400538b46de1.json
+-rw-rw-rw-   0        0        0   388936 2022-06-12 12:08:37.000000 dhnx-0.0.3/examples/optimisation/import_osm_invest/cache/903a1cce4672d6407005a0987af22234541cf2db.json
+-rw-rw-rw-   0        0        0   257211 2022-06-12 12:27:24.000000 dhnx-0.0.3/examples/optimisation/import_osm_invest/cache/a066ce375a9610f6e73aee6308323ff3e8730025.json
+-rw-rw-rw-   0        0        0   331146 2022-10-05 12:05:50.000000 dhnx-0.0.3/examples/optimisation/import_osm_invest/cache/b307460ce8dbac4b730d58dc916862ea6b3d0c2b.json
+-rw-rw-rw-   0        0        0    75393 2022-10-05 12:08:01.000000 dhnx-0.0.3/examples/optimisation/import_osm_invest/cache/b6082021ce9cc8db2eda422ac1c45f8c31458c87.json
+-rw-rw-rw-   0        0        0   920036 2022-06-12 12:28:27.000000 dhnx-0.0.3/examples/optimisation/import_osm_invest/cache/b813e218813f04893b6dbbe09874870ef2162f24.json
+-rw-rw-rw-   0        0        0   441784 2022-06-12 12:07:32.000000 dhnx-0.0.3/examples/optimisation/import_osm_invest/cache/c0a1c57c2db7648ce34d3a0afa1abe0473b2441a.json
+-rw-rw-rw-   0        0        0    30177 2022-06-12 12:05:44.000000 dhnx-0.0.3/examples/optimisation/import_osm_invest/cache/c93baa87a5806c3186608705172718bc6dab4f98.json
+-rw-rw-rw-   0        0        0   776268 2022-06-12 11:48:32.000000 dhnx-0.0.3/examples/optimisation/import_osm_invest/cache/ca5208264922cba77bc7855ba655f3a0c3dedfef.json
+-rw-rw-rw-   0        0        0   174403 2022-06-12 12:03:39.000000 dhnx-0.0.3/examples/optimisation/import_osm_invest/cache/fc1c1f3d1ef4f0279131edced8e1f3476a92ae33.json
+-rw-rw-rw-   0        0        0     6630 2023-04-19 08:22:25.000000 dhnx-0.0.3/examples/optimisation/import_osm_invest/import_osm_invest.py
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.443552 dhnx-0.0.3/examples/optimisation/import_osm_invest/invest_data/
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.797400 dhnx-0.0.3/examples/optimisation/import_osm_invest/invest_data/consumers/
+-rw-rw-rw-   0        0        0       84 2023-04-19 08:22:25.000000 dhnx-0.0.3/examples/optimisation/import_osm_invest/invest_data/consumers/bus.csv
+-rw-rw-rw-   0        0        0       40 2023-04-19 08:22:25.000000 dhnx-0.0.3/examples/optimisation/import_osm_invest/invest_data/consumers/demand.csv
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.797400 dhnx-0.0.3/examples/optimisation/import_osm_invest/invest_data/network/
+-rw-rw-rw-   0        0        0      125 2023-04-19 08:22:25.000000 dhnx-0.0.3/examples/optimisation/import_osm_invest/invest_data/network/pipes.csv
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.813022 dhnx-0.0.3/examples/optimisation/import_osm_invest/invest_data/producers/
+-rw-rw-rw-   0        0        0       85 2023-04-19 08:22:25.000000 dhnx-0.0.3/examples/optimisation/import_osm_invest/invest_data/producers/bus.csv
+-rw-rw-rw-   0        0        0       24 2023-04-19 08:22:25.000000 dhnx-0.0.3/examples/optimisation/import_osm_invest/invest_data/producers/source.csv
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.813022 dhnx-0.0.3/examples/optimisation/introduction/
+-rw-rw-rw-   0        0        0     2303 2023-04-19 08:22:25.000000 dhnx-0.0.3/examples/optimisation/introduction/introduction.py
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.457420 dhnx-0.0.3/examples/optimisation/introduction/invest_data/
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.813022 dhnx-0.0.3/examples/optimisation/introduction/invest_data/consumers/
+-rw-rw-rw-   0        0        0       84 2023-04-19 08:22:25.000000 dhnx-0.0.3/examples/optimisation/introduction/invest_data/consumers/bus.csv
+-rw-rw-rw-   0        0        0       40 2023-04-19 08:22:25.000000 dhnx-0.0.3/examples/optimisation/introduction/invest_data/consumers/demand.csv
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.813022 dhnx-0.0.3/examples/optimisation/introduction/invest_data/network/
+-rw-rw-rw-   0        0        0      125 2023-04-19 08:22:25.000000 dhnx-0.0.3/examples/optimisation/introduction/invest_data/network/pipes.csv
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.813022 dhnx-0.0.3/examples/optimisation/introduction/invest_data/producers/
+-rw-rw-rw-   0        0        0       85 2023-04-19 08:22:25.000000 dhnx-0.0.3/examples/optimisation/introduction/invest_data/producers/bus.csv
+-rw-rw-rw-   0        0        0       24 2023-04-19 08:22:25.000000 dhnx-0.0.3/examples/optimisation/introduction/invest_data/producers/source.csv
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.828643 dhnx-0.0.3/examples/optimisation/introduction/twn_data/
+-rw-rw-rw-   0        0        0      119 2023-04-19 08:22:25.000000 dhnx-0.0.3/examples/optimisation/introduction/twn_data/consumers.csv
+-rw-rw-rw-   0        0        0      112 2023-04-19 08:22:25.000000 dhnx-0.0.3/examples/optimisation/introduction/twn_data/forks.csv
+-rw-rw-rw-   0        0        0      546 2023-04-19 08:22:25.000000 dhnx-0.0.3/examples/optimisation/introduction/twn_data/pipes.csv
+-rw-rw-rw-   0        0        0       39 2023-04-19 08:22:25.000000 dhnx-0.0.3/examples/optimisation/introduction/twn_data/producers.csv
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.828643 dhnx-0.0.3/examples/optimisation/invest_with_existing/
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.457420 dhnx-0.0.3/examples/optimisation/invest_with_existing/invest_data/
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.828643 dhnx-0.0.3/examples/optimisation/invest_with_existing/invest_data/consumers/
+-rw-rw-rw-   0        0        0      110 2023-04-19 08:22:25.000000 dhnx-0.0.3/examples/optimisation/invest_with_existing/invest_data/consumers/bus.csv
+-rw-rw-rw-   0        0        0       43 2023-04-19 08:22:25.000000 dhnx-0.0.3/examples/optimisation/invest_with_existing/invest_data/consumers/demand.csv
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.828643 dhnx-0.0.3/examples/optimisation/invest_with_existing/invest_data/network/
+-rw-rw-rw-   0        0        0      147 2023-04-19 08:22:25.000000 dhnx-0.0.3/examples/optimisation/invest_with_existing/invest_data/network/pipes.csv
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.828643 dhnx-0.0.3/examples/optimisation/invest_with_existing/invest_data/producers/
+-rw-rw-rw-   0        0        0      108 2023-04-19 08:22:25.000000 dhnx-0.0.3/examples/optimisation/invest_with_existing/invest_data/producers/bus.csv
+-rw-rw-rw-   0        0        0       44 2023-04-19 08:22:25.000000 dhnx-0.0.3/examples/optimisation/invest_with_existing/invest_data/producers/source.csv
+-rw-rw-rw-   0        0        0     1674 2023-04-19 08:22:25.000000 dhnx-0.0.3/examples/optimisation/invest_with_existing/invest_with_existing.py
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.828643 dhnx-0.0.3/examples/optimisation/invest_with_existing/twn_data/
+-rw-rw-rw-   0        0        0      128 2023-04-19 08:22:25.000000 dhnx-0.0.3/examples/optimisation/invest_with_existing/twn_data/consumers.csv
+-rw-rw-rw-   0        0        0       65 2023-04-19 08:22:25.000000 dhnx-0.0.3/examples/optimisation/invest_with_existing/twn_data/forks.csv
+-rw-rw-rw-   0        0        0      378 2023-04-19 08:22:25.000000 dhnx-0.0.3/examples/optimisation/invest_with_existing/twn_data/pipes.csv
+-rw-rw-rw-   0        0        0       37 2023-04-19 08:22:25.000000 dhnx-0.0.3/examples/optimisation/invest_with_existing/twn_data/producers.csv
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.844262 dhnx-0.0.3/examples/optimisation/invest_with_existing/twn_data/sequences/
+-rw-rw-rw-   0        0        0       38 2023-04-19 08:22:25.000000 dhnx-0.0.3/examples/optimisation/invest_with_existing/twn_data/sequences/consumers-heat_flow.csv
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.844262 dhnx-0.0.3/examples/optimisation/minimal_network/
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.465425 dhnx-0.0.3/examples/optimisation/minimal_network/invest_data/
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.844262 dhnx-0.0.3/examples/optimisation/minimal_network/invest_data/consumers/
+-rw-rw-rw-   0        0        0       84 2023-04-19 08:22:25.000000 dhnx-0.0.3/examples/optimisation/minimal_network/invest_data/consumers/bus.csv
+-rw-rw-rw-   0        0        0       40 2023-04-19 08:22:25.000000 dhnx-0.0.3/examples/optimisation/minimal_network/invest_data/consumers/demand.csv
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.844262 dhnx-0.0.3/examples/optimisation/minimal_network/invest_data/network/
+-rw-rw-rw-   0        0        0      121 2023-04-19 08:22:25.000000 dhnx-0.0.3/examples/optimisation/minimal_network/invest_data/network/pipes.csv
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.844262 dhnx-0.0.3/examples/optimisation/minimal_network/invest_data/producers/
+-rw-rw-rw-   0        0        0       85 2023-04-19 08:22:25.000000 dhnx-0.0.3/examples/optimisation/minimal_network/invest_data/producers/bus.csv
+-rw-rw-rw-   0        0        0       24 2023-04-19 08:22:25.000000 dhnx-0.0.3/examples/optimisation/minimal_network/invest_data/producers/source.csv
+-rw-rw-rw-   0        0        0     1366 2023-04-19 08:22:25.000000 dhnx-0.0.3/examples/optimisation/minimal_network/minimal_network.py
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.859884 dhnx-0.0.3/examples/optimisation/minimal_network/twn_data/
+-rw-rw-rw-   0        0        0       45 2023-04-19 08:22:25.000000 dhnx-0.0.3/examples/optimisation/minimal_network/twn_data/consumers.csv
+-rw-rw-rw-   0        0        0       33 2023-04-19 08:22:25.000000 dhnx-0.0.3/examples/optimisation/minimal_network/twn_data/forks.csv
+-rw-rw-rw-   0        0        0      216 2023-04-19 08:22:25.000000 dhnx-0.0.3/examples/optimisation/minimal_network/twn_data/pipes.csv
+-rw-rw-rw-   0        0        0       28 2023-04-19 08:22:25.000000 dhnx-0.0.3/examples/optimisation/minimal_network/twn_data/producers.csv
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.465425 dhnx-0.0.3/examples/optimisation/optimisation_tutorial/
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.866389 dhnx-0.0.3/examples/optimisation/optimisation_tutorial/cache/
+-rw-rw-rw-   0        0        0    92444 2023-04-03 09:34:43.000000 dhnx-0.0.3/examples/optimisation/optimisation_tutorial/cache/000234cf69ecb32b91774c749533af761504b2b5.json
+-rw-rw-rw-   0        0        0    30419 2023-04-03 09:34:45.000000 dhnx-0.0.3/examples/optimisation/optimisation_tutorial/cache/c93baa87a5806c3186608705172718bc6dab4f98.json
+-rw-rw-rw-   0        0        0   172674 2023-04-03 09:34:41.000000 dhnx-0.0.3/examples/optimisation/optimisation_tutorial/cache/fc1c1f3d1ef4f0279131edced8e1f3476a92ae33.json
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.866389 dhnx-0.0.3/examples/optimisation/precalculation/
+-rw-rw-rw-   0        0        0      552 2023-04-19 08:22:25.000000 dhnx-0.0.3/examples/optimisation/precalculation/Pipe_data.csv
+-rw-rw-rw-   0        0        0     2739 2023-04-19 08:22:25.000000 dhnx-0.0.3/examples/optimisation/precalculation/hydraulic_precalculation.py
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.866389 dhnx-0.0.3/examples/simulation/
+-rw-rw-rw-   0        0        0      658 2023-04-19 08:22:25.000000 dhnx-0.0.3/examples/simulation/simulation_example.py
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.866389 dhnx-0.0.3/examples/simulation/single_pipe/
+-rw-rw-rw-   0        0        0       29 2021-07-08 17:37:48.000000 dhnx-0.0.3/examples/simulation/single_pipe/consumers.csv
+-rw-rw-rw-   0        0        0      116 2021-07-08 17:37:48.000000 dhnx-0.0.3/examples/simulation/single_pipe/pipes.csv
+-rw-rw-rw-   0        0        0       31 2021-07-08 17:37:48.000000 dhnx-0.0.3/examples/simulation/single_pipe/producers.csv
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.882015 dhnx-0.0.3/examples/simulation/single_pipe/sequences/
+-rw-rw-rw-   0        0        0       30 2021-07-08 17:37:48.000000 dhnx-0.0.3/examples/simulation/single_pipe/sequences/consumers-delta_temp_drop.csv
+-rw-rw-rw-   0        0        0       34 2021-07-08 17:37:48.000000 dhnx-0.0.3/examples/simulation/single_pipe/sequences/consumers-mass_flow.csv
+-rw-rw-rw-   0        0        0       35 2021-07-08 17:37:48.000000 dhnx-0.0.3/examples/simulation/single_pipe/sequences/environment-temp_env.csv
+-rw-rw-rw-   0        0        0       31 2021-07-08 17:37:48.000000 dhnx-0.0.3/examples/simulation/single_pipe/sequences/producers-temp_inlet.csv
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.882015 dhnx-0.0.3/examples/simulation/tree/
+-rw-rw-rw-   0        0        0       75 2021-07-08 17:37:48.000000 dhnx-0.0.3/examples/simulation/tree/consumers.csv
+-rw-rw-rw-   0        0        0       96 2021-07-08 17:37:48.000000 dhnx-0.0.3/examples/simulation/tree/forks.csv
+-rw-rw-rw-   0        0        0      192 2021-07-08 17:37:48.000000 dhnx-0.0.3/examples/simulation/tree/pipes.csv
+-rw-rw-rw-   0        0        0       46 2021-07-08 17:37:48.000000 dhnx-0.0.3/examples/simulation/tree/producers.csv
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.882015 dhnx-0.0.3/examples/simulation/tree/sequences/
+-rw-rw-rw-   0        0        0       41 2021-07-08 17:37:48.000000 dhnx-0.0.3/examples/simulation/tree/sequences/consumers-delta_temp_drop.csv
+-rw-rw-rw-   0        0        0       49 2021-07-08 17:37:48.000000 dhnx-0.0.3/examples/simulation/tree/sequences/consumers-mass_flow.csv
+-rw-rw-rw-   0        0        0       35 2021-07-08 17:37:48.000000 dhnx-0.0.3/examples/simulation/tree/sequences/environment-temp_env.csv
+-rw-rw-rw-   0        0        0       31 2021-07-08 17:37:48.000000 dhnx-0.0.3/examples/simulation/tree/sequences/producers-temp_inlet.csv
+-rw-rw-rw-   0        0        0      985 2023-04-19 08:32:47.966623 dhnx-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1196 2023-04-19 08:22:25.000000 dhnx-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.897635 dhnx-0.0.3/tests/
+-rw-rw-rw-   0        0        0        0 2021-07-08 17:37:48.000000 dhnx-0.0.3/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.465425 dhnx-0.0.3/tests/_files/
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.913256 dhnx-0.0.3/tests/_files/inconsistent_network_import/
+-rw-rw-rw-   0        0        0       47 2021-07-08 17:37:48.000000 dhnx-0.0.3/tests/_files/inconsistent_network_import/consumers.csv
+-rw-rw-rw-   0        0        0       64 2021-07-08 17:37:48.000000 dhnx-0.0.3/tests/_files/inconsistent_network_import/forks.csv
+-rw-rw-rw-   0        0        0      299 2021-07-08 17:37:48.000000 dhnx-0.0.3/tests/_files/inconsistent_network_import/pipes.csv
+-rw-rw-rw-   0        0        0       28 2021-07-08 17:37:48.000000 dhnx-0.0.3/tests/_files/inconsistent_network_import/producers.csv
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.465425 dhnx-0.0.3/tests/_files/investment/
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.465425 dhnx-0.0.3/tests/_files/investment/invest_options/
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.913256 dhnx-0.0.3/tests/_files/investment/invest_options/consumers/
+-rw-rw-rw-   0        0        0       87 2021-07-08 17:37:48.000000 dhnx-0.0.3/tests/_files/investment/invest_options/consumers/bus.csv
+-rw-rw-rw-   0        0        0       43 2021-07-08 17:37:48.000000 dhnx-0.0.3/tests/_files/investment/invest_options/consumers/demand.csv
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.913256 dhnx-0.0.3/tests/_files/investment/invest_options/network/
+-rw-rw-rw-   0        0        0      141 2021-07-08 17:37:48.000000 dhnx-0.0.3/tests/_files/investment/invest_options/network/pipes.csv
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.913256 dhnx-0.0.3/tests/_files/investment/invest_options/producers/
+-rw-rw-rw-   0        0        0       85 2021-07-08 17:37:48.000000 dhnx-0.0.3/tests/_files/investment/invest_options/producers/bus.csv
+-rw-rw-rw-   0        0        0       44 2021-07-08 17:37:48.000000 dhnx-0.0.3/tests/_files/investment/invest_options/producers/source.csv
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.928877 dhnx-0.0.3/tests/_files/investment/network/
+-rw-rw-rw-   0        0        0       45 2021-07-08 17:37:48.000000 dhnx-0.0.3/tests/_files/investment/network/consumers.csv
+-rw-rw-rw-   0        0        0       33 2021-07-08 17:37:48.000000 dhnx-0.0.3/tests/_files/investment/network/forks.csv
+-rw-rw-rw-   0        0        0      216 2021-07-08 17:37:48.000000 dhnx-0.0.3/tests/_files/investment/network/pipes.csv
+-rw-rw-rw-   0        0        0       28 2021-07-08 17:37:48.000000 dhnx-0.0.3/tests/_files/investment/network/producers.csv
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.928877 dhnx-0.0.3/tests/_files/looped_network_import/
+-rw-rw-rw-   0        0        0       80 2021-07-08 17:37:48.000000 dhnx-0.0.3/tests/_files/looped_network_import/consumers.csv
+-rw-rw-rw-   0        0        0       94 2021-07-08 17:37:48.000000 dhnx-0.0.3/tests/_files/looped_network_import/forks.csv
+-rw-rw-rw-   0        0        0      342 2021-07-08 17:37:48.000000 dhnx-0.0.3/tests/_files/looped_network_import/pipes.csv
+-rw-rw-rw-   0        0        0       52 2021-07-08 17:37:48.000000 dhnx-0.0.3/tests/_files/looped_network_import/producers.csv
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.928877 dhnx-0.0.3/tests/_files/looped_network_import/sequences/
+-rw-rw-rw-   0        0        0       41 2021-07-08 17:37:48.000000 dhnx-0.0.3/tests/_files/looped_network_import/sequences/consumers-delta_temp_drop.csv
+-rw-rw-rw-   0        0        0       49 2021-07-08 17:37:48.000000 dhnx-0.0.3/tests/_files/looped_network_import/sequences/consumers-mass_flow.csv
+-rw-rw-rw-   0        0        0       35 2021-07-08 17:37:48.000000 dhnx-0.0.3/tests/_files/looped_network_import/sequences/environment-temp_env.csv
+-rw-rw-rw-   0        0        0       33 2021-07-08 17:37:48.000000 dhnx-0.0.3/tests/_files/looped_network_import/sequences/producers-temp_inlet.csv
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.944498 dhnx-0.0.3/tests/_files/tree_network_import/
+-rw-rw-rw-   0        0        0       75 2021-07-08 17:37:48.000000 dhnx-0.0.3/tests/_files/tree_network_import/consumers.csv
+-rw-rw-rw-   0        0        0       76 2021-07-08 17:37:48.000000 dhnx-0.0.3/tests/_files/tree_network_import/forks.csv
+-rw-rw-rw-   0        0        0      192 2021-07-08 17:37:48.000000 dhnx-0.0.3/tests/_files/tree_network_import/pipes.csv
+-rw-rw-rw-   0        0        0       46 2021-07-08 17:37:48.000000 dhnx-0.0.3/tests/_files/tree_network_import/producers.csv
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.944498 dhnx-0.0.3/tests/_files/tree_network_import/sequences/
+-rw-rw-rw-   0        0        0       41 2021-07-08 17:37:48.000000 dhnx-0.0.3/tests/_files/tree_network_import/sequences/consumers-delta_temp_drop.csv
+-rw-rw-rw-   0        0        0       49 2021-07-08 17:37:48.000000 dhnx-0.0.3/tests/_files/tree_network_import/sequences/consumers-mass_flow.csv
+-rw-rw-rw-   0        0        0       35 2021-07-08 17:37:48.000000 dhnx-0.0.3/tests/_files/tree_network_import/sequences/environment-temp_env.csv
+-rw-rw-rw-   0        0        0       31 2021-07-08 17:37:48.000000 dhnx-0.0.3/tests/_files/tree_network_import/sequences/producers-temp_inlet.csv
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.944498 dhnx-0.0.3/tests/_files/tree_network_sim_expected_results/
+-rw-rw-rw-   0        0        0     7718 2023-04-19 08:22:25.000000 dhnx-0.0.3/tests/_files/tree_network_sim_expected_results/calc_pressure_loss.py
+-rw-rw-rw-   0        0        0     7716 2023-04-19 08:22:25.000000 dhnx-0.0.3/tests/_files/tree_network_sim_expected_results/calc_temp_drop.py
+drwxrwxrwx   0        0        0        0 2023-04-19 08:32:47.966623 dhnx-0.0.3/tests/_files/tree_network_sim_expected_results/sequences/
+-rw-rw-rw-   0        0        0       92 2023-04-18 08:58:29.000000 dhnx-0.0.3/tests/_files/tree_network_sim_expected_results/sequences/global-heat_losses.csv
+-rw-rw-rw-   0        0        0       60 2023-04-18 08:58:28.000000 dhnx-0.0.3/tests/_files/tree_network_sim_expected_results/sequences/global-pressure_losses.csv
+-rw-rw-rw-   0        0        0      248 2023-04-18 08:58:29.000000 dhnx-0.0.3/tests/_files/tree_network_sim_expected_results/sequences/nodes-temp_inlet.csv
+-rw-rw-rw-   0        0        0      289 2023-04-18 08:58:29.000000 dhnx-0.0.3/tests/_files/tree_network_sim_expected_results/sequences/nodes-temp_return.csv
+-rw-rw-rw-   0        0        0      176 2023-04-18 08:58:28.000000 dhnx-0.0.3/tests/_files/tree_network_sim_expected_results/sequences/pipes-dist_pressure_losses.csv
+-rw-rw-rw-   0        0        0      187 2023-04-18 08:58:29.000000 dhnx-0.0.3/tests/_files/tree_network_sim_expected_results/sequences/pipes-heat_losses.csv
+-rw-rw-rw-   0        0        0       64 2023-04-18 08:58:29.000000 dhnx-0.0.3/tests/_files/tree_network_sim_expected_results/sequences/pipes-mass_flow.csv
+-rw-rw-rw-   0        0        0      175 2023-04-18 08:58:28.000000 dhnx-0.0.3/tests/_files/tree_network_sim_expected_results/sequences/pipes_loc_pressure_losses.csv
+-rw-rw-rw-   0        0        0       61 2023-04-18 08:58:28.000000 dhnx-0.0.3/tests/_files/tree_network_sim_expected_results/sequences/producers-pump_power.csv
+-rw-rw-rw-   0        0        0     3658 2023-04-19 08:22:25.000000 dhnx-0.0.3/tests/helpers.py
+-rw-rw-rw-   0        0        0     3274 2023-04-19 08:22:25.000000 dhnx-0.0.3/tests/test_errors.py
+-rw-rw-rw-   0        0        0     1659 2023-04-19 08:22:25.000000 dhnx-0.0.3/tests/test_gistools.py
+-rw-rw-rw-   0        0        0     2435 2023-04-19 08:22:25.000000 dhnx-0.0.3/tests/test_integration.py
+-rw-rw-rw-   0        0        0     3995 2023-04-19 08:22:25.000000 dhnx-0.0.3/tests/test_precalc_hydraulic.py
+-rw-rw-rw-   0        0        0       44 2022-04-21 14:23:27.000000 dhnx-0.0.3/tests/test_requirements.txt
+-rw-rw-rw-   0        0        0     2200 2023-04-19 08:22:25.000000 dhnx-0.0.3/tests/test_results.py
+-rw-rw-rw-   0        0        0      833 2023-04-19 08:22:25.000000 dhnx-0.0.3/tests/test_units.py
+-rw-rw-rw-   0        0        0     2330 2023-04-19 08:22:25.000000 dhnx-0.0.3/tox.ini
```

### Comparing `dhnx-0.0.2rc1/LICENSE` & `dhnx-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dhnx-0.0.2rc1/PKG-INFO` & `dhnx-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: dhnx
-Version: 0.0.2rc1
+Version: 0.0.3
 Summary: Simulation and optimization of district heating and cooling networks
-Home-page: UNKNOWN
 Author: oemof developer group
 Author-email: jann.launer@rl-institut.de, johannes-roeder@uni-bremen.de
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/x-rst
 Provides-Extra: cartopy
 Provides-Extra: geopandas
 Provides-Extra: osmnx
+Provides-Extra: tests
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 |badge_travis| |badge_coverage| |readthedocs| |zenodo|
 
 ~~~~
 DHNx
@@ -111,15 +109,13 @@
     :target: https://coveralls.io/github/oemof-heat/DHNx?branch=dev
     :alt: Test coverage
 
 .. |badge_travis| image:: https://api.travis-ci.org/oemof/DHNx.svg?branch=dev
     :target: https://travis-ci.org/oemof/DHNx
     :alt: Build status
 
-.. |zenodo| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.4147049.svg
-   :target: https://doi.org/10.5281/zenodo.4147049
+.. |zenodo| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.5084392.svg
+   :target: https://doi.org/10.5281/zenodo.5084392
 
 .. |readthedocs| image:: https://readthedocs.org/projects/dhnx/badge/?version=latest
     :target: https://dhnx.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
-
-
```

### Comparing `dhnx-0.0.2rc1/README.rst` & `dhnx-0.0.3/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -95,13 +95,13 @@
     :target: https://coveralls.io/github/oemof-heat/DHNx?branch=dev
     :alt: Test coverage
 
 .. |badge_travis| image:: https://api.travis-ci.org/oemof/DHNx.svg?branch=dev
     :target: https://travis-ci.org/oemof/DHNx
     :alt: Build status
 
-.. |zenodo| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.4147049.svg
-   :target: https://doi.org/10.5281/zenodo.4147049
+.. |zenodo| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.5084392.svg
+   :target: https://doi.org/10.5281/zenodo.5084392
 
 .. |readthedocs| image:: https://readthedocs.org/projects/dhnx/badge/?version=latest
     :target: https://dhnx.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
```

### Comparing `dhnx-0.0.2rc1/dhnx/component_attrs/consumers.csv` & `dhnx-0.0.3/dhnx/component_attrs/consumers.csv`

 * *Files identical despite different names*

### Comparing `dhnx-0.0.2rc1/dhnx/component_attrs/pipes.csv` & `dhnx-0.0.3/dhnx/component_attrs/pipes.csv`

 * *Files identical despite different names*

### Comparing `dhnx-0.0.2rc1/dhnx/component_attrs/producers.csv` & `dhnx-0.0.3/dhnx/component_attrs/producers.csv`

 * *Files identical despite different names*

### Comparing `dhnx-0.0.2rc1/dhnx/dhn_from_osm.py` & `dhnx-0.0.3/dhnx/dhn_from_osm.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 
 except ImportError:
     print("Need to install geopandas to process osm data.")
 
 import pandas as pd
 
 try:
-    from shapely.ops import nearest_points
     from shapely.geometry import LineString
+    from shapely.ops import nearest_points
 
 except ImportError:
     print("Need to install shapely to download from osm.")
 
 
 def connect_points_to_network(points, nodes, edges):
     r"""
```

### Comparing `dhnx-0.0.2rc1/dhnx/gistools/connect_points.py` & `dhnx-0.0.3/dhnx/gistools/connect_points.py`

 * *Files 21% similar despite different names*

```diff
@@ -16,22 +16,26 @@
 try:
     import geopandas as gpd
 
 except ImportError:
     print("Need to install geopandas to process geometry data.")
 
 try:
-    from shapely.ops import cascaded_union, nearest_points
-    from shapely.geometry import Point, LineString, shape, MultiPoint
+    from shapely.geometry import LineString
+    from shapely.geometry import MultiPoint
+    from shapely.geometry import Point
+    from shapely.ops import nearest_points
+    from shapely.ops import unary_union
 except ImportError:
     print("Need to install shapely to process geometry.")
 
+import logging
+
 import numpy as np
 import pandas as pd
-import logging
 
 from . import geometry_operations as go
 
 
 def line_of_point(point, gdf_lines):
     """Gets index of geometry of a GeoDataFrame, a point is located next to,
       with a distance lower than 1e-8.
@@ -81,17 +85,16 @@
     line : shapely.geometry.LineString
     point : shapely.geometry.Point
 
     Returns
     -------
     shapely.geometry.Point
     """
-
-    s_1 = shape(line).boundary[0]
-    s_2 = shape(line).boundary[1]
+    s_1 = Point(line.coords[0])
+    s_2 = Point(line.coords[-1])
 
     g_1 = point_to_array(s_1)  # end point 1 of line
     g_2 = point_to_array(s_2)  # end point 2 of line
 
     x_1 = point_to_array(point)
 
     # calculate lotfusspunkt
@@ -112,18 +115,22 @@
 
 
 def create_object_connections(points, lines, tol_distance=1):
     """Connects points to a line network.
 
     Generally, the nearest point of the next line is used as connection the point.
     Depending on the geometry, there are 3 options, the connection is created:
+
     - nearest point is line ending => the connection line starts from this line ending
+
     - nearest point is on the next line:
+
       a) line endings are outside the tolerance => line is split and the nearest point
       is used as connection point
+
       b) line endings are within the tolerance distance => the next line ending is
       used as connection point
 
     The tolerance distance avoids the generation of short line elements.
     This is for example the case if two buildings are directly opposite of the street.
     Using simply the nearest point method could result in very short lines.
 
@@ -148,26 +155,46 @@
     """
     # check linestrings
     for _, c in lines.iterrows():
         if len(c['geometry'].coords) > 2:
             raise ValueError("The Linestrings must consists of simple lines,"
                              " with only two coordinates!")
 
+    # Pepare merging all the street lines
+    all_lines = lines['geometry']
+
+    # There seems to be a conflict between shapely and pygeos,
+    # which both use 'geos' internally, if both are installed.
+    # This can cause
+    # 'OSError exception: access violation reading 0xFFFFFFFFFFFFFFFF'.
+    #
+    # With shapely 1.8.0 and pygeos 0.12.0 it was observed that
+    # this sometimes even fails without error. In such a case
+    # mergedlines might only contain a single LineString (one street
+    # segment) instead of a MultiLineString (the combined network
+    # of all street segments). This completely messes up the
+    # following nearest_points().
+    #
+    # Wrapping the argument in 'list()' seems to be a valid workaround.
+    # It may come with a performance cost, as noted here:
+    # https://github.com/geopandas/geopandas/issues/1820
+    # https://github.com/geopandas/geopandas/issues/2171
+    # This issue may disappear when shapely 2.0 is released (then pygeos
+    # is merged with shapely).
+    mergedlines = unary_union(list(all_lines))
+    # mergedlines = unary_union(all_lines)  # TODO Try this with shapely 2.0
+
     # empty geopandas dataframe for house connections
-    conn_lines = gpd.GeoDataFrame()
+    conn_lines = gpd.GeoDataFrame(geometry=[], crs=lines.crs)
 
     # iterate over all houses
     for index, row in points.iterrows():
 
         house_geo = row['geometry']
 
-        # the same with the original lines
-        all_lines = lines['geometry']
-        mergedlines = cascaded_union(all_lines)
-
         # new nearest point method  ############ #########
         n_p = nearest_points(mergedlines, house_geo)[0]
 
         # get index of line which is closest to the house
         line_index = line_of_point(n_p, lines)
 
         # get geometry of supply line
@@ -178,67 +205,72 @@
         supply_line_p1 = Point(list(supply_line.coords)[1])
         supply_line_points = [supply_line_p0, supply_line_p1]
         supply_line_mulitpoints = MultiPoint(supply_line_points)
 
         if n_p in supply_line_points:
             # case that nearest point is a line ending
 
-            logging.info(
+            logging.debug(
                 'Connect buildings... id {}: '
                 'Connected to supply line ending (nearest point)'.format(index)
             )
 
             con_line = LineString([n_p, house_geo])
 
-            conn_lines = conn_lines.append({'geometry': con_line}, ignore_index=True)
+            conn_lines = pd.concat(
+                [gpd.GeoDataFrame(conn_lines, crs=lines.crs),
+                 gpd.GeoDataFrame(geometry=[con_line], crs=lines.crs)],
+                ignore_index=True)
 
         else:
 
             dist_to_endings = [x.distance(n_p) for x in supply_line_points]
 
             if min(dist_to_endings) >= tol_distance:
                 # line is split, no line ending is close to the nearest point
                 # this also means the original supply line needs to be deleted
 
-                logging.info(
+                logging.debug(
                     'Connect buildings... id {}: Supply line split'.format(index))
 
                 con_line = LineString([n_p, house_geo])
 
-                conn_lines = conn_lines.append({'geometry': con_line}, ignore_index=True)
+                conn_lines = pd.concat(
+                    [gpd.GeoDataFrame(conn_lines, crs=lines.crs),
+                     gpd.GeoDataFrame(geometry=[con_line], crs=lines.crs)],
+                    ignore_index=True)
 
                 lines.drop([line_index], inplace=True)
 
-                lines = lines.append(
-                    {'geometry': LineString([supply_line_p0, n_p])},
-                    ignore_index=True
-                )
-                lines = lines.append(
-                    {'geometry': LineString([n_p, supply_line_p1])},
-                    ignore_index=True
-                )
+                lines = pd.concat(
+                    [gpd.GeoDataFrame(lines, crs=lines.crs),
+                     gpd.GeoDataFrame(geometry=[
+                         LineString([supply_line_p0, n_p]),
+                         LineString([n_p, supply_line_p1])], crs=lines.crs)],
+                    ignore_index=True)
 
             else:
                 # case that one or both line endings are closer than tolerance
                 # thus, the next line ending is chosen
-                logging.info(
-                    'Connect buildings... id {}: Connected to Supply line ending '
-                    'due to tolerance'.format(index))
+                logging.debug(
+                    'Connect buildings... id {}: Connected to Supply line '
+                    'ending due to tolerance'.format(index))
 
                 conn_point = nearest_points(supply_line_mulitpoints, n_p)[0]
 
                 con_line = LineString([conn_point, house_geo])
 
-                conn_lines = conn_lines.append({'geometry': con_line}, ignore_index=True)
+                conn_lines = pd.concat(
+                    [gpd.GeoDataFrame(conn_lines, crs=lines.crs),
+                     gpd.GeoDataFrame(geometry=[con_line], crs=lines.crs)],
+                    ignore_index=True)
 
     logging.info('Connection of buildings completed.')
 
-    connection_lines = gpd.GeoDataFrame(conn_lines, crs=lines.crs)
-
-    return connection_lines, lines
+    return conn_lines, lines
 
 
 def check_geometry_type(gdf, types):
     """
     Checks, if a geodataframe has only the given geometry types in its GeoSeries.
 
     Parameters
@@ -271,29 +303,157 @@
 
     Returns
     -------
     geopandas.GeoDataFrame : GeoDataFrame with a point geometry.
 
     """
 
-    if gdf['geometry'].values[0].type == 'Point':
+    if gdf['geometry'].values[0].geom_type == 'Point':
         return gdf
 
-    if method == 'midpoint':
+    if method == 'midpoint' or method == 'boundary':
+        # (method 'boundary' is performed later and needs the centroid)
         gdf['geometry'] = gdf['geometry'].centroid
         return gdf
 
     raise ValueError(
-        'No other method than >midpoint< implemented!'
+        "No other methods than 'midpoint' and 'boundary' implemented!"
     )
 
 
+def run_point_method_boundary(
+        consumers_poly, consumers, producers_poly, producers,
+        lines_consumers, lines_producers):
+    """Run 'boundary' method for finding the building connection point.
+
+    The 'midpoint' method (using the centroid) must already have been run,
+    generating the default connection lines from street to centroid.
+
+    If there is only one intersection between that line and the boundary
+    of the building, this intersection point is used as the connection
+    point instead (and the connection line is shortened accordingly).
+
+    However, complex building shapes can produce multiple intersections. In
+    this case, the intersection with the 'convex hull' of the building is used
+    instead. This may result in connection points that do not touch an
+    actual building wall, but it should still be an improvement compared to
+    the 'midpoint' method.
+
+    In case of no intersections with the building boundary (possible for e.g.
+    U-shaped buildings), the original centroid is used.
+
+    Parameters
+    ----------
+    consumers_poly : geopandas.GeoDataFrame
+        Polygons of the consumer buildings. Point geometries are also allowed,
+        but they are not changed.
+    consumers : geopandas.GeoDataFrame
+        Points of the consumer buildings (as returned by 'midpoint' method).
+    producers_poly : geopandas.GeoDataFrame
+        Polygons of the producer buildings. Point geometries are also allowed,
+        but they are not changed.
+    producers : geopandas.GeoDataFrame
+        Points of the producer buildings (as returned by 'midpoint' method).
+    lines_consumers : geopandas.GeoDataFrame
+        Connection lines from street to each consumer point.
+    lines_producers : geopandas.GeoDataFrame
+        Connection lines from street to each producer point.
+
+    Returns
+    -------
+    consumers : geopandas.GeoDataFrame
+        Updated points of the consumer buildings.
+    producers : geopandas.GeoDataFrame
+        Updated points of the producer buildings.
+    lines_consumers : geopandas.GeoDataFrame
+        Updated connection lines from street to each consumer point.
+    lines_producers : geopandas.GeoDataFrame
+        Updated connection lines from street to each producer point.
+
+    """
+    logging.info('Run "boundary" method for finding the building connections')
+    # Cut the part off of each "line_consumer" that is within the building
+    # polygon. As a result, the heating grid will only reach to the wall of
+    # the building.
+    lines_consumers_n = gpd.GeoDataFrame(
+        geometry=lines_consumers.difference(consumers_poly, align=False))
+    # This produces a MultiLineString for complex building polygons, where
+    # the boundary and the simple lines from centroid to street intersect
+    # multiple times. This would not be a valid connection line. In those
+    # cases the 'convex hull' of the building is used instead.
+    lines_consumers_n.loc[lines_consumers_n.type == "MultiLineString"] = \
+        gpd.GeoDataFrame(geometry=lines_consumers.difference(
+            consumers_poly.convex_hull, align=False))
+
+    # Repeat for the producer lines
+    lines_producers_n = gpd.GeoDataFrame(geometry=lines_producers.difference(
+        producers_poly, align=False))
+    lines_producers_n.loc[lines_producers_n.type == "MultiLineString"] = \
+        gpd.GeoDataFrame(geometry=lines_producers.difference(
+            producers_poly.convex_hull, align=False))
+
+    # Now the "consumers" (point objects for each building) need to be
+    # updated to touch the end of the consumer_lines
+    consumers_n = gpd.GeoDataFrame(geometry=lines_consumers.intersection(
+        consumers_poly.boundary, align=False))
+    consumers_n.loc[consumers_n.type == "MultiPoint"] = \
+        gpd.GeoDataFrame(geometry=lines_consumers.intersection(
+            consumers_poly.convex_hull.boundary, align=False))
+
+    # Repeat for the producers
+    producers_n = gpd.GeoDataFrame(geometry=lines_producers.intersection(
+        producers_poly.convex_hull.boundary, align=False))
+    producers_n.loc[producers_n.type == "MultiPoint"] = \
+        gpd.GeoDataFrame(geometry=lines_producers.intersection(
+            producers_poly.convex_hull.boundary, align=False))
+
+    # Sometimes the centroid does not lie within a building and there may be
+    # no intersetions, i.e. the new point is an 'empty' geometry. This can
+    # happen if buildings are multipolygons, which is not forbidden.
+    # Sometimes the new lines are empty (e.g. because a street and a building
+    # object cross each other).
+    # In these cases the original geometry is used for points and lines.
+    mask = (consumers_n.is_empty | lines_consumers_n.is_empty)
+    consumers_n.loc[mask] = consumers.loc[mask].geometry
+    lines_consumers_n.loc[mask] = lines_consumers.loc[mask].geometry
+
+    mask = (producers_n.is_empty | lines_producers_n.is_empty)
+    producers_n.loc[mask] = producers.loc[mask].geometry
+    lines_producers_n.loc[mask] = lines_producers.loc[mask].geometry
+
+    # Now update all the original variables with the new data
+    consumers.geometry = consumers_n.geometry
+    producers.geometry = producers_n.geometry
+    lines_consumers = lines_consumers_n
+    lines_producers = lines_producers_n
+
+    return consumers, producers, lines_consumers, lines_producers
+
+
+def check_duplicate_geometries(gdf):
+    """Test the input GeoDataFrame for duplicate geometries and plot them."""
+    if gdf.duplicated(subset="geometry").any():
+        idx = gdf.duplicated(subset="geometry")
+        try:
+            import matplotlib.pyplot as plt
+            fig, ax = plt.subplots(dpi=200)
+            gdf.loc[~idx].plot(ax=ax, color='green')
+            gdf.loc[idx].plot(ax=ax, color='red')
+            plt.title("Red are duplicate geometries. Please fix!")
+            plt.show()
+        except ImportError:
+            logging.info("Install matplotlib to show a plot of the duplicate "
+                         "geometries.")
+        raise ValueError("GeoDataFrame has {} duplicate geometries"
+                         .format(len(gdf.loc[idx])))
+
+
 def process_geometry(lines, consumers, producers,
                      method='midpoint', projected_crs=4647,
-                     tol_distance=2):
+                     tol_distance=2, reset_index=True):
     """
     This function connects the consumers and producers to the line network, and prepares the
     attributes of the geopandas.GeoDataFrames for importing as dhnx.ThermalNetwork.
 
     The ids of the lines are overwritten.
 
     Parameters
@@ -302,62 +462,92 @@
         Potential routes for the DHS. Expected geometry Linestrings or MultilineStrings.
         The graph of this line network should be connected.
     consumers : geopandas.GeoDataFrame
         Location of demand/consumers. Expected geometry: Polygons or Points.
     producers : geopandas.GeoDataFrame
         Location of supply sites. Expected geometry: Polygons or Points.
     method : str
-        Method for creating the point if polygons are given for the consumers and producers.
+        Method for creating the point if polygons are given for the consumers
+        and producers. Method 'midpoint' uses the centroid of each building
+        polygon. Method 'boundary' moves the point to the boundary (wall) of
+        the building, along the line constructed from centroid to the street.
     multi_connections : bool
         Setting if a building should be connected to multiple streets.
     projected_crs : EPSG integer code
         EPSG Coordinate reference system number (eg 4647),
         which is used for the geometry operations.
         A projected crs must be used!
     tol_distance : float
         Tolerance distance at connection the points to the line network
         for choosing the end of the line instead of the lot.
+    reset_index : bool
+        If True, reset the index and ignore the existing index. If False,
+        use the existing index for consumer and producer identificators.
+        Default: True
 
     Returns
     -------
     dict : Dictionary with 4 geopandas.GeoDataFrames: The keys of the Dict are
            equal to the components of the dhnx.ThermalNetwork: 'forks', 'consumers',
            'producers', 'pipes'.
 
     """
+    if method == 'boundary':
+        # copies of the original polygons are needed for method 'boundary'
+        consumers_poly = go.check_crs(consumers, crs=projected_crs).copy()
+        producers_poly = go.check_crs(producers, crs=projected_crs).copy()
 
     # check whether the expected geometry is used for geo dataframes
     check_geometry_type(lines, types=['LineString', 'MultiLineString'])
     for gdf in [producers, consumers]:
         check_geometry_type(gdf, types=['Polygon', 'Point', 'MultiPolygon'])
+        check_duplicate_geometries(gdf)
 
-    # # split multilinestrings to single lines with only 1 starting and 1 ending point
+    # split multilinestrings to single lines with only 1 starting and 1 ending point
     lines = go.split_multilinestr_to_linestr(lines)
 
     # check and convert crs if it is not already the `projected_crs`
     lines = go.check_crs(lines, crs=projected_crs)
 
     for layer in [producers, consumers]:
         layer = go.check_crs(layer, crs=projected_crs)
         layer = create_points_from_polygons(layer, method=method)
-        layer.reset_index(inplace=True, drop=True)
-        layer.index.name = 'id'
-        if 'id' in layer.columns:
-            layer.drop(['id'], axis=1, inplace=True)
+        if reset_index:
+            layer.reset_index(inplace=True, drop=True)
+            layer.index.name = 'id'
+            if 'id' in layer.columns:
+                layer.drop(['id'], axis=1, inplace=True)
+        else:
+            if layer.index.has_duplicates:
+                raise ValueError("The index of input data has duplicate "
+                                 "values, which is not allowed")
         layer['lat'] = layer['geometry'].apply(lambda x: x.y)
         layer['lon'] = layer['geometry'].apply(lambda x: x.x)
 
     producers['id_full'] = 'producers-' + producers.index.astype('str')
     producers['type'] = 'G'
     consumers['id_full'] = 'consumers-' + consumers.index.astype('str')
     consumers['type'] = 'H'
 
     # Add lines to consumers and producers
-    lines_consumers, lines = create_object_connections(consumers, lines, tol_distance=tol_distance)
-    lines_producers, lines = create_object_connections(producers, lines, tol_distance=tol_distance)
+    lines_consumers, lines = create_object_connections(
+        consumers, lines, tol_distance=tol_distance)
+    lines_producers, lines = create_object_connections(
+        producers, lines, tol_distance=tol_distance)
+    if not reset_index:
+        # Connection lines are ordered the same as points. Match their indexes
+        lines_consumers.index = consumers.index
+        lines_producers.index = producers.index
+
+    if method == 'boundary':
+        # Can only be performed after 'midpoint' method
+        consumers, producers, lines_consumers, lines_producers = (
+            run_point_method_boundary(
+                consumers_poly, consumers, producers_poly, producers,
+                lines_consumers, lines_producers))
 
     # Weld continuous line segments together and cut loose ends
     lines = go.weld_segments(
         lines, lines_producers, lines_consumers,
         # debug_plotting=True,
     )
 
@@ -368,17 +558,18 @@
 
     # generate forks point layer
     forks = go.create_forks(lines)
 
     # concat lines
     lines_all = pd.concat([lines, lines_consumers, lines_producers], sort=False)
     lines_all.reset_index(inplace=True, drop=True)
-    lines_all.index.name = 'id'
-    if 'id' in lines_all.columns:
-        lines_all.drop(['id'], axis=1, inplace=True)
+    if reset_index:
+        lines_all.index.name = 'id'
+        if 'id' in lines_all.columns:
+            lines_all.drop(['id'], axis=1, inplace=True)
 
     # concat point layer
     points_all = pd.concat([
         consumers[['id_full', 'geometry']],
         producers[['id_full', 'geometry']],
         forks[['id_full', 'geometry']]],
         sort=False
```

### Comparing `dhnx-0.0.2rc1/dhnx/gistools/geometry_operations.py` & `dhnx-0.0.3/dhnx/gistools/geometry_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,23 +17,29 @@
     import geopandas as gpd
 
 except ImportError:
     print("Need to install geopandas to process geometry data.")
 
 try:
     from shapely import wkt
-    from shapely.ops import cascaded_union, nearest_points, linemerge
-    from shapely.geometry import Point, LineString, MultiLineString
+    from shapely.geometry import LineString
+    from shapely.geometry import MultiLineString
+    from shapely.geometry import Point
+    from shapely.geometry import mapping
+    from shapely.ops import linemerge
+    from shapely.ops import nearest_points
+    from shapely.ops import unary_union
 except ImportError:
     print("Need to install shapely to process geometry.")
 
-import pandas as pd
-import matplotlib.pyplot as plt
 import logging
 
+import matplotlib.pyplot as plt
+import pandas as pd
+
 
 def create_forks(lines):
     """
     Creates a forks(nodes) GeoDataFrame from a "line"-GeoDataFrame
     based on the end-points of each LineString.
 
     Also, an index for every fork is given, and the columns 'full-id' (="forks-" + index"),
@@ -42,26 +48,25 @@
     Parameters
     ----------
     lines : geopandas.GeoDataFrame
 
     Returns
     -------
     geopandas.GeoDataFrame : GeoDataFrame with Points as geometry.
-    """
 
-    nodes = gpd.GeoDataFrame()
+    """
+    nodes = gpd.GeoDataFrame(geometry=[], crs=lines.crs)
 
     for _, j in lines.iterrows():
         geom = j['geometry']
-        p_0 = Point(geom.boundary[0])
-        p_1 = Point(geom.boundary[-1])
-        nodes = nodes.append({'geometry': p_0}, ignore_index=True)
-        nodes = nodes.append({'geometry': p_1}, ignore_index=True)
-
-    nodes.crs = lines.crs
+        p_0 = Point(geom.boundary.geoms[0])
+        p_1 = Point(geom.boundary.geoms[-1])
+        nodes = pd.concat(
+            [nodes, gpd.GeoDataFrame(geometry=[p_0, p_1], crs=lines.crs)],
+            ignore_index=True)
 
     # transform geometry into wkt
     nodes["geometry_wkt"] = nodes["geometry"].apply(lambda geom: geom.wkt)
 
     # drop duplicates of geometry column
     nodes = nodes.drop_duplicates(["geometry_wkt"])
 
@@ -94,16 +99,16 @@
     Returns
     -------
     geopandas.GeoDataFrame
     """
 
     # add id to gdf_lines for starting and ending node
     # point as wkt
-    lines['b0_wkt'] = lines["geometry"].apply(lambda geom: geom.boundary[0].wkt)
-    lines['b1_wkt'] = lines["geometry"].apply(lambda geom: geom.boundary[-1].wkt)
+    lines['b0_wkt'] = lines["geometry"].apply(lambda geom: geom.boundary.geoms[0].wkt)
+    lines['b1_wkt'] = lines["geometry"].apply(lambda geom: geom.boundary.geoms[-1].wkt)
 
     lines['from_node'] = lines['b0_wkt'].apply(lambda x: nodes.at[x, 'id_full'])
     lines['to_node'] = lines['b1_wkt'].apply(lambda x: nodes.at[x, 'id_full'])
 
     lines.drop(axis=1, inplace=True, labels=['b0_wkt', 'b1_wkt'])
 
     return lines
@@ -132,15 +137,15 @@
     l_ids = []
     count = 0
 
     for r, c in gdf.iterrows():
 
         point = c['geometry']
         gdf_other = gdf.drop([r])
-        other_points = cascaded_union(gdf_other['geometry'])
+        other_points = unary_union(gdf_other['geometry'])
 
         # x1 = nearest_points(point, other_points)[0]
         x2 = nearest_points(point, other_points)[1]
 
         if point.distance(x2) <= radius:
             l_ids.append(r)
 
@@ -196,30 +201,31 @@
     new_lines = gpd.GeoDataFrame()
 
     # first: split MultiLineString into LineStrings
     for i, b in gdf_lines.iterrows():
 
         geom = b['geometry']
 
-        if geom.type == 'MultiLineString':
+        if geom.geom_type == 'MultiLineString':
 
             multilinestrings = []
-            for line in geom:
-                multilinestrings.append(line)
+
+            for line in mapping(geom)["coordinates"]:
+                multilinestrings.append(LineString(line))
 
             for multiline in multilinestrings:
                 new_row = b.copy()
                 new_row['geometry'] = multiline
-                new_lines = new_lines.append(
-                    new_row, ignore_index=True, sort=False)
+                new_lines = pd.concat([new_lines, new_row.to_frame().T],
+                                      ignore_index=True, sort=False)
 
             gdf_lines.drop(index=i, inplace=True)
 
-    gdf_lines = gdf_lines.append(
-        new_lines, ignore_index=True, sort=False)
+    gdf_lines = pd.concat([gdf_lines, new_lines], ignore_index=True,
+                          sort=False)
 
     gdf_lines['geometry'].crs = gdf_input.crs
 
     # second: split LineStrings into single Linestrings
     new_lines = gpd.GeoDataFrame()
     for i, b in gdf_lines.iterrows():
 
@@ -229,21 +235,21 @@
 
             num_new_lines = len(geom.coords) - 1
 
             for num in range(num_new_lines):
                 new_row = b.copy()
                 new_row['geometry'] = \
                     LineString([geom.coords[num], geom.coords[num + 1]])
-                new_lines = new_lines.append(
-                    new_row, ignore_index=True, sort=False)
+                new_lines = pd.concat([new_lines, new_row.to_frame().T],
+                                      ignore_index=True, sort=False)
 
             gdf_lines.drop(index=i, inplace=True)
 
-    gdf_lines = gdf_lines.append(
-        new_lines, ignore_index=True, sort=False)
+    gdf_lines = pd.concat([gdf_lines, new_lines], ignore_index=True,
+                          sort=False)
 
     gdf_lines['geometry'].crs = gdf_input.crs
 
     return gdf_lines
 
 
 def weld_segments(gdf_line_net, gdf_line_gen, gdf_line_houses,
@@ -308,17 +314,18 @@
 
     Returns
     -------
     gdf_line_net_new : GeoDataFrame
         Simplified potential pipe network.
 
     """
-    gdf_line_net_new = gpd.GeoDataFrame(geometry=[], crs=gdf_line_net.crs)
-    gdf_merged_all = gpd.GeoDataFrame(geometry=[], crs=gdf_line_net.crs)
-    gdf_deleted = gpd.GeoDataFrame(geometry=[], crs=gdf_line_net.crs)
+    crs = gdf_line_net.crs
+    gdf_line_net_new = gpd.GeoDataFrame(geometry=[], crs=crs)
+    gdf_merged_all = gpd.GeoDataFrame(geometry=[], crs=crs)
+    gdf_deleted = gpd.GeoDataFrame(geometry=[], crs=crs)
     # Merge generator and houses line DataFrames to 'external' lines
     gdf_line_ext = pd.concat([gdf_line_gen, gdf_line_houses])
 
     for _, b in gdf_line_net.iterrows():
         def debug_plot(neighbours, color='red'):
             """Plot base map, current segment (with color) and neighbours."""
             if debug_plotting:
@@ -326,72 +333,76 @@
                 gdf_line_net.plot(ax=ax, color='blue')
                 gdf_line_ext.plot(ax=ax, color='green')
                 if len(neighbours) > 0:  # Prevent empty plot warning
                     neighbours.plot(ax=ax, color='orange')
                 gpd.GeoDataFrame(geometry=[geom]).plot(ax=ax, color=color)
 
         geom = b.geometry  # The current line segment
+        gdf_b = gpd.GeoDataFrame(b.to_frame().T, crs=crs)
 
         if any_check(geom, gdf_merged_all, how='within'):
             # Drop this object, because it is contained within a merged object
             continue  # Continue with the next line segment
 
         # Find all neighbours of the current segment
         mask_neighbours = [geom.touches(g) for g in gdf_line_net.geometry]
         neighbours = gdf_line_net[mask_neighbours]
         # If all of the neighbours intersect with each other, it is the
         # last segement before an intersection, which can be removed
         for neighbour in neighbours.geometry:
             if all([neighbour.intersects(g) for g in neighbours.geometry]):
                 # Treat as if there was only one neighbour (like end segment)
-                neighbours = gpd.GeoDataFrame(geometry=[neighbour])
+                neighbours = gpd.GeoDataFrame(geometry=[neighbour], crs=crs)
                 break
 
         if len(neighbours) <= 1:
             # This is a potentially unused end segment
             unused = True
 
-            # Test if one end touches a 'external' line, while the other
-            # end touches touches a network line segment
-            p1 = geom.boundary[0]
-            p2 = geom.boundary[-1]
+            # Test if one end touches an 'external' line, while the other
+            # end touches a network line segment
+            p1 = geom.boundary.geoms[0]
+            p2 = geom.boundary.geoms[-1]
             p1_neighbours = [p1.intersects(g) for g in neighbours.geometry]
             p2_neighbours = [p2.intersects(g) for g in neighbours.geometry]
-            if any_check(p1, gdf_line_ext, how='touches') and p2_neighbours.count(True) > 0:
+            if (any_check(p1, gdf_line_ext, how='touches')
+               and p2_neighbours.count(True) > 0):
                 unused = False
-            elif any_check(p2, gdf_line_ext, how='touches') and p1_neighbours.count(True) > 0:
+            elif (any_check(p2, gdf_line_ext, how='touches')
+                  and p1_neighbours.count(True) > 0):
                 unused = False
 
             if unused:
                 # If truly unused, we can discard it to simplify the network
                 debug_plot(neighbours, color='white')
-                gdf_deleted = gdf_deleted.append(b, ignore_index=True)
+                gdf_deleted = pd.concat([gdf_deleted, gdf_b],
+                                        ignore_index=True)
             else:
                 # Keep it, if it touches a generator or a house
                 debug_plot(neighbours, color='black')
-                gdf_line_net_new = gdf_line_net_new.append(
-                    b, ignore_index=True)
+                gdf_line_net_new = pd.concat([gdf_line_net_new, gdf_b],
+                                             ignore_index=True)
             continue  # Continue with the next line segment
 
         if len(neighbours) > 2:
             # This segment has more than two neighbours. This means it is
             # part of an intersection, which we do not simplify futher.
             # However, we can check if either endpoint of the current segment
             # only has one neighbour. Then that one can still be merged.
-            p1 = geom.boundary[0]
-            p2 = geom.boundary[-1]
+            p1 = geom.boundary.geoms[0]
+            p2 = geom.boundary.geoms[-1]
             p1_neighbours = [p1.intersects(g) for g in neighbours.geometry]
             p2_neighbours = [p2.intersects(g) for g in neighbours.geometry]
             if p1_neighbours.count(True) == 1:  # Only one neighbour allowed
                 neighbours = neighbours[p1_neighbours]  # Neighbour to merge
             elif p2_neighbours.count(True) == 1:  # Only one neighbour allowed
                 neighbours = neighbours[p2_neighbours]  # Neighbour to merge
             else:  # Keep this segment. Multiple lines meet at an intersection
-                gdf_line_net_new = gdf_line_net_new.append(b,
-                                                           ignore_index=True)
+                gdf_line_net_new = pd.concat([gdf_line_net_new, gdf_b],
+                                             ignore_index=True)
                 debug_plot(neighbours, color='green')
                 continue  # Continue with the next line segment
 
         if len(neighbours) == 2:
             # There are excactly two separate neighbours that can be merged
             pass  # Run the rest of the loop
 
@@ -411,19 +422,20 @@
                 else:  # No not merge neighbour intersecting with external
                     continue
             elif any_check(neighbour, neighbours, how='touches'):
                 neighbours_list = []  # The two neighbours touch
                 break  # This is a intersection that cannot be simplified
             else:  # Choose neighbour for merging
                 neighbours_list.append(neighbour)
-        neighbours = gpd.GeoDataFrame(geometry=neighbours_list)
+        neighbours = gpd.GeoDataFrame(geometry=neighbours_list, crs=crs)
 
         if len(neighbours) == 0:
             # If no neighbours are left now, continue with next line segment
-            gdf_line_net_new = gdf_line_net_new.append(b, ignore_index=True)
+            gdf_line_net_new = pd.concat([gdf_line_net_new, gdf_b],
+                                         ignore_index=True)
             continue
 
         # Create list of all elements that should be merged
         lines = [geom] + list(neighbours.geometry)
         try:  # Works when all elements are LineStrings
             # Combine lines into a multi-linestring
             multi_line = MultiLineString(lines)
@@ -435,20 +447,21 @@
                 else:  # Linestring
                     lines_.append(line)
             # Now combine all of those into MultiLineString
             multi_line = MultiLineString(lines_)
 
         # Merge the MultiLineString into a single object
         merged_line = linemerge(multi_line)
-        gdf_merged = gpd.GeoDataFrame(geometry=[merged_line])
+        gdf_merged = gpd.GeoDataFrame(geometry=[merged_line], crs=crs)
         debug_plot(neighbours)  # Plot the segments before the merge
         debug_plot(gdf_merged, color='orange')  # ...and after the merge
-        gdf_line_net_new = gdf_line_net_new.append(gdf_merged,
-                                                   ignore_index=True)
-        gdf_merged_all = gdf_merged_all.append(gdf_merged, ignore_index=True)
+        gdf_line_net_new = pd.concat([gdf_line_net_new, gdf_merged],
+                                     ignore_index=True)
+        gdf_merged_all = pd.concat([gdf_merged_all, gdf_merged],
+                                   ignore_index=True)
 
     return gdf_line_net_new
 
 
 def any_check(geom_test, gdf, how):
     """Improve speed for an 'any()' test on a list comprehension.
```

### Comparing `dhnx-0.0.2rc1/dhnx/graph.py` & `dhnx-0.0.3/dhnx/graph.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 This file is part of project dhnx (). It's copyrighted
 by the contributors recorded in the version control history of the file,
 available from its original location:
 
 SPDX-License-Identifier: MIT
 """
 
-import pandas as pd
 import networkx as nx
+import pandas as pd
 
 
 def thermal_network_to_nx_graph(thermal_network):
     r"""
 
     Parameters
     ----------
@@ -105,12 +105,12 @@
     if var_name:
         pass
     elif series.name:
         var_name = series.name
     else:
         raise ValueError(r"Have to either pass Series with name or provide var_name.")
 
-    for index, value in series.iteritems():
+    for index, value in series.items():
 
         graph.edges[index][var_name] = value
 
     return graph
```

### Comparing `dhnx-0.0.2rc1/dhnx/input_output.py` & `dhnx-0.0.3/dhnx/input_output.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,22 +9,22 @@
 
 SPDX-License-Identifier: MIT
 """
 
 import logging
 import os
 
-from addict import Dict
-import pandas as pd
 import networkx as nx
 import numpy as np
+import pandas as pd
+from addict import Dict
 
 try:
-    from shapely.geometry import Point
     from shapely.geometry import LineString
+    from shapely.geometry import Point
 
 except ImportError:
     print("Need to install shapely to download from osm.")
 
 try:
     import geopandas as gpd
 
@@ -35,15 +35,14 @@
     import osmnx as ox
 
 except ImportError:
     print("Need to install osmnx to download from osm.")
 
 from dhnx.dhn_from_osm import connect_points_to_network
 
-
 logger = logging.getLogger()
 
 
 class NetworkImporter():
     r"""
     Generic Importer object for network.ThermalNetwork
     """
```

### Comparing `dhnx-0.0.2rc1/dhnx/model.py` & `dhnx-0.0.3/dhnx/model.py`

 * *Files identical despite different names*

### Comparing `dhnx-0.0.2rc1/dhnx/network.py` & `dhnx-0.0.3/dhnx/network.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,18 +12,21 @@
 """
 
 import os
 
 import pandas as pd
 
 from .graph import thermal_network_to_nx_graph
-from .optimization import optimize_operation, setup_optimise_investment, \
-    solve_optimisation_investment
 from .helpers import Dict
-from .input_output import CSVNetworkImporter, CSVNetworkExporter, load_component_attrs
+from .input_output import CSVNetworkExporter
+from .input_output import CSVNetworkImporter
+from .input_output import load_component_attrs
+from .optimization.optimization_models import optimize_operation
+from .optimization.optimization_models import setup_optimise_investment
+from .optimization.optimization_models import solve_optimisation_investment
 from .simulation import simulate
 
 dir_name = os.path.dirname(__file__)
 
 available_components = pd.read_csv(os.path.join(dir_name, 'components.csv'), index_col=0)
 
 component_attrs = load_component_attrs(os.path.join(dir_name, 'component_attrs'),
@@ -55,15 +58,15 @@
     sequences
     results
     graph
 
     Examples
     --------
     >>> from dhnx.network import ThermalNetwork
-    >>> tnw = ThermalNetwork('csv_folder')
+    >>> tnw = ThermalNetwork()
     >>> tnw.is_consistent()
     True
     """
     def __init__(self, dirname=None):
 
         self.available_components = available_components
         self.component_attrs = component_attrs
```

### Comparing `dhnx-0.0.2rc1/dhnx/optimization.py` & `dhnx-0.0.3/dhnx/optimization/optimization_models.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,23 +7,26 @@
 This file is part of project dhnx (). It's copyrighted
 by the contributors recorded in the version control history of the file,
 available from its original location:
 
 SPDX-License-Identifier: MIT
 """
 
-import os
 import logging
+import os
+
 import networkx as nx
-import pandas as pd
 import oemof.solph as solph
+import pandas as pd
 from oemof.solph import helpers
 
-from .optimization_dhs_nodes import add_nodes_dhs, add_nodes_houses
-from .model import OperationOptimizationModel, InvestOptimizationModel
+from dhnx.model import InvestOptimizationModel
+from dhnx.model import OperationOptimizationModel
+from dhnx.optimization.dhs_nodes import add_nodes_dhs
+from dhnx.optimization.dhs_nodes import add_nodes_houses
 
 
 class OemofOperationOptimizationModel(OperationOptimizationModel):
     r"""
     Implementation of an operation optimization model using oemof-solph.
     """
     def __init__(self, thermal_network):
@@ -137,54 +140,55 @@
 
         # Check 2
 
         ids_consumers = self.thermal_network.components['consumers'].index
 
         for p, q in self.thermal_network.components['pipes'].iterrows():
 
-            if (q['from_node'].split('-')[0] == "consumers") and (
-                    q['to_node'].split('-')[0] == "consumers"):
+            if (q['from_node'].split('-', 1)[0] == "consumers") and (
+                    q['to_node'].split('-', 1)[0] == "consumers"):
 
                 raise ValueError(
                     ""
                     "Pipe id {} goes from consumer to consumer. This is not "
                     "allowed!".format(p))
 
-            if (q['from_node'].split('-')[0] == "producers") and (
-                    q['to_node'].split('-')[0] == "producers"):
+            if (q['from_node'].split('-', 1)[0] == "producers") and (
+                    q['to_node'].split('-', 1)[0] == "producers"):
 
                 raise ValueError(
                     ""
                     "Pipe id {} goes from producers to producers. "
                     "This is not allowed!".format(p))
 
-            if ((q['from_node'].split('-')[0] == "producers") and (
-                    q['to_node'].split('-')[0] == "consumers")) or ((
-                        q['from_node'].split('-')[0] == "consumers") and (
-                            q['to_node'].split('-')[0] == "producers")):
+            if ((q['from_node'].split('-', 1)[0] == "producers") and (
+                    q['to_node'].split('-', 1)[0] == "consumers")) or ((
+                        q['from_node'].split('-', 1)[0] == "consumers") and (
+                            q['to_node'].split('-', 1)[0] == "producers")):
 
                 raise ValueError(
                     ""
                     "Pipe id {} goes from producers directly "
                     "to consumers, or vice versa. This is not allowed!"
                     "".format(p))
 
-            if (q['from_node'].split('-')[0] == "forks") and (
-                    q['to_node'].split('-')[0] == "consumers"):
+            if (q['from_node'].split('-', 1)[0] == "forks") and (
+                    q['to_node'].split('-', 1)[0] == "consumers"):
 
-                cons_id = q['to_node'].split('-')[1]
+                cons_id = q['to_node'].split('-', 1)[1]
 
                 if cons_id not in ids_consumers:
                     raise ValueError(
                         ""
-                        "The consumer of pipe id {} does not exist!".format(p))
+                        "The consumer {} of pipe id {} does not exist!"
+                        .format(cons_id, p))
 
         pipe_to_cons_ids = list(self.thermal_network.components['pipes']['to_node'].values)
-        pipe_to_cons_ids = [x.split('-')[1] for x in pipe_to_cons_ids
-                            if x.split('-')[0] == 'consumers']
+        pipe_to_cons_ids = [x.split('-', 1)[1] for x in pipe_to_cons_ids
+                            if x.split('-', 1)[0] == 'consumers']
 
         for id in list(self.thermal_network.components['consumers'].index):
             if id not in pipe_to_cons_ids:
                 raise ValueError(
                     "The consumer id {} has no connection the the grid!".format(id))
 
         # Check 3
@@ -335,15 +339,18 @@
 
         date_time_index = pd.date_range(self.settings['start_date'],
                                         periods=self.settings['num_ts'],
                                         freq=self.settings['frequence'])
 
         logging.info('Initialize the energy system')
 
-        self.es = solph.EnergySystem(timeindex=date_time_index)
+        self.es = solph.EnergySystem(
+            timeindex=date_time_index,
+            infer_last_interval=True,
+        )
 
         logging.info('Create oemof objects')
 
         # add houses and generation
         for typ in ['consumers', 'producers']:
             self.nodes, self.buses = add_nodes_houses(
                 self, self.nodes, self.buses, typ)
@@ -552,41 +559,65 @@
                 if isinstance(hp_type, str):
                     raise ValueError(
                         "Pipe id {} already has an investment > 0!".format(edge_id))
 
             df['hp_type'] = None
             df['capacity'] = float(0)
             df['direction'] = 0
+            df['status'] = float(0)
 
             for ahp in active_hp:
                 # p = df_hp[df_hp['label_3'] == ahp].squeeze()   # series of heatpipe
                 for r, c in df.iterrows():
                     if c[ahp + '.size'] > 0:
                         check_invest_label(c['hp_type'], id)
                         df.at[r, 'hp_type'] = ahp
                         df.at[r, 'capacity'] = c[ahp + '.size']
                         df.at[r, 'direction'] = c[ahp + '.direction']
+                        if ahp + '.status' in c.index:
+                            df.at[r, 'status'] = c[ahp + '.status']
 
         def recalc_costs_losses():
+            """
+            Calculates the investment costs and thermal losses for each
+            pipeline of the district heating network.
+            (This recalculation could also serve as check for comparing the
+            total pipeline costs with the objective value of oemof.solph
+            optimisation model)
+
+            Note
+            ----
+            With nonconvex investments (with binary variables) it could happen
+            that very low results of the decision variable occur (although
+            there is a minimum investment threshold), and that
+            the status variable could have values of almost 0 and almost 1.
+            This cost re-calculation does not round any of this results, and
+            transfers the results as they into a DataFrame containing all
+            pipes of the district heating network.
+
+            """
 
             df['costs'] = float(0)
             df['losses'] = float(0)
 
             for r, c in df.iterrows():
                 if c['capacity'] > 0:
                     hp_lab = c['hp_type']
                     # select row from heatpipe type table
                     hp_p = df_hp[df_hp['label_3'] == hp_lab].squeeze()
                     if hp_p['nonconvex'] == 1:
                         df.at[r, 'costs'] = c['length'] * (
-                            c['capacity'] * hp_p['capex_pipes'] + hp_p['fix_costs']
+                            c['capacity'] * hp_p['capex_pipes'] +  # noqa: W504
+                            hp_p['fix_costs'] * c['status']
                         )
                         df.at[r, 'losses'] = c['length'] * (
-                            c['capacity'] * hp_p['l_factor'] + hp_p['l_factor_fix']
+                            c['capacity'] * hp_p['l_factor'] +  # noqa: W504
+                            hp_p['l_factor_fix'] * c['status']
                         )
+
                     elif hp_p['nonconvex'] == 0:
                         df.at[r, 'costs'] = c['length'] * c['capacity'] * hp_p['capex_pipes']
                         # Note, that a constant loss is possible also for convex
                         df.at[r, 'losses'] = c['length'] * (
                             c['capacity'] * hp_p['l_factor'] + hp_p['l_factor_fix']
                         )
```

### Comparing `dhnx-0.0.2rc1/dhnx/optimization_add_components.py` & `dhnx-0.0.3/dhnx/optimization/add_components.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,36 +7,38 @@
 This file is part of project dhnx (). It's copyrighted
 by the contributors recorded in the version control history of the file,
 available from its original location:
 
 SPDX-License-Identifier: MIT
 """
 
-
 import oemof.solph as solph
-import dhnx.optimization_oemof_heatpipe as oh
+from oemof.network import Transformer
+
+import dhnx.optimization.oemof_heatpipe as oh
 
 
 def add_buses(it, labels, nodes, busd):
     """
-    This function initialises the oemof.solph.Bus classes of the energysystem based on the given
-    tabular information. Additionally, a sink or a source can be added to every bus and costs for
-    this source (shortage) or sink (excess) can be defined.
+    This function initialises the oemof.solph.Bus classes of the energysystem
+    based on the given tabular information. Additionally, a sink or a source
+    can be added to every bus and costs for this source (shortage) or sink
+    (excess) can be defined.
 
     The table must be given as follows:
 
     .. _bus_table:
 
     .. table:: Example for table of *Buses*
 
-        +---------+--------+--------+----------+----------------+--------------+
-        | label_2 | active | excess | shortage | shortage costs | excess costs |
-        +=========+========+========+==========+================+==============+
-        | heat    | 1      | 0      | 0        | 99999          | 99999        |
-        +---------+--------+--------+----------+----------------+--------------+
+        +---------+--------+--------+----------+----------------+-------------+
+        | label_2 | active | excess | shortage | shortage costs | excess costs|
+        +=========+========+========+==========+================+=============+
+        | heat    | 1      | 0      | 0        | 99999          | 99999       |
+        +---------+--------+--------+----------+----------------+-------------+
 
     Parameters
     ----------
     it : pd.DateFrame
         Table of attributes for Buses for the producers and consumers.
     labels : dict
         Dictonary containing tag1 and tag4 of label-tuple.
@@ -50,49 +52,52 @@
     list, dict : Updated list of nodes and dict of Buses.
     """
 
     for _, b in it.iterrows():
 
         labels['l_3'] = 'bus'
         labels['l_2'] = b['label_2']
-        l_bus = oh.Label(labels['l_1'], labels['l_2'], labels['l_3'], labels['l_4'])
+        l_bus = oh.Label(labels['l_1'], labels['l_2'], labels['l_3'],
+                         labels['l_4'])
 
         # check if bus already exists (due to infrastructure)
         if l_bus in busd:
             print('Bus bereits vorhanden:', l_bus)
 
         else:
             bus = solph.Bus(label=l_bus)
             nodes.append(bus)
 
             busd[l_bus] = bus
 
             if b['excess']:
                 labels['l_3'] = 'excess'
                 nodes.append(
-                    solph.Sink(label=oh.Label(
+                    solph.components.Sink(label=oh.Label(
                         labels['l_1'], labels['l_2'], labels['l_3'], labels['l_4']),
                         inputs={busd[l_bus]: solph.Flow(variable_costs=b['excess costs'])}))
 
             if b['shortage']:
                 labels['l_3'] = 'shortage'
                 nodes.append(
-                    solph.Source(label=oh.Label(
+                    solph.components.Source(label=oh.Label(
                         labels['l_1'], labels['l_2'], labels['l_3'], labels['l_4']),
                         outputs={busd[l_bus]: solph.Flow(variable_costs=b['shortage costs'])}))
 
     return nodes, busd
 
 
 def add_sources(on, it, c, labels, nodes, busd):
     """
-    The oemof.solph.Source components for the producers and consumers are initialised based on the
-    given tabular information of the investment_options of the OemofInvestOptimizationModel.
-    Time-series can also be used as attribute values for the outflow of the Source.
-    Therefore, a table with the filename 'source_timeseries' must be given.
+    The oemof.solph.Source components for the producers and consumers are
+    initialised based on the given tabular information of the
+    investment_options of the OemofInvestOptimizationModel.
+    Time-series can also be used as attribute values for the outflow of the
+    Source. Therefore, a table with the filename 'source_timeseries' must be
+    given.
 
     Parameters
     ----------
     on : OemofInvestOptimizationModel
     it : DataFrame
         Table of attributes for Sources for the producers and consumers.
     c : Series
@@ -130,39 +135,46 @@
         # general additional flow attributes
         for fa in flow_attr:
             outflow_args[fa] = cs[fa]
 
         # specific flow attributes
         # e.g. check for heat (label 2)
         # e.g. check for source (label 3)
-        spec_attr = [x for x in list(on.thermal_network.components[labels['l_1']].columns)
-                     if x.split('.')[-1] in on.oemof_flow_attr
-                     if x.split('.')[0] == labels['l_2']
-                     if x.split('.')[1] == labels['l_3']]
+        spec_attr = [
+            x for x in list(
+                on.thermal_network.components[labels['l_1']].columns)
+            if x.split('.')[-1] in on.oemof_flow_attr
+            if x.split('.')[0] == labels['l_2']
+            if x.split('.')[1] == labels['l_3']
+        ]
 
         for sa in spec_attr:
             if sa.split('.')[-1] in outflow_args.keys():
                 print(
-                    'General attribute <{}> of Label 2 <{}> and Label 3 <{}> (value: {}) will '
-                    'be replaced by specific data. New value for <{}>: {}'.format(
+                    'General attribute <{}> of Label 2 <{}> and '
+                    'Label 3 <{}> (value: {}) will '
+                    'be replaced by specific data. New value for <{}>: {}'
+                    ''.format(
                         sa.split('.')[-1], labels['l_2'], labels['l_3'],
                         outflow_args[sa.split('.')[-1]], labels['l_4'], c[sa]))
             outflow_args[sa.split('.')[-1]] = c[sa]
 
         # add timeseries data if present
         if ts_status:
-            ts_key = labels['l_4'].split('-')[1] + '_' + labels['l_2']
+            ts_key = labels['l_4'].split('-', 1)[1] + '_' + labels['l_2']
             for col in ts.columns.values:
                 if col.split('.')[0] == ts_key:
                     outflow_args[col.split('.')[1]] = ts[col].values
 
         nodes.append(
-            solph.Source(
+            solph.components.Source(
                 label=oh.Label(
-                    labels['l_1'], labels['l_2'], labels['l_3'], labels['l_4']),
+                    labels['l_1'], labels['l_2'], labels['l_3'],
+                    labels['l_4']
+                ),
                 outputs={
                     busd[(labels['l_1'], cs['label_2'], 'bus',
                           labels['l_4'])]: solph.Flow(**outflow_args)}))
 
     return nodes
 
 
@@ -190,31 +202,31 @@
 
     for _, de in it.iterrows():
         labels['l_3'] = 'demand'
         labels['l_2'] = de['label_2']
         # set static inflow values
         inflow_args = {'nominal_value': de['nominal_value'],
                        'fix': series['heat_flow'][
-                           labels['l_4'].split('-')[1]].values}
+                           labels['l_4'].split('-', 1)[1]].values}
 
         # create
         nodes.append(
-            solph.Sink(label=oh.Label(
+            solph.components.Sink(label=oh.Label(
                 labels['l_1'], labels['l_2'], labels['l_3'], labels['l_4']),
                 inputs={busd[(labels['l_1'], labels['l_2'], 'bus',
                               labels['l_4'])]: solph.Flow(**inflow_args)}))
 
     return nodes
 
 
 def add_transformer(it, labels, nodes, busd):
-    """Adds oemof.solph.Transformer objects to the list of components.
+    """Adds oemof.network.Transformer objects to the list of components.
 
-    If attribute `invest` is *True*, an `Investment` attribute is added to the outflow of the
-    Transformer.
+    If attribute `invest` is *True*, an `Investment` attribute is added to
+    the outflow of the Transformer.
 
     Parameters
     ----------
     it : pd.DataFrame
         Table of transformer attributes of the producers / consumers.
     labels : dict
         Dictonary containing specifications for label-tuple.
@@ -244,17 +256,18 @@
                 if t['eff_out_1'] == 'series':
                     print('noch nicht angepasst!')
 
                 epc_t = t['capex']
 
                 # create
                 nodes.append(
-                    solph.Transformer(
+                    Transformer(
                         label=oh.Label(
-                            labels['l_1'], labels['l_2'], labels['l_3'], labels['l_4']),
+                            labels['l_1'], labels['l_2'], labels['l_3'],
+                            labels['l_4']),
                         inputs={b_in_1: solph.Flow()},
                         outputs={b_out_1: solph.Flow(
                             variable_costs=t['variable_costs'],
                             summed_max=t['in_1_sum_max'],
                             investment=solph.Investment(
                                 ep_costs=epc_t + t['service'],
                                 maximum=t['max_invest'],
@@ -268,31 +281,32 @@
                     print('noch nicht angepasst!')
                     # for col in nd['timeseries'].columns.values:
                     #     if col.split('.')[0] == t['label']:
                     #         t[col.split('.')[1]] = nd['timeseries'][
                     #             col]
 
                 nodes.append(
-                    solph.Transformer(
+                    Transformer(
                         label=oh.Label(labels['l_1'], labels['l_2'], labels['l_3'],
                                        labels['l_4']),
                         inputs={b_in_1: solph.Flow()},
                         outputs={b_out_1: solph.Flow(
                             nominal_value=t['installed'],
                             summed_max=t['in_1_sum_max'],
                             variable_costs=t['variable_costs'])},
                         conversion_factors={b_out_1: t['eff_out_1']}))
 
     return nodes
 
 
 def add_storage(it, labels, nodes, busd):
-    """Adds oemof.solph.GenericStorage objects to the list of components.
+    """Adds oemof.solph.components.GenericStorage objects to the list of components.
 
-    If attribute `invest` is *True*, the investment version of the Storage is created.
+    If attribute `invest` is *True*, the investment version of the Storage is
+    created.
 
     Parameters
     ----------
     it : pd.DataFrame
         Table of storage attributes of the producers / consumers.
     labels : dict
         Dictonary containing specifications for label-tuple.
@@ -304,15 +318,18 @@
     Returns
     -------
     list : Updated list of nodes.
     """
 
     for _, s in it.iterrows():
 
-        label_storage = oh.Label(labels['l_1'], s['bus'], s['label'], labels['l_4'])
+        label_storage = oh.Label(
+            labels['l_1'], s['bus'], s['label'], labels['l_4']
+        )
+
         label_bus = busd[(labels['l_1'], s['bus'], 'bus', labels['l_4'])]
 
         if s['invest']:
 
             epc_s = s['capex']
 
             nodes.append(
@@ -345,15 +362,16 @@
                         'outflow_conversion_factor']))
 
     return nodes
 
 
 def add_heatpipes(it, labels, bidirectional, length, b_in, b_out, nodes):
     """
-    Adds *HeatPipeline* objects with *Investment* attribute to the list of oemof.solph components.
+    Adds *HeatPipeline* objects with *Investment* attribute to the list of
+    oemof.solph components.
 
     Parameters
     ----------
     it : pd.DataFrame
         Table of *Heatpipeline* attributes of the district heating grid
     labels : dict
         Dictonary containing specifications for label-tuple
@@ -388,15 +406,18 @@
         flow_bi_args = {
             'bidirectional': True, 'min': -1}\
             if bidirectional else {}
 
         nodes.append(oh.HeatPipeline(
             label=oh.Label(labels['l_1'], labels['l_2'],
                            labels['l_3'], labels['l_4']),
-            inputs={b_in: solph.Flow(**flow_bi_args)},
+            inputs={b_in: solph.Flow(
+                investment=solph.Investment(),
+                **flow_bi_args,
+            )},
             outputs={b_out: solph.Flow(
                 nominal_value=None,
                 **flow_bi_args,
                 investment=solph.Investment(
                     ep_costs=epc_p, maximum=t['cap_max'],
                     minimum=t['cap_min'], nonconvex=nc, offset=epc_fix,
                 ))},
@@ -447,15 +468,18 @@
         if gd['bidirectional_pipes'] else {}
 
     outflow_args = {'nonconvex': solph.NonConvex()} if t['nonconvex'] else {}
 
     nodes.append(oh.HeatPipeline(
         label=oh.Label(labels['l_1'], labels['l_2'],
                        labels['l_3'], labels['l_4']),
-        inputs={b_in: solph.Flow(**flow_bi_args)},
+        inputs={b_in: solph.Flow(
+            nominal_value=q['capacity'],
+            **flow_bi_args,
+        )},
         outputs={b_out: solph.Flow(
             nominal_value=q['capacity'],
             **flow_bi_args,
             **outflow_args,
         )},
         heat_loss_factor=hlf,
         heat_loss_factor_fix=hlff,
```

### Comparing `dhnx-0.0.2rc1/dhnx/optimization_dhs_nodes.py` & `dhnx-0.0.3/dhnx/optimization/dhs_nodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,16 +9,17 @@
 available from its original location:
 
 SPDX-License-Identifier: MIT
 """
 
 
 import oemof.solph as solph
-import dhnx.optimization_oemof_heatpipe as oh
-import dhnx.optimization_add_components as ac
+
+import dhnx.optimization.add_components as ac
+import dhnx.optimization.oemof_heatpipe as oh
 
 
 def add_nodes_dhs(opti_network, gd, nodes, busd):
     """
     Based on the *forks* and *pipes* of the *ThermalNetwork* of the
     *OemofInvestOptimisationModel*, the oemof-solph components for the district heating
     network optimisation are initialised.
```

### Comparing `dhnx-0.0.2rc1/dhnx/optimization_oemof_heatpipe.py` & `dhnx-0.0.3/dhnx/optimization/oemof_heatpipe.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,20 +10,22 @@
 
 SPDX-License-Identifier: MIT
 """
 # pylint: skip-file
 import warnings
 from collections import namedtuple
 
-from pyomo.core.base.block import SimpleBlock
-from pyomo.environ import (Set, NonNegativeReals, Var, Constraint)
-
-from oemof.solph.network import Transformer
-from oemof.solph.plumbing import sequence
+from oemof.network import Transformer
 from oemof.solph import Investment
+from oemof.solph._plumbing import sequence
+from pyomo.core.base.block import ScalarBlock
+from pyomo.environ import Constraint
+from pyomo.environ import NonNegativeReals
+from pyomo.environ import Set
+from pyomo.environ import Var
 
 
 class Label(namedtuple('solph_label', ['tag1', 'tag2', 'tag3', 'tag4'])):
     __slots__ = ()
 
     def __str__(self):
         """The string is used within solph as an ID, so it hast to be unique"""
@@ -41,30 +43,30 @@
     ----------
     length : float
         Length of HeatPipeline.
     heat_loss_factor : float
         Heat loss per length unit as fraction of the nominal power. Can also be
         defined by a series.
 
-    See also :py:class:`~oemof.solph.network.Transformer`.
 
     Note
     ----
-    This component is experimental. Use it with care.
+    This component is experimental. Use it with care. See also
+    :py:class:`~oemof.solph.network.Transformer`.
 
 
     The following sets, variables, constraints and objective parts are created
-     * :py:class:`~oemof.solph.custom.HeatPipelineBlock` (if no
-       Investment object present)
-     * :py:class:`~oemof.solph.custom.HeatPipelineInvestBlock` (if
+     * :py:class:`~dhnx.optimization.oemof_heatpipe.HeatPipelineBlock` (if no
        Investment object present)
+     * :py:class:`~dhnx.optimization.oemof_heatpipe.HeatPipelineInvestBlock`
+      (ifInvestment object present)
 
     Examples
     --------
-    example
+    # TODO : example
 
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         self.heat_loss_factor = sequence(kwargs.get('heat_loss_factor', 0))
@@ -111,29 +113,30 @@
                     "'heat_loss_factor_fix' is considered, even though the "
                     "investment might be zero! => A simple sink could be "
                     "the results. Hopefully, you know what you are doing.")
         else:
             self._set_nominal_value()
 
     def _check_flows_invest(self):
-        for flow in self.inputs.values():
-            if isinstance(flow.investment, Investment):
-                raise ValueError(
-                    "The investment must be defined at the Outputflow!")
+        # for flow in self.inputs.values():
+        #     if isinstance(flow.investment, Investment):
+        #         raise ValueError(
+        #             "The investment must be defined at the Outputflow!")
 
         for flow in self.outputs.values():
             if isinstance(flow.investment, Investment):
                 self._invest_group = True
 
     def _set_flows(self):
         # sets the input flow to investment
         for flow in self.inputs.values():
             flow.investment = Investment()
 
-    # set nominal values of in- and outflow equal in case of invest_group = False
+    # set nominal values of in- and outflow equal in case of
+    # invest_group = False
     def _set_nominal_value(self):
         i = list(self.inputs.keys())[0]
         o = list(self.outputs.keys())[0]
         if self.outputs[o].nominal_value is not None:
             self.inputs[i].nominal_value = \
                 self.outputs[o].nominal_value
         elif self.inputs[i].nominal_value is not None:
@@ -142,29 +145,28 @@
 
     def constraint_group(self):
         if self._invest_group is True:
             return HeatPipelineInvestBlock
         return HeatPipelineBlock
 
 
-class HeatPipelineBlock(SimpleBlock):  # pylint: disable=too-many-ancestors
+class HeatPipelineBlock(ScalarBlock):  # pylint: disable=too-many-ancestors
     r"""Block representing a pipeline of a district heating system.
-    :class:`~oemof.solph.custom.HeatPipeline`
+    :class:`~dhnx.optimization.oemof_heatpipe.HeatPipeline`
 
     **The following constraints are created:**
 
+    # TODO : Check and fix equations!
+
     .. _HeatPipelineBlock-equations:
 
-    .. math::
-        &
-        (1) \dot{Q}_{out}(t) = \dot{Q}_{in}(t) \cdot
-        \frac{\eta_{out}}{\eta_{in}} - \dot{Q}_{loss}(t)\\
-        &
-        (2) \dot{Q}_{loss}(t) = f_{loss}(t) \cdot l \cdot \dot{Q}_{nominal}
-        &
+    .. math:: \dot{Q}_{out}(t) = \dot{Q}_{in}(t) \cdot
+        \frac{\eta_{out}}{\eta_{in}} - \dot{Q}_{loss}(t)
+
+    .. math:: \dot{Q}_{loss}(t) = f_{loss}(t) \cdot l \cdot \dot{Q}_{nominal}
 
     The symbols used are defined as follows
     (with Variables (V) and Parameters (P)):
 
     .. csv-table::
         :header: "symbol", "attribute", "type", "explanation"
         :widths: 1, 1, 1, 1
@@ -203,18 +205,23 @@
         """
         if group is None:
             return None
 
         m = self.parent_block()
 
         self.HEATPIPES = Set(initialize=list(group))
-        self.CONVEX_HEATPIPES = Set(initialize=[
-            n for n in group if n.outputs[list(n.outputs.keys())[0]].nonconvex is None])
-        self.NONCONVEX_HEATPIPES = Set(initialize=[
-            n for n in group if n.outputs[list(n.outputs.keys())[0]].nonconvex is not None])
+        self.CONVEX_HEATPIPES = Set(
+            initialize=[n for n in group
+                        if n.outputs[list(n.outputs.keys())[0]].nonconvex
+                        is None]
+        )
+        self.NONCONVEX_HEATPIPES = Set(
+            initialize=[n for n in group
+                        if n.outputs[list(n.outputs.keys())[0]].nonconvex
+                        is not None])
 
         # Defining Variables
         self.heat_loss = Var(self.HEATPIPES, m.TIMESTEPS,
                              within=NonNegativeReals)
 
         def _heat_loss_rule_fix(block, n, t):
             """Rule definition for the heat loss depending on the nominal
@@ -236,53 +243,52 @@
             """Rule definition for the heat loss depending on the nominal
             capacity. Here, the losses can be "switched off".
             """
             o = list(n.outputs.keys())[0]
 
             expr = 0
             expr += - block.heat_loss[n, t]
-            expr += \
-                (n.heat_loss_factor[t] * m.flows[n, o].nominal_value + n.heat_loss_factor_fix[t]) *\
-                m.NonConvexFlow.status[n, o, t]
+            expr += (
+                n.heat_loss_factor[t] * m.flows[n, o].nominal_value
+                + n.heat_loss_factor_fix[t]
+            ) * m.NonConvexFlowBlock.status[n, o, t]
             return expr == 0
 
         self.heat_loss_equation_on_off = Constraint(
             self.NONCONVEX_HEATPIPES, m.TIMESTEPS, rule=_heat_loss_rule_on_off)
 
         def _relation_rule(block, n, t):
             """Link input and output flow and subtract heat loss."""
             i = list(n.inputs.keys())[0]
             o = list(n.outputs.keys())[0]
 
             expr = 0
             expr += - m.flow[n, o, t]
-            expr += m.flow[i, n, t] * n.conversion_factors[
-                o][t] / n.conversion_factors[i][t]
+            expr += m.flow[i, n, t]
             expr += - block.heat_loss[n, t]
             return expr == 0
 
         self.relation = Constraint(self.HEATPIPES, m.TIMESTEPS,
                                    rule=_relation_rule)
 
 
-class HeatPipelineInvestBlock(SimpleBlock):  # pylint: disable=too-many-ancestors
+class HeatPipelineInvestBlock(ScalarBlock):  # pylint: disable=too-many-ancestors
     r"""Block representing a pipeline of a district heating system.
     :class:`~oemof.solph.custom.HeatPipeline`
 
     **The following constraints are created:**
 
+    # TODO : Check and fix equations!
+
     .. _HeatPipelineInvestBlock-equations:
 
-    .. math::
-        &
-        (1) \dot{Q}_{out}(t) = \dot{Q}_{in}(t) \cdot
-        \frac{\eta_{out}}{\eta_{in}} - \dot{Q}_{loss}(t)\\
-        &
-        (2) \dot{Q}_{loss}(t) = f_{loss}(t) \cdot l \cdot \dot{Q}_{nominal}
-        &
+    .. math:: \dot{Q}_{out}(t) = \dot{Q}_{in}(t) \cdot
+        \frac{\eta_{out}}{\eta_{in}} - \dot{Q}_{loss}(t)
+
+    .. math:: \dot{Q}_{loss}(t) = f_{loss}(t) \cdot l \cdot \dot{Q}_{nominal}
 
     The symbols used are defined as follows
     (with Variables (V) and Parameters (P)):
 
     .. csv-table::
         :header: "symbol", "attribute", "type", "explanation"
         :widths: 1, 1, 1, 1
@@ -298,15 +304,14 @@
         Conversion factor of output flow (heat output)"
         ":math:`\eta_{in}`", ":py:obj:`conversion_factors[i][t]`", "P", "
         Conversion factor of input flow (heat input)"
         ":math:`f_{loss}(t)`", ":py:obj:`heat_loss_factor`", "P", "Specific
         heat loss factor for pipeline"
         ":math:`l`", ":py:obj:`length`", "P", "Length of heating pipeline"
 
-
     """
 
     CONSTRAINT_GROUP = True
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
@@ -322,18 +327,26 @@
         if group is None:
             return None
 
         m = self.parent_block()
 
         # Defining Sets
         self.INVESTHEATPIPES = Set(initialize=list(group))
-        self.CONVEX_INVESTHEATPIPES = Set(initialize=[
-            n for n in group if n.outputs[list(n.outputs.keys())[0]].investment.nonconvex is False])
-        self.NONCONVEX_INVESTHEATPIPES = Set(initialize=[
-            n for n in group if n.outputs[list(n.outputs.keys())[0]].investment.nonconvex is True])
+        self.CONVEX_INVESTHEATPIPES = Set(
+            initialize=[n for n in group
+                        if n.outputs[
+                            list(n.outputs.keys())[0]
+                        ].investment.nonconvex is False]
+        )
+        self.NONCONVEX_INVESTHEATPIPES = Set(
+            initialize=[n for n in group
+                        if n.outputs[
+                            list(n.outputs.keys())[0]
+                        ].investment.nonconvex is True]
+        )
 
         self.INVESTHEATPIPES_NO_DEMAND = Set(
             initialize=[n for n in group if len(n.outputs.keys()) == 1])
         self.INVESTHEATPIPES_WITH_DEMAND = Set(
             initialize=[n for n in group if len(n.outputs.keys()) == 2])
 
         # Defining Variables
@@ -342,48 +355,57 @@
 
         def _heat_loss_rule_convex(block, n, t):
             """Rule definition for constraint to connect the installed capacity
             and the heat loss
             """
             expr = 0
             expr += - block.heat_loss[n, t]
-            expr += n.heat_loss_factor[t] * m.InvestmentFlow.invest[n, list(n.outputs.keys())[0]]
+            expr += n.heat_loss_factor[t] * m.InvestmentFlowBlock.invest[
+                n, list(n.outputs.keys())[0]
+            ]
             expr += n.heat_loss_factor_fix[t]
             return expr == 0
         self.heat_loss_equation_convex = Constraint(
-            self.CONVEX_INVESTHEATPIPES, m.TIMESTEPS, rule=_heat_loss_rule_convex)
+            self.CONVEX_INVESTHEATPIPES, m.TIMESTEPS,
+            rule=_heat_loss_rule_convex
+        )
 
         def _heat_loss_rule_nonconvex(block, n, t):
             """Rule definition for constraint to connect the installed capacity
             and the heat loss
             """
             expr = 0
             expr += - block.heat_loss[n, t]
-            expr += n.heat_loss_factor[t] * m.InvestmentFlow.invest[n, list(n.outputs.keys())[0]]
+            expr += n.heat_loss_factor[t] * m.InvestmentFlowBlock.invest[
+                n, list(n.outputs.keys())[0]]
             expr += n.heat_loss_factor_fix[t] * \
-                m.InvestmentFlow.invest_status[n, list(n.outputs.keys())[0]]
+                m.InvestmentFlowBlock.invest_status[
+                    n, list(n.outputs.keys())[0]]
             return expr == 0
 
         self.heat_loss_equation_nonconvex = Constraint(
-            self.NONCONVEX_INVESTHEATPIPES, m.TIMESTEPS, rule=_heat_loss_rule_nonconvex)
+            self.NONCONVEX_INVESTHEATPIPES, m.TIMESTEPS,
+            rule=_heat_loss_rule_nonconvex
+        )
 
         def _relation_rule_no_demand(block, n, t):
             """Link input and output flow and subtract heat loss."""
             i = list(n.inputs.keys())[0]
             o = list(n.outputs.keys())[0]
 
             expr = 0
             expr += - m.flow[n, o, t]
-            expr += m.flow[i, n, t] * n.conversion_factors[
-                o][t] / n.conversion_factors[i][t]
+            expr += m.flow[i, n, t]
             expr += - block.heat_loss[n, t]
             return expr == 0
 
         self.relation_no_demand = Constraint(
-            self.INVESTHEATPIPES_NO_DEMAND, m.TIMESTEPS, rule=_relation_rule_no_demand)
+            self.INVESTHEATPIPES_NO_DEMAND, m.TIMESTEPS,
+            rule=_relation_rule_no_demand
+        )
 
         def _relation_rule_with_demand(block, n, t):
             """Link input and output flow and subtract heat loss."""
             i = list(n.inputs.keys())[0]
             o = list(n.outputs.keys())[0]
             d = list(n.outputs.keys())[1]
 
@@ -391,21 +413,25 @@
             expr += - m.flow[n, o, t]
             expr += m.flow[i, n, t] * n.conversion_factors[
                 o][t] / n.conversion_factors[i][t]
             expr += - block.heat_loss[n, t]
             expr += - m.flow[n, d, t]
             return expr == 0
         self.relation_with_demand = Constraint(
-            self.INVESTHEATPIPES_WITH_DEMAND, m.TIMESTEPS, rule=_relation_rule_with_demand)
+            self.INVESTHEATPIPES_WITH_DEMAND, m.TIMESTEPS,
+            rule=_relation_rule_with_demand
+        )
 
         def _inflow_outflow_invest_coupling_rule(block, n):  # pylint: disable=unused-argument
             """Rule definition of constraint connecting the inflow
-            `InvestmentFlow.invest of pipe with invested outflow `invest`
+            `InvestmentFlowBlock.invest of pipe with invested outflow `invest`
             by nominal_storage_capacity__inflow_ratio
             """
             i = list(n.inputs.keys())[0]
             o = list(n.outputs.keys())[0]
 
-            expr = (m.InvestmentFlow.invest[i, n] == m.InvestmentFlow.invest[n, o])
+            expr = (m.InvestmentFlowBlock.invest[i, n]
+                    == m.InvestmentFlowBlock.invest[n, o])
             return expr
         self.inflow_outflow_invest_coupling = Constraint(
-            self.INVESTHEATPIPES, rule=_inflow_outflow_invest_coupling_rule)
+            self.INVESTHEATPIPES, rule=_inflow_outflow_invest_coupling_rule
+        )
```

### Comparing `dhnx-0.0.2rc1/dhnx/plotting.py` & `dhnx-0.0.3/dhnx/plotting.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,32 +6,32 @@
 This file is part of project dhnx (). It's copyrighted
 by the contributors recorded in the version control history of the file,
 available from its original location:
 
 SPDX-License-Identifier: MIT
 """
 
-from collections import namedtuple
 import logging
+from collections import namedtuple
 
 import folium as fol
-from folium.features import DivIcon
-import matplotlib.pyplot as plt
 import matplotlib.collections as collections
+import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
+from folium.features import DivIcon
 
 logger = logging.getLogger()
 logger.setLevel(logging.INFO)
 
 cartopy_installed = True
 
 try:
-    from cartopy.io.img_tiles import Stamen
     from cartopy import crs as ccrs
+    from cartopy.io.img_tiles import Stamen
 
 except ImportError:
     logging.info("Cartopy is not installed. Background maps will not be drawn.")
     cartopy_installed = False
 
 
 class InteractiveMap():
@@ -130,15 +130,15 @@
         # note that I'm discarding the first and last for aesthetics
         # as I'm using markers to denote the start and end
         arrow_lats = np.linspace(p1.lat, p2.lat, n_arrows + 2)[1:n_arrows + 1]
         arrow_lons = np.linspace(p1.lon, p2.lon, n_arrows + 2)[1:n_arrows + 1]
 
         arrows = []
 
-        #creating each "arrow" and appending them to our arrows list
+        # creating each "arrow" and appending them to our arrows list
         for points in zip(arrow_lats, arrow_lons):
             arrows.append(
                 fol.RegularPolygonMarker(
                     location=points,
                     color=color, number_of_sides=3,
                     radius=size, rotation=rotation, fill=True))
```

### Comparing `dhnx-0.0.2rc1/dhnx/simulation.py` & `dhnx-0.0.3/dhnx/simulation.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 import warnings
 from functools import partial
 
 import networkx as nx
 import numpy as np
 import pandas as pd
 
-from .model import SimulationModel
-from .helpers import Dict, sum_ignore_none
 from .graph import write_edge_data_to_graph
+from .helpers import Dict
+from .helpers import sum_ignore_none
 from .input_output import save_results
-
+from .model import SimulationModel
 
 idx = pd.IndexSlice
 
 
 class SimulationModelNumpy(SimulationModel):
     r"""
     Implementation of a simulation model using numpy.
@@ -186,15 +186,15 @@
         select_scalars = [
             scalar[name].copy().rename(index=lambda x, prefix=component: prefix + '-' + str(x))
             for component, scalar in self.thermal_network.components.items()
             if name in scalar
         ]
 
         if select_scalars:
-            select_scalars = pd.concat(select_scalars, 0)
+            select_scalars = pd.concat(select_scalars, axis=0)
 
         else:
             select_scalars = None
 
         return select_scalars
 
     def _concat_sequences(self, name):
@@ -213,15 +213,15 @@
         """
         select_sequences = [
             d[name].copy().rename(columns=lambda x, prefix=component: prefix + '-' + x)
             for component, d in self.thermal_network.sequences.items()
             if name in d
         ]
 
-        concat_sequences = pd.concat(select_sequences, 1)
+        concat_sequences = pd.concat(select_sequences, axis=1)
 
         return concat_sequences
 
     @staticmethod
     def _set_producers_mass_flow(m):
         r"""
         Sets the mass flow of the producer.
@@ -648,16 +648,17 @@
             Pump power [W]
         """
         producers = [
             node for node, data in self.nx_graph.nodes(data=True)
             if data['component_type'] == 'Producer'
         ]
 
-        mass_flow_producers = \
-            self.results['pipes-mass_flow'].loc[:, idx[producers, :]].sum(axis=1)
+        mass_flow_producers = self.results['pipes-mass_flow'].iloc[
+            :, self.results['pipes-mass_flow'].columns.isin(
+                producers, level=0)].sum(axis=1)
 
         pump_power = mass_flow_producers * global_pressure_losses / (self.eta_pump * self.rho)
 
         return pump_power
 
     def _calculate_exponent_constant(self):
         r"""
```

### Comparing `dhnx-0.0.2rc1/dhnx.egg-info/PKG-INFO` & `dhnx-0.0.3/dhnx.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: dhnx
-Version: 0.0.2rc1
+Version: 0.0.3
 Summary: Simulation and optimization of district heating and cooling networks
-Home-page: UNKNOWN
 Author: oemof developer group
 Author-email: jann.launer@rl-institut.de, johannes-roeder@uni-bremen.de
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/x-rst
 Provides-Extra: cartopy
 Provides-Extra: geopandas
 Provides-Extra: osmnx
+Provides-Extra: tests
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 |badge_travis| |badge_coverage| |readthedocs| |zenodo|
 
 ~~~~
 DHNx
@@ -111,15 +109,13 @@
     :target: https://coveralls.io/github/oemof-heat/DHNx?branch=dev
     :alt: Test coverage
 
 .. |badge_travis| image:: https://api.travis-ci.org/oemof/DHNx.svg?branch=dev
     :target: https://travis-ci.org/oemof/DHNx
     :alt: Build status
 
-.. |zenodo| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.4147049.svg
-   :target: https://doi.org/10.5281/zenodo.4147049
+.. |zenodo| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.5084392.svg
+   :target: https://doi.org/10.5281/zenodo.5084392
 
 .. |readthedocs| image:: https://readthedocs.org/projects/dhnx/badge/?version=latest
     :target: https://dhnx.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
-
-
```

### Comparing `dhnx-0.0.2rc1/setup.py` & `dhnx-0.0.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,50 @@
 #!/usr/bin/env python
 
-from setuptools import setup
 import os
 
+from setuptools import setup
+
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(
     name='dhnx',
-    version='0.0.2rc1',
+    version='0.0.3',
     description='Simulation and optimization of district heating and cooling networks',
     author="oemof developer group",
     author_email='jann.launer@rl-institut.de, johannes-roeder@uni-bremen.de',
     long_description=read('README.rst'),
     long_description_content_type="text/x-rst",
     packages=[
         'dhnx',
         'dhnx.gistools',
+        'dhnx.optimization',
     ],
     package_data={
         'dhnx': [
             "*.csv",
             os.path.join("component_attrs", "*.csv"),
         ],
     },
     install_requires=[
         'pandas >= 0.18.0',
         'matplotlib',
         'networkx',
         'pillow',
         'folium',
         'addict',
-        'oemof.solph >= 0.4.0',
+        'oemof.solph >= 0.5.0',
         'scipy >= 1.5',
     ],
     extras_require={
         'cartopy': ['cartopy'],
         'geopandas': ['geopandas'],
         'osmnx': ['osmnx >= 0.16.1'],
+        "tests": [
+            "geopandas", "osmnx",
+            "CoolProp",
+        ],
     }
 )
```

