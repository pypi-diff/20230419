# Comparing `tmp/seeq_sysid-1.0.0.tar.gz` & `tmp/seeq_sysid-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seeq_sysid-1.0.0.tar", last modified: Wed Apr  5 16:48:04 2023, max compression
+gzip compressed data, was "seeq_sysid-1.0.1.tar", last modified: Wed Apr 19 15:55:10 2023, max compression
```

## Comparing `seeq_sysid-1.0.0.tar` & `seeq_sysid-1.0.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-04-05 16:48:04.297958 seeq_sysid-1.0.0/
--rw-rw-rw-   0        0        0     1087 2022-10-24 16:43:04.000000 seeq_sysid-1.0.0/LICENSE
--rw-rw-rw-   0        0        0       89 2022-10-24 16:43:04.000000 seeq_sysid-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0    16554 2023-04-05 16:48:04.282323 seeq_sysid-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0    13648 2023-04-05 16:35:41.000000 seeq_sysid-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-05 16:48:04.078334 seeq_sysid-1.0.0/seeq_sysid/
--rw-rw-rw-   0        0        0      114 2023-01-09 17:22:49.000000 seeq_sysid-1.0.0/seeq_sysid/__init__.py
--rw-rw-rw-   0        0        0     7551 2022-06-27 15:42:04.000000 seeq_sysid-1.0.0/seeq_sysid/__main__.py
--rw-rw-rw-   0        0        0     3750 2022-05-27 14:57:21.000000 seeq_sysid-1.0.0/seeq_sysid/_copy.py
--rw-rw-rw-   0        0        0       21 2023-04-03 16:29:28.000000 seeq_sysid-1.0.0/seeq_sysid/_version.py
--rw-rw-rw-   0        0        0    12024 2023-04-03 16:28:24.000000 seeq_sysid-1.0.0/seeq_sysid/app.py
-drwxrwxrwx   0        0        0        0 2023-04-05 16:48:04.109572 seeq_sysid-1.0.0/seeq_sysid/deployment_notebook/
--rw-rw-rw-   0        0        0     2145 2023-01-09 17:21:37.000000 seeq_sysid-1.0.0/seeq_sysid/deployment_notebook/sysid_notebook.ipynb
-drwxrwxrwx   0        0        0        0 2023-04-05 16:48:04.251062 seeq_sysid-1.0.0/seeq_sysid/gui/
--rw-rw-rw-   0        0        0      439 2022-05-27 14:57:21.000000 seeq_sysid-1.0.0/seeq_sysid/gui/__init__.py
--rw-rw-rw-   0        0        0     4850 2023-03-31 16:18:03.000000 seeq_sysid-1.0.0/seeq_sysid/gui/_backend.py
--rw-rw-rw-   0        0        0    11728 2023-03-14 10:30:21.000000 seeq_sysid-1.0.0/seeq_sysid/gui/app_bar.py
--rw-rw-rw-   0        0        0    28418 2023-03-13 13:55:23.000000 seeq_sysid-1.0.0/seeq_sysid/gui/app_sheet.py
--rw-rw-rw-   0        0        0     3665 2022-11-18 11:52:04.000000 seeq_sysid-1.0.0/seeq_sysid/gui/data_editor.py
--rw-rw-rw-   0        0        0     5331 2022-12-12 12:25:50.000000 seeq_sysid-1.0.0/seeq_sysid/gui/figure_card.py
--rw-rw-rw-   0        0        0     2240 2022-12-12 13:02:04.000000 seeq_sysid-1.0.0/seeq_sysid/gui/figure_table.py
--rw-rw-rw-   0        0        0    37361 2022-12-12 12:24:53.000000 seeq_sysid-1.0.0/seeq_sysid/gui/panels.py
--rw-rw-rw-   0        0        0     7542 2023-03-10 16:31:19.000000 seeq_sysid-1.0.0/seeq_sysid/gui/setup.py
--rw-rw-rw-   0        0        0     6477 2022-11-07 15:45:50.000000 seeq_sysid-1.0.0/seeq_sysid/gui/table_card.py
--rw-rw-rw-   0        0        0     3823 2023-02-12 16:20:31.000000 seeq_sysid-1.0.0/seeq_sysid/gui/transfer_card_result.py
--rw-rw-rw-   0        0        0     7696 2023-02-12 18:11:00.000000 seeq_sysid-1.0.0/seeq_sysid/gui/transfer_card_setup.py
--rw-rw-rw-   0        0        0    21431 2022-05-27 14:57:21.000000 seeq_sysid-1.0.0/seeq_sysid/gui/transfer_chip.py
--rw-rw-rw-   0        0        0    15235 2023-03-13 16:17:55.000000 seeq_sysid-1.0.0/seeq_sysid/gui/transfer_matrix.py
--rw-rw-rw-   0        0        0      619 2022-02-12 10:16:55.000000 seeq_sysid-1.0.0/seeq_sysid/gui/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-05 16:48:04.282323 seeq_sysid-1.0.0/seeq_sysid/model/
--rw-rw-rw-   0        0        0      141 2022-01-27 13:43:16.000000 seeq_sysid-1.0.0/seeq_sysid/model/__init__.py
--rw-rw-rw-   0        0        0    19633 2023-03-21 21:44:39.000000 seeq_sysid-1.0.0/seeq_sysid/model/arx.py
--rw-rw-rw-   0        0        0     1088 2022-05-27 14:57:21.000000 seeq_sysid-1.0.0/seeq_sysid/model/base.py
--rw-rw-rw-   0        0        0     6590 2023-04-05 15:29:31.000000 seeq_sysid-1.0.0/seeq_sysid/model/nn.py
--rw-rw-rw-   0        0        0     5472 2022-11-28 13:52:04.000000 seeq_sysid-1.0.0/seeq_sysid/model/ss.py
--rw-rw-rw-   0        0        0    10726 2023-03-21 21:44:50.000000 seeq_sysid-1.0.0/seeq_sysid/model/tf.py
--rw-rw-rw-   0        0        0    14204 2023-03-15 14:18:53.000000 seeq_sysid-1.0.0/seeq_sysid/model/tf_item.py
--rw-rw-rw-   0        0        0     1769 2023-03-21 21:45:21.000000 seeq_sysid-1.0.0/seeq_sysid/model/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-05 16:48:04.109572 seeq_sysid-1.0.0/seeq_sysid.egg-info/
--rw-rw-rw-   0        0        0    16554 2023-04-05 16:48:03.000000 seeq_sysid-1.0.0/seeq_sysid.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1011 2023-04-05 16:48:03.000000 seeq_sysid-1.0.0/seeq_sysid.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-05 16:48:03.000000 seeq_sysid-1.0.0/seeq_sysid.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      144 2023-04-05 16:48:03.000000 seeq_sysid-1.0.0/seeq_sysid.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-05 16:48:03.000000 seeq_sysid-1.0.0/seeq_sysid.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-05 16:48:04.297958 seeq_sysid-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1160 2023-04-03 16:46:56.000000 seeq_sysid-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 15:55:10.831762 seeq_sysid-1.0.1/
+-rw-rw-rw-   0        0        0     1087 2022-10-24 16:43:04.000000 seeq_sysid-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0       89 2022-10-24 16:43:04.000000 seeq_sysid-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    16627 2023-04-19 15:55:10.831762 seeq_sysid-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0    13705 2023-04-19 15:33:37.000000 seeq_sysid-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 15:55:10.784903 seeq_sysid-1.0.1/seeq_sysid/
+-rw-rw-rw-   0        0        0      114 2023-01-09 17:22:49.000000 seeq_sysid-1.0.1/seeq_sysid/__init__.py
+-rw-rw-rw-   0        0        0     7535 2023-04-19 15:24:52.000000 seeq_sysid-1.0.1/seeq_sysid/__main__.py
+-rw-rw-rw-   0        0        0     3750 2022-05-27 14:57:21.000000 seeq_sysid-1.0.1/seeq_sysid/_copy.py
+-rw-rw-rw-   0        0        0       23 2023-04-19 15:54:16.000000 seeq_sysid-1.0.1/seeq_sysid/_version.py
+-rw-rw-rw-   0        0        0    12024 2023-04-03 16:28:24.000000 seeq_sysid-1.0.1/seeq_sysid/app.py
+drwxrwxrwx   0        0        0        0 2023-04-19 15:55:10.800511 seeq_sysid-1.0.1/seeq_sysid/deployment_notebook/
+-rw-rw-rw-   0        0        0     2145 2023-01-09 17:21:37.000000 seeq_sysid-1.0.1/seeq_sysid/deployment_notebook/sysid_notebook.ipynb
+drwxrwxrwx   0        0        0        0 2023-04-19 15:55:10.831762 seeq_sysid-1.0.1/seeq_sysid/gui/
+-rw-rw-rw-   0        0        0      439 2022-05-27 14:57:21.000000 seeq_sysid-1.0.1/seeq_sysid/gui/__init__.py
+-rw-rw-rw-   0        0        0     4850 2023-03-31 16:18:03.000000 seeq_sysid-1.0.1/seeq_sysid/gui/_backend.py
+-rw-rw-rw-   0        0        0    11728 2023-03-14 10:30:21.000000 seeq_sysid-1.0.1/seeq_sysid/gui/app_bar.py
+-rw-rw-rw-   0        0        0    28418 2023-03-13 13:55:23.000000 seeq_sysid-1.0.1/seeq_sysid/gui/app_sheet.py
+-rw-rw-rw-   0        0        0     3665 2022-11-18 11:52:04.000000 seeq_sysid-1.0.1/seeq_sysid/gui/data_editor.py
+-rw-rw-rw-   0        0        0     5331 2022-12-12 12:25:50.000000 seeq_sysid-1.0.1/seeq_sysid/gui/figure_card.py
+-rw-rw-rw-   0        0        0     2240 2022-12-12 13:02:04.000000 seeq_sysid-1.0.1/seeq_sysid/gui/figure_table.py
+-rw-rw-rw-   0        0        0    37361 2022-12-12 12:24:53.000000 seeq_sysid-1.0.1/seeq_sysid/gui/panels.py
+-rw-rw-rw-   0        0        0     7542 2023-03-10 16:31:19.000000 seeq_sysid-1.0.1/seeq_sysid/gui/setup.py
+-rw-rw-rw-   0        0        0     6477 2022-11-07 15:45:50.000000 seeq_sysid-1.0.1/seeq_sysid/gui/table_card.py
+-rw-rw-rw-   0        0        0     3823 2023-02-12 16:20:31.000000 seeq_sysid-1.0.1/seeq_sysid/gui/transfer_card_result.py
+-rw-rw-rw-   0        0        0     7696 2023-02-12 18:11:00.000000 seeq_sysid-1.0.1/seeq_sysid/gui/transfer_card_setup.py
+-rw-rw-rw-   0        0        0    21431 2022-05-27 14:57:21.000000 seeq_sysid-1.0.1/seeq_sysid/gui/transfer_chip.py
+-rw-rw-rw-   0        0        0    15235 2023-03-13 16:17:55.000000 seeq_sysid-1.0.1/seeq_sysid/gui/transfer_matrix.py
+-rw-rw-rw-   0        0        0      619 2022-02-12 10:16:55.000000 seeq_sysid-1.0.1/seeq_sysid/gui/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-19 15:55:10.831762 seeq_sysid-1.0.1/seeq_sysid/model/
+-rw-rw-rw-   0        0        0      141 2022-01-27 13:43:16.000000 seeq_sysid-1.0.1/seeq_sysid/model/__init__.py
+-rw-rw-rw-   0        0        0    19633 2023-03-21 21:44:39.000000 seeq_sysid-1.0.1/seeq_sysid/model/arx.py
+-rw-rw-rw-   0        0        0     1088 2022-05-27 14:57:21.000000 seeq_sysid-1.0.1/seeq_sysid/model/base.py
+-rw-rw-rw-   0        0        0     6590 2023-04-05 15:29:31.000000 seeq_sysid-1.0.1/seeq_sysid/model/nn.py
+-rw-rw-rw-   0        0        0     5472 2022-11-28 13:52:04.000000 seeq_sysid-1.0.1/seeq_sysid/model/ss.py
+-rw-rw-rw-   0        0        0    10726 2023-03-21 21:44:50.000000 seeq_sysid-1.0.1/seeq_sysid/model/tf.py
+-rw-rw-rw-   0        0        0    14206 2023-04-19 14:51:05.000000 seeq_sysid-1.0.1/seeq_sysid/model/tf_item.py
+-rw-rw-rw-   0        0        0     1769 2023-03-21 21:45:21.000000 seeq_sysid-1.0.1/seeq_sysid/model/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-19 15:55:10.800511 seeq_sysid-1.0.1/seeq_sysid.egg-info/
+-rw-rw-rw-   0        0        0    16627 2023-04-19 15:55:10.000000 seeq_sysid-1.0.1/seeq_sysid.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1011 2023-04-19 15:55:10.000000 seeq_sysid-1.0.1/seeq_sysid.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 15:55:10.000000 seeq_sysid-1.0.1/seeq_sysid.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      152 2023-04-19 15:55:10.000000 seeq_sysid-1.0.1/seeq_sysid.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-19 15:55:10.000000 seeq_sysid-1.0.1/seeq_sysid.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 15:55:10.831762 seeq_sysid-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1168 2023-04-19 15:37:22.000000 seeq_sysid-1.0.1/setup.py
```

### Comparing `seeq_sysid-1.0.0/LICENSE` & `seeq_sysid-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `seeq_sysid-1.0.0/PKG-INFO` & `seeq_sysid-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seeq_sysid
-Version: 1.0.0
+Version: 1.0.1
 Summary: Seeq System Identification Addon
 Home-page: https://github.com/BYU-PRISM/Seeq
 Author: Junho Park, Mohammad Reza Babaei
 Author-email: jnho.park@gmail.com, babaei_mr@outlook.com
 License: MIT
 Description: <!-- workflow badges -->
         [![CodeQL](https://github.com/BYU-PRISM/Seeq/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/BYU-PRISM/Seeq/actions/workflows/codeql-analysis.yml)
@@ -205,14 +205,17 @@
         This notebook can also be used while debugging from your IDE. You can also
         create a whl first, install it on your virtual environment, and then
         run `developer_notebook.ipynb` notebook there.
         
         
         # Changelog
         
+        ## v1.0.1
+        - Notebook extensions and requirements update
+        
         ## v1.0.0
         - Minor improvements
         - Empty worksheet warning
         - Performance improvements
         
         ## v0.7.1
         - Hotfix: dependencies updated for R57>=
@@ -274,32 +277,31 @@
         ## v0.0.7
         
         - Neural Network Model (RNN) added
         - FIR Model added
         
         ## v0.0.6
         
-        - Installation made easier.
-        
+        - Installation made easier
         - N4SID method was removed temporarily.
         
         
         
         # Support
         
-        Code related issues (e.g. bugs, feature requests) can be created in the
+        Code-related issues (e.g. bugs, feature requests) can be created in the
         [issue tracker](https://github.com/BYU-PRISM/Seeq/issues)
         
         
         # Citation
         
         Please cite this work as:
         
         ```shell
