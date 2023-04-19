# Comparing `tmp/galaxywitness-0.2.3.1.tar.gz` & `tmp/galaxywitness-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galaxywitness-0.2.3.1.tar", max compression
+gzip compressed data, was "galaxywitness-0.2.4.tar", max compression
```

## Comparing `galaxywitness-0.2.3.1.tar` & `galaxywitness-0.2.4.tar`

### file list

```diff
@@ -1,13 +1,17 @@
--rw-r--r--   0        0        0     1074 2023-01-26 12:44:02.098783 galaxywitness-0.2.3.1/LICENSE
--rw-r--r--   0        0        0     2788 2023-01-26 12:44:02.098783 galaxywitness-0.2.3.1/README.md
--rw-r--r--   0        0        0      111 2023-01-26 12:44:02.494781 galaxywitness-0.2.3.1/galaxywitness/__init__.py
--rw-r--r--   0        0        0    12874 2023-01-26 12:44:02.494781 galaxywitness-0.2.3.1/galaxywitness/__main__.py
--rw-r--r--   0        0        0     7240 2023-01-26 12:44:02.494781 galaxywitness-0.2.3.1/galaxywitness/alpha_complex.py
--rw-r--r--   0        0        0    23057 2023-01-26 12:44:02.494781 galaxywitness-0.2.3.1/galaxywitness/ansi.txt
--rw-r--r--   0        0        0      542 2023-01-26 12:44:02.494781 galaxywitness-0.2.3.1/galaxywitness/ansiname.txt
--rw-r--r--   0        0        0     3917 2023-01-26 12:44:02.494781 galaxywitness-0.2.3.1/galaxywitness/base_complex.py
--rw-r--r--   0        0        0     2136 2023-01-26 12:44:02.494781 galaxywitness-0.2.3.1/galaxywitness/datasets.py
--rw-r--r--   0        0        0    16703 2023-01-26 12:44:02.494781 galaxywitness-0.2.3.1/galaxywitness/witness_complex.py
--rw-r--r--   0        0        0      563 2023-01-26 12:44:02.494781 galaxywitness-0.2.3.1/pyproject.toml
--rw-r--r--   0        0        0     3613 1970-01-01 00:00:00.000000 galaxywitness-0.2.3.1/setup.py
--rw-r--r--   0        0        0     3569 1970-01-01 00:00:00.000000 galaxywitness-0.2.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-04-19 17:34:11.972540 galaxywitness-0.2.4/LICENSE
+-rw-r--r--   0        0        0     2891 2023-04-19 17:34:11.972540 galaxywitness-0.2.4/README.md
+-rw-r--r--   0        0        0      138 2023-04-19 17:34:12.340551 galaxywitness-0.2.4/galaxywitness/__init__.py
+-rw-r--r--   0        0        0    16475 2023-04-19 17:34:12.340551 galaxywitness-0.2.4/galaxywitness/__main__.py
+-rw-r--r--   0        0        0     2224 2023-04-19 17:34:12.340551 galaxywitness-0.2.4/galaxywitness/alpha_complex.py
+-rw-r--r--   0        0        0    23057 2023-04-19 17:34:12.340551 galaxywitness-0.2.4/galaxywitness/ansi.txt
+-rw-r--r--   0        0        0      542 2023-04-19 17:34:12.340551 galaxywitness-0.2.4/galaxywitness/ansiname.txt
+-rw-r--r--   0        0        0     9519 2023-04-19 17:34:12.344551 galaxywitness-0.2.4/galaxywitness/base_complex.py
+-rw-r--r--   0        0        0     8522 2023-04-19 17:34:12.344551 galaxywitness-0.2.4/galaxywitness/clusterization.py
+-rw-r--r--   0        0        0     4596 2023-04-19 17:34:12.344551 galaxywitness-0.2.4/galaxywitness/datasets.py
+-rw-r--r--   0        0        0      808 2023-04-19 17:34:12.344551 galaxywitness-0.2.4/galaxywitness/manual_density.py
+-rw-r--r--   0        0        0     3032 2023-04-19 17:34:12.344551 galaxywitness-0.2.4/galaxywitness/rips_complex.py
+-rw-r--r--   0        0        0     1383 2023-04-19 17:34:12.344551 galaxywitness-0.2.4/galaxywitness/tests/test_betti.py
+-rw-r--r--   0        0        0     1451 2023-04-19 17:34:12.344551 galaxywitness-0.2.4/galaxywitness/tests/test_tomato.py
+-rw-r--r--   0        0        0    11505 2023-04-19 17:34:12.344551 galaxywitness-0.2.4/galaxywitness/witness_complex.py
+-rw-r--r--   0        0        0      953 2023-04-19 17:34:12.344551 galaxywitness-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     3844 1970-01-01 00:00:00.000000 galaxywitness-0.2.4/PKG-INFO
```

### Comparing `galaxywitness-0.2.3.1/LICENSE` & `galaxywitness-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `galaxywitness-0.2.3.1/README.md` & `galaxywitness-0.2.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # GalaxyWitness
 [![MIT License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat)](http://choosealicense.com/licenses/mit/)
 [![CodeFactor](https://www.codefactor.io/repository/github/davidosx/galaxywitness/badge/master)](https://www.codefactor.io/repository/github/davidosx/galaxywitness/overview/master)
 [![Documentation Status](https://readthedocs.org/projects/galaxywitness/badge/?version=latest)](https://galaxywitness.readthedocs.io/en/latest/?badge=latest)
+[![PyPI version](https://badge.fury.io/py/galaxywitness.svg)](https://badge.fury.io/py/galaxywitness)
 
 
 Package for topological data analysis of the big data. It is attempt to study distribution of galaxies in the universe via TDA. Based on [GUDHI](https://gudhi.inria.fr) and [Astropy](https://www.astropy.org)
 
 ## Requirements
 1. Python 3.8+ and pip
 2. git (for development)
```

