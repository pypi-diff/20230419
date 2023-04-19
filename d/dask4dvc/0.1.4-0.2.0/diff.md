# Comparing `tmp/dask4dvc-0.1.4.tar.gz` & `tmp/dask4dvc-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dask4dvc-0.1.4.tar", max compression
+gzip compressed data, was "dask4dvc-0.2.0.tar", max compression
```

## Comparing `dask4dvc-0.1.4.tar` & `dask4dvc-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,12 @@
--rw-r--r--   0        0        0    13576 2023-01-25 13:10:23.183284 dask4dvc-0.1.4/LICENSE
--rw-r--r--   0        0        0     1456 2023-04-13 11:02:16.857294 dask4dvc-0.1.4/README.md
--rw-r--r--   0        0        0      521 2023-01-25 13:44:53.309679 dask4dvc-0.1.4/dask4dvc/__init__.py
--rw-r--r--   0        0        0       76 2023-01-25 13:44:53.309679 dask4dvc-0.1.4/dask4dvc/cli/__init__.py
--rw-r--r--   0        0        0     6243 2023-04-18 15:37:16.965339 dask4dvc-0.1.4/dask4dvc/cli/main.py
--rw-r--r--   0        0        0     4447 2023-04-18 15:37:16.965339 dask4dvc-0.1.4/dask4dvc/methods.py
--rw-r--r--   0        0        0      166 2023-01-25 13:44:53.309679 dask4dvc-0.1.4/dask4dvc/utils/__init__.py
--rw-r--r--   0        0        0      413 2023-01-25 13:44:53.309679 dask4dvc-0.1.4/dask4dvc/utils/config.py
--rw-r--r--   0        0        0     1055 2023-04-13 11:02:16.867293 dask4dvc-0.1.4/dask4dvc/utils/dask.py
--rw-r--r--   0        0        0     5807 2023-04-18 13:10:44.129812 dask4dvc-0.1.4/dask4dvc/utils/dvc.py
--rw-r--r--   0        0        0      951 2023-01-25 13:44:53.309679 dask4dvc-0.1.4/dask4dvc/utils/git.py
--rw-r--r--   0        0        0      903 2023-04-13 12:46:43.228695 dask4dvc-0.1.4/dask4dvc/utils/main.py
--rw-r--r--   0        0        0     1290 2023-04-18 15:37:16.975339 dask4dvc-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2395 1970-01-01 00:00:00.000000 dask4dvc-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    13576 2023-01-25 13:10:23.183284 dask4dvc-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1637 2023-04-19 15:36:27.742838 dask4dvc-0.2.0/README.md
+-rw-r--r--   0        0        0      651 2023-04-19 15:02:16.124501 dask4dvc-0.2.0/dask4dvc/__init__.py
+-rw-r--r--   0        0        0       76 2023-01-25 13:44:53.309679 dask4dvc-0.2.0/dask4dvc/cli/__init__.py
+-rw-r--r--   0        0        0     2608 2023-04-19 15:36:27.742838 dask4dvc-0.2.0/dask4dvc/cli/main.py
+-rw-r--r--   0        0        0     3393 2023-04-19 15:36:27.742838 dask4dvc-0.2.0/dask4dvc/methods.py
+-rw-r--r--   0        0        0      142 2023-04-19 15:36:27.742838 dask4dvc-0.2.0/dask4dvc/utils/__init__.py
+-rw-r--r--   0        0        0      272 2023-04-19 15:36:27.742838 dask4dvc-0.2.0/dask4dvc/utils/config.py
+-rw-r--r--   0        0        0     1055 2023-04-13 11:02:16.867293 dask4dvc-0.2.0/dask4dvc/utils/dask.py
+-rw-r--r--   0        0        0      136 2023-04-19 15:36:27.742838 dask4dvc-0.2.0/dask4dvc/utils/main.py
+-rw-r--r--   0        0        0     1271 2023-04-19 15:36:27.742838 dask4dvc-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2536 1970-01-01 00:00:00.000000 dask4dvc-0.2.0/PKG-INFO
```

### Comparing `dask4dvc-0.1.4/LICENSE` & `dask4dvc-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dask4dvc-0.1.4/README.md` & `dask4dvc-0.2.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -3,19 +3,20 @@
 [![PyPI version](https://badge.fury.io/py/dask4dvc.svg)](https://badge.fury.io/py/dask4dvc)
 [![zincware](https://img.shields.io/badge/Powered%20by-zincware-darkcyan)](https://github.com/zincware)
 
 # Dask4DVC - Distributed Node Exectuion
 [DVC](dvc.org) provides tools for building and executing the computational graph locally through various methods. 
 The `dask4dvc` package combines [Dask Distributed](https://distributed.dask.org/) with DVC to make it easier to use with HPC managers like [Slurm](https://github.com/SchedMD/slurm).
 
+The `dask4dvc` package will try to run the DVC graph in parallel.
+
 ## Usage
 Dask4DVC provides a CLI similar to DVC.
 
 - `dvc repro` becomes `dask4dvc repro`.
-- `dvc exp run --run-all` becomes `dask4dvc run`.
 
 ### SLURM Cluster
 
 You can use `dask4dvc` easily with a slurm cluster.
 This requires a running dask scheduler:
 ```python
 from dask_jobqueue import SLURMCluster
@@ -29,7 +30,17 @@
     job_extra=['-N 1', '--cpus-per-task=1', '--tasks-per-node=64', "--gres=gpu:1"],
     scheduler_options={"port": 31415}
 )
 cluster.adapt()
 ```
 
 with this setup you can then run `dask4dvc repro --address 127.0.0.1:31415` on the example port `31415`.
+
+You can also use config files with `dask4dvc repro --config myconfig.yaml`.
+
+```yaml
+default:
+  SGECluster:
+    queue: regular
+    cores: 10
+    memory: 16 GB
+```
```

### Comparing `dask4dvc-0.1.4/dask4dvc/utils/dask.py` & `dask4dvc-0.2.0/dask4dvc/utils/dask.py`

 * *Files identical despite different names*

### Comparing `dask4dvc-0.1.4/pyproject.toml` & `dask4dvc-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 [tool.poetry]
 name = "dask4dvc"
-version = "0.1.4"
+version = "0.2.0"
 description = "Use dask to run the DVC graph"
 authors = ["zincwarecode <zincwarecode@gmail.com>"]
 license = "Apache-2.0"
 keywords=["data-science", "HPC", "dask", "DVC"]
 readme = "README.md"
 
 [tool.poetry.urls]
 repository = "https://github.com/zincware/dask4dvc"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 dask = "^2022.7.1"
 distributed = "^2022.7.1"
 dask-jobqueue = "^0.8.1"
-dvc = "^2.34.3"
+dvc = "^2.54.0"
 typer = {extras = ["all"], version = "^0.7.0"}
 bokeh = "^2"
 # for bokeh see https://distributed.dask.org/en/stable/changelog.html#v2022-11-1
-znflow = "^0.1.11"
 
 [tool.poetry.scripts]
 dask4dvc = 'dask4dvc.cli.main:app'
 
 [tool.poetry.group.dev.dependencies]
 jupyterlab = "^3.4.4"
 black = "^22.6.0"
```

### Comparing `dask4dvc-0.1.4/PKG-INFO` & `dask4dvc-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask4dvc
-Version: 0.1.4
+Version: 0.2.0
 Summary: Use dask to run the DVC graph
 License: Apache-2.0
 Keywords: data-science,HPC,dask,DVC
 Author: zincwarecode
 Author-email: zincwarecode@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -13,34 +13,34 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: bokeh (>=2,<3)
 Requires-Dist: dask (>=2022.7.1,<2023.0.0)
 Requires-Dist: dask-jobqueue (>=0.8.1,<0.9.0)
 Requires-Dist: distributed (>=2022.7.1,<2023.0.0)
-Requires-Dist: dvc (>=2.34.3,<3.0.0)
+Requires-Dist: dvc (>=2.54.0,<3.0.0)
 Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
-Requires-Dist: znflow (>=0.1.11,<0.2.0)
 Project-URL: repository, https://github.com/zincware/dask4dvc
 Description-Content-Type: text/markdown
 
 [![Coverage Status](https://coveralls.io/repos/github/zincware/dask4dvc/badge.svg?branch=main)](https://coveralls.io/github/zincware/dask4dvc?branch=main)
 ![PyTest](https://github.com/zincware/dask4dvc/actions/workflows/pytest.yaml/badge.svg)
 [![PyPI version](https://badge.fury.io/py/dask4dvc.svg)](https://badge.fury.io/py/dask4dvc)
 [![zincware](https://img.shields.io/badge/Powered%20by-zincware-darkcyan)](https://github.com/zincware)
 
 # Dask4DVC - Distributed Node Exectuion
 [DVC](dvc.org) provides tools for building and executing the computational graph locally through various methods. 
 The `dask4dvc` package combines [Dask Distributed](https://distributed.dask.org/) with DVC to make it easier to use with HPC managers like [Slurm](https://github.com/SchedMD/slurm).
 
+The `dask4dvc` package will try to run the DVC graph in parallel.
+
 ## Usage
 Dask4DVC provides a CLI similar to DVC.
 
 - `dvc repro` becomes `dask4dvc repro`.
-- `dvc exp run --run-all` becomes `dask4dvc run`.
 
 ### SLURM Cluster
 
 You can use `dask4dvc` easily with a slurm cluster.
 This requires a running dask scheduler:
 ```python
 from dask_jobqueue import SLURMCluster
@@ -55,7 +55,17 @@
     scheduler_options={"port": 31415}
 )
 cluster.adapt()
 ```
 
 with this setup you can then run `dask4dvc repro --address 127.0.0.1:31415` on the example port `31415`.
 
+You can also use config files with `dask4dvc repro --config myconfig.yaml`.
+
+```yaml
+default:
+  SGECluster:
+    queue: regular
+    cores: 10
+    memory: 16 GB
+```
+
```