-        seeq-sysid v0.6.1
+        seeq-sysid v1.0.1
         BYU PRISM Group https://apm.byu.edu/prism/
         https://github.com/BYU-PRISM/Seeq
         ```
         
 Keywords: Seeq Prism System Identification ARX FIR ARIMAX Subspace State-Space Neural-Network Addon Time-Series Transfer Function
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `seeq_sysid-1.0.0/README.md` & `seeq_sysid-1.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -197,14 +197,17 @@
 This notebook can also be used while debugging from your IDE. You can also
 create a whl first, install it on your virtual environment, and then
 run `developer_notebook.ipynb` notebook there.
 
 
 # Changelog
 
+## v1.0.1
+- Notebook extensions and requirements update
+
 ## v1.0.0
 - Minor improvements
 - Empty worksheet warning
 - Performance improvements
 
 ## v0.7.1
 - Hotfix: dependencies updated for R57>=
@@ -266,28 +269,27 @@
 ## v0.0.7
 
 - Neural Network Model (RNN) added
 - FIR Model added
 
 ## v0.0.6
 
-- Installation made easier.
-
+- Installation made easier
 - N4SID method was removed temporarily.
 
 
 
 # Support
 
-Code related issues (e.g. bugs, feature requests) can be created in the
+Code-related issues (e.g. bugs, feature requests) can be created in the
 [issue tracker](https://github.com/BYU-PRISM/Seeq/issues)
 
 
 # Citation
 
 Please cite this work as:
 
 ```shell
-seeq-sysid v0.6.1
+seeq-sysid v1.0.1
 BYU PRISM Group https://apm.byu.edu/prism/
 https://github.com/BYU-PRISM/Seeq
 ```
```

### Comparing `seeq_sysid-1.0.0/seeq_sysid/__main__.py` & `seeq_sysid-1.0.1/seeq_sysid/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from urllib.parse import urlparse
 from seeq import sdk, spy
 
 from seeq.spy import _url
 from ._copy import copy
 import seeq
 
-NB_EXTENSIONS = ['widgetsnbextension', 'plotlywidget', 'ipyvuetify', 'ipyvue']
+NB_EXTENSIONS = ['widgetsnbextension', 'ipyvuetify', 'ipyvue']
 DEPLOYMENT_FOLDER = 'deployment'
 SYSID_NOTEBOOK = "sysid_notebook.ipynb"
 DEFAULT_GROUP = ['Everyone']
 DEFAULT_USERS = []
 
 
 def install_app(sdl_url_, *, sort_key='a', permissions_group: list = None, permissions_users: list = None):
```

### Comparing `seeq_sysid-1.0.0/seeq_sysid/_copy.py` & `seeq_sysid-1.0.1/seeq_sysid/_copy.py`

 * *Files identical despite different names*

### Comparing `seeq_sysid-1.0.0/seeq_sysid/app.py` & `seeq_sysid-1.0.1/seeq_sysid/app.py`

 * *Files identical despite different names*

### Comparing `seeq_sysid-1.0.0/seeq_sysid/deployment_notebook/sysid_notebook.ipynb` & `seeq_sysid-1.0.1/seeq_sysid/deployment_notebook/sysid_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `seeq_sysid-1.0.0/seeq_sysid/gui/_backend.py` & `seeq_sysid-1.0.1/seeq_sysid/gui/_backend.py`

 * *Files identical despite different names*

### Comparing `seeq_sysid-1.0.0/seeq_sysid/gui/app_bar.py` & `seeq_sysid-1.0.1/seeq_sysid/gui/app_bar.py`

 * *Files identical despite different names*

### Comparing `seeq_sysid-1.0.0/seeq_sysid/gui/app_sheet.py` & `seeq_sysid-1.0.1/seeq_sysid/gui/app_sheet.py`

 * *Files identical despite different names*

### Comparing `seeq_sysid-1.0.0/seeq_sysid/gui/data_editor.py` & `seeq_sysid-1.0.1/seeq_sysid/gui/data_editor.py`

 * *Files identical despite different names*

### Comparing `seeq_sysid-1.0.0/seeq_sysid/gui/figure_card.py` & `seeq_sysid-1.0.1/seeq_sysid/gui/figure_card.py`

 * *Files identical despite different names*

### Comparing `seeq_sysid-1.0.0/seeq_sysid/gui/figure_table.py` & `seeq_sysid-1.0.1/seeq_sysid/gui/figure_table.py`

 * *Files identical despite different names*

### Comparing `seeq_sysid-1.0.0/seeq_sysid/gui/panels.py` & `seeq_sysid-1.0.1/seeq_sysid/gui/panels.py`

 * *Files identical despite different names*

### Comparing `seeq_sysid-1.0.0/seeq_sysid/gui/setup.py` & `seeq_sysid-1.0.1/seeq_sysid/gui/setup.py`

 * *Files identical despite different names*

### Comparing `seeq_sysid-1.0.0/seeq_sysid/gui/table_card.py` & `seeq_sysid-1.0.1/seeq_sysid/gui/table_card.py`

 * *Files identical despite different names*

### Comparing `seeq_sysid-1.0.0/seeq_sysid/gui/transfer_card_result.py` & `seeq_sysid-1.0.1/seeq_sysid/gui/transfer_card_result.py`

 * *Files identical despite different names*

### Comparing `seeq_sysid-1.0.0/seeq_sysid/gui/transfer_card_setup.py` & `seeq_sysid-1.0.1/seeq_sysid/gui/transfer_card_setup.py`

 * *Files identical despite different names*

### Comparing `seeq_sysid-1.0.0/seeq_sysid/gui/transfer_chip.py` & `seeq_sysid-1.0.1/seeq_sysid/gui/transfer_chip.py`

 * *Files identical despite different names*

### Comparing `seeq_sysid-1.0.0/seeq_sysid/gui/transfer_matrix.py` & `seeq_sysid-1.0.1/seeq_sysid/gui/transfer_matrix.py`

 * *Files identical despite different names*

### Comparing `seeq_sysid-1.0.0/seeq_sysid/gui/utils.py` & `seeq_sysid-1.0.1/seeq_sysid/gui/utils.py`

 * *Files identical despite different names*

### Comparing `seeq_sysid-1.0.0/seeq_sysid/model/arx.py` & `seeq_sysid-1.0.1/seeq_sysid/model/arx.py`

 * *Files identical despite different names*

### Comparing `seeq_sysid-1.0.0/seeq_sysid/model/base.py` & `seeq_sysid-1.0.1/seeq_sysid/model/base.py`

 * *Files identical despite different names*

### Comparing `seeq_sysid-1.0.0/seeq_sysid/model/nn.py` & `seeq_sysid-1.0.1/seeq_sysid/model/nn.py`

 * *Files identical despite different names*

### Comparing `seeq_sysid-1.0.0/seeq_sysid/model/ss.py` & `seeq_sysid-1.0.1/seeq_sysid/model/ss.py`

 * *Files identical despite different names*

### Comparing `seeq_sysid-1.0.0/seeq_sysid/model/tf.py` & `seeq_sysid-1.0.1/seeq_sysid/model/tf.py`

 * *Files identical despite different names*

### Comparing `seeq_sysid-1.0.0/seeq_sysid/model/tf_item.py` & `seeq_sysid-1.0.1/seeq_sysid/model/tf_item.py`

 * *Files 0% similar despite different names*

```diff
@@ -318,15 +318,15 @@
 
         self.ym[0].value = y[0]
         # self.ym[0].fstatus = 1
         self.ym[0].status = 0
 
         self.options.Solver = 3
         self.options.IMODE = 5
-        self.options.MAX_TIME = 120
+        self.options.MAX_TIME = 1800
         self.solve(disp=False)
 
         self.label = [tag_label + '_tf' for tag_label in y_df.columns]
         
         # save optimal values
         for (i, mv_i) in enumerate(self.mv):
             option_item: TransferOption = self.option_dict[mv_i]
@@ -432,11 +432,11 @@
             self.cspline(self.tc[i], self.um[i], self.t, u[i], bound_x=True)
 
         self.tt.value = t
         self.ym[0].value = 0
         self.ym[0].status = 1
 
         self.options.IMODE = 5
-        self.options.MAX_TIME = 120
+        self.options.MAX_TIME = 1800
         self.solve(disp=False)
 
         return self.ym.copy()
```

### Comparing `seeq_sysid-1.0.0/seeq_sysid/model/utils.py` & `seeq_sysid-1.0.1/seeq_sysid/model/utils.py`

 * *Files identical despite different names*

### Comparing `seeq_sysid-1.0.0/seeq_sysid.egg-info/PKG-INFO` & `seeq_sysid-1.0.1/seeq_sysid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seeq-sysid
-Version: 1.0.0
+Version: 1.0.1
 Summary: Seeq System Identification Addon
 Home-page: https://github.com/BYU-PRISM/Seeq
 Author: Junho Park, Mohammad Reza Babaei
 Author-email: jnho.park@gmail.com, babaei_mr@outlook.com
 License: MIT
 Description: <!-- workflow badges -->
         [![CodeQL](https://github.com/BYU-PRISM/Seeq/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/BYU-PRISM/Seeq/actions/workflows/codeql-analysis.yml)
@@ -205,14 +205,17 @@
         This notebook can also be used while debugging from your IDE. You can also
         create a whl first, install it on your virtual environment, and then
         run `developer_notebook.ipynb` notebook there.
         
         
         # Changelog
         
+        ## v1.0.1
+        - Notebook extensions and requirements update
+        
         ## v1.0.0
         - Minor improvements
         - Empty worksheet warning
         - Performance improvements
         
         ## v0.7.1
         - Hotfix: dependencies updated for R57>=
@@ -274,32 +277,31 @@
         ## v0.0.7
         
         - Neural Network Model (RNN) added
         - FIR Model added
         
         ## v0.0.6
         
-        - Installation made easier.
-        
+        - Installation made easier
         - N4SID method was removed temporarily.
         
         
         
         # Support
         
-        Code related issues (e.g. bugs, feature requests) can be created in the
+        Code-related issues (e.g. bugs, feature requests) can be created in the
         [issue tracker](https://github.com/BYU-PRISM/Seeq/issues)
         
         
         # Citation
         
         Please cite this work as:
         
         ```shell
-        seeq-sysid v0.6.1
+        seeq-sysid v1.0.1
         BYU PRISM Group https://apm.byu.edu/prism/
         https://github.com/BYU-PRISM/Seeq
         ```
         
 Keywords: Seeq Prism System Identification ARX FIR ARIMAX Subspace State-Space Neural-Network Addon Time-Series Transfer Function
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `seeq_sysid-1.0.0/seeq_sysid.egg-info/SOURCES.txt` & `seeq_sysid-1.0.1/seeq_sysid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seeq_sysid-1.0.0/setup.py` & `seeq_sysid-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from setuptools import setup, find_packages
 
 with open(file='README.md', mode='r') as readme_handle:
     long_description = readme_handle.read()
 
 setup(
     name='seeq_sysid',
-    version='1.0.0',
+    version='1.0.1',
     packages=find_packages(),
     url='https://github.com/BYU-PRISM/Seeq',
     license='MIT',
     author='Junho Park, Mohammad Reza Babaei',
     author_email='jnho.park@gmail.com, babaei_mr@outlook.com',
     description='Seeq System Identification Addon',
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
 	  'ipyvuetify>=1.5.1',
 	  'gekko>=1.0.6',
 	  'numpy',
-	  'pandas>=1.2.1',
-	  'plotly>=4.5.0',
+	  'pandas<2.0.0,>=1.2.1',
+	  'plotly>=5.10.0',
         'python-dateutil>=2.8.1',
 	  'tensorflow>=2.5',
 	  'keras-tuner==1.0.4',
 	  'scipy',
 	  'protobuf~=3.20',
     ],
     keywords='Seeq Prism System Identification ARX FIR ARIMAX Subspace State-Space Neural-Network Addon Time-Series Transfer Function',
```

