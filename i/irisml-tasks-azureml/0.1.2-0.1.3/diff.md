# Comparing `tmp/irisml-tasks-azureml-0.1.2.tar.gz` & `tmp/irisml-tasks-azureml-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irisml-tasks-azureml-0.1.2.tar", last modified: Fri Feb 17 22:34:43 2023, max compression
+gzip compressed data, was "irisml-tasks-azureml-0.1.3.tar", last modified: Wed Apr 19 07:26:46 2023, max compression
```

## Comparing `irisml-tasks-azureml-0.1.2.tar` & `irisml-tasks-azureml-0.1.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 22:34:43.068676 irisml-tasks-azureml-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-02-17 22:32:48.000000 irisml-tasks-azureml-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-02-17 22:34:43.068676 irisml-tasks-azureml-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-02-17 22:32:48.000000 irisml-tasks-azureml-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 22:34:43.064676 irisml-tasks-azureml-0.1.2/irisml/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 22:34:43.064676 irisml-tasks-azureml-0.1.2/irisml/azureml/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-02-17 22:32:48.000000 irisml-tasks-azureml-0.1.2/irisml/azureml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10282 2023-02-17 22:32:48.000000 irisml-tasks-azureml-0.1.2/irisml/azureml/azureml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 22:34:43.064676 irisml-tasks-azureml-0.1.2/irisml/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-02-17 22:32:48.000000 irisml-tasks-azureml-0.1.2/irisml/commands/cancel_aml.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-02-17 22:32:48.000000 irisml-tasks-azureml-0.1.2/irisml/commands/run_aml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 22:34:43.064676 irisml-tasks-azureml-0.1.2/irisml/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-02-17 22:32:48.000000 irisml-tasks-azureml-0.1.2/irisml/tasks/add_aml_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-02-17 22:32:48.000000 irisml-tasks-azureml-0.1.2/irisml/tasks/run_azureml_child.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 22:34:43.068676 irisml-tasks-azureml-0.1.2/irisml_tasks_azureml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-02-17 22:34:43.000000 irisml-tasks-azureml-0.1.2/irisml_tasks_azureml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-02-17 22:34:43.000000 irisml-tasks-azureml-0.1.2/irisml_tasks_azureml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-17 22:34:43.000000 irisml-tasks-azureml-0.1.2/irisml_tasks_azureml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-02-17 22:34:43.000000 irisml-tasks-azureml-0.1.2/irisml_tasks_azureml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-17 22:34:43.000000 irisml-tasks-azureml-0.1.2/irisml_tasks_azureml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-17 22:34:43.000000 irisml-tasks-azureml-0.1.2/irisml_tasks_azureml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-02-17 22:32:48.000000 irisml-tasks-azureml-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-02-17 22:34:43.068676 irisml-tasks-azureml-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 22:34:43.068676 irisml-tasks-azureml-0.1.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-02-17 22:32:48.000000 irisml-tasks-azureml-0.1.2/test/test_add_aml_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-02-17 22:32:48.000000 irisml-tasks-azureml-0.1.2/test/test_azureml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:26:46.692895 irisml-tasks-azureml-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-19 07:24:49.000000 irisml-tasks-azureml-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-04-19 07:26:46.692895 irisml-tasks-azureml-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-04-19 07:24:49.000000 irisml-tasks-azureml-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:26:46.688895 irisml-tasks-azureml-0.1.3/irisml/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:26:46.688895 irisml-tasks-azureml-0.1.3/irisml/azureml/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-19 07:24:49.000000 irisml-tasks-azureml-0.1.3/irisml/azureml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10290 2023-04-19 07:24:49.000000 irisml-tasks-azureml-0.1.3/irisml/azureml/azureml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:26:46.688895 irisml-tasks-azureml-0.1.3/irisml/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-19 07:24:49.000000 irisml-tasks-azureml-0.1.3/irisml/commands/cancel_aml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-04-19 07:24:49.000000 irisml-tasks-azureml-0.1.3/irisml/commands/run_aml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:26:46.692895 irisml-tasks-azureml-0.1.3/irisml/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-19 07:24:49.000000 irisml-tasks-azureml-0.1.3/irisml/tasks/add_aml_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-19 07:24:49.000000 irisml-tasks-azureml-0.1.3/irisml/tasks/run_azureml_child.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:26:46.692895 irisml-tasks-azureml-0.1.3/irisml_tasks_azureml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-04-19 07:26:46.000000 irisml-tasks-azureml-0.1.3/irisml_tasks_azureml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-19 07:26:46.000000 irisml-tasks-azureml-0.1.3/irisml_tasks_azureml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 07:26:46.000000 irisml-tasks-azureml-0.1.3/irisml_tasks_azureml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-19 07:26:46.000000 irisml-tasks-azureml-0.1.3/irisml_tasks_azureml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-19 07:26:46.000000 irisml-tasks-azureml-0.1.3/irisml_tasks_azureml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-19 07:26:46.000000 irisml-tasks-azureml-0.1.3/irisml_tasks_azureml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-19 07:24:49.000000 irisml-tasks-azureml-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-19 07:26:46.692895 irisml-tasks-azureml-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 07:26:46.692895 irisml-tasks-azureml-0.1.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-19 07:24:49.000000 irisml-tasks-azureml-0.1.3/test/test_add_aml_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-19 07:24:49.000000 irisml-tasks-azureml-0.1.3/test/test_azureml.py
```

### Comparing `irisml-tasks-azureml-0.1.2/LICENSE` & `irisml-tasks-azureml-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `irisml-tasks-azureml-0.1.2/PKG-INFO` & `irisml-tasks-azureml-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irisml-tasks-azureml
-Version: 0.1.2
+Version: 0.1.3
 Summary: Utility tools to use IrisML on AzureML
 Home-page: https://github.com/microsoft/irisml-tasks-azureml
 Author: irisdev
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `irisml-tasks-azureml-0.1.2/README.md` & `irisml-tasks-azureml-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `irisml-tasks-azureml-0.1.2/irisml/azureml/azureml.py` & `irisml-tasks-azureml-0.1.3/irisml/azureml/azureml.py`

 * *Files 6% similar despite different names*