### Comparing `galaxywitness-0.2.3.1/galaxywitness/__main__.py` & `galaxywitness-0.2.4/galaxywitness/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,35 +13,43 @@
             print("\t\t\t" + str1, end="")
 
     with open(site.getsitepackages()[0] + "/galaxywitness/ansiname.txt", encoding="utf-8") as ansiname:
         for str2 in ansiname:
             print("\t\t\t" + str2, end="")
 except OSError:
     print("\033[01;32mGalaxyWitness\033[0m\n")
-    print("\033[01;33mWarning: Can't load the banner!\033[0m")
+    print("\033[01;33mWarning: Can't load the banner! Dev version\033[0m")
 
 print("\n\t\tTo Infinity... and Beyond!\n\n")
 print("Loading...")
 #################################################
 
+from prompt_toolkit import PromptSession
+from prompt_toolkit.history import InMemoryHistory
+from prompt_toolkit.auto_suggest import AutoSuggestFromHistory
 
 import numpy as np
 import plotly.graph_objects as go
 import pandas as pd
 
 
 from astropy.coordinates import SkyCoord
 from astropy.coordinates import Distance
 from astropy import units as u
 
 
 from galaxywitness.base_complex import BaseComplex
 from galaxywitness.witness_complex import WitnessComplex
 from galaxywitness.alpha_complex import AlphaComplex
+from galaxywitness.rips_complex import RipsComplex
 from galaxywitness.datasets import Dataset
+from galaxywitness.clusterization import Clusterization
+
+session = PromptSession(history=InMemoryHistory(),
+                        auto_suggest=AutoSuggestFromHistory())
 
 MAX_DIM = 3
 
 
 def pause(t=1):
     time.sleep(t)
 
@@ -75,15 +83,15 @@
 
 def plot_data_cloud_alpha(landmarks, key_save, path_to_save):
     # plot point cloud
     fig = go.Figure(data=[go.Scatter3d(x=landmarks[:, 0],
                                        y=landmarks[:, 1],
                                        z=landmarks[:, 2],
                                        mode='markers',
-                                       marker=dict(size=2, color='orange'))])
+                                       marker=dict(size=1, color='orange'))])
 
     fig.update_layout(scene=dict(xaxis_title='X, Mpc',
                                  yaxis_title='Y, Mpc',
                                  zaxis_title='Z, Mpc'))
 
     if key_save == 'y':
         fig.write_image(path_to_save + '/plot_data_cloud.pdf')
@@ -95,21 +103,21 @@
     if key_anim == 'y':
         if key_fig == 'plotly':
             fil_complex.animate_simplex_tree_plotly(path_to_save=path_to_save)
         else:
             fil_complex.animate_simplex_tree(path_to_save=path_to_save)
 
     fil_complex.get_diagram(show=True, path_to_save=path_to_save)
-    fil_complex.get_barcode(show=True, path_to_save=path_to_save)
+    # fil_complex.get_barcode(show=True, path_to_save=path_to_save)
 
 
-def clustering(fil_complex, points, path_to_save):
+def clustering(fil_complex, points, r_max, path_to_save):
     print("ToMATo clustering...")
     t = time.time()