```diff
@@ -167,25 +167,25 @@
         """Create a dockerfile for AML Run.
 
         We set LD_LIBRARY_PATH so that tasks can install/load those libs when needed. For example, irisml-tasks-onnx requires those cuda runtimes.
         """
         label_statement = f'LABEL build-date={datetime.date.today()}' if self._add_docker_build_date else ''
         pip_packages_str = ' '.join([f'"{p}"' for p in self._pip_packages])
         pip_option = f' --extra-index-url {self._extra_index_url}' if self._extra_index_url else ''
-        return """FROM ubuntu:20.04
-RUN apt-get update && apt-get install -y --no-install-recommends python3-pip python3-venv python3.8-dev build-essential && rm -rf /var/lib/apt/lists/*
-RUN python3.8 -m venv /opt/python
+        return """FROM ubuntu:22.04
+RUN apt-get update && apt-get install -y --no-install-recommends python3-pip python3-venv python3.10-dev build-essential && rm -rf /var/lib/apt/lists/*
+RUN python3.10 -m venv /opt/python
 ENV PATH=/opt/python/bin:$PATH
 RUN pip install --no-cache-dir -U pip
 RUN pip install --no-cache-dir setuptools wheel
 {}
 RUN pip install --no-cache-dir --timeout 120 {} {}
-ENV LD_LIBRARY_PATH=/opt/python/lib/python3.8/site-packages/nvidia/cuda_runtime/lib:/opt/python/lib/python3.8/site-packages/nvidia/cublas/lib:$LD_LIBRARY_PATH
-ENV LD_LIBRARY_PATH=/opt/python/lib/python3.8/site-packages/nvidia/cudnn/lib:/opt/python/lib/python3.8/site-packages/nvidia/curand/lib:$LD_LIBRARY_PATH
-ENV LD_LIBRARY_PATH=/opt/python/lib/python3.8/site-packages/nvidia/nvtx/lib:/opt/python/lib/python3.8/site-packages/nvidia/cufft/lib:$LD_LIBRARY_PATH
+ENV LD_LIBRARY_PATH=/opt/python/lib/python3.10/site-packages/nvidia/cuda_runtime/lib:/opt/python/lib/python3.10/site-packages/nvidia/cublas/lib:$LD_LIBRARY_PATH
+ENV LD_LIBRARY_PATH=/opt/python/lib/python3.10/site-packages/nvidia/cudnn/lib:/opt/python/lib/python3.10/site-packages/nvidia/curand/lib:$LD_LIBRARY_PATH
+ENV LD_LIBRARY_PATH=/opt/python/lib/python3.10/site-packages/nvidia/nvtx/lib:/opt/python/lib/python3.10/site-packages/nvidia/cufft/lib:$LD_LIBRARY_PATH
 """.format(label_statement, pip_packages_str, pip_option)
 
     def _add_standard_packages(self, custom_packages):
         """Add standard packages so that there are no duplicates."""
         name_pattern = re.compile(r'^[a-zA-Z0-9.\-_]*')
         package_names = [name_pattern.match(p).group(0) for p in custom_packages]
         missing_packages = set(self.STANDARD_PACKAGES) - set(package_names)
```

### Comparing `irisml-tasks-azureml-0.1.2/irisml/commands/cancel_aml.py` & `irisml-tasks-azureml-0.1.3/irisml/commands/cancel_aml.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-azureml-0.1.2/irisml/commands/run_aml.py` & `irisml-tasks-azureml-0.1.3/irisml/commands/run_aml.py`

 * *Files 11% similar despite different names*

```diff
@@ -34,14 +34,21 @@
     parser.add_argument('--base_docker_image')
     parser.add_argument('--base_docker_image_registry')
     parser.add_argument('--no_docker_build_date_label', action='store_true')
     parser.add_argument('--use_sp_on_remote', '--sp', action='store_true', help="Use Service Principal id and secret on the AML job.")
 
     args = parser.parse_args()
 
+    if not args.workspace:
+        parser.error("Workspace name is required. Please set IRISML_AML_WORKSPACE_NAME or use --workspace option.")
+    if not args.subscription_id:
+        parser.error("Subscription ID is required. Please set IRISML_AML_SUBSCRIPTION_ID or use --subscription_id option.")
+    if not args.compute_target:
+        parser.error("Compute target is required. Please set IRISML_AML_COMPUTE_TARGET or use --compute_target option.")
+
     envs = args.env
     cache_url = os.getenv('IRISML_CACHE_URL') if not args.no_cache else None
     if cache_url and args.include_local_tasks:
         logger.warning("Cache is disabled since local task implementations are used.")
         cache_url = None
 
     job = Job(args.job_filepath, envs)
```

### Comparing `irisml-tasks-azureml-0.1.2/irisml/tasks/add_aml_tag.py` & `irisml-tasks-azureml-0.1.3/irisml/tasks/add_aml_tag.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-azureml-0.1.2/irisml_tasks_azureml.egg-info/PKG-INFO` & `irisml-tasks-azureml-0.1.3/irisml_tasks_azureml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irisml-tasks-azureml
-Version: 0.1.2
+Version: 0.1.3
 Summary: Utility tools to use IrisML on AzureML
 Home-page: https://github.com/microsoft/irisml-tasks-azureml
 Author: irisdev
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `irisml-tasks-azureml-0.1.2/irisml_tasks_azureml.egg-info/SOURCES.txt` & `irisml-tasks-azureml-0.1.3/irisml_tasks_azureml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `irisml-tasks-azureml-0.1.2/setup.cfg` & `irisml-tasks-azureml-0.1.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = irisml-tasks-azureml
-version = 0.1.2
+version = 0.1.3
 url = https://github.com/microsoft/irisml-tasks-azureml
 description = Utility tools to use IrisML on AzureML
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = irisdev
 license = MIT
```

### Comparing `irisml-tasks-azureml-0.1.2/test/test_add_aml_tag.py` & `irisml-tasks-azureml-0.1.3/test/test_add_aml_tag.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-azureml-0.1.2/test/test_azureml.py` & `irisml-tasks-azureml-0.1.3/test/test_azureml.py`

 * *Files identical despite different names*