-    tomato = fil_complex.tomato()
+    tomato = fil_complex.tomato(r_max)
     t = time.time() - t
 
     # tomato.plot_diagram()
     fig = go.Figure(data=[go.Scatter3d(x=points[:, 0],
                                        y=points[:, 1],
                                        z=points[:, 2],
                                        mode='markers',
@@ -122,160 +130,201 @@
     if path_to_save is not None:
         fig.write_image(path_to_save + "/tomato.pdf")
 
     fig.show()
 
     print(f"\033[F\U0001F345 clustering... done\033[01;32m \u2714\033[0m\
     in \033[01;32m{t}\033[0m sec.\n")
+    return tomato
 
 
 def download_prepared_datasets():
     ssl._create_default_https_context = ssl._create_unverified_context
     print("Choose one of available datasets:")
     print("\n\t---------- datasets -----------")
     print("\t\033[01;32m[1] <-> Galaxies_400K\033[0m")
-    print("\t\033[01;32m[2] <-> another dataset\033[0m")
+    print("\t\033[01;32m[2] <-> Galaxies_1KK\033[0m")
+    print("\t\033[01;32m[3] <-> go to ./data folder \033[0m")
     print("\t--------------------------------\n")
-    input_dataset = int(input(" > Enter number of dataset: "))
+    input_dataset = int(session.prompt(' > Enter number of dataset: ', auto_suggest=AutoSuggestFromHistory()))
     name = ''
     if input_dataset == 1:
         name = 'Galaxies_400K'
-    else:
-        print("will be implemented soon...")
+    elif input_dataset == 2:
+        name = 'Galaxies_1KK'
+    elif input_dataset == 3: return
 
     dataset = Dataset(name)
     dataset.download()
-    
+
+def download_custom():
+    print("Choose your TAP service:")
+    print("\n\t---------- services -----------")
+    print("\t\033[01;32m[1] <-> VOXastro\033[0m")
+    print("\t\033[01;32m[2] <-> Simbad (University of Strasbourg)\033[0m")
+    print("\t\033[01;32m[3] <-> NED (Caltech)\033[0m")
+    print("\t--------------------------------\n")
+    input_service = int(session.prompt(' > Your TAP service: ', auto_suggest=AutoSuggestFromHistory()))
+    input_size = int(session.prompt(' > Size of dataset: ', auto_suggest=AutoSuggestFromHistory()))
+    name = ''
+    if input_service == 1:
+        name = 'rcsed'
+    elif input_service == 2:
+        name = 'simbad'
+    elif input_service == 3:
+        name = 'ned'
+
+    dataset = Dataset(name)
+    dataset.download_via_tap(input_size)
+    # dataset.add_new_dataset("custom", "https://custom.com")
 
 def preconfiguration():
     print(f"\nSystem information: \033[01;32m{os.uname()}\033[0m")
     print("\nPreconfiguration:\n")
-    prepared = input(" > Do you want to use prepared datasets? [y/n]: ")
+    prepared = session.prompt(' > Do you want to use prepared datasets? [y/n]: ', auto_suggest=AutoSuggestFromHistory())
 
     if prepared == "y":
         download_prepared_datasets()
+    else:
+        download_custom()
 
     print("\nChoose file with your data [.csv file]:")
 
     data_tables = os.walk('./data')
 
     print(data_tables)
     elem = None
     print("\n\t---------- data -----------")
     for _, _, elem in data_tables:
         for name in elem:
             print(f"\t\033[01;32m[{elem.index(name) + 1}] <-> {name}\033[0m")
     print("\t---------------------------\n")
 
-    table_num = int(input(f" > Enter number of your table [1-{len(elem)}]: "))
+    table_num = int(session.prompt(f" > Enter number of your table [1-{len(elem)}]: ", auto_suggest=AutoSuggestFromHistory()))
     path = os.path.abspath('.') + '/data/' + elem[table_num - 1]
 
     print(f"Loading data from \033[01;32m{path}\033[0m...")
     t = time.time()
     df = pd.read_csv(path)
     t = time.time() - t
 
     print(f"Loading done\033[01;32m \u2714\033[0m in \033[01;32m{t}\033[0m sec.\
     We have data about \033[01;32m{len(df)}\033[0m galaxies.\n")
 
     return df
 
 
 def main():
-    doc_key = input(" > Do you want to open documentation? [y/n]: ")
+    doc_key = session.prompt(' > Do you want to open documentation? [y/n]: ', auto_suggest=AutoSuggestFromHistory())
     if doc_key == 'y':
         print("\nOpening documentation...")
         url = 'https://galaxywitness.rtfd.io' #'file://' + os.path.abspath('.') + '/docs/build/html/index.html'
         webbrowser.open(url, new=2)
         print("Done\033[01;32m \u2714\033[0m")
-    
+
     try:
         df = preconfiguration()
     except ValueError as e:
         raise Exception("\033[01;31mFolder 'data' does not exist or empty!\033[0m") from e
 
-    # readline.set_auto_history(True)
-    n_gal = int(input(f" > Enter number of galaxies [10-{len(df)}]: "))
+    n_gal = int(session.prompt(f" > Enter number of galaxies [10...{len(df)}]: ", auto_suggest=AutoSuggestFromHistory()))
 
-    type_of_complex = input(" > Enter type of complex [witness/alpha]: ")
+    print("Choose type of complex:")
+    print("\n\t---------- complexes -----------")
+    print("\t\033[01;32m[1] <-> Vietoris-Rips complex\033[0m")
+    print("\t\033[01;32m[2] <-> Alpha complex\033[0m")
+    print("\t\033[01;32m[3] <-> Witness complex\033[0m")
+    print("\t--------------------------------\n")
+    type_of_complex = int(session.prompt(" > Your complex: ", auto_suggest=AutoSuggestFromHistory()))
+    if type_of_complex == 1:
+        type_of_complex = "rips"
+    elif type_of_complex == 2:
+        type_of_complex = "alpha"
+    elif type_of_complex == 3:
+        type_of_complex = "witness"
 
     if type_of_complex == "witness":
-        n_landmarks = int(input(f" > Enter number of landmarks [10-{n_gal}]: "))
+        n_landmarks = int(session.prompt(f" > Enter number of landmarks [10...{n_gal}]: ", auto_suggest=AutoSuggestFromHistory()))
     else:
         n_landmarks = n_gal
 
     # n_jobs = int(input("Enter number of processes: "))
 
-    key_adv = input(" > Advanced configuration? [y/n]: ")
     r_max = 7.5
     first_witness = 0
     tomato_key = 'y'
-    column_names = ['RAJ2000_gal', 'DEJ2000_gal', 'z_gal']
+    column_names = []#['RAJ2000_gal', 'DEJ2000_gal', 'z_gal']
     isomap_eps = 0
     key_plot_cloud = 'y'
     key_anim = 'y'
     key_save = 'n'
     key_complex_type = 'gudhi'
     key_fig = 'mpl'
+    # max_edge_length = np.inf
+    sparse = None
+
+    key_plot_cloud = session.prompt(' > Do you want plot the point cloud? [y/n]: ', auto_suggest=AutoSuggestFromHistory())
+    key_anim = session.prompt(f" > Do you want watch the animation of {type_of_complex} filtration? [y/n]: ", auto_suggest=AutoSuggestFromHistory())
+    if key_anim == 'y':
+        key_fig = session.prompt(
+            " > What will we use for the animation of a filtered complex? [plotly(more slow, but more cool)/mpl(matplotlib)]: ", auto_suggest=AutoSuggestFromHistory())
+    key_save = session.prompt(" > Do you want save all plots to ./imgs? [y/n]: ", auto_suggest=AutoSuggestFromHistory())
+    tomato_key = session.prompt(" > Do you want run tomato clustering? [y/n]: ", auto_suggest=AutoSuggestFromHistory())
+    key_adv = session.prompt(" > Advanced configuration? [y/n]: ", auto_suggest=AutoSuggestFromHistory())
     if key_adv == 'y':
-        key_plot_cloud = input(" > Do you want plot the point cloud? [y/n]: ")
-        key_anim = input(f" > Do you want watch the animation of {type_of_complex} filtration? [y/n]: ")
-        if key_anim == 'y':
-            key_fig = input(
-                " > What will we use for the animation of a filtered complex? [plotly(more slow, but more cool)/mpl(matplotlib)]: ")
-        key_save = input(" > Do you want save all plots to \033[01;32m./imgs\033[0m? [y/n]: ")
-
-        key_complex_type = input(" > What type of simplicial complex will we use? [gudhi/custom]: ")
-        r_max = float(input(
-            " > Enter max value of filtration[\033[01;32m usually \u2264 15\033[0m, the more the slower calculate]: "))
-        tomato_key = input(" > Do you want run\033[01;32m tomato\033[0m clustering? [y/n]: ")
+        key_complex_type = session.prompt(" > What type of simplicial complex will we use? [gudhi/custom]: ", auto_suggest=AutoSuggestFromHistory())
+        r_max = float(session.prompt(
+            " > Enter max value of filtration [usually \u2264 15, the more the slower calculations]: ", auto_suggest=AutoSuggestFromHistory()))
+        if type_of_complex == "witness":
+            first_witness = int(session.prompt(f" > Enter first witness [range: 0...{len(df) - n_gal}]: ", auto_suggest=AutoSuggestFromHistory()))
         if r_max == -1:
             r_max = None
+        if type_of_complex == "rips":
+            sparse = float(session.prompt(" > Enter 'sparse' parameter to build sparse Rips or -1: ", auto_suggest=AutoSuggestFromHistory()))
+            if sparse == -1:
+                sparse = None
 
-        if type_of_complex == 'witness':
-            isomap_eps = float(input(" > Enter\033[01;32m isomap\033[0m parameter [0 - don't compute isomap metric]: "))
+        # if type_of_complex == 'witness':
+        #     isomap_eps = float(input(" > Enter\033[01;32m isomap\033[0m parameter [0 - don't compute isomap metric]: "))
 
-    # cosmology = input("Enter cosmology model: ")
+        # cosmology = input("Enter cosmology model: ")
 
     path_to_save = None
     time_list = list(time.localtime())
     time_str = ''
     for i in range(6):
         time_str += str(time_list[i])
 
     if key_save == 'y':
         path_to_save = os.path.abspath('.') + '/imgs/' + time_str + f"-{n_gal}-{n_landmarks}"
         if not os.path.isdir('imgs'):
             os.mkdir('imgs')
         os.mkdir(path_to_save)
 
-    if key_adv == 'y':
-        section()
-        print(f"Info about the handled table: \n\033[01;32m{df.info}\033[0m\n")
+    section()
+    print(f"Info about the handled table: \n\033[01;32m{df.info}\033[0m\n")
 
-        list_names = list(df)
-        pause()
-        print("\nChoosing names of 3 columns for right ascension [RA], declination [Dec] and redshift [z]:")
+    list_names = list(df)
+    pause()
+    print("\nChoosing names of 3 columns for right ascension [ra], declination [dec] and redshift [z]:")
 
-        print("\n\t---------- column names -----------")
-        for elem in list_names:
-            if list_names.index(elem) != 0:
-                print(f"\t\033[01;32m{list_names.index(elem)} <-> {elem}\033[0m")
+    print("\n\t---------- column names -----------")
+    for elem in list_names:
+        if list_names.index(elem) != 0:
+            print(f"\t\033[01;32m[{list_names.index(elem)}] <-> {elem}\033[0m")
 
-        print("\t-----------------------------------\n")
+    print("\t-----------------------------------\n")
 
-        column_nums = []
+    column_nums = []
 
-        for i in range(3):
-            column_nums.append(
-                int(input(f" > Choose number of column #{i + 1} of 3, from list above (column names): ")))
+    for name in ('ra', 'dec', 'z'):
+        column_nums.append(
+            int(session.prompt(f" > Choose column for {name}, from list above (column names): ", auto_suggest=AutoSuggestFromHistory())))
 
-        column_names = [list(df)[column_nums[0]], list(df)[column_nums[1]], list(df)[column_nums[2]]]
-        if type_of_complex == "witness":
-            first_witness = int(input(f" > Enter index of first witness [0-{df[column_names[2]].size - n_gal}]: "))
+    column_names = [list(df)[column_nums[0]], list(df)[column_nums[1]], list(df)[column_nums[2]]]
 
     section()
 
     print("Preprocessing data and plot the point cloud...")
 
     t = time.time()
 
@@ -323,28 +372,31 @@
     print(f"Computing persistence with {type_of_complex} filtration...")
 
     t = time.time()
     complex_ = BaseComplex()
     if type_of_complex == "witness":
         complex_.__class__ = WitnessComplex
         complex_.__init__(landmarks, witnesses, landmarks_idxs, isomap_eps=isomap_eps)
-    else:
+    elif type_of_complex == "alpha":
         complex_.__class__ = AlphaComplex
         complex_.__init__(points=landmarks)
+    else:
+        complex_.__class__ = RipsComplex
+        complex_.__init__(points=landmarks, max_edge_length=r_max, sparse=sparse)
 
     complex_.compute_simplicial_complex(d_max=MAX_DIM, r_max=r_max, custom=(key_complex_type == 'custom'))
 
-    if key_complex_type == 'gudhi':
-        magnitude_level = (r_max ** 2) / 2.0
+    if type_of_complex == 'alpha':
+        magnitude_levels = [(r_max ** 2),  (r_max ** 2) / 2.0, (r_max ** 2) / 2.0]
     else:
-        magnitude_level = r_max / 2.0
+        magnitude_levels = [r_max, r_max / 2.0,  r_max / 2.0]
 
     simplex_tree = complex_.simplex_tree
 
-    betti = complex_.get_persistence_betti(dim=MAX_DIM, magnitude=magnitude_level)
+    betti = complex_.get_persistence_betti(dim=MAX_DIM, magnitudes=magnitude_levels)
 
     t = time.time() - t
 
     print(f"\033[FComputing persistence with {type_of_complex} filtration... done\033[01;32m \u2714\033[0m in \033[01;32m{t}\033[0m sec.\n")
     pause()
 
     print("The \033[01;32msimplex tree\033[0m constructed \033[01;32m\u2714\033[0m")
@@ -361,17 +413,28 @@
 
     print("\033[F\033[F\033[FDrawing persistence diagram and barcode... done \033[01;32m \u2714\033[0m")
     pause()
 
     section()
 
     if tomato_key == 'y':
-        if type_of_complex == "witness":
-            clustering(complex_, complex_.witnesses, path_to_save)
-        else:
-            clustering(complex_, complex_.points, path_to_save)
+        if type_of_complex != "witness":
+            # clustering(complex_, complex_.witnesses, path_to_save, den_type, graph_type_)
+            tomato = clustering(complex_, complex_.points, r_max, path_to_save)
+
+            print("Warning: results down below is additional experimental functionality")
+            cl_1, cl_2 = Clusterization(points), Clusterization(points)
+            cl_1.import_clustering(tomato.labels_)
+            cl_2.tomato(r_max)
+            print("Draw clustering...")
+            cl_2.draw_clustering()
+            print("Draw projections of clustering on random planes...")
+            cl_2.draw_projections(2)
+            diff = cl_1.compare_clusterization(cl_2)
+            print(f"Test Difference between clusterings is \033[01;32m {diff}\033[0m")
+
 
 
 if __name__ == '__main__':
     print("\033[FLoading... done \033[01;32m\u2714\033[0m")
     pause()
     main()
```

### Comparing `galaxywitness-0.2.3.1/galaxywitness/ansi.txt` & `galaxywitness-0.2.4/galaxywitness/ansi.txt`

 * *Files identical despite different names*

### Comparing `galaxywitness-0.2.3.1/galaxywitness/ansiname.txt` & `galaxywitness-0.2.4/galaxywitness/ansiname.txt`

 * *Files identical despite different names*

### Comparing `galaxywitness-0.2.3.1/galaxywitness/witness_complex.py` & `galaxywitness-0.2.4/galaxywitness/witness_complex.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,25 +3,20 @@
 
 import multiprocessing as mp
 from joblib import Parallel, delayed
 from joblib import dump
 
 import numpy as np
 
-import matplotlib.pyplot as plt
-from matplotlib import colors
-from mpl_toolkits.mplot3d.art3d import Poly3DCollection
-import plotly.graph_objects as go
 
 from scipy.sparse import csr_matrix
 from scipy.sparse.csgraph import floyd_warshall
 
 # gudhi is needed to construct a simplex tree and to plot the persistence diagram.
 import gudhi
-from gudhi.clustering.tomato import Tomato
 
 from sklearn.metrics import pairwise_distances
 
 from galaxywitness.base_complex import BaseComplex
 
 # hard-coded
 #MAX_DIST_INIT = 100000
@@ -57,21 +52,19 @@
     # ]
 
     def __init__(self, landmarks, witnesses, landmarks_idxs, n_jobs = -1, isomap_eps = 0):
         """
         Constuctor
         
         """
-        super().__init__()
+        super().__init__(landmarks)
         
         self.landmarks = landmarks
         self.witnesses = witnesses
-        self.simplex_tree_computed = False
         self.landmarks_idxs = landmarks_idxs
-        self.simplex_tree = None
 
         self.distances = pairwise_distances(witnesses, landmarks, n_jobs = n_jobs)
             
         if isomap_eps > 0:
             #distances = pairwise_distances(witnesses, n_jobs = -1)
                         
             # todo: optimize
@@ -272,168 +265,59 @@
         :param path_to_save: place, where we are saving files
         :type  path_to_save: str
          
         """
         assert self.simplex_tree_computed
         
         gen = self.simplex_tree.get_filtration()
-        
-        verts = []
         gen = list(gen)
         scale = NUMBER_OF_FRAMES/gen[-1][1]
 
         for num in range(1, NUMBER_OF_FRAMES + 1):
-            fig = plt.figure()
-            ax = fig.add_subplot(projection = "3d")
-            if self.witnesses.shape[0] <= MAX_N_PLOT:
-                ax.scatter3D(self.witnesses[:MAX_N_PLOT, 0], 
-                self.witnesses[:MAX_N_PLOT, 1], 
-                self.witnesses[:MAX_N_PLOT, 2], 
-                s = 1, 
-                linewidths = 0.1)
-            ax.scatter3D(self.landmarks[:MAX_N_PLOT, 0], 
-                        self.landmarks[:MAX_N_PLOT, 1], 
-                        self.landmarks[:MAX_N_PLOT, 2], 
-                        s = 2, 
-                        linewidths = 1, 
-                        color = 'C1')
-                        
-            ax.set_xlabel('X, Mpc')
-            ax.set_ylabel('Y, Mpc')
-            ax.set_zlabel('Z, Mpc')
+            # if self.witnesses.shape[0] <= MAX_N_PLOT:
+            #     ax.scatter3D(self.witnesses[:MAX_N_PLOT, 0], 
+            #     self.witnesses[:MAX_N_PLOT, 1], 
+            #     self.witnesses[:MAX_N_PLOT, 2], 
+            #     s = 1, 
+            #     linewidths = 0.1)
             
-            for element in gen:
-                if element[1]*scale <= num:
-                    if len(element[0]) == 2:
-                        x = [self.landmarks[element[0][0]][0], 
-                        self.landmarks[element[0][1]][0]]
-                        
-                        y = [self.landmarks[element[0][0]][1], 
-                        self.landmarks[element[0][1]][1]]
-                        
-                        z = [self.landmarks[element[0][0]][2], 
-                        self.landmarks[element[0][1]][2]]
-                        
-                        ax.plot(x, y, z)
-                        
-                    if len(element[0]) == 3:
-                        x = [self.landmarks[element[0][0]][0], 
-                        self.landmarks[element[0][1]][0], 
-                        self.landmarks[element[0][2]][0]]
-                        
-                        y = [self.landmarks[element[0][0]][1], 
-                        self.landmarks[element[0][1]][1], 
-                        self.landmarks[element[0][2]][1]]
-                        
-                        z = [self.landmarks[element[0][0]][2], 
-                        self.landmarks[element[0][1]][2], 
-                        self.landmarks[element[0][2]][2]]
-                        
-                        verts.append(list(zip(x, y, z)))
-                        
-                        poly = Poly3DCollection(verts)
-                        
-                        poly.set_color(colors.rgb2hex(np.random.rand(3)))
-                        
-                        ax.add_collection3d(poly)
-                        
-                        verts.clear()
-              
-            ax.set_title(f"Animation of witness filtration: picture #{num} of {NUMBER_OF_FRAMES}")
-            
-            if path_to_save is not None:
-                plt.savefig(path_to_save + f"/picture{num}.png", dpi = 200)
-                
-            plt.show()
+            self.draw_simplicial_complex(num, num/scale, 'mpl', path_to_save)
+
             
     def animate_simplex_tree_plotly(self, path_to_save):
         """
         Draw animation of filtration (powered by plotly)
         
         :param path_to_save: place, where we are saving files
         :type  path_to_save: str 
         """
         assert self.simplex_tree_computed
         
         gen = self.simplex_tree.get_filtration()
-        
         gen = list(gen)
         scale = NUMBER_OF_FRAMES/gen[-1][1]
 
         for num in range(1, NUMBER_OF_FRAMES + 1):
-            data = []
-            if self.witnesses.shape[0] <= MAX_N_PLOT:
-                data.append(go.Scatter3d(x=self.witnesses[:MAX_N_PLOT, 0], 
-                                        y=self.witnesses[:MAX_N_PLOT, 1], 
-                                        z=self.witnesses[:MAX_N_PLOT, 2], 
-                                        mode='markers', 
-                                        marker=dict(size=1, color='blue')))
-            
-            data.append(go.Scatter3d(x=self.landmarks[:MAX_N_PLOT, 0], 
-                                    y=self.landmarks[:MAX_N_PLOT, 1], 
-                                    z=self.landmarks[:MAX_N_PLOT, 2], 
-                                    mode='markers',
-                                    marker=dict(size=2, color='orange')))
-            
-            for element in gen:
-                if element[1]*scale <= num:
-                    if len(element[0]) == 2:
-                        x = [self.landmarks[element[0][0]][0], 
-                        self.landmarks[element[0][1]][0]]
-                        
-                        y = [self.landmarks[element[0][0]][1], 
-                        self.landmarks[element[0][1]][1]]
-                        
-                        z = [self.landmarks[element[0][0]][2], 
-                        self.landmarks[element[0][1]][2]]
-                        
-                        data.append(go.Scatter3d(x=x,
-                                                y=y,
-                                                z=z, 
-                                                marker = dict(size=2, color='orange'),
-                                                line = dict(color=colors.rgb2hex(np.random.rand(3)), width=3)))
-                                                
-                    if len(element[0]) == 3:
-                        x = [self.landmarks[element[0][0]][0], 
-                        self.landmarks[element[0][1]][0], 
-                        self.landmarks[element[0][2]][0]]
-                        
-                        y = [self.landmarks[element[0][0]][1], 
-                        self.landmarks[element[0][1]][1], 
-                        self.landmarks[element[0][2]][1]]
-                        
-                        z = [self.landmarks[element[0][0]][2], 
-                        self.landmarks[element[0][1]][2], 
-                        self.landmarks[element[0][2]][2]]
-                        
-                        data.append(go.Mesh3d(x=x, 
-                                              y=y, 
-                                              z=z, 
-                                              color=colors.rgb2hex(np.random.rand(3)), 
-                                              opacity=0.8))
-              
-            fig = go.Figure(data=data)
-            
-            fig.update_layout(scene = dict(xaxis_title = "X, Mpc", 
-                                          yaxis_title = "Y, Mpc", 
-                                          zaxis_title = "Z, Mpc"))
-            
-            if path_to_save is not None:
-                fig.write_image(path_to_save + f"/picture{num}.pdf")
-                
-            fig.show()
-
-    def tomato(self):
-        """
-        ToMATo clustering with automatic choice of number of clusters. 
-        Hence clustering depends on filtered complex construction and 
-        max value of filtration.
-        
-        """
-        t = Tomato()
-        t.fit(self.witnesses)
-        t.n_clusters_ = self.betti[0]
-        return t
+            # if self.witnesses.shape[0] <= MAX_N_PLOT:
+            #     data.append(go.Scatter3d(x=self.witnesses[:MAX_N_PLOT, 0], 
+            #                             y=self.witnesses[:MAX_N_PLOT, 1], 
+            #                             z=self.witnesses[:MAX_N_PLOT, 2], 
+            #                             mode='markers', 
+            #                             marker=dict(size=1, color='blue')))
+
+            self.draw_simplicial_complex(num, num/scale, 'plotly', path_to_save)
+
+
+    # def tomato(self, max_fil_val=10):
+    #     """
+    #     ToMATo clustering with automatic choice of number of clusters.
+    #     Hence, clustering depends on filtered complex construction and
+    #     max value of filtration.
+
+    #     """
+
+    #     t = Tomato(density_type = 'manual', graph_type='manual')
+    #     t.fit(self.get_adjacency_list(max_fil_val), weights=self.density_class.foo(self.points))
+    #     t.n_clusters_ = self.betti[0]
+    #     return t
         
         
-            
-
```

### Comparing `galaxywitness-0.2.3.1/setup.py` & `galaxywitness-0.2.4/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,39 +1,115 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: galaxywitness
+Version: 0.2.4
+Summary: Package for topological data analysis of the big data. It is attempt to study distribution of galaxies in the universe via TDA
+Home-page: https://github.com/davidosx/GalaxyWitness
+License: MIT
+Author: David Miheev
+Author-email: me@davidkorol.life
+Requires-Python: >=3.8
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: astropy
+Requires-Dist: gudhi
+Requires-Dist: matplotlib
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: plotly
+Requires-Dist: prompt-toolkit
+Requires-Dist: pyvo
+Requires-Dist: scikit-learn
+Requires-Dist: tqdm
+Project-URL: Documentation, https://galaxywitness.rtfd.io/
+Project-URL: Repository, https://github.com/davidosx/GalaxyWitness
+Description-Content-Type: text/markdown
+
+# GalaxyWitness
+[![MIT License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat)](http://choosealicense.com/licenses/mit/)
+[![CodeFactor](https://www.codefactor.io/repository/github/davidosx/galaxywitness/badge/master)](https://www.codefactor.io/repository/github/davidosx/galaxywitness/overview/master)
+[![Documentation Status](https://readthedocs.org/projects/galaxywitness/badge/?version=latest)](https://galaxywitness.readthedocs.io/en/latest/?badge=latest)
+[![PyPI version](https://badge.fury.io/py/galaxywitness.svg)](https://badge.fury.io/py/galaxywitness)
+
+
+Package for topological data analysis of the big data. It is attempt to study distribution of galaxies in the universe via TDA. Based on [GUDHI](https://gudhi.inria.fr) and [Astropy](https://www.astropy.org)
+
+## Requirements
+1. Python 3.8+ and pip
+2. git (for development)
+
+OS X or Linux
+
+## Installation
+For the best experience, use python virtual environment:
+```sh
+pip3 install virtualenv
+virtualenv env (or python3 -m virtualenv galaxy-witness)
+. ./env/bin/activate
+```
+Install this package from PyPI via ```pip install galaxywitness```
+
+## Documentation
+You can find our technical documentation here: [Docs](https://galaxywitness.rtfd.io)
+### For developers
+[Sphinx](https://www.sphinx-doc.org/en/master/index.html) generates documentation for delelopers from sources in <code>./docs</code> folder. HTML files of documentation are in <code>./docs/build/html</code> and you can open it with browser. 
+If you want to build documentation yourself:
+```sh
+cd docs
+make html
+```
+or if you want to get .pdf with documentation:
+```sh
+cd docs
+make latexpdf
+```
+
+## Usage
+To run just type:
+```sh   
+python -m galaxywitness
+```
+
+In runtime the program will request you to choose file with your data. This file have to be in folder ```./data```
+
+If you want to finish a work with package and deactivate virtual environment just type:
+```sh
+deactivate
+```
+
+## Development
+You can use python virtual environment and install dependencies manually:
+### Create and activate a virtual environment
+This will create a new virtual environment called "galaxy-witness":
+```sh
+pip3 install virtualenv
+virtualenv galaxy-witness (or python3 -m virtualenv galaxy-witness)
+. ./galaxy-witness/bin/activate
+``` 
+This will clone the repository "GalaxyWitness" on your local machine, install dependencies and install this package 'galaxywitness':
+```sh
+git clone https://github.com/davidosx/GalaxyWitness
+cd GalaxyWitness
+pip install -r requirements.txt
+python setup.py install
+```
+
+Or poetry package manager:
+### Poetry
+```sh
+git clone https://github.com/davidosx/GalaxyWitness
+cd GalaxyWitness
+poetry install
+```
+
+### Uninstalling
+For uninstalling (include dependencies and an virtual environment):
+```sh
+rm -r GalaxyWitness
+rm -r galaxy-witness
+```
 
-packages = \
-['galaxywitness']
 
-package_data = \
-{'': ['*']}
 
-install_requires = \
-['Sphinx',
- 'astropy',
- 'gudhi',
- 'matplotlib',
- 'numpy',
- 'pandas',
- 'plotly',
- 'scikit-learn',
- 'sphinx-rtd-theme',
- 'tqdm']
-
-setup_kwargs = {
-    'name': 'galaxywitness',
-    'version': '0.2.3.1',
-    'description': 'Package for topological data analysis of the big data. It is attempt to study distribution of galaxies in the universe via TDA',
-    'long_description': '# GalaxyWitness\n[![MIT License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat)](http://choosealicense.com/licenses/mit/)\n[![CodeFactor](https://www.codefactor.io/repository/github/davidosx/galaxywitness/badge/master)](https://www.codefactor.io/repository/github/davidosx/galaxywitness/overview/master)\n[![Documentation Status](https://readthedocs.org/projects/galaxywitness/badge/?version=latest)](https://galaxywitness.readthedocs.io/en/latest/?badge=latest)\n\n\nPackage for topological data analysis of the big data. It is attempt to study distribution of galaxies in the universe via TDA. Based on [GUDHI](https://gudhi.inria.fr) and [Astropy](https://www.astropy.org)\n\n## Requirements\n1. Python 3.8+ and pip\n2. git (for development)\n\nOS X or Linux\n\n## Installation\nFor the best experience, use python virtual environment:\n```sh\npip3 install virtualenv\nvirtualenv env (or python3 -m virtualenv galaxy-witness)\n. ./env/bin/activate\n```\nInstall this package from PyPI via ```pip install galaxywitness```\n\n## Documentation\nYou can find our technical documentation here: [Docs](https://galaxywitness.rtfd.io)\n### For developers\n[Sphinx](https://www.sphinx-doc.org/en/master/index.html) generates documentation for delelopers from sources in <code>./docs</code> folder. HTML files of documentation are in <code>./docs/build/html</code> and you can open it with browser. \nIf you want to build documentation yourself:\n```sh\ncd docs\nmake html\n```\nor if you want to get .pdf with documentation:\n```sh\ncd docs\nmake latexpdf\n```\n\n## Usage\nTo run just type:\n```sh   \npython -m galaxywitness\n```\n\nIn runtime the program will request you to choose file with your data. This file have to be in folder ```./data```\n\nIf you want to finish a work with package and deactivate virtual environment just type:\n```sh\ndeactivate\n```\n\n## Development\nYou can use python virtual environment and install dependencies manually:\n### Create and activate a virtual environment\nThis will create a new virtual environment called "galaxy-witness":\n```sh\npip3 install virtualenv\nvirtualenv galaxy-witness (or python3 -m virtualenv galaxy-witness)\n. ./galaxy-witness/bin/activate\n``` \nThis will clone the repository "GalaxyWitness" on your local machine, install dependencies and install this package \'galaxywitness\':\n```sh\ngit clone https://github.com/davidosx/GalaxyWitness\ncd GalaxyWitness\npip install -r requirements.txt\npython setup.py install\n```\n\nOr poetry package manager:\n### Poetry\n```sh\ngit clone https://github.com/davidosx/GalaxyWitness\ncd GalaxyWitness\npoetry install\n```\n\n### Uninstalling\nFor uninstalling (include dependencies and an virtual environment):\n```sh\nrm -r GalaxyWitness\nrm -r galaxy-witness\n```\n\n\n',
-    'author': 'David Miheev',
-    'author_email': 'me@davidkorol.life',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8',
-}
-
-
-setup(**setup_kwargs)
```

